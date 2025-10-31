# 📘 Maxtera Documentation

**Product of MAXTERS LTD — “Your Money, Your Power.”**

Maxtera is a fintech platform that enables users to **buy data, airtime, and pay bills easily** — while maintaining full control over their wallet.  
Unlike traditional platforms, Maxtera allows users to **withdraw their balance anytime**, giving them true financial flexibility.

---

## 🏗️ System Architecture

| Layer | Stack |
|--------|-------|
| Frontend | **Next.js + TypeScript + TailwindCSS** |
| Backend | **Django REST Framework (Python)** |
| Database | **PostgreSQL** |
| Payment Gateway | **OnePipe API (for deposits & withdrawals)** |
| Hosting | **Vercel (frontend)**, **Render / AWS (backend)** |

---

## 📁 Repository Structure

| Repo | Description |
|------|--------------|
| [`Maxtera-backend`](https://github.com/Maxters-ltd/Maxtera-backend) | Django REST API — handles authentication, wallet, and transactions |
| [`Maxtera-frontend`](https://github.com/Maxters-ltd/Maxtera-frontend) | Next.js frontend — user dashboard and admin interface |
| `Maxtera-docs` | Technical documentation, setup guide, and system architecture |

---

## 🧩 Core Features

- 🔐 **Secure user authentication** (JWT + Transaction PIN)
- 💳 **Wallet system** (fund, transfer, withdraw)
- 🌐 **Data & airtime purchase** (via third-party APIs)
- 🧾 **Transaction history logs**
- 🏦 **API integration with OnePipe**
- 👑 **Admin dashboard** (for monitoring users and sales)

---

## 🧠 Technical Overview

### Backend Highlights
- Django + DRF architecture
- PostgreSQL database
- Modular apps: `users`, `wallet`, `transactions`, `bills`
- RESTful API structure with versioning

### Frontend Highlights
- Next.js 14 App Router
- TypeScript & TailwindCSS
- Reusable components (Navbar, Sidebar, Cards)
- Auth & Wallet context providers

---

## 🧰 Developer Setup (Backend)

```bash
git clone https://github.com/Maxters-ltd/Maxtera-backend.git
cd Maxtera-backend
pip install -r requirements.txt
python manage.py runserver


💻 Developer Setup (Frontend)

git clone https://github.com/Maxters-ltd/Maxtera-frontend.git
cd Maxtera-frontend
npm install
npm run dev


---

⚙️ Environment Variables

Backend .env.example

SECRET_KEY=your_django_secret_key
DATABASE_URL=postgres://user:password@localhost:5432/maxtera
API_BASE_URL=https://api.maxtera.com
ONEPIPE_SECRET_KEY=your_onepipe_secret_key

Frontend .env.example

NEXT_PUBLIC_API_BASE_URL=https://api.maxtera.com
NEXT_PUBLIC_APP_NAME=Maxtera
NEXT_PUBLIC_SUPPORT_EMAIL=support@maxtera.ng


---

🚀 Deployment

Frontend → Vercel

Backend → Render or AWS

Database → Managed PostgreSQL (Neon.tech / Supabase / AWS RDS)



---

🛠️ Roadmap

[ ] OnePipe integration for wallet funding

[ ] Admin analytics dashboard

[ ] Automated transaction reconciliation

[ ] Merchant API for third-party integration



---

📞 Contact

MAXTERS LTD
📧 support@maxtera.ng
🌐 www.maxtera.com
📍 Nigeria
---

📘 [View Full System Architecture](./SYSTEM_ARCHITECTURE.md)
---

© 2025 MAXTERS LTD — All rights reserved.
