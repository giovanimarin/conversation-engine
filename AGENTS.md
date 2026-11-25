# Development guidelines

Build the smallest functional MVP. Use Python, FastAPI, pytest, JSON Schema and SQLite for local development. Keep domain logic independent of WhatsApp, LLM and persistence. Prefer simple functions and cohesive classes; use dependency injection at external boundaries. Follow SOLID, DRY and KISS without speculative abstractions. Never commit secrets or real customer data. Use environment variables and synthetic fixtures. Run tests and lint before opening a PR; document limitations and do not claim unrun tests passed.
