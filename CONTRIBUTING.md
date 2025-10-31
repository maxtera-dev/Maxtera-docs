
# 🧑‍💻 Contributing to Maxtera

Thank you for your interest in contributing to **Maxtera** — a product of **MAXTERS LTD**.  
This document explains how we collaborate, structure commits, and ensure code quality across all repositories.

---

## 🧭 Repositories Overview

| Repository | Description |
|-------------|-------------|
| [`Maxtera-backend`](https://github.com/Maxters-ltd/Maxtera-backend) | Django REST API and core logic |
| [`Maxtera-frontend`](https://github.com/Maxters-ltd/Maxtera-frontend) | Next.js web client |
| [`Maxtera-docs`](https://github.com/Maxters-ltd/Maxtera-docs) | Documentation, architecture, and guidelines |

---

## ⚙️ Development Setup

1. **Fork** the relevant repository.  
2. **Clone** your fork:
   ```bash
   git clone https://github.com/<your-username>/Maxtera-backend.git

3. Create a feature branch:

git checkout -b feature/add-wallet-endpoint


4. Make your changes.


5. Run tests locally.


6. Commit with a clear message:

git commit -m "feat(wallet): added withdrawal API"


7. Push and create a Pull Request to the dev branch.




---

🏗️ Branch Naming Convention

Branch Type	Example

Main branch	main
Development branch	dev
New feature	feature/add-wallet-api
Bug fix	fix/login-error
Documentation	docs/update-readme
Hotfix	hotfix/patch-deploy



---

🧠 Commit Message Format

Follow the Conventional Commits pattern:

<type>(scope): <short description>

Examples:

feat(auth): add OTP verification

fix(api): resolve 500 error on payment

docs: update contribution guide


Allowed types: feat, fix, docs, style, refactor, test, chore, perf


---

🧪 Code Quality Rules

All Python code must follow PEP8.

Use black or isort for formatting (backend).

All TypeScript code must pass ESLint (frontend).

Every new function or component must include basic tests.



---

🧰 Tools & Dependencies

Area	Tools

Backend	Django, DRF, PostgreSQL
Frontend	Next.js, TypeScript, TailwindCSS
API Integration	OnePipe, vendor APIs
Version Control	Git + GitHub
Collaboration	Issues + Pull Requests



---

🚦 Pull Request Guidelines

✅ Open PRs only to the dev branch (never directly to main).
✅ Add clear description of what was changed and why.
✅ Include screenshots or API response examples if UI or endpoint-related.
✅ Assign reviewers (Admin or Lead Dev).
✅ Wait for review before merging.


---

📦 Release Workflow

1. Developers merge feature branches → dev


2. QA verifies changes on staging


3. Once approved → merged into main


4. Version tag created:
Example → v1.2.0




---

🧑‍🔬 Testing Standards

Backend → use pytest for unit and integration tests

Frontend → use Jest or React Testing Library

Environment variables should be mocked in tests



---

🧍 Code of Conduct

Be respectful, transparent, and constructive.
No spam commits, untested PRs, or unrelated issues.


---

🧾 License

This project is licensed under the MIT License.
By contributing, you agree that your contributions will be under the same license.


---

© 2025 MAXTERS LTD — All rights reserved.

---