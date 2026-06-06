# User Stories (INVEST Standard)

This page documents the user stories for the BHK88 Gaming Platform Telegram Bot, detailing the player flows (F1) and admin operational flows (F2).

### 👥 Part 1: Customer (Player) Stories
ផ្នែកនេះរៀបរាប់ពីដំណើរការដែលអតិថិជនចូលមកប្រើប្រាស់ Bot (F1: Registration, Login & Wallet Management)៖

* **User Story 1: Account Registration & Referral System**
  - **As a** new player,
  - **I want to** register an account by providing my name, phone number, and optional referral code,
  - **So that** I receive a unique 6-digit account number, a secure password, my referral code, and a deposit bonus rate (20% default, or 30% if referred).

* **User Story 2: Secure Login & Wallet Dashboard**
  - **As a** registered player,
  - **I want to** log in securely using my account number and password,
  - **So that** I can view my current balance, access my wallet dashboard, and request deposits or withdrawals.

* **User Story 3: Deposit Request with Payment Proof**
  - **As a** logged-in player,
  - **I want to** submit a deposit request by entering the amount and uploading a screenshot of my bank transfer receipt,
  - **So that** the admin can verify the payment and credit my wallet.

* **User Story 4: Withdrawal Request**
  - **As a** logged-in player,
  - **I want to** request a withdrawal by entering the amount,
  - **So that** the admin can process the payout to my bank account.

---

### 👨‍💼 Part 2: Admin (Platform Owner/Staff) Stories
ផ្នែកនេះរៀបរាប់ពីដំណើរការគ្រប់គ្រងរបស់សមាជិកហាង ឬបុគ្គលិក (F2: Transaction Verification & Referral Control)៖

* **User Story 5: Real-time Transaction Verification**
  - **As a** platform admin,
  - **I want to** receive instant notifications of player deposit/withdrawal requests with interactive inline buttons (`Approve` / `Reject`),
  - **So that** I can verify and update the transaction status immediately.

* **User Story 6: Automated Referral Tracking & Bonus**
  - **As a** platform owner,
  - **I want** the bot to automatically credit a referral bonus ($1.00) to the referrer when a new user registers using their code,
  - **So that** our player community grows organically through word of mouth.