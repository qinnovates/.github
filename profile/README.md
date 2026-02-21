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
| **QIF** | 11-band security architecture. The OSI model for the mind. v6.2.1. | [Whitepaper](https://qinnovate.com/whitepaper/) · [Interactive Explorer](https://qinnovate.com/lab/hourglass.html) |
| **TARA** | 103 attack-therapy technique pairs across 8 domains and 15 tactics. STIX 2.1 registry. | [Registry](https://qinnovate.com/TARA/) · [STIX Feed](https://qinnovate.com/api/stix.json) |
| **NISS** | First CVSS v4.0 extension for neural interfaces. 5 metrics: Biological Impact, Cognitive Integrity, Consent Violation, Reversibility, Neuroplasticity. | [Scoring](https://qinnovate.com/scoring/) |
| **NSP** | Post-quantum wire protocol (ML-KEM, ML-DSA, AES-256-GCM) for BCI data links. Under 4% implant power overhead. | [Spec](https://qinnovate.com/nsp/) |
| **Runemate** | Rendering pipeline: HTML-to-bytecode today, code-to-visual-cortex tomorrow. Vision restoration is the goal. | [Spec](https://qinnovate.com/runemate/) |
| **qtara** | Python SDK for TARA registry management and STIX export. | [PyPI](https://pypi.org/project/qtara/) |

### Open API

The full TARA dataset is available as a public JSON API. No auth required.

| Endpoint | What It Returns |
|----------|----------------|
| [`/api/tara.json`](https://qinnovate.com/api/tara.json) | All 103 techniques with CVSS v4.0 vectors, NISS scores, DSM-5-TR diagnostic mappings, physics feasibility constraints, therapeutic analogs, FDA status, safe dosing parameters, governance requirements, and engineering specs. |
| [`/api/stix.json`](https://qinnovate.com/api/stix.json) | Same data as a STIX 2.1 Bundle. Drop it into any STIX-compatible threat intel platform. |

Each technique includes: attack mechanism, QIF band mapping, dual-use classification (attack vs. therapy), clinical conditions treated by the same mechanism, regulatory crosswalk (FDA, IEC, ISO), DSM-5-TR codes (primary and secondary), and physics coupling parameters.

### Tools

| Tool | Description |
|------|-------------|
| [**neurowall**](https://github.com/qinnovates/qinnovate/tree/main/tools/neurowall) | Neural firewall neckband prototype. OpenBCI + NSP + post-quantum crypto. |
| [**macshield**](https://github.com/qinnovates/macshield) | Network-aware macOS hardening. Auto-hardens on untrusted WiFi, relaxes on trusted networks. `brew install qinnovates/macshield/macshield` |
| [**autodidactive**](https://github.com/qinnovates/qinnovate/tree/main/tools/autodidactive) | Adaptive learning platform. |

### Governance

12 published neuroethics and regulatory compliance documents covering accessibility, informed consent, pediatric protections, FDA/EU MDR crosswalk, UNESCO alignment, and post-deployment ethics.

[Browse governance docs](https://github.com/qinnovates/qinnovate/tree/main/governance) · [Transparency statement](https://github.com/qinnovates/qinnovate/blob/main/governance/TRANSPARENCY.md)

### Published Work

- **Academic Preprint:** [DOI: 10.5281/zenodo.18640105](https://doi.org/10.5281/zenodo.18640105) (28 pages, 6 figures, CC-BY 4.0, v1.4)
- **TARA Registry:** [103 BCI attack-therapy technique pairs](https://qinnovate.com/TARA/)
- **qtara SDK:** `pip install qtara` ([PyPI](https://pypi.org/project/qtara/))
- **Blog:** [18 posts on BCI security research](https://qinnovate.com/publications/)

### Repositories

| Repo | Description |
|------|-------------|
| [**qinnovate**](https://github.com/qinnovates/qinnovate) | Core monorepo. QIF framework, TARA registry, NSP protocol, governance, preprint, website, and tools. |
| [**firefly**](https://github.com/qinnovates/firefly) | Privacy-first journaling app for kids. Local-first architecture, COPPA/GDPR/CCPA compliant. |

---

<div align="center">

*Open standards for the neural frontier. Apache 2.0.*

</div>
