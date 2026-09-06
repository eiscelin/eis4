# Savings Pro

Static single-page marketing site. The entire app is `index.html` (no build step, no backend, no dependencies).

## Running
`docker compose -f docker-compose.base44.yml up -d` — serves `index.html` via nginx on host port 3000.

## Notes
- No credentials or external services required.
- Forms (login/signup) are demo-only stubs; they show a notice on submit and do not call any backend.
