# Savings Pro — Base44 Dev Environment

## What this is
A single static `index.html` marketing/landing page ("Savings Pro"). No build step, no backend, no dependencies, no external services, no secrets.

## Running it
```
docker compose -f docker-compose.base44.yml up -d
```
Serves `index.html` via `nginx:alpine` on host port 3000, bind-mounted read-only so edits appear on browser refresh.

## Verifying
- `curl -sf http://localhost:3000/` returns the HTML page (title "Savings Pro").
- The login/signup modals are demo-only (no real auth backend).

## Notes
- No live-reload dev server; nginx serves the file directly. Call `reload_preview` after edits to refresh the preview iframe.
