# Hi, I’m Paul

I turn everyday needs into practical web applications, with a focus on clear interfaces, useful features and deployable products.

I’m looking for opportunities where I can contribute to digital products and keep developing my technical skills. My personal projects combine product exploration, hands-on iteration and AI-assisted development.

## Featured project — Sightline

**A Counter-Strike 2 demo analysis platform, in production for my esports team.**

Import match demos and get a 2D and 3D replay, team and player analytics, scouting reports and an AI assistant that answers questions about the team's own matches.

[Explore the project and source code →](https://github.com/BoooJ/sightline)

![Sightline 3D replay on Dust2](https://raw.githubusercontent.com/BoooJ/sightline/main/docs/screenshots/replay-3d.jpg)

- FastAPI (Python) backend that parses demos into 32 Hz replays, SQLite with migrations, Docker deployment.
- React and TypeScript interface, with a WebGL (three.js) 3D replay: maps exported from the game, animated player models and ragdoll physics computed in a Web Worker.
- AI assistant (Claude or Gemini) grounded on the team's match data.
- Integrations: n8n automations, a Chrome extension, a TeamSpeak plugin in C++ and a mobile app.
- 1,400+ automated tests, run in CI on every push.

**My role:** defining the product with my team, prioritizing features and directing the work with AI coding assistance (specs, test-first plans, independent reviews), then deploying and running it in production. The repository explains the architecture and how it was built.

## Featured project — Mangathèque

**A self-hosted manga reader for my household, installable on iPhone, iPad and PC.**

Search a public manga catalogue, read in manga (right-to-left), page or vertical-scroll mode, download chapters to read offline in airplane mode, and export them as CBZ or PDF. Each family member has their own account and their own downloads.

*Private repository — I'm happy to walk through the code and architecture on request.*

- SvelteKit 2 and Svelte 5 in strict TypeScript, Node 24 and SQLite, packaged as a Docker image and served over HTTPS behind Caddy.
- Deployed on a VPS that already runs another production app: verified backups, config validation before reload and a before/after state check, so that app never went down.
- A server-side proxy that plays fair with the content API: rate limiters, automatic pause when asked to slow down, a circuit breaker and a size-capped image cache.
- Installable PWA: service worker, per-user offline downloads in IndexedDB that resume where they stopped.
- CBZ and PDF exports streamed page by page, to stay within a 512 MB memory limit.
- Security by default: scrypt password hashing, `__Host-` session cookies, login rate limiting and a strict Content Security Policy.
- About 600 unit tests (Vitest) and end-to-end browser tests (Playwright) against a fake API server, so no test ever hits the real service.

**My role:** defining the need and taking every product decision, then directing an AI-driven workflow end to end: a design document checked by six independent AI reviewers, a shared contract and a 14-task test-first plan (about 350 steps), one coding agent per task followed by an independent review agent, and a step-by-step production deployment run from my own machine, with the server keys never leaving it.

## Featured project — Caderno

**A personal Portuguese-learning notebook, inspired by life in Brazil.**

Translate between French and Brazilian Portuguese, save useful vocabulary, add personal notes and look up verb conjugations from a mobile-friendly interface.

[Explore the project and source code →](https://github.com/BoooJ/caderno)

![Caderno desktop interface](https://raw.githubusercontent.com/BoooJ/caderno/main/docs/images/desktop.png)

- React and TypeScript interface, designed for mobile and desktop.
- Express API and persistent SQLite storage.
- 60 built-in verbs, custom verb imports and notebook export.
- PWA with offline reading of previously loaded content.
- Automated tests and a Docker deployment setup.

**My role:** defining the problem, shaping the product, prioritizing features and iterating on the result with AI coding assistance. The repository explains the implementation, trade-offs and current limitations.

## What I value

- Building around a real user need.
- Keeping interfaces understandable and comfortable on a phone.
- Making personal data portable.
- Documenting what works, what is tested and what still needs improvement.
