# Grok session bootstrap — FBS / CPE / Isolation paper

**Read this file first** in any new session in this repo.  
**Author:** Albert Mathews  
**Repo:** `FBSControlExperiment`  
**Last updated:** 2026-07-22  

---

## 0. Where to work (agents / sessions)

| Rule | Detail |
|------|--------|
| **Edit the main repo** | Create, edit, rename, and delete files **directly in the main repository checkout** (`…/PLOS bio/FBSControlExperiment`), **not** in a Grok/git worktree unless the user explicitly names a worktree path. |
| **Session start** | Read **this file**, then open the stream’s main markdown (`rN.md` / `pN.md`) for the topic you are working on. |
| **TODOs** | Maintain per-stream TODO lists in that stream’s main markdown (`r1.md`, `r2.md`, `p1.md`, …). Do not invent parallel TODO systems. |
| **Prefer update over reinvent** | Extend existing CSVs, notes, and frameworks rather than replacing them. |

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

## 2. Repo structure

### 2.1 Naming convention

| Prefix | Meaning | Role in the paper |
|--------|---------|-------------------|
| **`r`** | **Research** topic | Empirical work that supports the thesis (corpora, scoring, experiment, labeling). |
| **`p`** | **Prediction** topic | Discussion-side ramifications of the research (history patterns, EV particle layer, genetics inheritance). |

Numbered folders are streams. Each stream has a **main markdown entrypoint** named after the stream (`r2.md`, `p1.md`, …). That file is the first place to look for scope, status, and **TODOs** for that topic.

### 2.2 Top-level layout

```text
FBSControlExperiment/
  grok.md                 ← session bootstrap (this file)
  README.md               ← human-facing repo summary
  tex/                    ← working draft, bibliography, LaTeX helpers
    DRAFT.md
    references.bib
    clsi-table7-descriptors.tex
  r1_isolation_standards_and_practice/   ← Isolation practice + guidelines corpus
  r2_negative_controls/                  ← control-tier scoring of Isolation papers
  r3_image_labeling/                     ← CRO image labeling / CPE descriptors
  p1_history/                            ← P1: historical medium / FBS practice
  p2_virus_EV_indistinguishable_refs/    ← P2: EV–virus particle indistinguishability
  p3_genetics/                           ← P3: sequence / reference inheritance (parked)
```

### 2.3 Stream entrypoints (look here first)

| Stream | Folder | Main file | Topic |
|--------|--------|-----------|--------|
| **R1** | `r1_isolation_standards_and_practice/` | *(add `r1.md` if missing)* | Institutional Isolation protocols + Isolation-paper corpus (FBS pre/post, CPE endpoint filter) |
| **R2** | `r2_negative_controls/` | `r2.md` | Quality/incidence of Isolation-stage negative controls (tiers A–D); uses R1 PDFs |
| **R3** | `r3_image_labeling/` | `r3.md` | Human (or assisted) labeling of CRO microscope images for CPE-like morphology |
| **P1** | `p1_history/` | `p1.md` | **Prediction / interest:** published history of serum–nutrient practice → dual media |
| **P2** | `p2_virus_EV_indistinguishable_refs/` | `p2.md` | **Prediction:** purification/EM will not uniquely define virions vs EVs |
| **P3** | `p3_genetics/` | `p3.md` | **Prediction (parked):** sequence/database inheritance from confounded Isolates |

Supporting artifacts (CSVs, protocols, agent reviews, quote archives) live **inside** the same stream folder as the work they support.

### 2.4 Copyrighted material (`refs/`)

| Rule | Detail |
|------|--------|
| **Location** | PDFs and other copyrighted full texts live only under **`*/refs/`** inside the relevant stream (e.g. `r1_…/refs/isolation_practice/`, `p1_history/refs/`). |
| **Git ignore** | `.gitignore` contains **`*/refs/`**. **Never commit PDFs or other full-text copyrighted works.** |
| **What *is* committed** | Quotes, CSVs, notes, screening logs, and analysis markdown derived from those sources. |
| **Agent duty** | Before adding files under `refs/`, confirm they remain ignored. Never `git add -f` PDFs. Do not paste entire copyrighted PDFs into tracked files. |
| **Local-only** | `refs/` may exist only on the author’s main machine; clones/worktrees without those folders are normal. |

Extracts and notes that *are* tracked (e.g. `p1_history/_notes/`) must stay quote-sized and attributable, not full-text dumps of books/papers.

---

## 3. Argument spine (reader-facing order)

1. Institutional Isolation protocol is largely **uniform**: dual media + CPE as primary viral effect; roots in mid-century culture operability (Enders-era tradition), later **codified**.
2. Institutions prescribe **lower serum/enrichment at/near infection** and (in principle) **parallel negative controls**.
3. Isolation **publications** largely **follow** the FBS/enrichment reduction (**R1** corpus).
4. Isolation **publications** often **do not** implement **audit-able** Isolation-stage negative controls (**R2** tiers A–D).
5. **Rationales** for serum drop are **heterogeneous** → practice looks **empirically locked** for readable CPE/Isolates.
6. Historical interest (**P1**): what does the published record say about serum/nutrient use from ~1900 until institutional prescription? No required “win” outcome.
7. Proper negative control = same maintenance/FBS step, **no virus**.
8. **CRO experiment:** no virus; 10% vs 2% FBS → CPE-like morphology (CLSI-mapped; Zenodo data). **R3** = image-labeling follow-on.
9. Therefore CPE under Isolation conditions is **not virus-specific**; CPE-based Isolation/titer are not standalone proof of a discrete viral agent in culture.
10. **Prediction P2:** purification/EM of culture products will not uniquely define a second particle class → **EV literature**.
11. **Prediction P3 (optional/parked):** sequence and database claims that rest on CPE-defined Isolates inherit under-determination.
12. Field should re-examine practices and claims that **inherit** confounded Isolation endpoints (process critique, not “virology is false”).

**Do not overclaim:** Non-specificity of CPE ≠ proof that “nothing infectious exists.” Scope: *inside classical Isolation–CPE–purify practice…*

---

## 4. Mindset for research and drafting

### Epistemic stance

- **There is no right or wrong outcome to hunt for** on history (P1) or control prevalence — only what the record shows.
- Prefer **process critique** over slogans.
- State premises so critics attack **empirical links**.
- **Quote-backed** claims; no inventing methods from “standard practice.”
- **Negative findings** and **counterexamples** are results (log them).
- Ambiguity → **worse/more conservative** tier or “unknown,” not optimistic upgrade.

### Isolation control tiers (`r2_negative_controls/control-cultures.md`)

| Tier | Meaning |
|------|---------|
| **A** | Isolation-stage negative culture control + matched conditions (M1–M6), including serum/enrichment |
| **B** | Isolation-stage NC named but match not verifiable |
| **C** | NC exists but wrong stage and/or explicit mismatch |
| **D** | No culture-level NC for Isolation/infection work |

Results: `control-cultures-overview.csv` + `control-cultures-justification-notes.md` (agent reviews applied). Corpus PDFs: `r1_…/refs/` (not re-copied into R2).

### P1 historical research (`p1_history/`)

- Entry: `p1.md` (TODOs). Protocol: `P1_research.md`. Findings: `P1_synthesis.md`, `P1_useful.csv`, `P1_quotes.md`.
- Window: ~**1900 → institutional prescription** of dual growth/maintenance.
- Variable: **serum/nutrient enrichment** broadly (not only “FBS %”).
- IDs: **`P1-###`** (screened / useful / notes / PDF filenames).
- PDFs: `p1_history/refs/` (ignored). Notes extracts: `p1_history/_notes/`.

### Writing style

- Precise, complete sentences; tables for parallel facts.
- **Isolation** capital-I when meaning the virological operation.
- Cite corpus IDs (`VI##`, `P1-###`) for traceability.
- Draft: `tex/DRAFT.md` (incomplete Results/Discussion); final paper may become LaTeX later.

---

## 5. Related repos

| Repo | Role |
|------|------|
| **This** (`FBSControlExperiment`) | Empirical Isolation/CPE/FBS + history + draft + predictions |
| **EV** (`Cpe2extraCellularVesicles`) | Longer EV–virus purification/EM draft; cite as particle-layer support for **P2** |

Do not re-derive full EV biogenesis here; do not re-prove CPE in the EV paper.

---

## 6. Status snapshot (2026-07-22)

### Done / strong

| Workstream | Status |
|------------|--------|
| **Thesis / combined paper framing** | Agreed; pipeline not two stapled papers |
| **R1 institutional guidelines** | ATCC, CLSI M41, ASM CPE, WOAH, NEADL, etc. (`institution-guideline-protocol-refs.*`) |
| **R1 Isolation FBS reduction** | Corpus CSVs; PDFs under `r1_…/refs/` |
| **R2 control tiers A–D** | Framework + **28/28 PDFs** scored; agent reviews; post-remediation: **A=4, B=6, C=1, D=17** |
| **CRO experiment** | In draft; Zenodo dataset; CLSI Table 7 work (`tex/clsi-table7-descriptors.tex`) |
| **P1 history** | Protocol + multi-round search; **~24 useful** sources; Schmidt ch.3 1969; 1950s dual-medium primaries |
| **R3 image labeling** | Auto-labeling failed (Zenodo report); human-labeling paths in progress (`r3.md`) |

### In progress / thin

| Workstream | Gap |
|------------|-----|
| **`tex/DRAFT.md`** | Results/Discussion incomplete; needs tables/figures from corpora |
| **R2** | Optional user re-check of agent-remediated tiers |
| **P1** | Optional more primaries (leads P1-044–050); keep synthesis aligned with CSVs |
| **P2** | Framing still weak; needs dedicated reading + Discussion integration |
| **P3** | Parked / optional short Discussion note |
| **README Zenodo** | Paper Zenodo link still placeholder |

### Isolation control tier summary (post-remediation)

| Tier | n | Role in argument |
|------|---|------------------|
| A | 4 | Rare audit-able matched Isolation-stage NC |
| B | 6 | Mock named, conditions under-specified |
| C | 1 | Wrong-stage NC only (VI25) |
| D | 17 | No culture NC described |

### P1 headline patterns (provisional)

1. Early culture used **constrained enrichment** (ultrafiltrate, hydrolysates), not only rich whole serum.  
2. Mid-century: **simplify** media; **serum can inhibit** virus/CPE readability.  
3. Explicit **growth (high serum) → maintenance (low/no serum)** by early 1950s (e.g. Melnick) and fully **recipe-codified** by Schmidt 1969 (often **2% FBS**).  
4. Heterogeneous practice remains (high-serum “maintenance,” serum-free infection that *creates* CPE — Boyle RVF).  
5. No single published experiment that deconfounds serum-as-IV on uninoculated monolayers to *found* Isolation CPE specificity.

---

## 7. Key file map (by stream)

| Path | Use |
|------|-----|
| `grok.md` | **This file** — session start |
| `README.md` | Public/repo summary |
| `tex/DRAFT.md` | Working paper prose |
| `tex/references.bib` | Bibliography (partial) |
| `r1_…/isolation-refs-overview.csv` | Isolation paper FBS pre/post |
| `r1_…/institution-guideline-protocol-refs.md` | Guideline mapping |
| `r1_…/refs/` | Isolation + protocol PDFs (**ignored**) |
| `r2_…/r2.md` | R2 entry + TODOs |
| `r2_…/control-cultures.md` | A–D framework |
| `r2_…/control-cultures-overview.csv` | Tier scores |
| `r3_…/r3.md` | R3 entry + labeling TODOs/status |
| `p1_history/p1.md` | P1 entry + TODOs |
| `p1_history/P1_research.md` | History search protocol |
| `p1_history/P1_screened.csv` / `P1_useful.csv` | Screen + extract |
| `p1_history/P1_quotes.md` / `P1_synthesis.md` | Quotes + synthesis |
| `p1_history/refs/` | Historical PDFs (**ignored**) |
| `p2_…/p2.md` | P2 entry + TODOs |
| `p2_…/p2_HANDOFF.md` | Ontology stack / EV hinge (layers 0–3) |
| `p2_…/refs/` | EV PDFs (**ignored**) |
| `p3_genetics/p3.md` | P3 parked note + TODOs |

---

## 8. Empirical anchors (do not lose)

### CRO (no virus)

- Vero E6 (ATCC CRL-1586); Path A **10%** FBS vs Path B **2%** FBS.  
- Light microscopy + TEM; Zenodo: `https://doi.org/10.5281/zenodo.17928456`  
- CLSI M41 Table 7 descriptors for CPE-like language.  
- Automated labeling failed; rely on CRO-described image subset for correlation claims until R3 advances.

### Confound structure

| Independent | Dependent |
|-------------|-----------|
| Inoculum yes/no | CPE / “viral” morphology |
| FBS / maintenance conditions | |

### Institutional end markers (modern)

- CLSI M41-A: growth ~10%, maintenance 1–3%, CPE primary.  
- ATCC: lower viral serum; NOTE 5 → **2%** (attachment).  
- ASM CPE protocol: maintenance **2%** serum + uninoculated well.  
- Schmidt 1969 ch.3: growth **10–20%** → maintenance **~2%** or serum-free (`p1_history/refs/P1-008…`).

---

## 9. How to start a new session

1. Read **`grok.md`** (this file).  
2. Open the stream main file: `rN.md` or `pN.md` (TODOs live there).  
3. Load the supporting files named in that stream (CSVs, protocol notes, draft sections).  
4. Prefer **updating existing CSVs/notes** over reinventing frameworks.  
5. When scoring papers: **quotes the user can search**; conservative tiers.  
6. File ops: **main repo path only**, unless the user says otherwise.

### Opening prompt templates

**Continue draft:**
```text
Read grok.md and tex/DRAFT.md. Advance the paper draft using the argument spine;
integrate R2 control-tier table and P1 historical findings without overclaiming.
```

**Continue controls (R2):**
```text
Read grok.md and r2_negative_controls/r2.md, then control-cultures.md.
[task on isolation control scoring]
```

**Continue history (P1):**
```text
Read grok.md, p1_history/p1.md, P1_research.md, and P1_synthesis.md.
Process new PDFs in p1_history/refs/ or continue search leads P1-044–050.
```

**Continue EV prediction (P2):**
```text
Read grok.md, p2_virus_EV_indistinguishable_refs/p2.md, and p2_HANDOFF.md.
[task: framing / synthesis for Discussion particle layer]
```

---

## 10. Guardrails (rhetorical)

1. Attack: confounded design; weak controls; non-discriminating purification — not “all of virology is a conspiracy.”  
2. **Inheritance:** titers, Isolates, stocks, and particle claims that rest only on confounded CPE inherit uncertainty.  
3. Scope claims with **“under standard Isolation/maintenance conditions.”**  
4. One Vero E6 CRO is **preliminary**; generalize carefully.  
5. P2 EV section = field consensus synthesis + logical prediction, not a new wet purification of uninoculated vs inoculated unless we run it.  
6. P1 history: **descriptive patterns** first; “consistent with lock-in” only lightly in Discussion.

---

## 11. Suggested next work (priority order)

1. Ensure every stream has a clear main `rN.md` / `pN.md` with current TODOs (add `r1.md` if still missing).  
2. **User review** of control-tier scores (optional freeze).  
3. **Paper tables/figures:** isolation FBS pre/post; control tiers A–D; institutional rationale matrix; P1 timeline of medium practice.  
4. **Advance `tex/DRAFT.md`:** Methods (CRO + corpora), Results (tables), Discussion (P1 history + P2 EV + inheritance).  
5. Strengthen **P2** framing from `p2.md` TODOs.  
6. Optional P1 primaries: Baron & Low 1958 (**P1-048**); Youngner 1954 (**P1-046**); Weller *J Immunol* 1952 (**P1-045**).  
7. Fill paper Zenodo link in README when ready.

---

## 12. Glossary

| Term | Meaning here |
|------|----------------|
| **Isolation** | Operational culture recovery / detection (CPE-centered) |
| **Isolate** | Product of Isolation (not pure substance) |
| **CPE** | Cytopathic / cytopathogenic effect |
| **Maintenance medium** | Post-growth / infection medium, usually lower enrichment |
| **R streams** | Empirical research topics supporting the thesis |
| **P streams** | Prediction / discussion ramifications of the research |
| **P1** | Historical interest: published evolution of medium / serum practice |
| **P2** | Prediction: particle purification non-discriminating → EV literature |
| **P3** | Prediction (parked): genetics / sequence-reference inheritance |
| **Tier A–D** | Quality of Isolation-stage negative culture controls |
| **`refs/`** | Local-only copyrighted full texts; gitignored via `*/refs/` |

---

*End of bootstrap. Update status and stream TODOs when major workstreams change.*
