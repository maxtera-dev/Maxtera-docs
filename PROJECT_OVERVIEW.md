# 💼 Project Overview — Maxtera

**Product of MAXTERS LTD**  
🪙 *“Your Money, Your Power”*

Maxtera is a next-generation fintech platform designed to empower users with **true control over their digital wallet** — allowing them to buy data, airtime, and pay bills easily, while also being able to **withdraw their balance anytime**.

---

## 🚀 Vision

To become the **most flexible and user-driven fintech system** in Africa — where every user has total control over their money, without platform restrictions.

> Maxtera = Financial Freedom + Digital Simplicity

---

## 🎯 Core Mission

1. Provide users with the ability to buy **all data types** (Gifting, SME, Corporate).  
2. Offer **affordable airtime and bill payments**.  
3. Introduce **instant wallet withdrawals**, unlike other fintechs that lock user funds.  
4. Build a **modern, transparent financial platform** using secure APIs and scalable architecture.

---

## 🧩 Key Features

| Feature | Description |
|----------|--------------|
| 🔐 **Authentication & PIN** | Secure login, password, and transaction PIN |
| 💳 **Wallet System** | Fund, transfer, withdraw, and track all balances |
| 📱 **Data & Airtime** | Buy Gifting, SME, and Corporate data bundles |
| 🧾 **Bill Payments** | Pay for electricity, TV, education, etc. |
| 🧠 **Admin Dashboard** | Control system APIs, monitor users, view transactions |
| 🌍 **API Integrations** | Connect with OnePipe and third-party data vendors |

---

## 🏗️ System Structure

| Layer | Stack |
|--------|-------|
| Backend | Django REST Framework (Python) |
| Frontend | Next.js + TypeScript + TailwindCSS |
| Database | PostgreSQL |
| Payment Gateway | OnePipe API |
| Hosting | Render (backend) + Vercel (frontend) |

---

## 🔗 How It Works (Simplified Flow)

1️⃣ **User Registration**
   - User signs up with phone + email  
   - Verifies OTP  
   - Creates transaction PIN  

2️⃣ **Wallet Funding**
   - Uses OnePipe to fund via card, transfer, or USSD  

3️⃣ **Purchases**
   - Buys data, airtime, or bills directly  
   - Transaction is logged in real-time  

4️⃣ **Withdrawal**
   - User can withdraw balance to any Nigerian bank account  
   - Process handled by OnePipe APIs  

---

## 🧠 User Roles

| Role | Description |
|------|-------------|
| **Customer** | End-user — buys data, airtime, pays bills, withdraws |
| **Admin** | Manages users, vendors, transactions |
| **Developer** | Builds and maintains system APIs and frontend |
| **Partner Vendor** | Supplies data/airtime APIs for integration |

---

## 💡 Business Model

- **Revenue Sources:**
  - Small margin on each data/airtime/bill transaction  
  - Vendor partnership commissions  
  - Transaction fees (e.g., ₦10–₦20 per wallet activity)

- **Unique Advantage:**
  - Users aren’t locked into spending — they can withdraw anytime.  
  - Supports multiple data vendors for best prices.

---

## 🔐 Compliance & Licensing

- Registered under **MAXTERS LTD**  
- Business type: **Software Development & Financial Services**  
- Uses **licensed payment aggregator (OnePipe)** for banking compliance  

---

## 🌐 Repositories Overview

| Repository | Description |
|-------------|-------------|
| [`Maxtera-backend`](https://github.com/Maxters-ltd/Maxtera-backend) | Django REST API (wallet, users, transactions) |
| [`Maxtera-frontend`](https://github.com/Maxters-ltd/Maxtera-frontend) | Next.js dashboard |
| [`Maxtera-docs`](https://github.com/Maxters-ltd/Maxtera-docs) | Documentation, architecture, and developer guides |

---

## 📅 Current Development Status

✅ Database setup  
✅ User registration & login  
✅ Wallet & transaction system  
✅ Data & airtime integration (tested)  
🚧 OnePipe integration in progress  
🚧 Admin panel setup  
🚧 Public launch soon  

---

## 📞 Contact

**MAXTERS LTD**  
📧 support@maxtera.ng  
🌐 [www.maxtera.com](https://www.maxtera.com)  
📍 Nigeria  

---

**© 2025 MAXTERS LTD — All rights reserved.**