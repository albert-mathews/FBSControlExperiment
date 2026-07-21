# Grok session bootstrap — FBS / CPE / Isolation paper

**Read this file first** in any new session in this repo.  
**Author:** Albert Mathews  
**Repo:** `FBSControlExperiment`  
**Last updated:** 2026-07-21  

Deeper backups: `HANDOFF.md` (ontology stack), `P2_research.md` / `P2_synthesis.md` (history protocol + findings), `control-cultures.md` (control tiers), `DRAFT.md` (working narrative).

---

## 1. What we are writing

**One combined paper** (not two separate articles), with two supporting layers under one pipeline thesis:

1. **Detection layer (this repo’s empirical core):** Under standard virus Isolation practice, **cytopathic effect (CPE)** is not a virus-specific detector because culture systems jointly change **inoculum** and **serum/nutrient enrichment** (typically growth ~10% FBS → maintenance ~1–3% / 2% FBS), while reading CPE as proof of virus.
2. **Particle layer (EV literature synthesis):** Field consensus that EVs and “virions” are not cleanly separable by physical purification/EM is **what you would expect** if the culture step never uniquely grounded a second particle class.

**Hinge sentence (keep):**

> EV indistinguishability is not a late technical annoyance — it is what you would expect if the “second particle class” (virions) was never observationally grounded in the first place.

**Capitalized Isolation:** virology’s operational product of culture / CPE / passage (an **Isolate**). Does **not** mean chemical purity.

**Target venue spirit:** methods-critical, evidence-first (PLOS-style process critique). Prefer process and controls over slogans.

---

## 2. Argument spine (reader-facing order)

Use this as the paper’s logical order (refined in session; supersedes older “three pillars + contagion” framing):

1. Institutional Isolation protocol is largely **uniform**: dual media + CPE as primary viral effect; roots in mid-century culture operability (Enders-era tradition), later **codified**.
2. Institutions prescribe **lower serum/enrichment at/near infection** and (in principle) **parallel negative controls**.
3. Isolation **publications** largely **follow** the FBS/enrichment reduction (corpus evidence).
4. Isolation **publications** often **do not** implement **audit-able** Isolation-stage negative controls (control tiers A–D).
5. **Rationales** for serum drop are **heterogeneous** (attachment, overgrowth, inhibitors, none) → no single evidence-based consensus; practice looks **empirically locked** for readable CPE/Isolates.
6. Historical interest (**P2**): what does the published record say about serum/nutrient use from ~1900 until institutional prescription? No required “win” outcome.
7. Proper negative control = same maintenance/FBS step, **no virus**.
8. **CRO experiment:** no virus; 10% vs 2% FBS → CPE-like morphology (CLSI-mapped; Zenodo data).
9. Therefore CPE under Isolation conditions is **not virus-specific**; CPE-based Isolation/titer are not standalone proof of a discrete viral agent in culture.
10. **Prediction P1:** purification/EM of culture products will not uniquely define a second particle class → **EV literature**.
11. **Prediction / interest P2:** published history of medium practice should be reconstructable (and was searched without forcing a story).
12. Field should re-examine practices and claims that **inherit** confounded Isolation endpoints (process critique, not “virology is false”).

**Do not overclaim:** Non-specificity of CPE ≠ proof that “nothing infectious exists.” Scope: *inside classical Isolation–CPE–purify practice…*

---

## 3. Mindset for research and drafting

### Epistemic stance

- **There is no right or wrong outcome to hunt for** on history (P2) or control prevalence — only what the record shows.
- Prefer **process critique** over slogans.
- State premises so critics attack **empirical links**.
- **Quote-backed** claims; no inventing methods from “standard practice.”
- **Negative findings** and **counterexamples** are results (log them).
- Ambiguity → **worse/more conservative** tier or “unknown,” not optimistic upgrade.

### Isolation control tiers (`control-cultures.md`)

| Tier | Meaning |
|------|---------|
| **A** | Isolation-stage negative culture control + matched conditions (M1–M6), including serum/enrichment |
| **B** | Isolation-stage NC named but match not verifiable |
| **C** | NC exists but wrong stage and/or explicit mismatch |
| **D** | No culture-level NC for Isolation/infection work |

Decision tree, forbidden guesswork, and serum special rule are codified in `control-cultures.md`. Results: `control-cultures-overview.csv` + `control-cultures-justification-notes.md` (agent reviews applied).

### P2 historical research (`P2_research.md`)

- Window: ~**1900 → institutional prescription** of dual growth/maintenance (not pre/post-Enders by design).
- Variable: **serum/nutrient enrichment** broadly (not only “FBS %”).
- Multi-round search; every citation **screened** (Y/B/N); useful rows extracted; quotes in `P2_quotes.md`.
- End markers (Schmidt 1969, CLSI, ATCC, ASM…) end the *evolution* search; later texts mainly transmit.

### Writing style

- Precise, complete sentences; tables for parallel facts.
- **Isolation** capital-I when meaning the virological operation.
- Cite corpus IDs (VI##, P2-###) for traceability.
- Draft lives in `DRAFT.md` (incomplete Results/Discussion); final paper may become LaTeX later.

---

## 4. Related repos

| Repo | Path | Role |
|------|------|------|
| **This** | `.../PLOS bio/FBSControlExperiment` | Empirical Isolation/CPE/FBS + history + draft |
| **EV** | `.../PLOS bio/Cpe2extraCellularVesicles` | EV–virus purification/EM ontology draft; cite as particle layer |

Do not re-derive full EV biogenesis here; do not re-prove CPE in the EV paper.

---

## 5. Status snapshot (2026-07-21)

### Done / strong

| Workstream | Status |
|------------|--------|
| **Thesis / combined paper framing** | Agreed; pipeline not two stapled papers |
| **Institutional guidelines** | ATCC, CLSI M41, ASM CPE, WOAH, NEADL, etc. extracted (`institution-guideline-protocol-refs.*`, `DRAFT.md`) |
| **Isolation literature FBS reduction** | Corpus CSVs + PDFs under `wrk/isolation_practice/` |
| **Control tiers A–D** | Framework + **28/28 PDFs** scored; agent reviews; post-remediation: **A=4, B=6, C=1, D=17** |
| **CRO experiment** | Described in draft; Zenodo dataset; CLSI Table 7 descriptor work (`clsi-table7-descriptors.tex`) |
| **P2 history** | Protocol + multi-round search; **~24 useful** sources; Schmidt **ch.3 1969 full** (screenshots); 1950s dual-medium primaries (e.g. Melnick 10%→serum-free; Li “horse serum inhibitory”; Boyle serum toggles CPE) |
| **Agent reviews** | `agent1_review.md` … `agent3_review.md` on control tiers |

### In progress / thin

| Workstream | Gap |
|------------|-----|
| **DRAFT.md** | Results/Discussion incomplete; needs tables/figures from corpora |
| **Control corpus** | User may still re-check agent-remediated tiers |
| **P2** | Optional more primaries (leads P2-044–050); synthesis counts slightly stale vs latest CSVs |
| **EV section** | Not yet fully drafted into this paper’s Discussion |
| **Zenodo / README** | Placeholder link still empty in README |

### Isolation control tier summary (post-remediation)

| Tier | n | Role in argument |
|------|---|------------------|
| A | 4 | Rare audit-able matched Isolation-stage NC |
| B | 6 | Mock named, conditions under-specified |
| C | 1 | Wrong-stage NC only (VI25) |
| D | 17 | No culture NC described |

### P2 headline patterns (provisional)

1. Early culture used **constrained enrichment** (ultrafiltrate, hydrolysates), not only rich whole serum.  
2. Mid-century: **simplify** media; **serum can inhibit** virus/CPE readability.  
3. Explicit **growth (high serum) → maintenance (low/no serum)** by early 1950s (e.g. Melnick) and fully **recipe-codified** by Schmidt 1969 (often **2% FBS**).  
4. Heterogeneous practice remains (high-serum “maintenance,” serum-free infection that *creates* CPE — Boyle RVF).  
5. No single published experiment that deconfounds serum-as-IV on uninoculated monolayers to *found* Isolation CPE specificity.

---

## 6. Key file map

| Path | Use |
|------|-----|
| `grok.md` | **This file** — session start |
| `HANDOFF.md` | Ontology layers 0–3; EV link |
| `DRAFT.md` | Working paper prose |
| `control-cultures.md` | A–D framework |
| `control-cultures-overview.csv` | Tier scores |
| `control-cultures-justification-notes.md` | Quote-backed justifications |
| `isolation-refs-overview.csv` | Isolation paper FBS pre/post |
| `isolation-refs-endpoint-analysis-filtering.md` | CPE endpoint filter notes |
| `institution-guideline-protocol-refs.md` | Guideline mapping |
| `P2_research.md` | History search protocol |
| `P2_search_log.md` | Round-by-round queries |
| `P2_screened.csv` / `P2_useful.csv` | History screen + extract |
| `P2_quotes.md` | Verbatim historical quotes |
| `P2_synthesis.md` | History findings for Discussion |
| `references.bib` | Bibliography (partial) |
| `wrk/isolation_practice/` | Isolation paper PDFs |
| `wrk/isolation_protocols/` | Guideline PDFs |
| `wrk/p2_history/` | Historical PDFs + `_notes/` extracts |
| `wrk/virus_EV_indistinguishable_refs/` | EV PDFs (also in EV repo) |

---

## 7. Empirical anchors (do not lose)

### CRO (no virus)

- Vero E6 (ATCC CRL-1586); Path A **10%** FBS vs Path B **2%** FBS.  
- Light microscopy + TEM; Zenodo: `https://doi.org/10.5281/zenodo.17928456`  
- CLSI M41 Table 7 descriptors for CPE-like language.  
- Automated labeling failed; rely on CRO-described image subset for correlation claims.

### Confound structure

| Independent | Dependent |
|-------------|-----------|
| Inoculum yes/no | CPE / “viral” morphology |
| FBS / maintenance conditions | |

### Institutional end markers (modern)

- CLSI M41-A: growth ~10%, maintenance 1–3%, CPE primary.  
- ATCC: lower viral serum; NOTE 5 → **2%** (attachment).  
- ASM CPE protocol: maintenance **2%** serum + uninoculated well.  
- Schmidt 1969 ch.3: growth **10–20%** → maintenance **~2%** or serum-free (full chapter in `wrk/p2_history/P2-008...`).

---

## 8. How to start a new session

1. Read **`grok.md`** (this file).  
2. If work is **controls:** open `control-cultures.md` + overview CSV + justification notes.  
3. If work is **history:** open `P2_research.md` + latest `P2_useful.csv` / `P2_quotes.md`.  
4. If work is **drafting:** open `DRAFT.md` + this spine (§2).  
5. If work is **EV particle layer:** read `HANDOFF.md` Layer 2–3; optionally switch to EV repo.  
6. Prefer **updating existing CSVs/notes** over reinventing frameworks.  
7. When scoring papers: **quotes the user can search**; conservative tiers.

### Opening prompt templates

**Continue draft:**
```text
Read grok.md and DRAFT.md. Advance the paper draft using the argument spine;
integrate control-tier table and P2 historical findings without overclaiming.
```

**Continue controls:**
```text
Read grok.md and control-cultures.md. [task on isolation control scoring]
```

**Continue P2:**
```text
Read grok.md, P2_research.md, and P2_synthesis.md. Process new PDFs in wrk/p2_history/
or continue search leads P2-044–050.
```

---

## 9. Guardrails (rhetorical)

1. Attack: confounded design; weak controls; non-discriminating purification — not “all of virology is a conspiracy.”  
2. **Inheritance:** titers, Isolates, stocks, and particle claims that rest only on confounded CPE inherit uncertainty.  
3. Scope claims with **“under standard Isolation/maintenance conditions.”**  
4. One Vero E6 CRO is **preliminary**; generalize carefully.  
5. EV section = field consensus synthesis + logical prediction, not a new wet purification of uninoculated vs inoculated unless we run it.  
6. History: **descriptive patterns** first; “consistent with lock-in” only lightly in Discussion.

---

## 10. Suggested next work (priority order)

1. **User review** of control-tier scores (optional freeze).  
2. **Paper tables/figures:** isolation FBS pre/post; control tiers A–D; institutional rationale matrix; P2 timeline of medium practice.  
3. **Advance `DRAFT.md`:** Methods (CRO + corpora), Results (tables), Discussion (P1 EV + P2 history + inheritance).  
4. Optional P2 PDFs: Baron & Low 1958 (**P2-048**, PMID 13568747); Youngner 1954 (**P2-046**, PMID 13155547); Weller *J Immunol* 1952 (**P2-045**, PMID 13022978).  
5. Wire short **EV subsection** from EV-repo refs.  
6. Fill Zenodo link in README when ready.

---

## 11. Glossary

| Term | Meaning here |
|------|----------------|
| **Isolation** | Operational culture recovery / detection (CPE-centered) |
| **Isolate** | Product of Isolation (not pure substance) |
| **CPE** | Cytopathic / cytopathogenic effect |
| **Maintenance medium** | Post-growth / infection medium, usually lower enrichment |
| **P1** | Prediction: particle purification non-discriminating → EV literature |
| **P2** | Historical interest: published evolution/lock-in of medium practice |
| **Tier A–D** | Quality of Isolation-stage negative culture controls |

---

*End of bootstrap. Update the status section when major workstreams change.*
