<h1 align="center">Almena Network</h1>

<p align="center">
  <strong>Decentralized communication. Owned by you. Trusted by no one else.</strong>
</p>

<p align="center">
  <a href="https://almena.network">Website</a> &middot;
  <a href="https://docs.almena.network">Documentation</a>
</p>

---

## What is Almena Network?

Almena Network is a decentralized communication platform. Messages are end-to-end encrypted and routed through onion paths over a permissionless network of operator-run nodes. No central server stores user content or metadata.

Design priorities: peer-to-peer and federated architectures, user sovereignty over data, open protocols, and privacy as a first-class concern.

---

## Repositories

| Repository | Role | Stack |
|------------|------|-------|
| **[client](https://github.com/almena-network/client)** | End-user P2P messenger — identity, contacts, messaging UI, calls, and group conversations. Targets desktop (macOS, Windows, Linux) and mobile (iOS, Android). | Tauri v2 · Rust · React · TypeScript |
| **[node](https://github.com/almena-network/node)** | Network node software — bundles a **service-node** daemon (onion routing relay, message storage, swarm replication) and a **blockchain-node** daemon (proof-of-work chain, on-chain staking, service-node registry). Ships as a desktop operator app. | Tauri v2 · Rust (Cargo workspace) · React · TypeScript |
| **[docs](https://github.com/almena-network/docs)** | Official documentation site. Sections for users, integrators, and developers. Bilingual **English / Spanish**. | Docusaurus 3 · pnpm |
| **[web](https://github.com/almena-network/web)** | Public marketing and landing site at [almena.network](https://almena.network). Covers the messenger product and network infrastructure. Bilingual **English / Spanish**. | Astro 6 · pnpm |

Each repository's **README** is the source of truth for setup, tasks, and contribution guidelines.

---

## How it fits together

- The **client** sends and receives messages through **service nodes** using layered onion encryption. No service node sees both sender and recipient.
- **Service nodes** and **blockchain nodes** are run by independent operators using the **node** desktop app. The blockchain tracks which service nodes are active and enforces staking.
- Wire format and cryptographic primitives (Ed25519, X25519, ChaCha20-Poly1305, BLAKE2b) are defined in the `almena-protocol` crate inside the `node` repository. The `client` depends on it directly so both ends stay byte-compatible.
- **Docs** and **web** are static sites; they describe and promote the components above.

---

## Quick links

- [client](https://github.com/almena-network/client)
- [node](https://github.com/almena-network/node)
- [docs](https://github.com/almena-network/docs)
- [web](https://github.com/almena-network/web)
- [Website](https://almena.network)
- [Documentation](https://docs.almena.network)
