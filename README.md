<h1 align="center">Samuel Ng'ang'a</h1>

<p align="center">
  <b>Full-stack developer · Nairobi, Kenya 🇰🇪</b><br/>
  <i>I build web apps, data dashboards and AI-powered tools, and I care about security from day one.</i>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&center=true&width=560&lines=Full-stack+Developer;Team+Leader;Moringa+School+graduate;Shipping+real+software+as+a+dev+intern;Security-minded+by+default;Open+to+junior+full-stack+roles" alt="Typing SVG" />
</p>

<p align="center">
  <a href="https://portfolio-iota-three.vercel.app/"><img src="https://img.shields.io/badge/-Portfolio-000000?logo=vercel&logoColor=white&style=for-the-badge" alt="Portfolio" /></a>
  <a href="https://linkedin.com/in/samuel-ng-ang-a-065471391"><img src="https://img.shields.io/badge/-LinkedIn-0A66C2?logo=linkedin&logoColor=white&style=for-the-badge" alt="LinkedIn" /></a>
  <img src="https://img.shields.io/badge/-Moringa%20School%20Graduate-F15A24?style=for-the-badge" alt="Moringa School graduate" />
  <a href="mailto:your-email@example.com"><img src="https://img.shields.io/badge/-Email-D14836?logo=gmail&logoColor=white&style=for-the-badge" alt="Email" /></a>
</p>

---

## 👋 About

I'm a software developer who started coding in **September 2024** and graduated from **Moringa School** (Software Development) in 2026. I'm currently a **software development intern** on an enterprise platform, and I take on **freelance** projects under **GaryTech**.

I learn by building, and I like understanding a system layer by layer, from the database to the UI, before I change it.

## 🎓 Education

**Moringa School, Nairobi · Software Development** · Graduated 2026

An intensive, project-based program covering the full stack:

- **Frontend:** HTML, CSS, JavaScript, React
- **Backend:** Python, Flask, REST API design, authentication
- **Databases:** SQL, data modelling and ORMs
- **Practices:** Git and GitHub workflows, testing, pair programming, Agile delivery
- **Capstone and group projects:** built and shipped full-stack apps in teams under deadlines

## 🧭 Leadership and teamwork

- **Team leader** on team projects: I split the work into Jira stories, ran stand-ups and sprint planning, reviewed pull requests and kept delivery on schedule
- **Design to code:** I turn Figma wireframes and prototypes into responsive, pixel-accurate UIs, and I mock up features in Figma before building them
- **Agile/Scrum:** I work in sprints with backlog grooming, estimates and retros, tracked in Jira
- **Mentoring:** I help teammates debug, walk them through Git workflows and code-review etiquette, and write docs so others can onboard fast

## 📊 At a glance

| | |
|---|---|
| 🧑‍💻 Commits to my main project | **365+** in under 4 months |
| 🔀 Pull requests merged | **145+**, every change goes through a PR and CI |
| 🧪 Backend test suites | **22** Jest + Supertest suites on an in-memory MongoDB |
| 🗂️ Data models / API modules | **35** Mongoose models · **38** Express route modules |
| 👥 User roles supported | **9**, from customer to super admin |
| 📈 GitHub contributions (last year) | **899** |

## 💼 What I'm working on

### Enterprise platform (internship)

- Building **analytics dashboards** in **Apache Superset**, backed by SQL views on a layered data warehouse (raw → ETL → analytics-ready)
- Shipping features in a large multi-tenant **Java · Spring MVC · MyBatis · PostgreSQL** codebase through a build-and-deploy pipeline
- Learning the end-to-end business workflow so features fit how customers actually operate

### E-commerce platform *(private repo, code walkthrough on request)*

A full-stack store **plus a full back office**, built solo. **v1.0.0 released**; development continues with a PR-based workflow.

**Storefront**
- Browse, search, cart, checkout, order history and **installment plans**
- **Payments:** M-Pesa STK Push, PayPal and Stripe
- **Installable PWA** frontend (React 19 + Vite + Tailwind)

**Back office**

| Area | What I built |
|---|---|
| 🏭 ERP | Suppliers, purchase orders, worker management and worker payouts |
| 🚚 Delivery | Driver roster, task assignment, **live GPS tracking over Socket.IO**, delivery reviews and complaints |
| 🎟️ Promotions | Coupon and discount engine with rules and limits |
| ⭐ Retention | Loyalty points for repeat customers |
| 📦 Inventory | Low-stock alerts for admins, back-in-stock alerts for customers |
| 👔 HR | Three-level staff hierarchy with HR as the central authority |
| 🎫 Ticketing | Bug/feature tracker with a Super Admin → Middle Admin → Developer assignment chain |
| 📑 Reporting | Multi-stage report chains (Staff → Middle Admin → HR → Super Admin) with downloadable reports |
| 📈 Analytics | Revenue and operations dashboards (Recharts) |
| 🩺 Reliability | Server-health monitor with incident tracking |

**Security**
- JWT auth, **email OTP verification**, Google Sign-In, rolling sessions and idle timeouts
- Helmet, rate limiting, NoSQL-injection sanitising, CSRF/CORS configuration
- **Security dashboard** with risk signals, account flags, temporary suspensions and an immutable moderation audit log
- **Attack simulations** (brute force, impossible travel) to prove the defences actually trigger, plus security regression tests

**Engineering**
- Event-driven architecture with real-time notifications over Socket.IO
- **CI/CD on GitHub Actions:** Trivy vulnerability scan → `npm audit` → Jest with coverage → frontend lint and build → deploy
- **Docker** images for backend and frontend, plus a Docker Compose stack for local dev
- Dependabot keeps dependencies current, and every bump goes through CI

### 🐛 Bugs I've hunted down

- **Silent CI timeouts after a MongoDB driver upgrade.** Every test suite started timing out, which looked like a network or database problem. The real cause: driver 7.6 loads a module via dynamic `import()`, which fails silently inside Jest's CommonJS sandbox. Fixed by running Jest with `--experimental-vm-modules`.
- **Migrating to Mongoose 9.** Old `pre('save', next)` hooks crashed, and aggregation-pipeline updates threw errors unless `{ updatePipeline: true }` was passed. One of those errors was being swallowed by a `try/catch` that only logged it. I found and fixed both.

## 📂 Public projects

| Project | What it is | Stack |
|---|---|---|
| [Jarvis-Ollama-version](https://github.com/devbysamcloudy/Jarvis-Ollama-version) | Local AI assistant powered by Ollama | Python, Ollama |
| [exp-system-generator-frontend](https://github.com/devbysamcloudy/exp-system-generator-frontend) | Frontend for the exp system generator | JavaScript |
| [exp-system-generator-backend](https://github.com/devbysamcloudy/exp-system-generator-backend) | Backend API for the exp system generator | Python |
| [Texas-Hold-em-game](https://github.com/devbysamcloudy/Texas-Hold-em-game) | Texas Hold'em card game | Python |

## 🛠 Tech stack

**Frontend**

![React](https://img.shields.io/badge/-React-61DAFB?logo=react&logoColor=black&style=for-the-badge)
![Vite](https://img.shields.io/badge/-Vite-646CFF?logo=vite&logoColor=white&style=for-the-badge)
![Tailwind](https://img.shields.io/badge/-Tailwind-06B6D4?logo=tailwindcss&logoColor=white&style=for-the-badge)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?logo=javascript&logoColor=black&style=for-the-badge)
![PWA](https://img.shields.io/badge/-PWA-5A0FC8?logo=pwa&logoColor=white&style=for-the-badge)

**Backend**

![Node.js](https://img.shields.io/badge/-Node.js-339933?logo=nodedotjs&logoColor=white&style=for-the-badge)
![Express](https://img.shields.io/badge/-Express-000000?logo=express&logoColor=white&style=for-the-badge)
![Socket.IO](https://img.shields.io/badge/-Socket.IO-010101?logo=socketdotio&logoColor=white&style=for-the-badge)
![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white&style=for-the-badge)
![Flask](https://img.shields.io/badge/-Flask-000000?logo=flask&logoColor=white&style=for-the-badge)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?logo=fastapi&logoColor=white&style=for-the-badge)
![Java](https://img.shields.io/badge/-Java-ED8B00?logo=openjdk&logoColor=white&style=for-the-badge)
![Spring](https://img.shields.io/badge/-Spring-6DB33F?logo=springboot&logoColor=white&style=for-the-badge)

**Databases and data**

![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?logo=postgresql&logoColor=white&style=for-the-badge)
![MySQL](https://img.shields.io/badge/-MySQL-4479A1?logo=mysql&logoColor=white&style=for-the-badge)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?logo=mongodb&logoColor=white&style=for-the-badge)
![Superset](https://img.shields.io/badge/-Apache%20Superset-20A6C9?logo=apachesuperset&logoColor=white&style=for-the-badge)

**Payments**

![M-Pesa](https://img.shields.io/badge/-M--Pesa-00A650?style=for-the-badge)
![Stripe](https://img.shields.io/badge/-Stripe-635BFF?logo=stripe&logoColor=white&style=for-the-badge)
![PayPal](https://img.shields.io/badge/-PayPal-00457C?logo=paypal&logoColor=white&style=for-the-badge)

**DevOps, testing and security**

![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white&style=for-the-badge)
![GitHub Actions](https://img.shields.io/badge/-GitHub%20Actions-2088FF?logo=githubactions&logoColor=white&style=for-the-badge)
![Jenkins](https://img.shields.io/badge/-Jenkins-D24939?logo=jenkins&logoColor=white&style=for-the-badge)
![Jest](https://img.shields.io/badge/-Jest-C21325?logo=jest&logoColor=white&style=for-the-badge)
![Trivy](https://img.shields.io/badge/-Trivy-1904DA?logo=aqua&logoColor=white&style=for-the-badge)
![Git](https://img.shields.io/badge/-Git-F05032?logo=git&logoColor=white&style=for-the-badge)
![Linux](https://img.shields.io/badge/-Linux-FCC624?logo=linux&logoColor=black&style=for-the-badge)

**Design and collaboration**

![Figma](https://img.shields.io/badge/-Figma-F24E1E?logo=figma&logoColor=white&style=for-the-badge)
![Jira](https://img.shields.io/badge/-Jira-0052CC?logo=jira&logoColor=white&style=for-the-badge)
![Postman](https://img.shields.io/badge/-Postman-FF6C37?logo=postman&logoColor=white&style=for-the-badge)
![Scrum](https://img.shields.io/badge/-Agile%20%2F%20Scrum-6E40C9?style=for-the-badge)

**Also explored:** Phaser 3 (game dev), XGBoost (ML), OpenAI and Ollama integrations

## 📈 GitHub stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=devbysamcloudy&show_icons=true&count_private=true&theme=tokyonight&hide_border=true" alt="GitHub stats" />
  <img height="165" src="https://streak-stats.demolab.com?user=devbysamcloudy&theme=tokyonight&hide_border=true" alt="GitHub streak" />
</p>

## 🤝 Let's work together

I'm open to **junior full-stack roles** and **freelance projects**. If you need someone who can lead a team, turn a Figma design into a shipped feature, debug patiently and keep learning, let's talk.

📫 [Email](mailto:your-email@example.com) · [LinkedIn](https://linkedin.com/in/samuel-ng-ang-a-065471391) · [Portfolio](https://portfolio-iota-three.vercel.app/)
