# Architecture

WhatsApp adapter (later) -> conversation service -> LLM adapter -> schema validation and session persistence -> mock destination.

The service receives a session ID, message and externally supplied JSON Schema. The LLM proposes extracted updates and a natural response based on history and current data. Application code validates updates, preserves prior values unless explicitly corrected, checks required fields, and requires explicit confirmation of the current data before dispatch. Never invent missing values. Keep state outside the model. No fixed question sequence. Use SQLite locally; choose durable storage before Cloud Run deployment. Start with simulated messages and a fake LLM for tests. Real LLM provider configurable via environment. No real business integrations.
