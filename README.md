<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/header/banner-dark.svg">
  <img src="./assets/header/banner-light.svg" width="100%" alt="Paul Morel, AI engineer with a cybersecurity background. ISEP 2026, open to opportunities. From a real need to a release: spec, AI agents, review.">
</picture>

<p align="center">
  <a href="https://boooj.github.io/en/"><img alt="Portfolio: boooj.github.io" src="https://img.shields.io/badge/Portfolio-boooj.github.io-1d6b58?style=flat-square&logo=githubpages&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/morel-paul"><img alt="LinkedIn: morel-paul" src="https://img.shields.io/badge/LinkedIn-morel--paul-0A66C2?style=flat-square"></a>
  <a href="https://boooj.github.io/en/#contact"><img alt="Open to opportunities: contact" src="https://img.shields.io/badge/Open_to-opportunities-2ea043?style=flat-square"></a>
  <img alt="English C1" src="https://img.shields.io/badge/English-C1-59636e?style=flat-square">
</p>

## 👋 Hi, I’m Paul

**AI engineer with a cybersecurity background.** I turn everyday needs into practical web applications, with a focus on clear interfaces, useful features and deployable products. My personal projects combine product exploration, hands-on iteration and AI-assisted development.

- 🎓 Cybersecurity engineering at **ISEP**, Paris (class of 2026), with an Erasmus semester at ISCTE Lisbon in machine learning and computer science.
- 💼 Final-year internship at **Good iD**, a Google partner integrator: two internal tools in production, for customer support and inventory.
- 📦 Earlier internship at **The Lost Recordings**: a Node.js service that requests La Poste shipping slips as soon as an order is ready.
- 🤖 I work with AI coding agents (Claude Code, Codex): I shape the product and the specs, they write the code, I review, test and ship it.
- 🔎 Looking for an AI engineering, software, cloud or cybersecurity role, in France or abroad.

## ✨ Featured projects

- 🎯 **[Sightline](#-sightline)**: Counter-Strike 2 demo analysis platform<br><sub>🟢 In production for my esports team · 📂 public code</sub>
- 📱 **[Sightline mobile](#-sightline-mobile)**: its pocket companion, on the web and Android<br><sub>🟢 Live · 📂 public code</sub>
- 📚 **[Mangathèque](#-mangathèque)**: self-hosted manga reader for my household<br><sub>🟢 Live · 🔒 private code</sub>
- 📒 **[Caderno](#-caderno)**: Portuguese-learning notebook<br><sub>🟢 Live, password access · 📂 public code</sub>
- 🛒 **[AI-built e-commerce shops](#-ai-built-e-commerce-shops)**: Shopify shops coded and illustrated by AI<br><sub>🟢 First paid orders in Sept. 2026 · 🔒 private</sub>
- 🚧 **[Up next: CS2 training servers](#-upcoming--cs2-training-servers-for-my-team)**: on-demand practice servers for my team, the training side of Sightline<br><sub>🟡 In planning, November 2026</sub>

### 🎯 Sightline

**A Counter-Strike 2 demo analysis platform, in production for my esports team.**

Import match demos and get a 2D and 3D replay, team and player analytics, scouting reports and an AI assistant that answers questions about the team's own matches.

🔗 [Explore the project and source code →](https://github.com/BoooJ/sightline)

![Sightline 3D replay on Dust2](https://raw.githubusercontent.com/BoooJ/sightline/main/docs/screenshots/replay-3d.jpg)

- ⚙️ FastAPI (Python) backend that parses demos into 32 Hz replays, SQLite with migrations, Docker deployment.
- 🖥️ React and TypeScript interface, with a WebGL (three.js) 3D replay: maps exported from the game, animated player models and ragdoll physics computed in a Web Worker.
- 🤖 AI assistant (Claude or Gemini) grounded on the team's match data.
- 🔌 Integrations: n8n automations, a Chrome extension, a TeamSpeak plugin in C++ and a mobile app.
- ✅ 1,400+ automated tests, run in CI on every push.

🧭 **My role:** defining the product with my team, prioritizing features and directing the work with AI coding assistance (specs, test-first plans, independent reviews), then deploying and running it in production. The repository explains the architecture and how it was built.

### 📱 Sightline mobile

**The pocket companion to Sightline, designed around the moments a player actually picks up their phone.**

Before the match, prepare for the opponent; right after it, read your own debrief; during practice, keep a map's grenades in view next to the keyboard; over time, follow your progress. Same accounts and same data as the web app, plus a notebook for the team's strategies and personal notes.

🔗 [Explore the source code →](https://github.com/BoooJ/sightline/tree/main/mobile) (the `mobile/` folder of the Sightline repository)

<p>
  <img src="./assets/sightline-mobile/aujourdhui.webp" width="180" alt="Today screen: a review-ready card for the last match, a prep card for the next opponent with the maps, recent form and a grenade shortcut.">
  <img src="./assets/sightline-mobile/preparation.webp" width="180" alt="Opponent prep on Inferno: stat tiles and key points, each with a reliability indicator.">
  <img src="./assets/sightline-mobile/bilan.webp" width="180" alt="Match review: rating, K-D, ADR and KAST against the player's average, then the three costliest deaths.">
  <img src="./assets/sightline-mobile/lineup.webp" width="180" alt="Lineup sheet: zoomed radar with the trajectory, vertical and horizontal angles and a copy-command button.">
</p>

<sub>Demo mode, iPhone format: public professional matches embedded in the app, no account needed.</sub>

- 🧱 Expo SDK 58, React Native and expo-router in TypeScript, with TanStack Query and Reanimated.
- 📲 One codebase, two free channels: an installable web app served by the Sightline backend, and an Android APK built in the cloud with EAS. No app-store fees.
- ⏱️ A home screen that knows what moment it is: the next match comes first with a countdown, and a debrief less than 24 hours old goes ahead of everything else.
- 📊 Opponent prep where every figure shows its reliability and sample size, so two rounds are never presented as a trend.
- 📐 Grenade lineups made for a phone propped next to the keyboard: the screen stays on, the angles are large and the practice command copies in one tap.
- 🗓️ Upcoming matches with the opponent's likely maps, shown in each team member's local time.
- ♿ Accessible by design: screen-reader labels, a one-sentence summary for every chart, and simple fades instead of motion when the user asks for less animation.
- 🧪 Unit tests on the app's logic (Vitest), and a demo that weighs about 400 KB of embedded data.

🧭 **My role:** product and UI/UX design (moments of use, screens, visual system), the specification, verification and release. The code is written by AI agents (Claude Code); the first version went live in two days.

### 📚 Mangathèque

**A self-hosted manga reader for my household, installable on iPhone, iPad and PC.**

Search a public manga catalogue, read in manga (right-to-left), page or vertical-scroll mode, download chapters to read offline in airplane mode, and export them as CBZ or PDF. Each family member has their own account and their own downloads.

🔒 *Private repository — I'm happy to walk through the code and architecture on request.*

- 🧱 SvelteKit 2 and Svelte 5 in strict TypeScript, Node 24 and SQLite, packaged as a Docker image and served over HTTPS behind Caddy.
- 🛡️ Deployed on a VPS that already runs another production app: verified backups, config validation before reload and a before/after state check, so that app never went down.
- 🚦 A server-side proxy that plays fair with the content API: rate limiters, automatic pause when asked to slow down, a circuit breaker and a size-capped image cache.
- 📲 Installable PWA: service worker, per-user offline downloads in IndexedDB that resume where they stopped.
- 📄 CBZ and PDF exports streamed page by page, to stay within a 512 MB memory limit.
- 🔐 Security by default: scrypt password hashing, `__Host-` session cookies, login rate limiting and a strict Content Security Policy.
- 🧪 About 600 unit tests (Vitest) and end-to-end browser tests (Playwright) against a fake API server, so no test ever hits the real service.

🧭 **My role:** defining the need and taking every product decision, then directing an AI-driven workflow end to end: a design document checked by six independent AI reviewers, a shared contract and a 14-task test-first plan (about 350 steps), one coding agent per task followed by an independent review agent, and a step-by-step production deployment run from my own machine, with the server keys never leaving it.

### 📒 Caderno

**A personal Portuguese-learning notebook, inspired by life in Brazil.**

Translate between French and Brazilian Portuguese, save useful vocabulary, add personal notes and look up verb conjugations from a mobile-friendly interface.

🔗 [Explore the project and source code →](https://github.com/BoooJ/caderno)

![Caderno desktop interface](https://raw.githubusercontent.com/BoooJ/caderno/main/docs/images/desktop.png)

- 🖥️ React and TypeScript interface, designed for mobile and desktop.
- 🗄️ Express API and persistent SQLite storage.
- 📖 60 built-in verbs, custom verb imports and notebook export.
- 📲 PWA with offline reading of previously loaded content.
- 🧪 Automated tests and a Docker deployment setup.

🧭 **My role:** defining the problem, shaping the product, prioritizing features and iterating on the result with AI coding assistance. The repository explains the implementation, trade-offs and current limitations.

### 🛒 AI-built e-commerce shops

**Shopify dropshipping shops whose code and visuals are produced by AI, with every release still under my control.**

Since August 2026 I have been launching Shopify shops on small European markets, in languages I do not always speak. AI coding agents write the theme code and image and video models produce the ad visuals. I decide what gets built, review and test every release, and run the shops.

🔒 *Private work — products, suppliers, pricing and the marketing playbook are intentionally left out. The diagrams below show how the work is organised and checked.*

🟩 In green, the steps I never delegate.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/ecommerce/agents-dark.svg">
  <img src="./assets/ecommerce/agents-light.svg" width="600" alt="Who does what: I set products, markets, pricing and specs; coding agents write the theme code and image and video models make the ad visuals; I review and approve the code and select and edit the visuals, or send them back; credentials, bank details and identity are never delegated.">
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/ecommerce/release-loop-dark.svg">
  <img src="./assets/ecommerce/release-loop-light.svg" width="600" alt="The release loop: describe the change, agent writes the code, restore point, my review, publish one file at a time, live test; anything off goes back to the start, and every batch is logged with the rollback command.">
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/ecommerce/verification-dark.svg">
  <img src="./assets/ecommerce/verification-light.svg" width="600" alt="How changes are verified: my tests and pre-launch audits surface defects, an agent codes the fix, I validate it on the live shop, and a rule is written down when the defect could come back.">
</picture>

- 📜 Working rules written for the agents: nothing goes live without my approval; one file at a time, so the shop settings are never overwritten; a full copy of the live theme before every batch; nothing private in the files served; credentials, bank details and identity handled by me alone.
- 🔍 Pre-launch audit: 29 URLs returning the expected 200, 301 and 404 responses, 293 resources loaded across three pages without a single 404, and no third-party scripts.
- ⚡ Lighthouse mobile, in lab conditions: accessibility 100, SEO 100, performance between 52 and 76.
- 🌍 Domains, payments and translated versions live in September 2026, and the first real, paid orders the same month.

🧭 **My role:** choosing products, markets and pricing; writing the specifications and arbitrating trade-offs; setting up domains, payments and shop settings; testing every release; art-directing the ads, generated by AI and then edited. The code is written by AI agents (Claude Code, Codex).

## 🚧 Upcoming — CS2 training servers for my team

**On-demand Counter-Strike 2 practice servers with training modes, built for my esports team: the training side of Sightline.**

Sightline shows the team what went wrong in a match; this project gives each player a private server to work on it. From a web dashboard, a player picks a mode and a map, starts a server and joins in one click, and the session results come back to the dashboard.

🗓️ *In planning: specification and observation phase, November 2026.*

- 🧩 Training modes driven by one scenario engine (spawns, bot behaviour, weapons, reset and win conditions) and per-map data files, instead of one plugin per mode: aim, prefire, retakes, spray transfer, AWP and grenade practice.
- 🔌 Game-server plugins in C# on CounterStrikeSharp (Metamod), talking to the web backend for access control and session stats.
- 🖥️ Web dashboard with Steam sign-in, a team allowlist and live server status; servers start on demand and stop when idle to keep hosting costs low.
- 🏗️ Built first against a local CS2 dedicated server; team hosting chosen once the first modes are measured (managed CS2 hosting or a dedicated machine).
- ➡️ Next step after that: link Sightline's match analysis to recommended training modes.

🧭 **My role:** studying how existing training platforms behave from a player's point of view, writing the specification for each mode, choosing the hosting, and directing the AI-assisted build and tests.

## 🧰 What these projects are built with

🤖 **AI** &nbsp; ![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=claude&logoColor=white) ![Codex](https://img.shields.io/badge/Codex-1f2328?style=flat-square) ![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)

🖥️ **Front end** &nbsp; ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![three.js](https://img.shields.io/badge/three.js-1f2328?style=flat-square&logo=threedotjs&logoColor=white) ![SvelteKit](https://img.shields.io/badge/SvelteKit-FF3E00?style=flat-square&logo=svelte&logoColor=white) ![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white) ![PWA](https://img.shields.io/badge/PWA-5A0FC8?style=flat-square&logo=pwa&logoColor=white)

⚙️ **Back end and data** &nbsp; ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white) ![Express](https://img.shields.io/badge/Express-1f2328?style=flat-square&logo=express&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)

🚀 **Ship and test** &nbsp; ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Caddy](https://img.shields.io/badge/Caddy-1F88C0?style=flat-square&logo=caddy&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white) ![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square)

🔌 **Automation and commerce** &nbsp; ![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white) ![Google Apps Script](https://img.shields.io/badge/Google_Apps_Script-4285F4?style=flat-square&logo=googleappsscript&logoColor=white) ![Shopify](https://img.shields.io/badge/Shopify-7AB55C?style=flat-square&logo=shopify&logoColor=white)

## 💡 What I value

- 🎯 Building around a real user need.
- 📱 Keeping interfaces understandable and comfortable on a phone.
- 📦 Making personal data portable.
- 📝 Documenting what works, what is tested and what still needs improvement.

## 📫 Get in touch

The best place to start is my [portfolio](https://boooj.github.io/en/): each project page sets out the context and my exact role, and my internship tools come with a mock-up you can try. You can also find me on [LinkedIn](https://www.linkedin.com/in/morel-paul).
