# 🔐 Maxtera Security Policy

**Product of MAXTERS LTD — “Your Money, Your Power.”**

This document defines the **security standards and access rules** for all developers, contributors, and team members working on the Maxtera ecosystem.

---

## 🧱 1. Access Control

| Role | Access Level | Notes |
|------|---------------|-------|
| Owner | Full | Business founder — manages all repositories |
| Admin | High | May merge pull requests and manage branches |
| Maintainer | Medium | Reviews and merges code after approval |
| Contributor | Limited | Can only submit PRs, cannot merge |
| Read-only | None | Can view repos, but not modify anything |

- Only the **Owner** may invite or remove members.  
- All members **must enable Two-Factor Authentication (2FA)** on GitHub.  
- Sensitive files (`.env`, credentials, secrets) must never be uploaded or shared in commits.

---

## 🧩 2. Secure Coding Standards

- Follow **PEP8** (for Python) and **Prettier/ESLint** (for TypeScript).
- Avoid hardcoding secrets or API keys in source files.
- Use **environment variables** (`.env`) for all credentials.
- Validate all user inputs to prevent injection attacks.
- Always sanitize data before database writes.
- Never expose detailed error messages in production.

---

## 🔑 3. Environment Variables

Developers must use `.env.example` files as a reference.  
Real `.env` files must **only exist locally** on development machines.

Example backend `.env` file:
SECRET_KEY=your_django_secret_key DATABASE_URL=postgres://user:password@localhost:5432/maxtera ONEPIPE_SECRET_KEY=your_onepipe_secret_key

Example frontend `.env` file:
NEXT_PUBLIC_API_BASE_URL=https://api.maxtera.com NEXT_PUBLIC_APP_NAME=Maxtera NEXT_PUBLIC_SUPPORT_EMAIL=support@maxtera.ng

Never share or commit these credentials to GitHub.

---

## ⚙️ 4. Repository Protection

- `main` branch is protected — only admins may merge.
- Require **Pull Request (PR) review** before merging.
- Disallow force pushes and direct commits to `main`.
- Automatically delete merged branches (to keep clean repo).

---

## 🧠 5. API & Payment Gateway Security

- All external APIs (e.g. OnePipe) must use **sandbox keys** for testing.
- Only production servers may use **live keys**, stored securely in `.env` files.
- Use HTTPS for all backend requests.
- Never log sensitive data (PINs, tokens, user info).

---

## 💬 6. Reporting Security Issues

If you discover a vulnerability, please **report it privately** via:
- 📧 Email: security@maxtera.ng
- 📞 Or contact the Owner directly.

Do not publicly post vulnerabilities on GitHub Issues.

---

## 🚫 7. Forbidden Actions

- Sharing private repo access without permission.
- Uploading production data or credentials.
- Copying or selling Maxtera source code.
- Installing unauthorized packages or libraries.

Violations will lead to immediate removal and possible legal action.

---

## 🧾 8. Review Policy

All code changes must pass:
1. Automated CI checks (if enabled)
2. Manual review by Admin or Maintainer
3. Testing in a sandbox environment before production deploy

---

## 🛡️ 9. Deployment Security

- Backend hosted on Render / AWS with HTTPS enforced
- Frontend hosted on Vercel / Netlify
- Database backups encrypted with AES-256
- Access limited by IP and user roles

---

## 📞 Contact

**MAXTERS LTD — Security Team**  
📧 security@maxtera.ng  
🌐 [www.maxtera.com](https://www.maxtera.com)

---

**© 2025 MAXTERS LTD — All rights reserved.**
