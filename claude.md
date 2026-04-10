# Project Constitution: Plumbing Landing Page

## Data Schemas (gemini.md)
### Repository Configuration
- `name`: "Plumbing Landing page"
- `visibility`: [To be confirmed - Public/Private]
- `remote_url`: [To be generated]

## Behavioral Rules
1. **Deterministic Execution:** Use the 3-layer architecture for all deployment steps.
2. **Reliability First:** Verify remote connection before pushing.
3. **Clean Payload:** Use `.gitignore` to avoid pushing environmental or temporary files.

## Architectural Invariants
- Core logic in `Plumbing project/`.
- Local ephemeral files in `.tmp/`.
- SOPs in `architecture/`.
