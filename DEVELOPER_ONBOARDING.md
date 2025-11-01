# 👩‍💻 Maxtera Developer Onboarding Guide
Welcome to **Maxtera**, a fintech platform by **MAXTERS LTD** — empowering users with financial freedom.  
This guide helps you set up your local development environment, understand the project structure, and start contributing confidently.

---

## 🧩 1. Overview
Maxtera consists of two major codebases:

| Component | Tech Stack | Repository |
|------------|-------------|-------------|
| Backend API | Django + DRF + PostgreSQL | [maxtera-backend](https://github.com/maxters-ltd/maxtera-backend) |
| Frontend UI | Next.js + TypeScript + TailwindCSS | [maxtera-frontend](https://github.com/maxters-ltd/maxtera-frontend) |
| Documentation | Markdown + GitHub | [maxtera-docs](https://github.com/maxters-ltd/maxtera-docs) |

---

## ⚙️ 2. Prerequisites
Ensure you have the following installed on your system:

### For Backend
- Python 3.10+
- pip / pipenv / poetry
- PostgreSQL
- Git
- Docker (optional, for containerization)
- Postman (for API testing)

### For Frontend
- Node.js 18+
- npm or yarn
- Git
- Vercel CLI (optional for deployment preview)

---

## 🪜 3. Setup Instructions

### Backend Setup
```bash
# Clone repo
git clone https://github.com/maxters-ltd/maxtera-backend.git
cd maxtera-backend

# Create virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Setup environment
cp .env.example .env
# Edit the .env file and add your credentials (DB, SECRET_KEY, etc.)

# Apply migrations
python manage.py migrate

# Run server
python manage.py runserver

Backend runs at:
👉 http://127.0.0.1:8000


---

Frontend Setup

# Clone repo
git clone https://github.com/maxters-ltd/maxtera-frontend.git
cd maxtera-frontend

# Install dependencies
npm install

# Setup environment
cp .env.example .env
# Add API base URL:
# NEXT_PUBLIC_API_BASE_URL=http://127.0.0.1:8000

# Run the app
npm run dev

Frontend runs at:
👉 http://localhost:3000


---

🧠 4. Project Structure (Overview)

Each repo includes:

README.md → Quick setup guide

CONTRIBUTING.md → How to contribute safely

ROADMAP.md → Current project status & upcoming milestones

.env.example → Example environment variables



---

🌱 5. Branching Rules

We follow a Git branching model for safety and clarity:

Branch	Purpose

main	Stable production-ready code
develop	Integration branch for latest tested features
feature/*	New features in progress (e.g., feature/wallet-system)
bugfix/*	For fixing bugs
hotfix/*	Urgent patches after deployment


Example

git checkout -b feature/add-onpipe-integration
# After coding
git push origin feature/add-onpipe-integration


---

✅ 6. Code Standards

Python (Backend)

Follow PEP8 style guide

Use descriptive variable names

Include docstrings for all public methods

Keep functions <50 lines


TypeScript (Frontend)

Use ESLint + Prettier

Prefer functional components + hooks

Keep components modular and reusable

CSS handled via Tailwind classes



---

🧪 7. Testing

Backend

python manage.py test

Frontend

npm test


---

🧩 8. Collaboration Workflow

1. Fork the repo and create your own branch.


2. Implement your changes.


3. Test thoroughly.


4. Open a Pull Request (PR) to the develop branch.


5. PRs are reviewed before merging to main.




---

🧭 9. Communication

All collaboration is tracked via:

GitHub Issues — For tasks and bugs

GitHub Projects — For roadmap tracking

README / ROADMAP / DOCS — Always up to date



---

🤝 10. Welcome Aboard

You’re officially part of the Maxtera Development Team 🎉
Build responsibly, test thoroughly, and push confidently!

> 💬 Contact: support@maxtera.ng
🌐 Website: https://maxtera.com



---