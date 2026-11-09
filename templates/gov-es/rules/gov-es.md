---
trigger: always_on
description: "Spanish Constitutional Hierarchy, AGE Ministerial Competence Routing, and BOE Statutory Citation Rules (gov-es)"
---

# Spanish Statutory & Public Administration Corpus Rules (`gov-es`)

## Scope & Surface Target
- **Template Pack**: `templates/gov-es/` (`context-stack`).
- **Knowledge Domain**: `jurisdictional-normative` (`public:knowledge:jurisdictional-normative`, `E3..E1`).

## Normative Invariants (`GOV-ES-01..03`)

1. **`GOV-ES-01` (Art. 9.3 CE Normative Hierarchy & Epistemic Precedence)**:
   - Enforce strict constitutional and statutory precedence (`EPISTEMIC_PRECEDENCE_VIOLATION` on override):
     1. **`E3` (Supreme Constitutional & EU Primary Law)**: Constitución Española de 1978 (`BOE-A-1978-31229`) and EU Treaties / Regulations (`TFUE`).
     2. **`E3` (Parliamentary Statutes)**: Leyes Orgánicas (`Art. 81 CE`), Leyes Ordinarias, Reales Decretos Legislativos (`Art. 82 CE`), and Reales Decretos-Leyes (`Art. 86 CE`).
     3. **`E2` (Executive Regulations)**: Reales Decretos del Consejo de Ministros (`Art. 97 CE`) and Órdenes Ministeriales.
     4. **`E1` (Administrative & Pedagogical Guidance)**: Resoluciones, Instrucciones, Circulares, and `M1..M2` citizen/enterprise compliance guides (`docs/guides/`).
2. **`GOV-ES-02` (Ministerial Organigram & Territorial Competence Routing `AGE / CCAA / EELL`)**:
   - Every regulatory requirement must be categorized by:
     - **Competent Ministerial Area (`AGE` — Ley 40/2015 `LRJSP`)**: Hacienda & Fiscalidad, Economía & Transformación Digital, Transición Ecológica & Economía Circular (`MITECO`), Industria & Ciencia, Trabajo & PRL (`MITES`), or Sanidad & Consumo.
     - **Territorial Jurisdiction (`Art. 137–158 CE` + `geo-es`)**: Exclusive State (`Art. 149.1 CE`), Autonomous Community (`CCAA`, including Foral regimes `ES-PV`/`ES-NC` and Canary Islands `ES-CN` REF), or Local Entity (`EELL` — Ley 7/1985 `LRBRL`).
3. **`GOV-ES-03` (Official `BOE` Identifier & `citation_receipt` Provenance)**:
   - Every statutory citation must include its official Boletín Oficial del Estado identifier (`BOE-A-YYYY-NNNNN`), effective consolidation status, and a verifiable `citation_receipt` (`gov-es::docs/...#<slug>@<digest16>:<E3..E1>`).

## Verification & Sign-Off Gates
- [ ] Verify zero drift via `zcg diff-project`.
- [ ] Confirm every statute cites its `BOE-A-YYYY-NNNNN` identifier and competent ministerial or territorial authority.
