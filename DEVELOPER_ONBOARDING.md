# 👩‍💻 Maxtera Developer Onboarding Guide

Welcome to **Maxtera**, a fintech platform by **MAXTERS LTD** — empowering users to buy data, airtime, pay bills, and manage their wallets securely.

This document is designed to help new developers get started quickly and maintain consistent development standards.

---

## 🧩 1. Project Overview

**Architecture:**
- **Backend:** Django + Django REST Framework (Python 3.x)
- **Frontend:** Next.js + TypeScript + TailwindCSS
- **Database:** PostgreSQL
- **Docs:** Markdown-based in `maxtera-docs` repo
- **Integrations:** OnePipe API (for deposits, withdrawals, and transfers)

**Repositories:**
| Component | Repository | Description |
|------------|-------------|-------------|
| Backend | [maxtera-backend](https://github.com/maxters-ltd/maxtera-backend) | API, authentication, and core business logic |
| Frontend | [maxtera-frontend](https://github.com/maxters-ltd/maxtera-frontend) | Web client (dashboard and user interface) |
| Documentation | [maxtera-docs](https://github.com/maxters-ltd/maxtera-docs) | Documentation hub for architecture, onboarding, and business guides |

---

## ⚙️ 2. Local Setup

### Prerequisites
Ensure the following are installed:
- **Git**
- **Python 3.10+**
- **Node.js 18+**
- **PostgreSQL**
- **npm or yarn**
- **VS Code (recommended)**

---

### 🧠 Backend Setup (Django)

```bash
# Clone repository
git clone https://github.com/maxters-ltd/maxtera-backend.git
cd maxtera-backend

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate   # (or venv\Scripts\activate on Windows)

# Install dependencies
pip install -r requirements.txt

# Setup environment variables
cp .env.example .env

# Run migrations
python manage.py migrate

# Start development server
python manage.py runserver

Default URL: http://127.0.0.1:8000


---

💻 Frontend Setup (Next.js)

# Clone repository
git clone https://github.com/maxters-ltd/maxtera-frontend.git
cd maxtera-frontend

# Install dependencies
npm install

# Setup environment
cp .env.example .env.local

# Start the dev server
npm run dev

Frontend runs on: http://localhost:3000


---

🔐 3. Environment Variables

Each repo contains .env.example.
Developers should copy and rename it to .env or .env.local before running.

Example Backend Variables:

SECRET_KEY=your_django_secret_key
DEBUG=True
DATABASE_URL=postgres://user:password@localhost:5432/maxtera

Example Frontend Variables:

NEXT_PUBLIC_API_BASE_URL=http://127.0.0.1:8000
NEXT_PUBLIC_APP_NAME=Maxtera
NEXT_PUBLIC_SUPPORT_EMAIL=support@maxtera.ng


---

🧭 4. Git & Branch Rules

Branch	Purpose

main	Stable production code only
dev	Development and testing
feature/*	New features (e.g., feature/wallet-module)
fix/*	Bug fixes (e.g., fix/payment-error)


Workflow:

1. Create a branch from dev


2. Commit changes using clear messages (e.g., feat: add OnePipe integration)


3. Submit a pull request (PR) to dev


4. PRs are reviewed before merging to main




---

🧠 5. Coding Standards

Backend (Django)

Follow PEP8 style guide.

Use serializers and viewsets properly.

Write reusable utility functions.

Include docstrings for all models and APIs.


Frontend (Next.js)

Use TypeScript for all components.

Follow folder-based architecture (pages, components, services).

Use Axios for HTTP calls.

Store global state using Context or Zustand.


Commit Message Convention

feat: add new transaction endpoint
fix: resolve wallet balance mismatch
refactor: improve data service logic
docs: update API docs


---

🧪 6. Testing & Quality

Backend: pytest or Django’s TestCase

Frontend: jest or react-testing-library

Run tests before any pull request.



---

🚀 7. Deployment (Staging & Production)

Environment	Platform	Repo

Backend	Render / Railway	maxtera-backend
Frontend	Vercel / Netlify	maxtera-frontend
Docs	GitHub Pages (optional)	maxtera-docs



---

🔑 8. Access & Security

API keys, secrets, and credentials are managed by the project admin (Maxters Ltd).

Never push .env files or credentials to GitHub.

Report any security concerns in SECURITY.md.



---

👥 9. Support Contacts

Role	Contact

Technical Lead	dev@maxtera.ng
Project Owner	admin@maxters.ng
Support	support@maxtera.ng



---

Welcome aboard 🚀
You’re now part of Maxtera — Your Money, Your Power.

---