# Definition of Done

## Phase 0 — Repo bootstrap (this PR)

- [x] `ima-jin/jin` exists, **public**.
- [x] Scaffold: README (apps-table row, port, "fork this to build a vertical" note, namespace note), `.env.example`, DoD doc, LICENSE, `.gitignore`, CI stub.
- [x] Port assigned + documented: dev `3402` / prod `7402` (next free client pair).
- [ ] CI green on first PR.

## Phase 1 — MVP: "prove identity → establish presence"

- [ ] **DID auth** — existing sovereign login handshake (challenge → sign → verify → session). Human authenticates as their own DID.
- [ ] **Idle presence surface** — post-auth, the presence glyph (spinning logo), idle. Framed as the first object in the scene.
- [ ] **Shell/domain seam documented** — the interface where a vertical's intent vocabulary plugs in, real even in the MVP.
- [ ] **Security invariant enforced** — unauthed sees static DID-login only; agent backend connects only post-session, server-layer gate (not client redirect).

**MVP DoD:** a human authenticates with their DID → lands on a live idle presence surface on dev; the shell/domain seam is a documented interface.

## Phase 2 — Roadmap articulated in this repo

- [ ] v0.1 action/confirm loop (source: imajin-ai #1369, #1366-line, #1293).
- [ ] Connectors Jin orchestrates (imajin-ai #1228, #1373).
- [ ] Forkability-hardening thread (keep the shell/domain seam clean + conformant).
- [ ] Intention-inference vision (imajin-ai #1198, #1211–#1216).
- [ ] UI schema / object model (imajin-ai #1386) — rehome here.
- [ ] OSC ambient fan-out (imajin-ai #1385) — rehome here.

## Phase 3 — Migration / cleanup

- [ ] App-native imajin-ai issues (#1198, #1211–#1216, #1369) move or close → `ima-jin/jin` equivalents.
- [ ] Platform/kernel/connector issues (#1228, #1366-line, #1373) STAY on imajin-ai (Jin consumes them).
- [ ] Pointer on app-related imajin-ai issues: "app work now tracked in ima-jin/jin."
