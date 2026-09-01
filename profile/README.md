<div align="center">

<img src="https://sncfoundation.github.io/logos/sncf-512.png" width="120" alt="SNCF logo">

# 💩 Sheet-Native Computing Foundation

**The CNCF — if the control plane were a Google Sheet.**

A vendor-neutral home for *Sheet-Native Computing*: a gloriously over-committed parody of the
cloud-native world that **actually runs**. Every project's control plane is a spreadsheet — and
behind the joke is real, tested code: a scheduler with failover, a certification pipeline that
mints verifiable serials, and a live federated demo across three real Google Sheets.

[Website](https://sncfoundation.github.io) ·
[Landscape](https://sncfoundation.github.io/landscape.html) ·
[Live Demo](https://sncfoundation.github.io/demo.html) ·
[Certification](https://sncfoundation.github.io/certification.html) ·
[People](https://sncfoundation.github.io/people.html) ·
[Governance](https://github.com/sncfoundation/governance)

</div>

---

## Wait — what's actually real?

All of it runs. The spreadsheet really is the cluster.

- **A real scheduler.** [`sheeternetes-onprem`](https://github.com/sncfoundation/sheeternetes-onprem)
  bin-packs pods by CPU/RAM, keeps them sticky, fails over when a node goes silent, and honors
  cordon / drain / migrate / affinity / taints — a pure, unit-tested function with CI.
- **A kubelet that runs containers.** `kubelet.sh` turns any Docker host into a node against a
  desktop `.xlsx` *or* a Google Sheet — same verb contract, air-gap-friendly.
- **Cross-substrate live migration.** `bridge.py` moves a workload from a local Excel cluster to
  a Google Sheets cluster make-before-break, with auto-rollback and two-way federation sync.
- **Verifiable certification.** Open an issue → a GitHub Action mints a serial (e.g. `SFE000001`)
  into a public registry. [19 exam programs, achievement ranks](https://sncfoundation.github.io/certification.html).
- **A live demo.** [Three real Google Sheets](https://sncfoundation.github.io/demo.html) running
  one federated app across web / data / edge tiers.
- **~30 repos**, a [landscape](https://sncfoundation.github.io/landscape.html), governance, and a
  [roadmap](https://github.com/sncfoundation/governance) — plus an external contributor or two.

## Featured projects

| Project | What | |
|---------|------|--|
| [**sheeternetes**](https://github.com/sncfoundation/sheeternetes) | Spreadsheet-native container orchestration — the flagship (kubelet + `skctl` + cert pipeline). | 🏛️ Load-Bearing |
| [**sheeternetes-onprem**](https://github.com/sncfoundation/sheeternetes-onprem) | Bare-metal apiserver over Excel/LibreOffice — scheduler, failover, cordon/drain/migrate, tested + CI. | 🏛️ Load-Bearing |
| [**sncfoundation.github.io**](https://github.com/sncfoundation/sncfoundation.github.io) | The website, landscape, live demo, and the CSFE registry. | 🏛️ Load-Bearing |
| [**sheethub**](https://github.com/sncfoundation/sheethub) | A GitLab-style DevOps forge on a spreadsheet. | 📝 Unsaved Draft |
| [**sheetlux-cd**](https://github.com/sncfoundation/sheetlux-cd) | GitOps delivery — our Argo CD. | 💾 Autosaving |
| [**sheetfana**](https://github.com/sncfoundation/sheetfana) | Dashboards rendered in-sheet — our Grafana. | 📝 Unsaved Draft |

See the full [**SNCF Landscape**](https://sncfoundation.github.io/landscape.html) — every project,
by category and maturity tier.

## Get involved

- 🎓 Get [certified](https://sncfoundation.github.io/certification.html) — verifiable, with a serial number, across 19 programs.
- 🌱 Propose a project: [New Project Proposal](https://github.com/sncfoundation/governance/issues/new?template=new-project-proposal.yml).
- 🛠️ Grab a [good first issue](https://github.com/sncfoundation/sheeternetes/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22).

> The SNCF does not recommend running production on a spreadsheet. If you do, please film the
> save dialog. It reconciles. 💩
