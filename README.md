# gov-es — Sovereign Epistemic Knowledge Corpus (`v1.0.0`)

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](VERSION)
[![ZeroCloudGravity](https://img.shields.io/badge/ZeroCloudGravity-v1.0.0-0F766E.svg)](https://github.com/mtwuser/zero-cloud-gravity)
[![Epistemic Grade](https://img.shields.io/badge/epistemic_grade-E3..E1-1D4ED8.svg)](docs/README.md)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

> **Spain Constitutional (`CE 1978`), AGE Ministerial Organigram & BOE Statutory Corpus** (`layer_role: knowledge`, `precedence: 20`, `stewardship_stage: public-community`).

## 1. Epistemic Corpus Index (`1:1:1` Progressive Disclosure)

All sections expose deterministic `rcap1` (`L0 -> L3`) capsules and cryptographic `citation_receipt` anchors (`<layer>::<file>#<slug>@<sha256_16>:<E3..E0>`):

| Tier | Credibility | Document |
| :--- | :--- | :--- |
| **Index** | `E2` | [`docs/README.md`](docs/README.md) |
| **Guide (`M1 -> M4`)** | `E1` | [Statutory Compliance, Ministerial Routing & BOE Navigation Guide (`M1 -> M4` — `E1`)](docs/guides/01_statutory_compliance_and_boe_navigation_guide.md) |
| **Architecture & Taxonomy** | `E3` | [Constitutional Hierarchy, State Powers & Normative Pyramid (`E3`)](docs/architecture/01_constitutional_hierarchy_and_state_powers.md) |
| **Primary Reference** | `E3/E2` | [AGE Ministerial Organigram, Public Policy Categorization & Core Statutes (`E2/E3`)](docs/reference/01_age_ministerial_organigram_and_competences.md) |

## 2. Mounting & Querying from Any `ZeroCloudGravity` Node

Link or mount this corpus into a personal (`<persona>-pc`, `<persona>-tutor`), research, or enterprise node without cloud dependencies:

```bash
zcg link <your-node-dir> --target https://github.com/mtwuser/gov-es.git --relation knowledge-feed
zcg consult-layer <your-node-dir> --layer gov-es --query "<topic>" --tier flash
```

## 3. Layer Setup Blueprint (`State U2: configured`)

- **Node ID & Role**: `gov-es` (`knowledge`, `precedence: 20`, `surface_veracity_mode: full-open-source`)
- **1-Hop Upstream Engine**: [`mtwuser/zero-cloud-gravity`](https://github.com/mtwuser/zero-cloud-gravity)
- **Active Template Packs**: `business-base`, `corporate-operations`, `science-base`, `scientific-methodology`, `gov-es`, `knowledge-stewardship-portal`
- **Mission, Scope & Core Invariants**: Primary-source jurisdictional and statutory corpus (`E3..E1`) covering the Spanish Constitution (`CE 1978`), AGE ministerial organigram, and BOE normative hierarchy with deterministic `citation_receipt` anchors.
- **Downstream Topology**: Consumed read-only via `knowledge-feed` links or `layers/*` subtrees across academic, scientific, public-sector, and enterprise nodes.
- **Authorized Layer Steward**: `gov-es Knowledge Steward <mtwuser@users.noreply.github.com>`
