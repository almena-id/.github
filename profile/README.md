# Almena ID

**Self-sovereign identity, held by people and spoken over DIDComm.**

Almena ID is an open platform for decentralized digital identity. People keep their identity and their credentials in a wallet on their own device; organizations issue and verify credentials through the registry; and every exchange between them travels end-to-end encrypted over [DIDComm Messaging v2.0](https://identity.foundation/didcomm-messaging/spec/v2.0/), through mediators that never see what they carry.

Launching on **November 11, 2026** at [almena.id](https://almena.id).

## Principles

- **Your identity is yours.** Keys are born on your device from a recovery phrase and never leave it. No account, no central store of who you are.
- **Private by design.** Every contact gets a DID of its own, so no two parties can link you. Mediators queue sealed messages and relay calls without reading either.
- **Built on open standards.** W3C DIDs and Verifiable Credentials, DIDComm v2.0 and its protocols, and the Agent2Agent (A2A) protocol — no proprietary lock-in.
- **Everywhere.** One wallet for Android, iOS, macOS, Linux and Windows.

## Post-quantum lab

Identity has to outlive the cryptography it rests on. Alongside the platform, Almena ID runs a laboratory for post-quantum cryptography: it tries quantum-resistant key agreement and signature schemes, such as ML-KEM and ML-DSA, against DIDs, DIDComm and credentials, so the network can move to them before today's keys stop being safe.

## Repositories

| Repository | What it is |
|------------|------------|
| [wallet](https://github.com/almena-id/wallet) | The Almena Wallet: holds your identity, contacts, messages, calls and credentials. Tauri v2 + React, on mobile and desktop. |
| [mediator](https://github.com/almena-id/mediator) | A DIDComm v2.0 mailbox and relay for wallets, with live pickup, push wake-ups and TURN credentials for calls. Rust. |
| [registry](https://github.com/almena-id/registry) | The web portal where organizations set up their tenant, issuers, verifiers and credential templates. Next.js. |
| [api](https://github.com/almena-id/api) | The backend behind the registry: tenants, DIDs, templates and issuance. FastAPI on PostgreSQL. |
| [ledger](https://github.com/almena-id/ledger) | The ledger of the Almena Network. |
| [almena](https://github.com/almena-id/almena) | The `almena` command-line interface. |
| [agent](https://github.com/almena-id/agent) | The Almena AI agent, reachable by other agents over A2A. Python + Claude. |
| [spec](https://github.com/almena-id/spec) | The platform specification, published in English and Spanish. |
| [landing](https://github.com/almena-id/landing) | The site at [almena.id](https://almena.id). Astro. |
| [develop](https://github.com/almena-id/develop) | The whole network on one machine, behind a single Caddy, for local development. |

## Get involved

Almena ID is under active development. Read the specification, open an issue or start a discussion in the repository it concerns — feedback on the protocols and the user experience is especially welcome.
