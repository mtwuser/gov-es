---
epistemic_grade: E3
---

# Constitutional Hierarchy, State Powers & Normative Pyramid (`gov-es` — `E3`)

> **Epistemic Credibility Grade: `E3` (Supreme Constitutional & Statutory Law — Non-Overridable Primary Truth)**
>
> This architecture specification codifies the structural organization of the **Constitución Española de 1978 (`BOE-A-1978-31229`)**, the separation of state powers, the competence distribution matrix (`Art. 148` vs. `Art. 149.1 CE`), and the Spanish normative hierarchy (`Art. 9.3 CE`) for deterministic legal routing across consumer layers ([01_age_ministerial_organigram_and_competences.md](../reference/01_age_ministerial_organigram_and_competences.md)).

---

## 1. Structure of the Spanish Constitution of 1978 (`BOE-A-1978-31229`) [E3]

> **Exon [E3]:** *The Spanish Constitution (`Art. 1–169 CE`, `BOE-A-1978-31229`) is the supreme norm binding all citizens and public authorities (`Art. 9.1 CE`), organized into a Preliminary Title and 10 Titles separating Legislative (`Cortes Generales`), Executive (`Gobierno y Administración`), Judicial (`Poder Judicial`), and Constitutional (`Tribunal Constitucional`) powers.*

The table below maps every constitutional block of the `CE 1978` to its institutional authority, core legal guarantees, and downstream regulatory substrate:

| Constitutional Block | Articles (`CE`) | Institutional & Substantive Scope | Core Legal Principles & Consumer Application |
| :--- | :--- | :--- | :--- |
| **Título Preliminar** | `Art. 1–9` | Social and democratic Rule of Law (*Estado social y democrático de Derecho*), national sovereignty (`Art. 1.2`), parliamentary monarchy (`Art. 1.3`), and **`Art. 9.3` guarantees** | **Normative Hierarchy (`Jerarquía Normativa`)**, legality, publicity of norms (`BOE`), non-retroactivity of unfavorable sanctions, legal certainty (*seguridad jurídica*), and prohibition of arbitrariness. |
| **Título I** | `Art. 10–55` | Fundamental Rights (`Art. 15–29`), Citizens' Rights (`Art. 30–38`) & Guiding Socio-Economic Principles (`Art. 39–52`) | Human dignity (`Art. 10.1`), equality (`Art. 14`), data privacy & digital rights (`Art. 18.4` $\rightarrow$ `RGPD`/`LO 3/2018`), freedom of enterprise (`Art. 38`), health protection (`Art. 43`), and environmental stewardship (`Art. 45` $\rightarrow$ `Ley 7/2022`). |
| **Título II** | `Art. 56–65` | **The Crown (`La Corona`)** — Head of State | Symbolic unity and permanence of the State (`Art. 56.1`), sanction and promulgation of laws (`Art. 62.a`), and countersignature requirement (*refrendo*, `Art. 64`). |
| **Título III** | `Art. 66–96` | **Cortes Generales — Legislative Power (`Congreso de los Diputados` & `Senado`)** | Bicameral legislative authority (`Art. 66.2`), enactment of **Leyes Orgánicas (`Art. 81`)**, **Leyes Ordinarias**, legislative delegation (`Art. 82` `RDLeg`), urgency decrees (`Art. 86` `RDL`), and international treaties (`Art. 93–96`). |
| **Título IV & V** | `Art. 97–116` | **Government & Public Administration (`Título IV`)** and Parliamentary Accountability (`Título V`) | **`Art. 97`**: Executive direction and regulatory power (*potestad reglamentaria*). **`Art. 103.1`**: Objective service under efficacy, hierarchy, decentralization, and full submission to Law ([01_age_ministerial_organigram_and_competences.md](../reference/01_age_ministerial_organigram_and_competences.md)). |
| **Título VI** | `Art. 117–127` | **Judicial Power (`Poder Judicial` — governed by `CGPJ`, `LOPJ 6/1985`)** | Jurisdictional exclusivity and independence (`Art. 117.1–3`), free justice where provided by law (`Art. 119`), and Public Prosecutor legality defense (*Ministerio Fiscal*, `Art. 124`). |
| **Título VII** | `Art. 128–136` | **Economy & Public Finance (`Economía y Hacienda`)** | Equitable progressive tax system (`Art. 31` & `Art. 133` $\rightarrow$ `Ley 58/2003 LGT`), General State Budgets (`Art. 134` `PGE`), budgetary stability (`Art. 135`), and *Tribunal de Cuentas* (`Art. 136`). |
| **Título VIII** | `Art. 137–158` | **Territorial Organization of the State (`Estado Autonómico`)** | Municipalities (`Art. 140`), Provinces (`Art. 141`), and **17 Autonomous Communities + 2 Autonomous Cities (`Art. 143–158`, `geo-es`)**; competence distribution under `Art. 148` and `Art. 149.1`. |
| **Título IX & X** | `Art. 159–169` | **Constitutional Court (`TC`, `LOTC 2/1979`)** & **Constitutional Reform (`Título X`)** | Unconstitutionality appeals (`Art. 161.1.a`), *recurso de amparo* (`Art. 53.2`, `Art. 161.1.b`), competence conflicts (`Art. 161.1.c`), and ordinary (`Art. 167`, `3/5`) vs. aggravated (`Art. 168`, `2/3` + dissolution + referendum) reform. |

---

## 2. The 5-Tier Spanish Normative Pyramid (`GOV-ES-01`) [E3]

> **Exon [E3]:** *Under `Art. 9.3 CE` and `Art. 1.2` of the Civil Code, any provision contradicting a higher-ranking norm is null and void (`Lex Superior Derogat Inferiori`), while state vs. autonomous norms interact strictly by material competence (`Principio de Competencia`, `Art. 148–150 CE`).*

All legal instruments indexed in `gov-es` map deterministically onto five hierarchical ranks and parliamentary cut-points:

1. **Tier 1 (`E3` — Supreme Constitutional & EU Primary Law)**:
   - **Constitución Española (`BOE-A-1978-31229`)** and **European Union Primary Law (`TUE`, `TFUE`)** plus directly applicable **EU Regulations (`Art. 288 TFUE`, `Art. 93 CE`)** under the principle of primacy of EU law within transferred competences.
2. **Tier 2 (`E3` — Primary Parliamentary Statutes & Norms with Force of Law / *Rango de Ley*)**:
   - **Ley Orgánica (`LO`, `Art. 81 CE`)**: Requires **absolute majority of the Congress (`>= 176` of `350` deputies)** in a final vote on the entire draft (`N = 176` pass vs. `N - 1 = 175` rejection); strictly reserved for fundamental rights (`Art. 15–29 CE`), Statutes of Autonomy, and the general electoral regime (`LOREG 5/1985`, `LOPDGDD 3/2018`).
   - **Ley Ordinaria (`Ley`)**: Enacted by simple majority of present members in Congress and Senate (or Plenary/Commission under `Art. 75 CE`).
   - **Real Decreto Legislativo (`RDLeg`, `Art. 82–85 CE`)**: Government-enacted consolidated text (*texto refundido*) or articulated text under explicit parliamentary delegation (never allowed on `Ley Orgánica` matters).
   - **Real Decreto-Ley (`RDL`, `Art. 86 CE`)**: Provisional urgency decree in cases of *extraordinaria y urgente necesidad*; cannot affect basic State institutions, Title I rights, CCAA regimes, or electoral law, and **must be expressly validated or repealed by Congress within `30` business days (`N <= 30`)** of promulgation.
   - **Leyes Autonómicas (`CCAA`)**: Enacted by the `17` Unicameral Autonomous Parliaments within their Statute of Autonomy competences; relate to State laws via **competence (`Art. 148/149`)**, not subordination.
3. **Tier 3 (`E2` — Supreme Executive Regulations / *Reglamentos Ejecutivos*)**:
   - **Real Decreto (`RD`)** approved by the Council of Ministers (*Consejo de Ministros*) or the President of the Government (`Art. 97 CE` & `Art. 24.1 Ley 50/1997 del Gobierno`), plus Autonomous **Decretos** of CCAA Governing Councils.
4. **Tier 4 (`E2` — Departmental & Local Ordinances)**:
   - **Orden Ministerial (`OM`)** (`Art. 4.1.b` & `Art. 24.1.f Ley 50/1997`), Autonomous *Órdenes de Consejería*, and Municipal *Ordenanzas Locales* / *Reglamentos Orgánicos* (`Ley 7/1985 LRBRL`).
5. **Tier 5 (`E1` — Administrative Instructions, Technical Guides & Soft Law)**:
   - **Resoluciones, Instrucciones y Circulares** (`Art. 6 Ley 40/2015 LRJSP`) issued by Secretaries of State or Directorates-General, `AEPD`/`CCN-CERT`/`INSST` technical guides, and adaptive `M1..M4` explanations ([01_statutory_compliance_and_boe_navigation_guide.md](../guides/01_statutory_compliance_and_boe_navigation_guide.md)).

---

## 3. Constitutional Competence Distribution Matrix (`Art. 148` vs. `Art. 149.1` vs. `Art. 149.3 CE`) [E3]

> **Exon [E3]:** *When resolving multi-layer regulatory applicability across Spain (`gov-es` + `geo-es`), verify whether the subject is Exclusive State (`Art. 149.1`), Shared Basic State Legislation + CCAA Development/Execution, or Devolved CCAA Competence (`Art. 148` & Statutes of Autonomy).*

The table below codifies the three constitutional competence regimes governing operational compliance in Spain:

| Competence Regime (`CE 1978`) | Constitutional Anchor | Normative & Executive Authority | Representative Subject Areas (`AREA-01..07`) |
| :--- | :--- | :--- | :--- |
| **1. Exclusive Full State Competence** *(Legislation + Execution)* | `Art. 149.1` (`1ª, 3ª, 6ª, 8ª, 9ª, 10ª, 14ª`) | `Cortes Generales` + `AGE` Ministries (`100%` nationwide uniformity) | Nationality/immigration (`2ª`), international relations (`3ª`), Defense (`4ª`), Administration of Justice (`5ª`), **Mercantile, Penal & Penitentiary Legislation (`6ª`)**, **Intellectual & Industrial Property (`9ª` — `OEPM`)**, Customs & Foreign Trade (`10ª`), and General State Finance (`14ª`, subject to Foral/Canary regimes). |
| **2. Shared Competence: State *Bases* + CCAA Development & Execution** | `Art. 149.1` (`13ª, 16ª, 18ª, 23ª, 25ª, 30ª`) | State enacts **Basic Legislation (`E3` minimum floor)**; `CCAA` enact development norms and execute permits/inspections | General economic planning (`13ª`), **Health bases & pharmaceutical products (`16ª`)**, **Common Administrative Procedure & Public Contracts (`18ª` — `Ley 39/2015`, `Ley 9/2017`)**, **Basic Environmental Protection (`23ª` — `Ley 7/2022`, CCAA *normas adicionales de protección*)**, Energy/Mining bases (`25ª`), and Academic Degrees (`30ª`). |
| **3. Exclusive State Legislation + CCAA Execution** | `Art. 149.1` (`7ª, 17ª`) | State holds `100%` legislative monopoly (Laws + Executive Regulations); `CCAA` manage inspection/execution services | **Labor Legislation (`7ª` — `Estatuto de los Trabajadores`, `Ley 31/1995 PRL`)** and Social Security basic legislation (`17ª`). |
| **4. Devolved Autonomous & Municipal Competences** | `Art. 148.1`, Statutes of Autonomy & `Art. 25 LRBRL` | `CCAA` Parliaments/Councils and `8,132` Municipalities (`Ayuntamientos`) | **Urban planning, land use & housing (`Art. 148.1.3ª`)**, agriculture/forestry within economic planning (`148.1.7ª`), regional transport, tourism (`148.1.18ª`), and municipal activity licenses / urban waste collection (`Ley 7/1985`). |

### 3.1. Closing Clause & Residual Rules (`Art. 149.3 CE`)

Under `Art. 149.3 CE`, three closing safeguards resolve any competence gap:
- **Residual Attribution**: Matters not expressly attributed to the State may belong to the `CCAA` by virtue of their Statutes of Autonomy; matters not assumed by Statutes belong to the State.
- **Prevalence Clause (`Cláusula de Prevalencia`)**: State norms prevail in case of conflict over everything not attributed to the exclusive competence of the `CCAA`.
- **Supplementary Clause (`Cláusula de Supletoriedad`)**: State law is, in all cases, supplementary (*supletorio*) to the law of the Autonomous Communities.
