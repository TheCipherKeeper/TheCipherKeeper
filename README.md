## Hi, I'm TheCipherKeeper

I build tools and training grounds for offensive security and incident
response. Everything runs on-prem, in the open — no SaaS, no phone-home. Fork
it, break it, learn from it.

- 🛠️ Currently building **[CyberCity](#cybercity)** — a digital twin of a
  city's IT/OT infrastructure (hospitals, power grid, transit, banks, courts)
  as a cyber-range for red/blue team exercises.
- 📄 Résumé / CV: [thecipherkeeper.github.io](https://thecipherkeeper.github.io)
- ✉️ Reach me via GitHub Issues on any of my projects

---

### CyberCity

A modular cyber-range: each repository is one composable layer of the same
system — same network model, different concerns. Runs on your own
Proxmox / K8s; no SaaS, nothing phones home.

| | Repository | Layer |
|---|---|---|
| 🏙️ | [cybercity](https://github.com/TheCipherKeeper/cybercity) | **Cover** — showcase + the single canonical composition (`COMPOSITION.md`) |
| 🗂️ | [cybercity-data](https://github.com/TheCipherKeeper/cybercity-data) | **Data** (Python) — declarative model: 46 orgs / 263 services / 464 links, validator, builder, IP allocator, scenario authoring |
| ⚙️ | [cybercity-engine](https://github.com/TheCipherKeeper/cybercity-engine) | **Runtime** (Go) — event-driven core, two graphs (topological + causal), tick loop, scoring, replay |
| 🎛️ | [cybercity-manage](https://github.com/TheCipherKeeper/cybercity-manage) | **Control plane** (Python) — provisioning, reset/rollback (ZFS), segment isolation, quotas; places the collector |
| 📡 | [cybercity-collector](https://github.com/TheCipherKeeper/cybercity-collector) | **Collector** (Rust) — out-of-band, per-host, read-only telemetry; signed events to the engine over Kafka |
| 🖥️ | [cybercity-ui](https://github.com/TheCipherKeeper/cybercity-ui) | **UI** (TypeScript) — interactive service map, event timeline, red/blue dashboards |

Start here for the big picture — composition, contracts, and the trust
boundary in one place:
[`cybercity/COMPOSITION.md`](https://github.com/TheCipherKeeper/cybercity/blob/main/COMPOSITION.md).

---

### Tech

`Go` · `Rust` · `Python` · `TypeScript` · `Kubernetes` · `Cilium` · `PostgreSQL`
· `Proxmox` · `Ansible` · `Terraform` · `YAML` as a first-class citizen

---

### How I work with AI

- **LLM is a co-pilot, not the boss.** It drafts YAML and code; it doesn't make
  architectural calls.
- **Validators are the contract.** Every AI-generated change runs the repo's
  gate — `ruff`/`mypy`/`pytest` (data), `go test`/`go vet` (engine),
  `cargo test` (collector).
- **One entity per iteration.** No "the whole city at once" generations — one
  organization, one service, one link, then validate.
- **Reproducibility.** Deterministic allocation (`--seed`), fixed key order,
  replayable scenarios.

---

<sub>
🛡️ Public projects, public process. Everything here is a portfolio piece —
use, fork, break, learn. Issues and PRs welcome on the active repos.
</sub>