# Omid Alighadr

**Backend & DevOps engineer** · Python · 5 years of experience

I build and operate backend services and automation: asynchronous Python services,
third-party API integrations, background job processing, and the Docker / CI tooling around them.

## Selected work

**[persian-cover-engine](https://github.com/omidalighadr/persian-cover-engine)** — Python library and CLI that
renders Persian (RTL) cover images with correct shaping, WCAG-checked palettes and a layout that stays inside
Instagram's profile-grid crop. Typed (`mypy --strict`), tested, CI on Python 3.10–3.13, Docker image.

**Samery** *(private)* — a single-user AI assistant on Telegram. It retrieves content from configured sources,
answers questions, analyses documents and generates images.

- ~17.6K lines of Python, 50+ commands, 9 background workers (job queue, scheduler, reminders, price alerts, …)
- Pluggable LLM layer: Gemini by default, any OpenAI-compatible endpoint, model fallback
- Reference checker that matches citations to a reference list and verifies them against CrossRef/DOI;
  "not found" is never reported as "fake"
- Runs as a managed service with a local Telegram Bot API server in Docker

The source is private; I'm happy to walk through the design.

## How I work

- Secrets live in environment files, never in code.
- Verify instead of guess wherever the data can be checked.
- Public code is typed, linted and tested.

## Skills

Focused on building and running Telegram bots.

- **Bot development:** Python · asyncio · python-telegram-bot · Telegram Bot API (including a self-hosted Bot API server)
- **Integrations:** httpx · REST APIs · LLM APIs (Gemini / OpenAI-compatible) · CrossRef
- **Data & jobs:** SQLite · background workers · schedulers
- **Deployment:** Docker · GitHub Actions · Linux / macOS service management
- **Quality:** pytest · Ruff · mypy
