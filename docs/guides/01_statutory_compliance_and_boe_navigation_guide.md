---
epistemic_grade: E1
---

# Statutory Compliance, Ministerial Routing & BOE Navigation Guide (`M1 -> M4` — `gov-es` `E1`)

> **Epistemic Credibility Grade: `E1` (Adaptive `M1..M4` Civic, Academic & Enterprise Compliance Guide)**
>
> This practical guide explains how citizens and students (`M1..M2`), operational engineering/finance leads (`M3`), and legal/compliance auditors (`M4`) navigate the *Boletín Oficial del Estado (`BOE`)* and bind operational decisions to canonical `E3/E2` anchors in [01_constitutional_hierarchy_and_state_powers.md](../architecture/01_constitutional_hierarchy_and_state_powers.md) and [01_age_ministerial_organigram_and_competences.md](../reference/01_age_ministerial_organigram_and_competences.md).

---

## 1. Anatomy of Official `BOE` Identifiers & Consolidated Texts (`BOE-A-YYYY-NNNNN`) [E1]

> **Exon [E1]:** *Always cite the `BOE` **Texto Consolidado** (`BOE-A-YYYY-NNNNN`) rather than isolated amending provisions, verifying the latest consolidation timestamp (`Última actualización publicada`) before sealing a `citation_receipt` ([01_age_ministerial_organigram_and_competences.md](../reference/01_age_ministerial_organigram_and_competences.md)).*

Every primary statute in Spain carries a permanent, machine-verifiable identifier issued by the *Agencia Estatal Boletín Oficial del Estado*:

| `BOE` Identifier Component | Canonical Pattern / Example | Meaning & Verification Rule |
| :--- | :--- | :--- |
| **Series Prefix (`BOE-A-`)** | `BOE-A-2015-10565` (`Ley 39/2015 LPACAP`) | `Section I` (*Disposiciones Generales*) and `Section III` general acts; `BOE-B-` denotes `Section IV/V` announcements and public tenders. |
| **Publication Year (`YYYY`)** | `1978`, `2015`, `2022` | Year of publication in the Official Gazette (which may differ by `+1` year from late-December enactment dates, e.g., `LOMLOE` enacted Dec 2020). |
| **Sequential Act Number (`NNNNN`)** | `31229` (`CE 1978`), `5809` (`Ley 7/2022`) | Unique annual sequence number assigned by the `BOE` registry. |
| **Consolidated Text (`Texto Consolidado`)** | `https://www.boe.es/buscar/act.php?id=BOE-A-2015-10565` | Integrates all subsequent legislative amendments, repeals, and Constitutional Court annulments with article-level effective dates. |

---

## 2. Deterministic 3-Step Workflow to Categorize & Apply Public Regulations (`GOV-ES-01..03`) [E1]

> **Exon [E1]:** *Resolve any Spanish compliance question in three deterministic hops: (1) map the activity to `AREA-01..07`, (2) verify normative rank (`E3 > E2 > E1`) and `ISO 3166-2:ES` territorial regime, and (3) anchor the decision with an HMAC-verifiable `citation_receipt`.*

Whenever a project, school/university lab, or enterprise department needs to verify regulatory compliance in Spain, execute these three steps:

1. **Step 1 — Map the Activity to its Competent Ministerial Domain (`AREA-01..07`)**:
   - Consult Section 2 of [01_age_ministerial_organigram_and_competences.md](../reference/01_age_ministerial_organigram_and_competences.md):
     - *Taxation, e-invoicing (`Veri*factu` / `TicketBAI`), or public tenders (`< 15,000` / `< 40,000 EUR`)?* $\rightarrow$ **`AREA-01` (Hacienda)**.
     - *Company incorporation (`SL`), directors' liability, patents, or trade secrets?* $\rightarrow$ **`AREA-02` (Justicia / `OEPM`)**.
     - *Personal data (`RGPD`/`LOPDGDD`), `ENS` cybersecurity, or `AI Act` risk tiering?* $\rightarrow$ **`AREA-03` (Transformación Digital / `AEPD` / `CCN-CERT`)**.
     - *Circular economy (`Art. 4–5 Ley 7/2022`), emissions, water basins, or biodiversity?* $\rightarrow$ **`AREA-04` (`MITECO`)**.
     - *Pressure/thermal equipment (`RD 809/2021`), R&D credits, or `LOMLOE`/`LOSU` curricula?* $\rightarrow$ **`AREA-05` (`MINTUR` / `MICIU`)**.
     - *Employment contracts, occupational safety (`LPRL`), or lab chemical/biological agents?* $\rightarrow$ **`AREA-06` (`MITES` / `INSST`)**.
     - *Consumer `3`-year warranty (`TRLGDCU`), food-contact materials, or plant health?* $\rightarrow$ **`AREA-07` (`Sanidad` / `Consumo` / `MAPA`)**.
2. **Step 2 — Check Normative Rank (`Art. 9.3 CE`) & Competence Matrix (`Art. 148/149 CE` + `geo-es`)**:
   - Verify in [01_constitutional_hierarchy_and_state_powers.md](../architecture/01_constitutional_hierarchy_and_state_powers.md) whether the matter is Exclusive State (`Art. 149.1.6ª/7ª/9ª`) or Shared Basic State + `CCAA` Additional Protection (`Art. 149.1.23ª` environment, `Art. 149.1.16ª` health), and check `ISO 3166-2:ES` for Foral (`ES-PV`, `ES-NC`) or Canary (`ES-CN`) fiscal rules.
3. **Step 3 — Query via `rcap1` (`L1 -> L3`) and Seal a `citation_receipt`**:
   - Query `gov-es` at compact `L1` resolution first, unfold only the target section to `L3` when drafting binding gates, and store the `citation_receipt`:

```bash
# Compact L1 discovery across gov-es (~85% token savings)
make consult LAYER=gov-es QUERY="Contratos Menores LCSP"
```

---

## 3. Progressive `M1 -> M4` Consumer Adaptation Matrix [E1]

> **Exon [E1]:** *The same authoritative `gov-es` corpus serves secondary/university students (`M1..M2`), engineering/finance leads (`M3`), and fiduciary legal auditors (`M4`) without duplicating statutory truth.*

The table below shows how `ZeroCloudGravity` adapts disclosure depth across operator mastery levels:

| Mastery Level | Target Persona | Primary `gov-es` Entry Point & Resolution | Practical Outcome in the Consumer Workspace |
| :--- | :--- | :--- | :--- |
| **`M1`** | Secondary / High School Civic Education Student | `docs/guides/` (`L1` / `L2`) + Section 1 of [01_constitutional_hierarchy_and_state_powers.md](../architecture/01_constitutional_hierarchy_and_state_powers.md) | Understands separation of powers (`Cortes`, `Gobierno`, `Jueces`, `TC`), Fundamental Rights, and the `17 CCAA + 2 Cities` model. |
| **`M2`** | Law / Public Admin Undergraduate or Startup Founder | Section 2 of [01_constitutional_hierarchy_and_state_powers.md](../architecture/01_constitutional_hierarchy_and_state_powers.md) + `AREA-01..03` (`L2`) | Distinguishes `Ley Orgánica` (`176` deputies) vs. `RD-Ley` (`30` days), `SL` incorporation (`Ley 18/2022`), and `LPACAP` `10`-day deadlines. |
| **`M3`** | Departmental Lead (`dept-iso-finance`, `dept-iso-eng`, `dept-iso-bio`) | Full `AREA-01..07` & Quantitative Cut-Points in [01_age_ministerial_organigram_and_competences.md](../reference/01_age_ministerial_organigram_and_competences.md) (`L2 -> L3`) | Binds software/hardware/financial acceptance tests (`N` vs. `N ± 1`) directly to `LCSP`, `LOPDGDD`, `ENS`, `RD 809/2021`, and `Ley 7/2022`. |
| **`M4`** | General Counsel, DPO, or Public Compliance Officer (`dept-iso-legal`) | Full `E3` Competence Matrix (`Art. 148/149.1/149.3 CE`) + Cross-Layer `citation_receipt` Audit (`L3`) | Enforces fiduciary `precedence: 5` legal vetoes and audits `CITATION_DRIFT_DETECTED` whenever `gov-es` updates consolidated `BOE` digests. |
