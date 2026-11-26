# Security

Acroblade is a static site: no server code, no database, no accounts, no stored personal data.

- Pages ship a strict Content-Security-Policy (no plugins, no framing, no form posts, scripts only from this site and the PeerJS CDN used by the game).
- Multiplayer uses WebRTC / secure WebSocket (wss) only. The matchmaking server limits message size, rate, rooms and (optionally) allowed origins.
- The Windows installer is unsigned: check its SHA-256 against `SHA256.txt` before running.
- Never enter passwords or personal info in the game. Acroblade never asks for them.

Report a vulnerability: open a private "Security advisory" in this repository (Security tab).
