# Enterprise Software Approval Management App

An internal governance application built with the **Grit Framework** (Go + Next.js + PostgreSQL) designed to streamline software procurement requests, track IT/security compliance, and prevent shadow IT within the organization.

---

## 🚀 Tech Stack

- **Backend:** Go (Gin + GORM)
- **Frontend:** Next.js (React + TypeScript + Tailwind CSS)
- **Database:** PostgreSQL
- **Architecture:** Monorepo (Powered by Grit & Turborepo)

---

## 👥 Core Roles & Permissions

1. **Requester (Employee):** Submit software requests, track approval statuses, and view approved software catalog.
2. **Line Manager:** Initial budget and business-need assessment for department members.
3. **IT Admin:** Technical compatibility check, SSO integration feasibility, and duplicate tool detection.
4. **Security Team:** Compliance, data privacy (GDPR/ISO), and risk assessment.
5. **Finance / Procurement:** Cost review, vendor negotiation, and license allocation.

---

## 📋 Key Features

- **Smart Request Form:** Dynamic inputs for software name, business justification, estimated cost, user count, and licensing type.
- **Conditional Workflow Engine:** Automated routing based on predefined rules (e.g., low-cost tools bypass security; high-cost or cloud-storage tools require full multi-department sign-off).
- **Approved Software Catalog:** A centralized knowledge base of pre-vetted tools to prevent redundant purchases.
- **Audit Logs & Dashboard:** Real-time tracking of pending bottlenecks, departmental software spend, and upcoming renewals.

---

## ⚙️ Getting Started (Local Development)

### Prerequisites
- Go (v1.22+)
- Node.js (v18+)
- PostgreSQL
- Grit CLI installed (`go install github.com/MUKE-coder/grit/cmd/grit@latest`)

### 1. Clone & Setup
```bash
# Clone the repository
git clone <your-repository-url>
cd software-approval-app

# Install dependencies
go mod download
cd frontend && npm install
