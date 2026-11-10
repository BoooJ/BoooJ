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
