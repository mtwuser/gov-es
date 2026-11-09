# Statutory Compliance, Ministerial Routing & BOE Navigation Guide (`M1 -> M4` — `gov-es` `E1`)

> **Epistemic Credibility Grade: `E1` (Adaptive `M1..M4` Civic & Enterprise Compliance Guide)**
>
> This guide explains how citizens (`M1..M2`), corporate operational departments (`M3`), and legal/compliance officers (`M4`) classify public regulatory obligations using `gov-es` (`01_constitutional_hierarchy_and_state_powers.md` and `01_age_ministerial_organigram_and_competences.md`).

---

## 1. 3-Step Workflow to Categorize & Apply Public Information (`GOV-ES-01..03`)

Whenever a project, department, or citizen needs to verify legal compliance in Spain, follow these three deterministic steps:

1. **Step 1 — Identify the Ministerial Area (`AREA-01..07` in `01_age_ministerial_organigram_and_competences.md`)**:
   - *Tax, invoicing, or public procurement?* $\rightarrow$ `AREA-01` (Hacienda / `AEAT` — `LGT`, `IVA/IS`, `LCSP`).
   - *Company formation, contracts, patents, or trade secrets?* $\rightarrow$ `AREA-02` (Justicia / `OEPM` — `LSC`, `Ley 24/2015`, `Ley 1/2019`).
   - *Software, websites, personal data, or cybersecurity?* $\rightarrow$ `AREA-03` (Transformación Digital / `AEPD` / `CCN` — `LOPDGDD`, `ENS`, `LSSI`).
   - *Biomass valorization, circular economy, or biodiversity?* $\rightarrow$ `AREA-04` (`MITECO` — `Ley 7/2022`, `RD 630/2013`).
   - *Industrial machinery, thermal reactors, or R&D?* $\rightarrow$ `AREA-05` (`MINTUR` / `MICIU` — `Ley 21/1992`, `Ley 14/2011`).
   - *Workplace safety, laboratory locks, or biological agents?* $\rightarrow$ `AREA-06` (`MITES` / `INSST` — `Ley 31/1995 PRL`, `RD 664/1997`).
   - *Food-contact materials (`AISI 316`) or consumer labeling?* $\rightarrow$ `AREA-07` (`Sanidad` / `AESAN` — `Ley 17/2011`).
2. **Step 2 — Verify Normative Rank (`E3` vs. `E2` vs. `E1`) & Territorial Scope (`geo-es`)**:
   - Check the normative pyramid (`01_constitutional_hierarchy_and_state_powers.md`) and the `ISO 3166-2:ES` region (`geo-es`) to account for Foral (`ES-PV`, `ES-NC`) or Canary Islands (`ES-CN`) specificities.
3. **Step 3 — Query via `make consult` and Anchor with `citation_receipt`**:
   - Run `make consult LAYER=gov-es QUERY="<keyword>"` and record the returned `citation_receipt` (`gov-es::docs/reference/01_age_ministerial_organigram_and_competences.md#<slug>@<digest>:E2`) in your departmental ledger (`corporate/` or `docs/`).

---

## 2. Progressive `M1 -> M4` Consumer Adaptation Matrix

| Mastery Level | Target Persona | Recommended Consultation Depth |
| :--- | :--- | :--- |
| **`M1` / `M2`** | Citizen, Student, or Junior Developer | Start with this guide (`docs/guides/`) to understand the 3-tier state structure (`AGE`, `CCAA`, `EELL`) and which Ministry governs each domain. |
| **`M3`** | Departmental Lead (`dept-iso-finance`, `dept-iso-bio`, `dept-iso-eng`) | Cross-reference `AREA-01..07` in `docs/reference/01_age_ministerial_organigram_and_competences.md` to bind operational gates (`FIN-*`, `BIO-*`, `TECH-*`) to their `BOE-A-*` statutes. |
| **`M4`** | Legal Counsel / DPO / Compliance Auditor (`dept-iso-legal`) | Audit primary `E3` constitutional and parliamentary provisions (`docs/architecture/01_constitutional_hierarchy_and_state_powers.md`) and verify `CITATION_DRIFT_DETECTED` across all dependent layers. |
