## Hi, I'm TheCipherKeeper

I build tools and training grounds for offensive security and incident response.
Public projects live in the open, on-prem by design.

- 🛠️ Currently building **[CyberCity](#cybercity)** — a cyber-range that simulates
  an entire city (hospitals, power grid, transit, banks, courts) for red/blue
  team exercises.
- 📄 Résumé / CV: [thecipherkeeper.github.io](https://thecipherkeeper.github.io)
- ✉️ Reach me via GitHub Issues on any of my projects

---

### CyberCity

A modular cyber-range: each repo is one composable piece of the system.
Same network model — different layers. No SaaS, no telemetry back to me,
runs on your own Proxmox / K8s.

| | Repository | What it does |
|---|---|---|
| 🎯 | [cybercity](https://github.com/TheCipherKeeper/cybercity) | Cover / showcase repo for the whole composition |
| ⚙️ | [cybercity-engine](https://github.com/TheCipherKeeper/cybercity-engine) | Go runtime: event-sourced engine, network validator, K8s manifest renderer |
| 🗺️ | [cybercity-data](https://github.com/TheCipherKeeper/cybercity-data) | 30 organizations, 95 services, decoy hosts in `network.yml` |
| 🖥️ | [cybercity-ui](https://github.com/TheCipherKeeper/cybercity-ui) | 2D city map, event timeline, red/blue dashboards |
| 📡 | [cybercity-agents](https://github.com/TheCipherKeeper/cybercity-agents) | Log/SIEM collectors inside city segments |
| 🏗️ | [cybercity-blueprints](https://github.com/TheCipherKeeper/cybercity-blueprints) | Proxmox VM provisioning (Ansible/Terraform) |

Read the philosophy first: [`master.md`](https://github.com/TheCipherKeeper/cybercity-engine/blob/main/master.md).

---

### Tech

`Go` · `Kubernetes` · `Cilium` · `PostgreSQL` · `Ansible` · `Terraform`
`Proxmox` · `Rust` (selectively) · `YAML` as a first-class citizen

---

### How I work with AI

- **LLM is a co-pilot, not the boss.** I use it to draft YAML, not to make decisions.
- **Validators are the contract.** Every AI-generated change goes through `go test`.
- **One entity per iteration.** No "30 organizations at once" generations.
- **Reproducibility.** Deterministic mode, fixed key order, replayable scenarios.

---

<sub>
🛡️ Public projects, public process. Anything here is a portfolio piece —
use, fork, break, learn. Issues and PRs are welcome on the active repos.
</sub>
