# MVP requirements

- Load an external JSON Schema with field descriptions and required fields.
- Collect multiple fields from free text, in any order, with natural follow-up questions.
- Persist session history and structured data; isolate sessions.
- Support explicit corrections; missing/unknown values must not be fabricated. Required unknown values remain incomplete unless schema permits them.
- Validate data independently of the LLM; ask for confirmation before dispatch; invalidate confirmation after changes.
- Dispatch confirmed valid data to a mock only, avoiding duplicate submissions.
- Demonstrate two schemas without changing core code: marketing onboarding and family tasks.
- Integrate official WhatsApp Cloud API after simulated conversation works; verify webhook authenticity and deduplicate events.
- Out of scope: dashboard, billing, multi-tenancy, workflow designer, real business backend.
