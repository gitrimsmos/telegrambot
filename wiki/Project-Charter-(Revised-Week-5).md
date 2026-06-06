# Tech Nova Solutions - Project Charter

Welcome to the official project documentation for our Telegram Bot solution. This bot is developed as part of the Software Project Development course (2026).

## 1. Problem Statement
The target online cosmetic (BHK88-Online) currently handles all customer inquiries, product consultations, and order processing manually through direct messaging. This approach leads to slow response times during peak hours, frequent human errors in tracking stock/orders, and a complete lack of centralized Customer Relationship Management (CRM) data. 

**Why a Telegram Bot instead of a website or standalone app?**
* **Zero Friction for Users:** In Cambodia, Telegram is already widely installed and used daily. Customers do not need to download a new app or register on an external website.
* **Low Development Cost:** Building and deploying a Telegram bot is faster and more cost-effective for an SME than maintaining native mobile apps or complex e-commerce websites.

## 2. Project Objectives (SMART)
* **Specific:** Develop an automated Telegram Bot that allows users to browse cosmetic products, manage a virtual shopping cart, place orders, and submit payment proofs directly inside the chat, while storing CRM data in a central database.
* **Measurable:** The bot must successfully handle at least 10 concurrent users with a response time of under 2 seconds per interaction.
* **Achievable:** Given a team of 5 members and using Python (telebot), building the core functionality within the remaining 7 weeks is highly realistic.
* **Relevant:** The solution directly addresses the SME's core issue by automating the sales funnel and centralizing customer records.
* **Time-bound:** Full system delivery, testing, and deployment must be completed by Week 12.

## 3. Scope Boundaries
### In-Scope (Features we WILL build)
* **User Onboarding & CRM Registration:** Automatically capture and save the user's Telegram ID, name, and phone number upon first interaction.
* **Interactive Product Catalog:** Display cosmetic items categorized by type (e.g., Skincare, Makeup) with clear images, pricing, and descriptions.
* **Shopping Cart System:** Allow users to add/remove items, view cart summaries, and adjust quantities before checking out.
* **Order Placement & Payment Upload:** Guide users through submitting their shipping address and uploading a screenshot of their Bakong/Bank payment receipt.

### Out-of-Scope (Features we will NOT build)
* **Direct Bank API Integration:** Real-time automated transaction verification will not be supported; receipt verification remains manual via an admin dashboard view.
* **Multi-Language Support:** The bot interface will strictly support a single language (Khmer) for this initial release phase.

## 4. Technical Constraints
* **Budget:** $0 (Utilizing free tiers of GitHub, Railway, and managed database services suitable for a course project).
* **Platform:** Telegram Bot API using Python (telebot).
* **Database:** SQLite to ensure full data persistence for user sessions, active carts, and order history.