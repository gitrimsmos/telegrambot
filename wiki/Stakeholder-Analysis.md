# Stakeholder Analysis

| Stakeholder | Power (H/L) | Interest (H/L) | Role/Engagement |
| :--- | :--- | :--- | :--- |
| **SME Owner** (BHK88 Gaming Platform) | High | High | **Primary Sponsor / Client:** Approves the business logic, deposit/withdrawal approval flow, and validates if the bot meets operational requirements. |
| **End User** (Platform Players) | Low | High | **Target Audience:** Uses the bot to register accounts, request deposits/withdrawals, and manage their gaming wallets. Drives UI/UX requirements. |
| **Instructor** (Course Dean) | High | High | **Academic Auditor:** Audits technical architecture (Python (telebot)/SQLite), code quality, GitHub Git flow, and proper project management tracking. |
| **Project Team** (Tech Nova) | Medium | High | **Execution Team:** Responsible for project management, frontend/backend development, testing, and continuous deployment (DevOps). |
| **Telegram API** | High | Low | **External Dependency:** Provides the fundamental technical infrastructure. System must strictly adhere to its API rate limits and updates. |

## Management Strategy
* **SME Owner (BHK88 Platform Owner):** Conduct weekly status updates and reviews to align on transaction verification guidelines, deposit bonus rates, and operational security requirements. Utilize the GitHub Project board to track tasks.
* **End User (Platform Players):** Simplify the onboarding experience by auto-generating credentials, streamline the Bakong/Bank payment proof submission, and ensure instant feedback notifications on deposit/withdrawal status.
* **Instructor (Course Dean):** Maintain a strict git branch-based workflow with clear commit messages, provide comprehensive thread-safe database documentation, and keep the project board and wiki updated for academic reviews.
* **Telegram API:** Implement rate-limit management, connection timeout error-handling, and robust callback query exceptions to guarantee maximum bot uptime and reliable performance.