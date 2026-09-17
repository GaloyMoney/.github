# The technology provider for banks embracing the future

**Galoy is building the core banking system for software-native banks. One ledger for dollars, euros, Bitcoin, and stablecoins.**

The Galoy core is written in Rust around an event-sourced, double-entry ledger. Capabilities are built as modules with explicit contracts, enforced at compile time, and the whole system is deployed and operated as one.

Inside the core:

- **Multi-currency ledger:** dollars, euros, Bitcoin, and stablecoins in one double-entry accounting model
- **Payments:** ACH, Fedwire, RTP and FedNow, Lightning, and major stablecoins
- **Digital-asset lending:** term loans and lines of credit collateralized by digital assets, with real-time collateral marking and configurable margin calls.
- **Governance:** maker-checker approvals wired into credit and withdrawal flows, with every action logged
- **Custody:** custody-independent by design. Banks bring their own qualified custodian.

A de novo institution starts on the Galoy core directly. An incumbent bank can adopt a single module deployed alongside the core it runs today.

## Open source

We open source components for Bitcoin payments, accounting, event sourcing, and reliability infrastructure so builders can inspect, adapt, and reuse them:

| Repository | What it does |
|---|---|
| [drua](https://github.com/GaloyMoney/drua) | The open-source harness Galoy uses to run AI agents against its own banking codebase: credential isolation, human approval gates, and a full record of every action. |
| [cala](https://github.com/GaloyMoney/cala) | Double-entry accounting ledger for high-throughput financial applications |
| [es-entity](https://github.com/GaloyMoney/es-entity) | Persist event-sourced entities in PostgreSQL |
| [bria](https://github.com/GaloyMoney/bria) | Wallet infrastructure for on-chain Bitcoin operations at scale |
| [stablesats-rs](https://github.com/GaloyMoney/stablesats-rs) | Bitcoin deposits that hold USD-denominated value |
| [job](https://github.com/GaloyMoney/job) | Durable background job runner backed by PostgreSQL |
| [obix](https://github.com/GaloyMoney/obix) | Outbox and inbox patterns for reliable message passing between services |

## Track record

The team behind the Galoy core ran the Bitcoin Beach Wallet in El Salvador at national scale from 2019 to 2025. Galoy is ISO 27001:2022 certified.

---

Learn how the Galoy core fits your institution at [galoy.io](https://galoy.io)
