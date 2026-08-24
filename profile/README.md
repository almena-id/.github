<h1 align="center">Almena Network</h1>

<p align="center">
  <strong>A decentralized network. No account, no central authority, no personal data.</strong>
</p>

<p align="center">
  <a href="https://almena.network">almena.network</a>
</p>

---

## What Almena is

A decentralized network, peer-to-peer over [iroh](https://github.com/n0-computer/iroh), and
**`almena`** is the application at the centre of it: one codebase — Tauri 2, Rust, React — for
Windows, macOS and Linux. **The application is the node**: there is no daemon beside it and no
API between the two, and the network is composed of the computers taking part in it.

Almena on a phone or a tablet is a **client** of that network rather than a node of it, and it
is built separately, in `client`.

A participant is a key generated on its own device. There is no account and no sign-up, and
nothing ever asks who is behind it.

A node belongs to the network whose configuration it read — `almena.network` for production,
`dev.almena.network` for development — published in DNS under that origin and signed, so a
zone the project runs hands a node a document and never a decision. The origin is the
operator's to replace, and a node that already knows peers never asks again.

> **Under construction.** No release has been published, and the peer-to-peer layer is not
> written yet: a build today joins no network, and its first screen says exactly that.

## Principles

- **Transparency.** No telemetry, no analytics, no crash reporting, no update ping, in any
  build — a program of ours contacts only hosts its operator asked for. What is not built yet
  is stated on the screen rather than invented.
- **Anonymity.** A key on a device, and no name of ours above it.
- **No personal data.** Never stored — not encrypted, not hashed, not temporarily.
- **Traceability.** Every document that matters is signed and checkable offline by anyone
  holding it, traceable to a key and no further.

Two standing decisions travel with them: **no central authority** — switching off everything
the project runs leaves the network running — and **IPv6 only**.

## Repositories

| Repository | What it is |
| --- | --- |
| [almena](https://github.com/almena-network/almena) | The application, and the node itself, on Windows, macOS and Linux. Tauri 2 · Rust · React · TypeScript. |
| [client](https://github.com/almena-network/client) | Almena on a phone or a tablet: a client of the network, not a node of it. |
| [agent](https://github.com/almena-network/agent) | `almena-agent`, the AI agent the application runs beside itself. Python. |
| [web](https://github.com/almena-network/web) | The public site at [almena.network](https://almena.network). Astro. |

Each repository's own `README` is the source of truth for what it needs and how to build and
run it. The project's working agreements — the rules the code is held to — live in a repository
of their own, `almena-network`.
