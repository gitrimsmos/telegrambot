# Meeting Minutes Log

## 🗓️ Week 8 - Sprint 3 Database Integration & Live Command Demo
* **Date:** May 30, 2026
* **Time:** 10:30 AM - 12:00 PM
* **Location:** DUC 
* **Facilitator:** Sreyleak (PM)

### 👥 Attending:
ស្រីលាក់, នេត, ផាន់ណា, រីម, រ៉ាម៉ន

### 🎯 Meeting Objectives & Decisions:
i. ពិភាក្សា និងរៀបចំប្លង់ទំនាក់ទំនងទិន្នន័យផ្លូវការ Physical ERD សម្រាប់តារាងស្នូល (users, deposits, withdrawals, products) ដាក់ចូល Wiki។
ii. សម្រេចបង្កើតកូដបង្កើត Database ផ្លូវការ `bot.db` រក្សាទុកក្នុងកូដ ដោយមិនប្រើប្រាស់ការចុចបង្កើតផ្ទាល់លើ GUI ឡើយ។
iii. រៀបចំសរសេរកូដទាញទិន្នន័យផ្ទាល់ (Dynamic Reads) ពី Database បង្ហាញនៅលើ Telegram តាមរយៈ Command `/start`។
iv. ធ្វើបច្ចុប្បន្នភាព GitHub Project Board សម្រាប់ Sprint ដោយភ្ជាប់ Issue ទៅកាន់ឈ្មោះ Developer ផ្ទាល់។

### 🛠️ Action Items:
* **ស្រីលាក់ & រ៉ាម៉ន :** បង្កើត Sprint column លើ Project Board, Assign ឈ្មោះសមាជិកឱ្យចំភារកិច្ច និងរៀបចំរចនាសម្ព័ន្ធ Wiki។
* **រីម & ផាន់ណា:** គូររូបប្លង់ Physical ERD ដែលមាន Data Types ច្បាស់លាស់ និងគូសខ្សែបន្ទាត់ PK/FK ត្រឹមត្រូវ យកទៅផុសក្នុងទំព័រ System Architecture។
* **នេត :** សរសេរកូដ Python (telebot) ភ្ជាប់មុខងារអានទិន្នន័យចេញពី SQLite មកបង្ហាញនៅលើ Bot ពេលវាយ Command `/start`។

---

## 🗓️ Week 7 - Sprint 2 Planning & State Management Discussion
* **Date:** May 30, 2026
* **Time:** 10:30 AM - 11:30 AM
* **Location:** DUC Software Lab
* **Facilitator:** Sreyleak (PM)

### 👥 Attending:
ស្រីលាក់, នេត, ផាន់ណា, រីម, រ៉ាម៉ន

### 🎯 Meeting Objectives & Decisions:
i. ក្រុមការងារបានសម្រេចចិត្តព្រាង User Stories ចំនួន ៣ ទៅ ៥ ឱ្យស្របតាមស្តង់ដារ INVEST សម្រាប់ដាក់ក្នុងទំព័រ `User Stories`។
ii. រៀបចំរចនាសម្ព័ន្ធលំហូរការសន្ទនា (Conversation Flowchart) ដើម្បីគ្រប់គ្រងស្ថានភាពអ្នកប្រើប្រាស់ (State Management / FSM) សម្រាប់ Telegram Bot។
iii. ធ្វើបច្ចុប្បន្នភាពនៅលើ GitHub Project Board ដោយត្រូវ Assign ឈ្មោះមនុស្សគ្រប់កិច្ចការក្នុង Week 7។

### 🛠️ Action Items:
* **ស្រីលាក់ & រ៉ាម៉ន:** សរសេរអត្ថបទ INVEST User Stories ៣-៥ ដាក់ក្នុង Wiki និងរៀបចំ Assign មនុស្សលើ Board។
* **រីម & ផាន់ណា:** ជួយរៀបចំគូររូបប្លង់ Conversation Flowchart យកទៅ Embed ក្នុង Wiki ផ្នែក System Architecture nudge។
* **នេត:** សរសេរកូដ Backend Python (telebot) គ្រប់គ្រង State (FSM Logic) ការពារកុំឱ្យ Bot គាំងពេល User វាយខុស។

---

## 🗓️ Week 6 - Sprint 1 Implementation & Database Setup
* **Date:** May 23, 2026
* **Time:** 10:00 AM - 11:30 AM
* **Location:** DUC Software Lab
* **Facilitator:** Sreyleak (PM)

### 👥 Attending:
ស្រីលាក់, នេត, ផាន់ណា, រីម, រ៉ាម៉ន

### 🎯 Decisions Made:
i. Finalized SQLite as the database engine for lightweight local testing and thread-safe operations.
ii. Structured the database schema to include `users`, `deposits`, and `withdrawals` tables.
iii. Agreed to use `pyTelegramBotAPI` (`telebot` in Python) for fast prototyping of the conversational bot.

### 🛠️ Action Items:
* **ស្រីលាក់​ & រ៉ាម៉ន:** Setup GitHub repo and write initial documentation templates.
* **រីម :** Develop the user registration handlers and auto-generation of 6-digit account numbers.
* **នេត & ផាន់ណា:** Write test cases for registration inputs and user verification.

---

## 🗓️ Week 5 - Project Realignment
* **Date:** May 16, 2026
* **Time:** 09:00 AM - 10:30 AM
* **Location:** DUC Software Lab
* **Facilitator:** Sreyleak (PM)

### 👥 Attending:
ស្រីលាក់, នេត, ផាន់ណា, រីម, រ៉ាម៉ន

### 🎯 Decisions Made:
i. Selected the BHK88 Gaming Platform - Deposit, Withdrawal & CRM Bot mockup.
ii. Reset the repository to remove leaked API keys.
iii. Finalized Python (telebot) as the backend language (Updated Tech Stack to: Python (telebot) + SQLite).

### 🛠️ Action Items:
* **ស្រីលាក់:** To finish the Wiki setup and link the first 3 Issues to the Project Board.

---
*(Add new entries at the top of this page every week)*