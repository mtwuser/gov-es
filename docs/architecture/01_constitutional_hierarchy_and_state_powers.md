# Constitutional Hierarchy, State Powers & Normative Pyramid (`gov-es` — `E3`)

> **Epistemic Credibility Grade: `E3` (Supreme Constitutional & Statutory Law — Non-Overridable Primary Truth)**
>
> This architecture specification codifies the structural organization of the **Constitución Española de 1978 (`BOE-A-1978-31229`)**, the separation of state powers, and the Spanish normative hierarchy (`Art. 9.3 CE`) for deterministic legal routing across consumer layers.

---

## 1. Structure of the Spanish Constitution of 1978 (`BOE-A-1978-31229` — `E3`)

The Spanish Constitution (`CE`) is the supreme norm of the legal order, organized into a Preliminary Title and 10 Titles (`Art. 1–169 CE`):

| Constitutional Block | Articles (`CE`) | Institutional & Substantive Scope | Core Legal Principles & Consumer Application |
| :--- | :--- | :--- | :--- |
| **Título Preliminar** | `Art. 1–9` | Social and democratic Rule of Law (*Estado social y democrático de Derecho*), national sovereignty, parliamentary monarchy, and **`Art. 9.3` guarantees** | **Normative Hierarchy (`Jerarquía Normativa`)**, legality, publicity of norms, non-retroactivity of unfavorable sanctions, and legal certainty (*seguridad jurídica*). |
| **Título I** | `Art. 10–55` | Fundamental Rights, Public Liberties & Guiding Socio-Economic Principles | Dignity (`Art. 10`), equality (`Art. 14`), data privacy & digital rights (`Art. 18.4` $\rightarrow$ `RGPD`/`LOPDGDD`), freedom of enterprise (`Art. 38`), health (`Art. 43`), and environmental protection (`Art. 45` $\rightarrow$ Circular Economy). |
| **Título II & III** | `Art. 56–96` | The Crown (`Título II`) & **Cortes Generales — Legislative Power (`Título III`: Congreso & Senado)** | Enactment of **Leyes Orgánicas (`Art. 81`)**, **Leyes Ordinarias**, legislative delegation (`Art. 82` Real Decreto Legislativo), urgency decrees (`Art. 86` Real Decreto-Ley), and international treaties (`Art. 93–96`). |
| **Título IV & V** | `Art. 97–116` | **Government & Public Administration (`Título IV`)** and Parliamentary Relations (`Título V`) | **`Art. 97`**: Executive regulatory power (*potestad reglamentaria*). **`Art. 103.1`**: Public Administration serves general interests objectively under efficacy, hierarchy, decentralization, and full submission to Law (`Ley 39/2015` & `Ley 40/2015`). |
| **Título VI & IX** | `Art. 117–127`, `159–165` | **Judicial Power (`Título VI` — `CGPJ`)** & **Constitutional Court (`Título IX` — `TC`)** | Jurisdictional exclusivity (`Art. 117`), prosecutorial legality (`Art. 124`), unconstitutionality appeals (`Art. 161`), and *recurso de amparo* for fundamental rights (`Art. 53.2`). |
| **Título VII** | `Art. 128–136` | **Economy & Public Finance (`Economía y Hacienda`)** | Equitable tax system (`Art. 31` & `Art. 133` $\rightarrow$ `LGT 58/2003`), General State Budgets (`Art. 134` `PGE`), budgetary stability (`Art. 135`), and Court of Audit (`Art. 136` *Tribunal de Cuentas*). |
| **Título VIII** | `Art. 137–158` | **Territorial Organization of the State (`Estado Autonómico`)** | Municipalities (`Art. 140`), Provinces (`Art. 141`), and **17 Autonomous Communities + 2 Autonomous Cities (`Art. 143–158`, `geo-es`)**; competence distribution between CCAA (`Art. 148`) and Exclusive State powers (`Art. 149.1`). |

---

## 2. The 5-Tier Spanish Normative Pyramid (`GOV-ES-01` — `E3 -> E1`)

Under `Art. 9.3 CE` and `Art. 1.2` of the Civil Code (*"Carecerán de validez las disposiciones que contradigan otra de rango superior"*), norms are strictly ordered by rank:

1. **Tier 1 (`E3` — Supreme Law)**: **Constitución Española (`BOE-A-1978-31229`)** and **EU Primary / Directly Applicable Law (`TFUE`, EU Regulations)** (`Art. 93 CE`).
2. **Tier 2 (`E3` — Primary Parliamentary Statutes / *Rango de Ley*)**:
   - **Ley Orgánica (`LO`, `Art. 81 CE`)**: Requires absolute majority of Congress; reserved for fundamental rights (`Art. 15–29 CE`), Statutes of Autonomy (*Estatutos de Autonomía*), and general electoral regime (e.g., `LO 3/2018 LOPDGDD`).
   - **Ley Ordinaria (`Ley`)**, **Real Decreto Legislativo (`RDLeg`, `Art. 82 CE` consolidated texts)**, and **Real Decreto-Ley (`RDL`, `Art. 86 CE`)** (plus Autonomous Community Laws within their `Art. 148/149` competence).
3. **Tier 3 (`E2` — Supreme Executive Regulations)**: **Real Decreto (`RD`)** approved by the Council of Ministers (*Consejo de Ministros*, `Art. 97 CE` & `Art. 24 Ley 50/1997 del Gobierno`).
4. **Tier 4 (`E2` — Departmental Regulations)**: **Orden Ministerial (`OM`)** issued by a Minister within their departmental competence (`Art. 4.1.b Ley 50/1997`).
5. **Tier 5 (`E1` — Administrative Instructions & Technical Guides)**: **Resoluciones, Instrucciones y Circulares** (`Art. 6 Ley 40/2015 LRJSP`) issued by Secretaries of State or Directorates-General, plus `M1..M2` explanatory guides (`docs/guides/`).
