# Hi, I'm TheCipherKeeper

I build **reproducible, self-hosted systems for cyber training and incident
analysis** — with explicit trust boundaries, observable behavior, and automation
that can be verified instead of trusted blindly.

My current focus is [CyberCity](https://github.com/TheCipherKeeper/cybercity):
a digital twin of urban IT/OT infrastructure for red/blue team exercises.

## Featured work

### [CyberCity](https://github.com/TheCipherKeeper/cybercity)

A modular cyber range where a city is modeled as code: organizations, networks,
services, reachability, scenarios, and vulnerabilities. The runtime records a
trusted event stream and a causal graph, so an exercise can be observed,
scored, replayed, and explained.

- Designed for private Proxmox and Kubernetes infrastructure
- Event-driven core with topological and causal graphs
- Out-of-band observation across trusted and untrusted network planes
- Declarative scenarios and deterministic builds
- No required SaaS or external telemetry

Start with the
[project overview](https://github.com/TheCipherKeeper/cybercity#readme) or open
the
[canonical system composition](https://github.com/TheCipherKeeper/cybercity/blob/main/COMPOSITION.md)
for architecture, boundaries, contracts, and current status.

### [ADDM](https://github.com/TheCipherKeeper/addm)

An agent-driven development methodology for projects built by one person and
software agents. It defines a reproducible path from an ordered backlog to
implementation, independent review, CI evidence, squash merge, and a verified
test deployment.

## Engineering principles

- **Evidence over confidence.** Tests, validators, CI, and observable behavior
  decide whether a change works.
- **One fact, one authority.** Contracts and architectural decisions have a
  canonical home instead of drifting between documents.
- **Determinism matters.** Fixed inputs, seeded generation, pinned methodology,
  and replayable events make failures explainable.
- **Trust boundaries are structural.** Untrusted workloads cannot become their
  own source of truth.
- **AI is an implementer, not a product owner.** Agents can choose technical
  details; product intent and system boundaries remain human decisions.
- **Self-hosted by design.** Projects should remain useful without mandatory
  cloud services or phone-home telemetry.

## Tools I reach for

`Go` · `Rust` · `Python` · `TypeScript` · `PostgreSQL` · `Kafka / Redpanda` ·
`Kubernetes` · `Cilium` · `Proxmox` · `Terraform` · `Docker` · `GitHub Actions`

## Elsewhere

- Portfolio and résumé: [thecipherkeeper.github.io](https://thecipherkeeper.github.io)
- Project discussions: open an issue in the relevant repository

---

<sub>Public projects, public process. Explore the architecture, run the checks,
break things responsibly, and share what you learn.</sub>
