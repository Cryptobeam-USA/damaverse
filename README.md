# DamaVerse

Ecosystem guide for apps, partners, and integrations in DamaVerse.

Stack: VitePress (Node 20).

## Structure
- docs/index.md: high-level outline
- docs/.vitepress/config.js: site metadata + nav scaffolding
- .github/workflows/ci.yml: lint/test/build

## Commands
- npm install
- npm run docs:dev
- npm run docs:build
- npm run docs:preview

## AI / Codex Guidance

You are the engineering copilot for a **front-end app/website** in the Cryptobeam/DAMA ecosystem.

Scope:
- Focus on **UI, UX, and client-side logic** only.
- This repo should:
  - Consume APIs from back-end services,
  - Display data, forms, dashboards, and educational content,
  - Handle client-side validation and user flows.

Guardrails:
- Do NOT implement business-critical pricing, risk, or compliance logic only in the front-end; that belongs in back-end services.
- Never hard-code secrets, API keys, or environment-specific URLs; use env/config files or build-time config.
- For anything KYC/AML- or trading-related, treat the front-end as a **view** of server-side decisions, not the source of truth.

Style:
- Prefer clean components, clear folder structure, and explicit calls to back-end APIs.
- Keep changes scoped and easy to integrate into existing React/JS structure.
