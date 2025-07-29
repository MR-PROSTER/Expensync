# 💸 Expensync

**Decentralized Multi-Vendor Expense Tracker**

Expensync is a secure, blockchain-powered platform for managing and tracking expenses submitted by employees and vendors in organizations. It leverages decentralized storage, encryption, and transparent workflows to streamline approvals and maintain financial integrity — all while being simple to use with traditional Web2 company-based logins.

---

![image alt](https://github.com/MR-PROSTER/Expensync/blob/580fab44ba2c5b387f333814b8326f3a8ce6064d/Frontend/Dashboard.webp)

## 🚀 Features

- ✅ **Decentralized File Storage** using IPFS
- ✅ **Web2-based Company Login System** (no wallets required)
- ✅ **Role-based Dashboards** for Admins (Approvers) and Employees
- ✅ **Submit & Track Expenses** by category, vendor, and project
- ✅ **Encrypted Submissions & Tamper-proof Logs**
- ✅ **Approval Workflows** with real-time status tracking
- ✅ **Blockchain Ledger Integration** via Ganache
- ✅ **Subscription Tiers**: Gold, Platinum, Diamond
- ✅ **Real-time Feedback System**
- ✅ **Sleek Animations** using Motion.dev
- ✅ **Responsive UI/UX** built with Tailwind CSS

---

## 🧑‍💻 Tech Stack

| Technology   | Purpose                                |
| ------------ | -------------------------------------- |
| Next.js      | Frontend Framework                     |
| Tailwind CSS | UI Styling                             |
| Motion.dev   | Smooth UI animations                   |
| TypeScript   | Static typing for safer development    |
| IPFS         | Decentralized File Storage             |
| Express.js   | Backend APIs                           |
| MongoDB      | Database for expenses and user records |
| Ganache      | Local Blockchain for logging approvals |

---

## 📦 API Overview

### `POST /api/expenses`

Submit a new expense
**Request Body:**

```json
{
  "vendorName": "Acme Corp",
  "submittedBy": "Jane Doe",
  "projectName": "Marketing",
  "expenseType": "Software",
  "amount": 1200,
  "receiptIPFS": "ipfs://Qm123...",
  "status": "Pending"
}
```

## Implementation Details

### i. Frontend

- **Web (`/web/`):** Built using ReactJS and Next.js. Provides a dashboard for the accounts team with access to all documents, analytics, and tools for budget management and verification.
  - Components for document display, analytics charts, user management, and budget setting.
  - Connects to backend APIs for document retrieval, budget information, and analytics data.
- **Mobile (`/mobile/`):** Developed in Flutter, focusing on ease of receipt submission, real-time budget tracking, and AI chatbot integration for user support.
  - Features include camera/upload for receipt submission, chatbot interface, and budget overview.
  - Interfaces with backend for document upload, chatbot queries, and budget updates.

### ii. Backend

- **Blockchain (`/blockchain/`):** Handles transaction logging for document submission, hashing, and time-stamping. Ensures receipts are auditable and tamper-proof.
  - Includes smart contracts (Solidity or custom solution) for managing document hashes and time-stamps.
  - Interfaces with Avalanche or Quorum networks.
- **File Storage (`/storage/`):** Documents are uploaded and pinned to IPFS, providing decentralized and reliable access.
  - Integration scripts for IPFS pinning/unpinning.
  - Metadata linking receipts to transaction hashes.
- **Authentication (`/auth/`):** Managed through Supabase, offering secure user management and session tracking.
  - Provides JWT-based authentication for web and mobile clients.

### iii. AI Components

- **Mobile OCR (`/mobile/ocr/`):** Automatically extracts key data from receipts to minimize manual entry (implementation pending).
- **AI Chatbot (`/ai/chatbot/`):** Available in both mobile and web, leveraging LangChain and a lightweight LLM/BERT for contextual responses and budget queries.
- **Fraud Detection (`/ai/fraud_detection/`):** Monitors each document upload, comparing with historical fraud patterns for early detection (model/approach TBD).
- **Analytics AI (`/ai/analytics/`):** Processes spending data to generate graphs, budget comparisons, and actionable insights using LLMs.

### iv. API Call Formats & Handling

- **Backend APIs (`/api/`):**
  - RESTful endpoints for user authentication, document upload, budget management, analytics retrieval, and blockchain operations.
  - API documentation (to be provided upon finalization).

### v. Overall Design

- **UI/UX:**
  - Mobile app: Prioritizes fast receipt capture, clear budget visibility, and easy interaction with the chatbot.
  - Web dashboard: Optimized for data review, document verification, analytics, and streamlined workflow for the accounts team.

### vi. Minimum Requirements

All contributors must maintain the required set of software and environments until the end of the hackathon. Details to be specified by the team leads.

---

## Directory Structure

```
/
├── web/                 # Web frontend (ReactJS + Next.js)
├── mobile/              # Mobile app (Flutter)
│    └── ocr/            # OCR module for receipt extraction (TBD)
├── blockchain/          # Smart contracts and blockchain integration
├── storage/             # IPFS integration and file handling logic
├── auth/                # Authentication and Supabase management
├── ai/                  # AI modules (chatbot, fraud detection, analytics)
│    ├── chatbot/
│    ├── fraud_detection/
│    └── analytics/
├── api/                 # Backend API definitions and handlers
├── docs/                # Documentation and API specs
└── README.md            # Project overview (this file)
```

---

## Code Overview

- **web/**: Contains all the React/Next.js components, pages, and API integration for the accounts team's dashboard.
- **mobile/**: Flutter codebase for the worker-facing app, including UI, business logic, and integration for OCR and chatbot.
- **blockchain/**: Smart contract source code (e.g., Solidity), deployment scripts, and blockchain interaction modules.
- **storage/**: Scripts and utilities for integrating with IPFS, handling document uploads, and managing file hashes.
- **auth/**: Supabase configuration, user management scripts, and authentication middleware.
- **ai/**:
  - **chatbot/**: Code for the AI assistant, RAG logic, and integration with LangChain/LLM.
  - **fraud_detection/**: ML/LLM models and scripts for document analysis.
  - **analytics/**: Data aggregation and visualization logic, including AI-driven insights.
- **api/**: REST API implementation, routing, and controller logic for all app features.
- **docs/**: Contains setup instructions, architecture diagrams, and API docs.

---

## Contributing

- Please raise an issue or pull request for any proposed changes.
- For significant feature modifications, notify the maintainers in advance.

## License

MIT License © 2025 [M Praneeth]

## Contact

For queries, contact the project maintainers or open an issue in the repository.

---
