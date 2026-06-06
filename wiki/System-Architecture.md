# 🏗️ System Architecture

This page outlines the technical architecture, data model, and state management flow of the BHK88 Gaming Platform Telegram Bot.

## 1. High-Level Architecture Diagram
The system is built on a client-server architecture utilizing the Telegram Bot API as the gateway, a Python backend handling the state machine, and a local SQLite database for persistent storage.

```mermaid
graph TD
    User["📱 Platform Player (Client)"]
    Admin["👨‍💼 Shop Admin / Operator"]
    TelegramAPI["💬 Telegram Bot API Gateway"]
    BotServer["🐍 Python Backend (telebot)"]
    SQLite["🗄️ SQLite Database (bot.db)"]
    FileSystem["📁 Local File System (Screenshots)"]

    User <-->|1. Interactions / Commands / Receipts| TelegramAPI
    Admin <-->|4. Approve / Reject Decisions| TelegramAPI
    TelegramAPI <-->|2. Long Polling Updates| BotServer
    BotServer <-->|3. CRUD Operations| SQLite
    BotServer <-->|5. Read / Write Media| FileSystem
```

---

## 2. Database Schema (SQLite)
The application utilizes a relational database structure designed to support users, referral relationships, and transactional histories (deposits and withdrawals).

```mermaid
erDiagram
    USERS {
        int id PK
        string account_number UK "6-digit unique number"
        string name
        string phone
        string ref_code UK "Unique referral code"
        string referred_by "ref_code of referrer"
        string password
        string customer_type "new / old"
        real balance
        int telegram_id
    }
    DEPOSITS {
        int id PK
        int user_id FK
        real amount
        real bonus_amount
        string status "pending / approved / rejected"
        string screenshot_file_id
        timestamp created_at
    }
    WITHDRAWALS {
        int id PK
        int user_id FK
        real amount
        string status "pending / approved / rejected"
        string khqr_file_id
        timestamp created_at
    }

    USERS ||--o{ DEPOSITS : "submits"
    USERS ||--o{ WITHDRAWALS : "requests"
```

---

## 3. Core Component Roles
* **Telegram Client (UI):** Users interact exclusively through interactive buttons (`InlineKeyboardMarkup`) and text inputs, ensuring sub-2-second response latency.
* **Python Backend (`telebot`):** 
  - Manages session storage for multi-step tasks (e.g., registration steps, deposit/withdrawal creation).
  - Handles thread-safe SQLite connection pools.
  - Implements the FSM (Finite State Machine) using step-handlers.
* **SQLite Database (`bot.db`):** Fast, file-based database handling user profiles, financial balances, and referral links.
* **Admin Approval Gateway:** The bot pushes deposit and withdrawal verification requests directly to the designated `ADMIN_CHAT_ID`. Admins approve or reject transactions using inline buttons, which automatically updates user balances and sends instant notification receipts to the user.