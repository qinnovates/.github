<div align="center">

# Qinnovates

**Security research and open-source tooling for brain-computer interfaces.**

[Website](https://qinnovate.com) · [Preprint](https://doi.org/10.5281/zenodo.18640105) · [Blog](https://qinnovate.com/news/) · [API](https://qinnovate.com/api/tara.json)

</div>

Built by [Kevin Qi](https://qinnovate.com/about/) — 15 years in security engineering, now applied to the brain-computer interface stack. Designing since [AGFX (2003)](https://web.archive.org/web/20070107073424/http://s8.invisionfree.com:80/AGFX/), building security infrastructure since 2011.

---

**Researchers** → [Preprint](https://doi.org/10.5281/zenodo.18640105) · [Threat taxonomy](https://qinnovate.com/TARA/) · [Governance](https://github.com/qinnovates/qinnovate/tree/main/governance)<br>
**Developers** → [Install](#install) · [API](#open-api) · [Monorepo guide](https://github.com/qinnovates/qinnovate#project-structure)<br>
**Everyone else** → [What is this?](https://qinnovate.com/framework/) · [Blog](https://qinnovate.com/news/)

---

## Research

QIF is an 11-band hourglass security architecture for BCIs — 7 neural bands, a physical interface boundary (I0), and 3 silicon bands.

| Component | Purpose | Links |
|-----------|---------|-------|
| **QIF** | Hourglass architecture spanning neural, interface, and silicon bands | [Whitepaper](https://qinnovate.com/whitepaper/) · [Guide](https://qinnovate.com/framework/) |
| **TARA** | Attack-therapy technique pairs across biological domains, structured as a STIX 2.1 registry | [Registry](https://qinnovate.com/TARA/) · [Atlas](https://qinnovate.com/atlas/tara/) |
| **NISS** | CVSS v4.0 scoring extension for neural interfaces | [Calculator](https://qinnovate.com/scoring/) |
| **NSP** | Post-quantum wire protocol for BCI data links | [Spec](https://qinnovate.com/tools/nsp/) |
| **Runemate** | Rendering pipeline for vision restoration. HTML-to-bytecode compiler today, targeting visual cortex output long-term | [Spec](https://qinnovate.com/tools/runemate/) |

> All components are proposed research, not adopted standards. [Full status & limitations](https://github.com/qinnovates/qinnovate/tree/main/governance)

<details>
<summary><strong>Cite this work</strong></summary>

```bibtex
@misc{qi2026securing,
  title     = {Securing Neural Interfaces: Architecture, Threat Taxonomy, and Neural Impact Scoring for Brain-Computer Interfaces},
  author    = {Qi, Kevin},
  year      = {2026},
  doi       = {10.5281/zenodo.18640105},
  url       = {https://doi.org/10.5281/zenodo.18640105},
  publisher = {Zenodo},
  note      = {Preprint, CC-BY 4.0}
}
```

</details>

### Open API

No auth required.

| Endpoint | What You Get |
|----------|-------------|
| [`/api/tara.json`](https://qinnovate.com/api/tara.json) | Full TARA registry — CVSS, NISS, DSM-5-TR, physics, therapy, governance |
| [`/api/stix.json`](https://qinnovate.com/api/stix.json) | Same data as a STIX 2.1 Bundle for threat intel platforms |

---

## Use

### Install

```bash
claude install qinnovates/quorum          # Multi-agent reasoning for Claude Code
brew install qinnovates/macshield/macshield  # macOS network-aware hardening
pip install qtara                          # Python SDK for TARA registry
```

### Tools

| Tool | What It Does | Platform |
|------|-------------|----------|
| [**Quorum**](https://github.com/qinnovates/quorum) | Multi-agent reasoning for Claude Code. Expert swarms, dialectic mode, hallucination detection | Claude Code |
| [**macshield**](https://github.com/qinnovates/macshield) | Network-aware macOS hardening. Auto-hardens on untrusted WiFi | macOS |
| [**qtara**](https://pypi.org/project/qtara/) ([source](https://github.com/qinnovates/qinnovate/tree/main/shared/qtara)) | Python SDK for TARA registry management and STIX export | Python |
| [**Neurowall**](https://github.com/qinnovates/qinnovate/tree/main/tools/neurowall) | Neural firewall neckband prototype. OpenBCI + NSP + post-quantum crypto | Hardware / Python |
| [**Dogma**](https://github.com/qinnovates/dogma) | Pet wellness tracker. LiDAR camera (6 modes), health monitoring, Dog Finder with haptic/audio guidance | iOS / Swift |
| [**QIF-LiDAR**](https://github.com/qinnovates/qinnovate/tree/main/tools/qif-lidar) | iPhone depth sensing for vision prosthesis research | iOS / Swift |
| [**Open Neural Atlas**](https://github.com/qinnovates/neurosim) | Interactive 3D brain visualization with BCI electrode mapping | Web |

Questions or feedback? [Open an issue](https://github.com/qinnovates/qinnovate/issues).

---

## Explore

Interactive tools on [qinnovate.com](https://qinnovate.com).

| Resource | What It Is |
|----------|-----------|
| [QIF Framework Guide](https://qinnovate.com/framework/) | Walkthrough of the 11-band hourglass architecture |
| [Threat Atlas](https://qinnovate.com/atlas/tara/) | Visual atlas of attack-therapy technique pairs |
| [TARA Registry](https://qinnovate.com/TARA/) | Searchable registry with filtering, scoring, and export |
| [NISS Calculator](https://qinnovate.com/scoring/) | Neural impact scoring tool |
| [BCI Explorer](https://qinnovate.com/research/bci-explorer/) | Devices, protocols, and security considerations |
| [Glossary](https://qinnovate.com/glossary/) | Terminology reference for neurosecurity concepts |

---

## Read

| What | Link |
|------|------|
| Academic preprint (CC-BY 4.0) | [DOI: 10.5281/zenodo.18640105](https://doi.org/10.5281/zenodo.18640105) |
| Blog — BCI security research | [qinnovate.com/news](https://qinnovate.com/news/) |
| Governance & ethics (12 docs) | [Neuroethics](https://github.com/qinnovates/qinnovate/blob/main/governance/QIF-NEUROETHICS.md) · [Informed Consent](https://github.com/qinnovates/qinnovate/blob/main/governance/INFORMED_CONSENT_FRAMEWORK.md) · [All docs](https://github.com/qinnovates/qinnovate/tree/main/governance) |

---

## Repositories

| Repo | What | Stack |
|------|------|-------|
| [**qinnovate**](https://github.com/qinnovates/qinnovate) | Core monorepo — framework, registry, protocol, governance, preprint, website, tools | TypeScript, Astro, Python |
| [**quorum**](https://github.com/qinnovates/quorum) | Multi-agent reasoning plugin for Claude Code | Claude Code skill |
| [**dogma**](https://github.com/qinnovates/dogma) | Pet wellness tracker. LiDAR camera, health monitoring, Dog Finder accessibility | iOS / Swift |
| [**neurosim**](https://github.com/qinnovates/neurosim) | Open Neural Atlas — 3D brain visualization, electrode mapping | TypeScript, Three.js |
| [**macshield**](https://github.com/qinnovates/macshield) | Network-aware macOS hardening | Shell |
| [**homebrew-tools**](https://github.com/qinnovates/homebrew-tools) | Homebrew tap for qinnovates tools | Ruby |
| [**mindloft**](https://github.com/qinnovates/mindloft) | Creative workshop — ideas, experiments, tools | Private |

---

### Creative & Learning

Music under **justbrowser** — [Spotify](https://open.spotify.com/artist/4gZIMNI8AKnuGoYbcOzZc3) · [SoundCloud](https://soundcloud.com/search?q=keviano%20kulhi) · [All Tracks](https://github.com/qinnovates/qinnovate/tree/main/docs/learn/music/justbrowser)

Learning — [Autodidactive](https://qinnovate.com/learn/autodidactive/) · [Calculus Labs](https://qinnovate.com/learn/autodidactive/labs/calculus-fundamentals.html)

Design origins (2003-2005) — [DeviantArt](https://www.deviantart.com/kevq) · [AGFX forum (Wayback)](https://web.archive.org/web/20070107073424/http://s8.invisionfree.com:80/AGFX/)

---

<div align="center">

Apache 2.0

</div>
