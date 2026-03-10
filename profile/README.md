<div align="center">

# Qinnovates

**Original security research and open-source tooling for brain-computer interfaces.**

[Website](https://qinnovate.com) · [Preprint](https://doi.org/10.5281/zenodo.18640105) · [TARA Registry](https://qinnovate.com/TARA/) · [API](https://qinnovate.com/api/tara.json)

</div>

---

### QIF Framework

The Quantified Interconnection Framework is an 11-band hourglass security architecture for BCIs: 7 neural bands (N7 Neocortex to N1 Spinal Cord), a physical interface boundary (I0, the electrode-tissue junction), and 3 silicon bands (S1 Analog to S3 Radio/Wireless).

| Component | What It Does | Links |
|-----------|-------------|-------|
| **QIF** | 11-band security architecture. The OSI model for the mind. | [Whitepaper](https://qinnovate.com/whitepaper/) · [Framework](https://qinnovate.com/framework/) |
| **TARA** | BCI attack-therapy technique pairs across multiple domains and tactics. STIX 2.1 registry. | [Registry](https://qinnovate.com/TARA/) · [STIX Feed](https://qinnovate.com/api/stix.json) |
| **NISS** | First CVSS v4.0 extension for neural interfaces. Metrics: Biological Impact, Cognitive Integrity, Consent Violation, Reversibility, Neuroplasticity. | [Scoring](https://qinnovate.com/scoring/) |
| **NSP** | Post-quantum wire protocol (ML-KEM, ML-DSA, AES-256-GCM) for BCI data links. Under 4% implant power overhead. | [Spec](https://qinnovate.com/tools/nsp/) |
| **Runemate** | Rendering pipeline: HTML-to-bytecode today, code-to-visual-cortex tomorrow. Vision restoration is the goal. | [Spec](https://qinnovate.com/tools/runemate/) |
| **qtara** | Python SDK for TARA registry management and STIX export. | [PyPI](https://pypi.org/project/qtara/) |

### Open API

The full TARA dataset is available as a public JSON API. No auth required.

| Endpoint | What It Returns |
|----------|----------------|
| [`/api/tara.json`](https://qinnovate.com/api/tara.json) | All techniques with CVSS v4.0 vectors, NISS scores, DSM-5-TR diagnostic mappings, physics feasibility constraints, therapeutic analogs, FDA status, safe dosing parameters, governance requirements, and engineering specs. |
| [`/api/stix.json`](https://qinnovate.com/api/stix.json) | Same data as a STIX 2.1 Bundle. Drop it into any STIX-compatible threat intel platform. |

Each technique includes: attack mechanism, QIF band mapping, dual-use classification (attack vs. therapy), clinical conditions treated by the same mechanism, regulatory crosswalk (FDA, IEC, ISO), DSM-5-TR codes (primary and secondary), and physics coupling parameters.

### Tools

| Tool | Description |
|------|-------------|
| [**neurowall**](https://github.com/qinnovates/qinnovate/tree/main/tools/neurowall) | Neural firewall neckband prototype. OpenBCI + NSP + post-quantum crypto. |
| [**macshield**](https://github.com/qinnovates/macshield) | Network-aware macOS hardening. Auto-hardens on untrusted WiFi, relaxes on trusted networks. `brew install qinnovates/macshield/macshield` |

### Learning Resources

| Resource | Description |
|----------|-------------|
| [**Autodidactive**](https://qinnovate.com/learn/autodidactive/) | Mobile-first daily learning app. 45 historical figures across 7 disciplines. Spaced repetition, post-it note wall, bookmarking. ([Source](https://github.com/qinnovates/qinnovate/tree/main/docs/learn/autodidactive)) |
| [**Calculus Fundamentals**](https://qinnovate.com/learn/autodidactive/labs/calculus-fundamentals.html) | Interactive lab — limits, derivatives, integrals |
| [**Calculus & Signals**](https://qinnovate.com/learn/autodidactive/labs/calculus-signals.html) | Interactive lab — signal processing with calculus |
| [**Calculus & BCI Limits**](https://qinnovate.com/learn/autodidactive/labs/calculus-bci-limits.html) | Interactive lab — calculus applied to BCI constraints |
| [**QIF Framework**](https://qinnovate.com/framework/) | Comprehensive walkthrough of the 11-band hourglass security architecture. |
| [**BCI Explorer**](https://qinnovate.com/research/bci-explorer/) | Interactive explorer for BCI devices, protocols, and security considerations. |
| [**Threat Atlas**](https://qinnovate.com/atlas/tara/) | Interactive atlas of BCI attack-therapy technique pairs. |
| [**Glossary**](https://qinnovate.com/glossary/) | Terminology reference for QIF, TARA, NISS, and neurosecurity concepts. |

### Music — justbrowser

Original music encoding philosophy, neuroscience, and personal narrative into sound.

| Track | Genre | Links |
|-------|-------|-------|
| **Sawdust** | Dark gospel blues / soul | [Spotify](https://open.spotify.com/artist/4gZIMNI8AKnuGoYbcOzZc3) |
| **Principals of Ethics** | Cinematic neo-soul gospel | [Lyrics & Analysis](https://github.com/qinnovates/qinnovate/tree/main/docs/learn/music/justbrowser/neuroethics/principals-of-ethics.md) |

[Listen on Spotify](https://open.spotify.com/artist/4gZIMNI8AKnuGoYbcOzZc3) · [SoundCloud](https://soundcloud.com/search?q=keviano%20kulhi) · [All tracks](https://github.com/qinnovates/qinnovate/tree/main/docs/learn/music/justbrowser)

### Governance

Neuroethics and regulatory compliance documents covering accessibility, informed consent, pediatric protections, FDA/EU MDR crosswalk, UNESCO alignment, and post-deployment ethics.

[Browse governance docs](https://github.com/qinnovates/qinnovate/tree/main/governance) · [Transparency statement](https://github.com/qinnovates/qinnovate/blob/main/governance/TRANSPARENCY.md)

### Published Work

- **Academic Preprint:** [DOI: 10.5281/zenodo.18640105](https://doi.org/10.5281/zenodo.18640105) (CC-BY 4.0)
- **TARA Registry:** [BCI attack-therapy technique pairs](https://qinnovate.com/TARA/)
- **qtara SDK:** `pip install qtara` ([PyPI](https://pypi.org/project/qtara/))
- **Blog:** [BCI security research posts](https://qinnovate.com/news/)

### Repositories

| Repo | Description |
|------|-------------|
| [**qinnovate**](https://github.com/qinnovates/qinnovate) | Core monorepo. QIF framework, TARA registry, NSP protocol, governance, preprint, website, and tools. |
| [**mindloft**](https://github.com/qinnovates/mindloft) | Creative workshop: ideas, experiments, and tools. Private. |

---

<div align="center">

*Open standards for the neural frontier. Apache 2.0.*

</div>
