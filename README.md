# Back4app xray container

Minimal container that runs xray with a VLESS + WebSocket inbound. TLS is
terminated by the platform edge; xray itself listens in plaintext on `$PORT`.

Set these environment variables in the Back4app dashboard (never commit
real values here):

- `UUID` — the VLESS user id (generate a fresh UUIDv4 per deploy)
- `WS_PATH` — the WebSocket path, e.g. `/ws`
- `PORT` — set by the platform
