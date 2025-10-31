# 🔌 Maxtera API Reference

Base URL:
https://api.maxtera.com/api/v1/

Authentication:  
- Token Type → Bearer (JWT)  
- Header Example:

Authorization: Bearer <your-access-token>

---

## 👤 Authentication

### POST /auth/register/
Registers a new user.

**Request**
```json
{
"email": "user@example.com",
"password": "mypassword",
"phone": "08012345678"
}

Response

{
  "message": "Account created successfully",
  "user_id": 23
}


---

POST /auth/login/

Logs in a user and returns JWT tokens.

Request

{
  "email": "user@example.com",
  "password": "mypassword"
}

Response

{
  "access": "jwt_token_here",
  "refresh": "refresh_token_here"
}


---

💰 Wallet

GET /wallet/balance/

Retrieves current wallet balance for authenticated user.

Response

{
  "balance": 5400.00,
  "currency": "NGN"
}


---

POST /wallet/fund/

Initiates deposit (via OnePipe integration).

Request

{
  "amount": 2000,
  "method": "onepipe"
}

Response

{
  "status": "pending",
  "reference": "MPX-23019482"
}


---

📶 Airtime

POST /airtime/purchase/

Purchases airtime through integrated API.

Request

{
  "network": "MTN",
  "amount": 100,
  "phone_number": "08012345678"
}

Response

{
  "status": "success",
  "reference": "MTN-20250130-001"
}


---

📡 Data

POST /data/purchase/

Purchases data bundle.

Request

{
  "network": "AIRTEL",
  "plan": "1GB",
  "phone_number": "08012345678"
}

Response

{
  "status": "success",
  "reference": "AIRTEL-DATA-001"
}


---

🧾 Bills

POST /bills/pay/

Pays cable, electricity, or other bills.

Request

{
  "service_type": "DSTV",
  "smartcard_number": "1234567890",
  "amount": 4800
}

Response

{
  "status": "success",
  "transaction_id": "BILL-4567"
}


---

📜 Transactions

GET /transactions/

Fetches user transaction history.

Response

[
  {
    "id": 1,
    "type": "Airtime",
    "amount": 100,
    "status": "success",
    "created_at": "2025-10-29T14:25:43Z"
  }
]


---

🧠 All endpoints are subject to authentication unless stated otherwise.
🔐 Do not share your access tokens publicly.


---

© 2025 MAXTERS LTD — All Rights Reserved

---