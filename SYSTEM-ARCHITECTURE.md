
🏗️ Maxtera System Architecture (GitHub Setup)

Maxtera is divided into two main repositories, following clean separation of concerns — one for backend (API + business logic) and one for frontend (UI + user experience).


---

🧠 1. Maxtera Backend (Django + DRF)

Repository: https://github.com/Maxters-ltd/Maxtera-backend

Purpose:
Handles all the core operations — authentication, wallet management, data/airtime/bills APIs, and integrations (like OnePipe).

Key technologies:

Python 3.x

Django + Django REST Framework

PostgreSQL

Docker (optional)

JWT Authentication


Main folders:

Maxtera-backend/
├── apps/
│   ├── users/
│   ├── wallet/
│   ├── data/
│   ├── airtime/
│   ├── bills/
│   └── transactions/
├── maxtera/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md

Deployment suggestion:
Host on Render, Railway, or AWS EC2.


---

💻 2. Maxtera Frontend (Next.js + TypeScript + TailwindCSS)

Repository: https://github.com/Maxters-ltd/Maxtera-frontend

Purpose:
Provides the customer-facing dashboard for users to manage accounts, buy data, airtime, pay bills, and withdraw funds.

Key technologies:

Next.js 14 (App Router)

TypeScript

TailwindCSS + shadcn/ui

Axios for API calls

Zustand or React Context for state management


Main folders:

Maxtera-frontend/
├── public/
│   └── assets/logo.png
├── src/
│   ├── pages/
│   ├── components/
│   ├── layouts/
│   ├── services/
│   ├── context/
│   ├── styles/
│   ├── utils/
│   └── types/
├── package.json
├── tsconfig.json
├── .env.example
├── .gitignore
└── README.md

Deployment suggestion:
Host on Vercel (best for Next.js) or Netlify.


---

🔗 How They Connect

1. Backend API Base URL

Hosted API (e.g., https://api.maxtera.com)



2. Frontend consumes the API

Example:

axios.get(`${process.env.NEXT_PUBLIC_API_BASE_URL}/api/wallet/balance/`);



3. Authentication

Uses JWT tokens — stored securely in httpOnly cookies or localStorage.
