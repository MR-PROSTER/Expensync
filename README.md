# 💸 Expensync

<div align="center">

**Decentralized Multi-Vendor Expense Tracker**

*Secure, blockchain-powered platform for managing and tracking expenses with transparent workflows and financial integrity*

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=next.js&logoColor=white)](https://nextjs.org/)
[![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat&logo=flutter&logoColor=white)](https://flutter.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![IPFS](https://img.shields.io/badge/IPFS-65C2CB?style=flat&logo=ipfs&logoColor=white)](https://ipfs.io/)

</div>

---

## 📱 Preview

### Web Dashboard
<div align="center">
  <img src="https://github.com/MR-PROSTER/Expensync/blob/437011b80407f0b02044e2ca44532e2e9267e073/Frontend/Dashboard.webp" alt="Dashboard Overview" width="90%" style="margin: 10px;"/>
</div>

<div align="center">
  <img src="https://github.com/MR-PROSTER/Expensync/blob/437011b80407f0b02044e2ca44532e2e9267e073/Frontend/Trips.webp" alt="Trips Management" width="90%" style="margin: 10px;"/>
</div>


### Mobile Application
<div align="center">
  <img src="https://github.com/MR-PROSTER/Expensync/blob/437011b80407f0b02044e2ca44532e2e9267e073/Frontend/Phone.webp" width="80%" style="margin: 10px;"/>
</div>

---

## 🚀 Features

<table>
<tr>
<td width="50%">

### 🔐 **Security & Blockchain**
- ✅ **Decentralized File Storage** using IPFS
- ✅ **Blockchain Ledger Integration** via Ganache
- ✅ **Encrypted Submissions & Tamper-proof Logs**
- ✅ **Fraud Detection AI** for expense validation

</td>
<td width="50%">

### 👥 **User Experience**
- ✅ **Web2-based Company Login** (no wallets required)
- ✅ **Role-based Dashboards** for Admins and Employees
- ✅ **Real-time Feedback System**
- ✅ **Sleek Animations** using Motion.dev

</td>
</tr>
<tr>
<td width="50%">

### 📊 **Management & Analytics**
- ✅ **Submit & Track Expenses** by category, vendor, project
- ✅ **Approval Workflows** with real-time status tracking
- ✅ **AI-powered Analytics** for spending insights
- ✅ **Budget Management** with automated tracking

</td>
<td width="50%">

### 📱 **Multi-Platform**
- ✅ **Responsive Web Dashboard** for administrators
- ✅ **Flutter Mobile App** for expense submission
- ✅ **OCR Integration** for automatic receipt processing
- ✅ **AI Chatbot** for user support

</td>
</tr>
</table>

---

## 🛠️ Tech Stack

<div align="center">

| **Frontend** | **Backend** | **Blockchain** | **AI/ML** |
|:---:|:---:|:---:|:---:|
| ![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white) | ![Express.js](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge) | ![Ethereum](https://img.shields.io/badge/Ganache-FF6C37?style=for-the-badge) | ![TensorFlow](https://img.shields.io/badge/AI%20Analytics-FF6F00?style=for-the-badge) |
| ![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white) | ![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white) | ![IPFS](https://img.shields.io/badge/IPFS-65C2CB?style=for-the-badge&logo=ipfs&logoColor=white) | ![OpenAI](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge) |
| ![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white) | ![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white) | ![Solidity](https://img.shields.io/badge/Solidity-363636?style=for-the-badge&logo=solidity&logoColor=white) | ![OCR](https://img.shields.io/badge/OCR-4285F4?style=for-the-badge) |
| ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white) | ![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white) | - | ![Fraud Detection](https://img.shields.io/badge/Fraud%20Detection-DC382D?style=for-the-badge) |

</div>

---

## 🏗️ Architecture Overview

```mermaid
graph TB
    A[Mobile App - Flutter] --> B[Backend APIs]
    C[Web Dashboard - Next.js] --> B
    B --> D[MongoDB Database]
    B --> E[Supabase Auth]
    B --> F[IPFS Storage]
    B --> G[Blockchain - Ganache]
    B --> H[AI Services]
    
    H --> I[OCR Processing]
    H --> J[Fraud Detection]
    H --> K[Analytics AI]
    H --> L[Chatbot]
    
    style A fill:#02569B,color:#fff
    style C fill:#000,color:#fff
    style F fill:#65C2CB,color:#fff
    style G fill:#FF6C37,color:#fff
    style H fill:#FF6F00,color:#fff
```

---

## 📂 Project Structure

```
📦 Expensync/
├── 🌐 web/                    # Web frontend (ReactJS + Next.js)
│   ├── components/            # Reusable UI components
│   ├── pages/                 # Next.js pages and routing
│   ├── styles/                # Tailwind CSS configurations
│   └── utils/                 # Helper functions and utilities
├── 📱 mobile/                 # Mobile app (Flutter)
│   ├── lib/                   # Flutter source code
│   ├── assets/                # Images, fonts, and resources
│   └── ocr/                   # OCR module for receipt extraction
├── ⛓️ blockchain/             # Smart contracts and blockchain integration
│   ├── contracts/             # Solidity smart contracts
│   ├── migrations/            # Deployment scripts
│   └── truffle-config.js      # Blockchain configuration
├── 🗄️ storage/               # IPFS integration and file handling
│   ├── ipfs-config.js         # IPFS node configuration
│   └── file-handlers/         # Upload/download utilities
├── 🔐 auth/                   # Authentication and Supabase management
│   ├── supabase-config.js     # Database and auth setup
│   └── middleware/            # Authentication middleware
├── 🤖 ai/                     # AI modules and services
│   ├── chatbot/               # AI assistant and RAG logic
│   ├── fraud_detection/       # ML models for expense validation
│   ├── analytics/             # Data analysis and insights
│   └── ocr/                   # Optical character recognition
├── 🔌 api/                    # Backend API definitions and handlers
│   ├── routes/                # Express.js routes
│   ├── controllers/           # Business logic controllers
│   └── models/                # Data models and schemas
├── 📚 docs/                   # Documentation and API specs
│   ├── api-reference.md       # API documentation
│   ├── setup-guide.md         # Installation instructions
│   └── architecture.md        # System architecture details
└── 📋 README.md               # Project overview (this file)
```

---

## 🚀 Quick Start

### Prerequisites

```bash
# Required software versions
Node.js >= 16.0.0
Flutter >= 3.0.0
MongoDB >= 5.0
Ganache CLI >= 6.12.0
```

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/expensync.git
   cd expensync
   ```

2. **Install dependencies**
   ```bash
   # Backend dependencies
   npm install
   
   # Frontend dependencies
   cd web && npm install
   
   # Mobile dependencies
   cd ../mobile && flutter pub get
   ```

3. **Environment setup**
   ```bash
   # Copy environment template
   cp .env.example .env
   
   # Configure your environment variables
   # - MongoDB connection string
   # - Supabase credentials
   # - IPFS node configuration
   # - Blockchain network settings
   ```

4. **Start the services**
   ```bash
   # Start blockchain (Ganache)
   npm run blockchain:start
   
   # Deploy smart contracts
   npm run contracts:deploy
   
   # Start backend server
   npm run server:dev
   
   # Start web frontend
   npm run web:dev
   
   # Start mobile app (requires Android/iOS emulator)
   npm run mobile:dev
   ```

---

## 📊 API Reference

### Core Endpoints

#### 💰 Expense Management

```http
POST /api/expenses
```

**Submit a new expense**

```json
{
  "vendorName": "Acme Corp",
  "submittedBy": "Jane Doe",
  "projectName": "Marketing Campaign",
  "expenseType": "Software License",
  "amount": 1200.00,
  "receiptIPFS": "ipfs://QmYourHashHere...",
  "description": "Annual software subscription",
  "status": "Pending"
}
```

#### 📈 Analytics

```http
GET /api/analytics/dashboard
```

**Get dashboard analytics**

```json
{
  "totalRevenue": 268419,
  "newVendors": 32,
  "activeProjects": 15,
  "auditSyncRate": 98,
  "expenditureGraph": [...],
  "recentTransactions": [...]
}
```

### 🔐 Authentication

All API endpoints require authentication via JWT tokens:

```http
Authorization: Bearer <your-jwt-token>
```

---

## 🎯 Subscription Tiers

<div align="center">

| Feature | **Gold** | **Platinum** | **Diamond** |
|:--------|:--------:|:------------:|:-----------:|
| Monthly Expenses | 500 | 2,000 | Unlimited |
| Team Members | 10 | 50 | Unlimited |
| AI Analytics | ✅ Basic | ✅ Advanced | ✅ Premium |
| Fraud Detection | ❌ | ✅ | ✅ |
| Custom Integrations | ❌ | ✅ Limited | ✅ Full |
| **Price/Month** | **$29** | **$99** | **$299** |

</div>

---

## 🤝 Contributing

We welcome contributions from the community! Please follow these steps:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

### Development Guidelines

- Follow the existing code style and conventions
- Write comprehensive tests for new features
- Update documentation for any API changes
- Ensure all CI/CD checks pass before submitting

---

## 📱 Mobile App Features

<table>
<tr>
<td width="50%">

### 📸 **Quick Expense Capture**
- Camera integration for receipt scanning
- OCR for automatic data extraction
- Offline submission capability
- Bulk upload functionality

</td>
<td width="50%">

### 💬 **AI Assistant**
- Natural language expense queries
- Budget tracking and alerts
- Spending pattern insights
- 24/7 chat support

</td>
</tr>
</table>

---

## 🔒 Security Features

- **End-to-end encryption** for all expense data
- **Blockchain immutability** for audit trails
- **Multi-factor authentication** for admin accounts
- **Role-based access control** (RBAC)
- **Automated fraud detection** using AI/ML
- **GDPR compliant** data handling

---

## 📞 Support & Contact

<div align="center">

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:support@expensync.com)
[![Documentation](https://img.shields.io/badge/Docs-000000?style=for-the-badge&logo=gitbook&logoColor=white)](https://docs.expensync.com)
[![GitHub Issues](https://img.shields.io/badge/Issues-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/your-username/expensync/issues)

</div>

For technical support or feature requests, please:
- 📧 Email us at **support@expensync.com**
- 🐛 Report bugs via [GitHub Issues](https://github.com/your-username/expensync/issues)
- 📖 Check our [Documentation](https://docs.expensync.com)

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

<div align="center">

**Built with ❤️ by [M Praneeth](https://github.com/your-username)**

*Empowering organizations with transparent, secure, and intelligent expense management*

[![Star this repo](https://img.shields.io/github/stars/your-username/expensync?style=social)](https://github.com/your-username/expensync)
[![Fork this repo](https://img.shields.io/github/forks/your-username/expensync?style=social)](https://github.com/your-username/expensync/fork)

</div>
