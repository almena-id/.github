<h1 align="center">Almena Network</h1>

<p align="center">
  <strong>Decentralized identity. Owned by you. Trusted by everyone.</strong>
</p>

<p align="center">
  <a href="https://almena.network">Website</a> &middot;
  <a href="https://docs.almena.network">Documentation</a>
</p>

---

## What is Almena Network?

Almena Network is a decentralized identity platform built on W3C standards (DIDs, Verifiable Credentials). People and organizations can create, issue, and verify digital identities without a single intermediary owning the directory.

The platform roadmap also includes decentralized applications, persistence, messaging, coordination, and ordering.

---

## Repositories

Day-to-day development happens in **independent repositories**. Clone and contribute in the repo that matches what you are working on.

| Repository | Role | Stack (high level) |
|------------|------|---------------------|
| **[almena](https://github.com/almena-network/almena)** | Core platform: **daemon** (gRPC API and node logic), **desktop** app (issuers and requesters), **CLI** (operator TUI), and **protobuf** definitions shared by clients. | Rust (tonic, daemon and tooling), Tauri v2 + React + Vite for the desktop shell |
| **[wallet](https://github.com/almena-network/wallet)** | **Holder** experience: DIDs, credentials, and keys on device; mobile-first UI. Integrates with the daemon over **HTTP REST** (`/api/v1/…`), not gRPC. | Tauri v2 + React + TypeScript |
| **[registry](https://github.com/almena-network/registry)** | Operator-facing portal for creating and managing on-network registries (for example credential issuers). | Next.js (App Router) + React + TypeScript |
| **[docs](https://github.com/almena-network/docs)** | Official documentation site: user guides, integrator-oriented material, and developer deep-dives. Bilingual **English** and **Spanish**. | Docusaurus, pnpm |
| **[web](https://github.com/almena-network/web)** | Public marketing and landing experience aligned with [almena.network](https://almena.network). | Astro, pnpm |

Each repository’s **README** is the source of truth for setup, tasks, and contribution.

---

## Integration at a glance

- **Almena** (desktop) and the **CLI** talk to **almenad** over **gRPC** using the canonical protos in the **almena** repo.
- The **wallet** uses the daemon’s **REST** surface for the flows that require a signed, HTTP-friendly contract.
- **Docs** and **web** ship as static sites; they describe and promote the same components above.

---

## Quick links

- [almena](https://github.com/almena-network/almena) (daemon, desktop, CLI, proto)
- [wallet](https://github.com/almena-network/wallet)
- [registry](https://github.com/almena-network/registry)
- [docs](https://github.com/almena-network/docs)
- [web](https://github.com/almena-network/web)
- [Website](https://almena.network)
- [Documentation](https://docs.almena.network)
