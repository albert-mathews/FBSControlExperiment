# P2 synthesis (provisional)

**Date:** 2026-07-20  
**Protocol:** `P2_research.md` v0.1  
**Artifacts:** `P2_search_log.md`, `P2_screened.csv` (40 rows), `P2_useful.csv` (16 rows), `P2_quotes.md`  
**Status:** Provisional after Rounds 0–4 + **Round 6 user PDF ingestion**. **Not** claimed as bibliographic saturation. Further rounds can reopen under protocol §10.

### Round 6 update (user PDFs in `wrk/p2_history/`)

Full-text re-extracts raised confidence for **P2-001, P2-002, P2-005, P2-015, P2-017**. New user IDs:

| ID | Paper | P2 relevance |
|----|--------|----------------|
| **P2-200** | Smith SE 1961 *A Maintenance Medium for Tissue Culture Virus Studies* | Explicit definition of **maintenance medium** as virus-study medium; **serum-free** liver-digest ultrafiltrate in Earle BSS; cells **grown** on lactalbumin + serum |
| **P2-201** | Hsiung GD 1961 primary cell cultures review | **2% horse serum** can **inhibit** polio plaques; protein-free overlays discussed — supports “serum can interfere” lineage |

**P2-017 confirmed counterexample:** growth **20%** sheep serum → maintenance **10%** sheep serum (still high; not modern 2%).

### Round 7 update (more user PDFs + re-search)

| User file | Canonical | Finding |
|-----------|-----------|---------|
| **P2-04** | **P2-004** Melnick & Riordan 1952 | **Protein-free** lactalbumin medium; Hanks–Simms + Simms ultrafiltrate + lactalbumin; serum/embryo extract **replaced**; CPE still used; uninoculated controls imaged |
| **P2-203** | **P2-018** Boyle 1964 RVF | Growth **199 + 10% calf serum** → **serum-free maintenance** for titration; **CPE appears when serum is omitted**; with serum, RVF can grow **without** obvious CPE; plaques still need serum in overlay |
| **P2-204** | **P2-035** Rosenbaum ~1963 | Growth **MEM + 10% FCS**; MACRO maintenance **MEM + 5% horse serum**; microtitration keeps growth medium |
| **P2-036** PDF | notice only | AJPH book notice of Lennette/Schmidt 4th ed — **not** full methods chapter |
| **P2-020** | Hematian 2016 | Re-confirmed **no** serum recipe |

**Strongest new interpretive point (Boyle):** medium enrichment can **toggle whether CPE is the readable endpoint** for the same virus — not only “help cells live longer.” That is directly relevant to non-specificity / confounded endpoints under Isolation conditions.

**Re-search leads still needing PDFs:** Li & Schaeffer 1953 (*Science*) **P2-042**; Melnick–Opton assay methods with **2% calf serum** snippet **P2-043**.

### Round 8 — Full Schmidt Chapter 3 (P2-008) — major end-marker locked

User supplied **entire** Ch. 3 (*Tissue Culture Technics for Diagnostic Virology*, 4th ed. 1969, book pp. ~79–178) as screenshots. Readable.

**Institutional dual-medium pattern is explicit and quantitative by 1969:**

| Role | Typical serum (Schmidt recipes) |
|------|----------------------------------|
| Growth | **10–20%** FBS (or 5% bovine for monkey kidney; 10% human serum for some continuous lines) |
| Maintenance / viral propagation | **Serum-free preferred**, else **~2% FBS** (or **5%** for some continuous-line maintenance mixes); L-15 + **2% FBS** for some respiratory viruses |
| Transition | Remove growth medium **before virus**; wash BSS if growth serum may contain inhibitors |

Also: CPE as main Isolation readout; **uninoculated control tubes** for spontaneous/nonspecific degeneration; toxic clinical inocula can cause non-viral degeneration.

This is the cleanest pre-CLSI **diagnostic** codification of the growth/maintenance split we have found. Combined with Melnick protein-free work and Boyle’s serum-dependent CPE, P2 historical layer is now strong enough for paper use with remaining gaps noted as optional.

---

## 1. What was asked

How serum / nutrient enrichment was used in virus tissue and cell culture from ~1900 until institutional protocols prescribed a dual growth/maintenance (often low-serum) recipe — without requiring a preferred evolutionary story.

---

## 2. Search effort (counts)

| Item | n |
|------|---|
| Screened IDs | 42 |
| Useful (Y) | 18 |
| Borderline (B) | 15 |
| Not useful (N) | 9 |
| (Y+B+N) | 42 |
| Explicit counterexample useful rows | ≥2 (P2-017 high-serum maintenance; P2-018 serum-free infection medium) |
| End-marker institutional sources | CLSI M41, ATCC guide, ASM CPE protocol, UK SMI V_39, Lennette/Schmidt diagnostic manuals |

Databases/tools used: web search (PubMed-like indexes via Scholar/web), PMC snippets, ATCC web guide, Nobel PDF full text, project in-repo protocols, WHO IRIS / DTIC snippets.

**Limits (honest):** Many 1950s primary PDFs remain paywalled or incomplete OCR; several useful rows are medium-confidence. Non-English literature not systematically processed. Cumitech / full Lennette-Schmidt chapter text not fully extracted.

---

## 3. Descriptive patterns (with IDs)

### Pattern A — Early operable virus culture used **non-whole-serum / reduced-protein** fluids and long observation

- **P2-001/P2-003:** BSS + **ox serum ultrafiltrate**; frequent medium replenishment; multi-week viability; CPE and pH endpoints.  
- Not yet the modern “10% FBS → 2% FBS” label, but **enrichment is already constrained** relative to rich whole-serum growth systems.

### Pattern B — Mid-century methods actively **strip or simplify protein/serum** for polio TC

- **P2-004:** Melnick & Riordan **protein-free** nutrient media replacing serum–embryo-extract proteins (lactalbumin hydrolysate path).  
- Shows published **optimization of medium composition** for virus culture success, not only silent tradition.

### Pattern C — Dual **growth vs maintenance** language is present by the diagnostic era and later textbooks state it as settled

- **P2-035 (1963):** tube cultures “changed to maintenance.”  
- **P2-015:** after ~3 days → maintenance with **1% serum or serum-free**.  
- **P2-009 (Fenner textbook):** FCS **5–10%** for growth; after monolayer + inoculation → maintenance with **little or no serum**.  
- **P2-010/011/012/016:** modern institutional codification **10% → ~2%** (or 1–3%), with **heterogeneous rationales** (overgrowth, inhibitors, attachment, or none).

### Pattern D — **Heterogeneous practice** in-window (counterexamples)

- **P2-017 (1961):** “maintenance medium” still **10% sheep serum** (vaccinia / sheep kidney).  
- **P2-018 (1964):** **serum-free** maintenance for RVF inoculation.  
- Together: “maintenance” does **not** always mean modern 2% FBS; the word is older and broader.

### Pattern E — We did **not** find a single continuous, famous experimental series that *only* titrates serum % on matched uninoculated monolayers to invent Isolation CPE specificity

- No screened source in this pass is a clean “serum-as-sole-IV on uninfected cells” foundation for the Isolation recipe.  
- Absence is **informative for methods genealogy**, not proof of absence of all lab notebooks.

### Pattern F — Institutional **end markers** (window upper bound)

By the time of widely used diagnostic manuals and later CLSI/ATCC/ASM-type documents, the dual-medium / low-serum maintenance pattern is **prescribed**, not argued as a new discovery:

| Marker | Role |
|--------|------|
| Lennette & Schmidt diagnostic procedures (1960s–69 chapter lineage) | Diagnostic TC technics codification |
| CLSI M41-A (2006) | Explicit 10% vs 1–3% + CPE |
| ATCC Virology Guide | Lower viral serum; NOTE 5 → 2% attachment |
| ASM CPE protocol | Maintenance 2% serum + uninoculated well |
| UK SMI V_39 | Growth 10% / maintenance 2% tables |

For the paper: **evolution search ends at first clear prescription wave**; later sources mainly **transmit**.

---

## 4. Consistency with the P2 “interest” (light interpretation)

| Interest element | Provisional fit |
|------------------|-----------------|
| Reduced enrichment at infection appears before today’s brand-name 2% FBS | **Supported** (ultrafiltrate, protein-free media, maintenance little/no serum language) |
| A neat published high→low FBS titration inventing the recipe | **Not found** in this pass |
| Practice becomes **institutional prescription** | **Supported** (end markers) |
| Single evidence-based rationale across history | **Not supported** (attachment vs overgrowth vs inhibitors vs none; high-serum “maintenance” still appears) |
| Empirical lock-in selected on culture endpoints | **Plausible / consistent** with early CPE operability + medium simplification, but **not proven** as a documented selection experiment |

**Bottom line for the paper:**  
The published record is **compatible with early embedding of reduced/simpler enrichment for long culture observation**, later **codified** as growth vs maintenance (often ~2% serum), with **heterogeneous practice and rationales**. It does **not** supply a clean, deconfounded experimental origin story for low-FBS CPE Isolation. That is a legitimate historical finding, not a failed search.

---

## 5. What remains open (next rounds if reopened)

1. Full-text extraction of Melnick 1952/53, Dulbecco 1954 methods sections, Schmidt 1969 chapter.  
2. Systematic 1950–1965 *J Immunol / PSGBM / J Exp Med* full-text scan for “maintenance medium” + % serum.  
3. Non-English (French/German Japanese diagnostic manuals).  
4. Pre-1940 vaccinia/yellow fever TC medium recipes (P2-025/026 borderline).  
5. Independent replication pass: second operator re-runs Family B/D queries only.

---

## 6. Relationship to main empirical paper

P2 is **contextual**. It does not replace:

- CRO serum-only control  
- Isolation corpus FBS reduction prevalence  
- Control-tier A–D results  
- EV particle-layer synthesis  

Use this synthesis in Discussion as: *historical embedding and institutionalization of medium practice*, with limits stated.

---

*Provisional synthesis end.*
