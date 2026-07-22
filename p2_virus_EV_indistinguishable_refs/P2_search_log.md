# P2 search log

**Protocol:** `P2_research.md` v0.1  
**Synthesizer:** grok-primary  
**Main repo path:** `p2_virus_EV_indistinguishable_refs/`  
**Date opened:** 2026-07-22  

---

## Round 0 — Scaffold (2026-07-22)

| Action | Result |
|--------|--------|
| Protocol | `P2_research.md` v0.1 written (P1-style: inclusion, metrics taxonomy, anti-colleague bias, counterexample family) |
| Artifacts created | `P2_search_log.md`, `P2_screened.csv`, `P2_useful.csv`, `P2_quotes.md` (provisional), `agent_reviews/` |
| Pre-existing local PDFs | 8 files under `refs/` treated as **seeds only**, not as complete corpus |

---

## Round 1 — Seeds + transparent bias (2026-07-22)

### 1.1 Seed list (local `refs/`)

| ID | File / paper |
|----|----------------|
| P2-001 | Nolte-’t Hoen et al. 2016 PNAS perspective |
| P2-002 | McNamara & Dittmer 2020 J Neuroimmune Pharmacol (modern techniques) |
| P2-003 | Zhou, McNamara & Dittmer 2020 Viruses (purification + RNA) |
| P2-004 | Raab-Traub & Dittmer 2017 Nat Rev Microbiol |
| P2-005 | Meckes & Raab-Traub 2011 J Virol minireview |
| P2-006 | Giannessi et al. 2020 Viruses (HIV/HCV/SARS) |
| P2-007 | Moulin et al. 2023 IJMS (two intertwined entities) |
| P2-008 | van Niel, D’Angelo & Raposo 2018 Nat Rev Mol Cell Biol (EV cell biology) |

**Bias note:** Seeds over-weight UNC/Dittmer/Raab-Traub/Nolte-’t Hoen network and general EV biology. Round 2 deliberately leaves this neighborhood.

### 1.2 Seed outcomes

- All 8 screened; **P2-001–007 = Y** (identity/separation language).  
- **P2-008 = B** (foundational EV biology; limited virus-separation claims — keep for biogenesis background, not as dilemma primary).  

### 1.3 One-hop snowball from seeds (abstract/title screen)

Leads harvested from seed bibliographies and abstract cross-refs (not full-text snowball yet):

| Lead | Rationale |
|------|-----------|
| Gould et al. 2003 PNAS Trojan exosome | Foundational continuum hypothesis |
| Bess et al. 1997 Virology microvesicles in HIV preps | Pre-exosome era co-purification primary |
| Gluschankof et al. 1997 Virology cell membrane vesicles HIV | Parallel 1997 primary |
| Cantin et al. 2008 J Virol CD45 discrimination | Marker-based separation attempt |
| Ott 2008 Methods Mol Biol / related CD45 subtilisin | Purification protocol for clean HIV proteomics |
| Feng et al. 2013 Nature eHAV / membrane hijacking | Enveloped HAV resembles exosomes |
| Bukong et al. 2014 / Ramakrishnaiah et al. 2013 HCV + exosomes | Infectious RNA in EV-like fractions |
| Théry et al. 2018 MISEV | Standards; purity / contamination context |
| Pegtel et al. 2010 EBV miRNA via exosomes | Viral cargo in EVs (identity of particle type) |

Logged as P2-009 onward in `P2_screened.csv`.

---

## Round 2 — Systematic web queries (2026-07-22)

**Platforms:** Web search (PubMed/PMC/publisher landing pages via web tools). Full PubMed API not used this session.  
**Cap:** Screen top ~15–25 relevance hits per family; log that deeper recall remains for later rounds.

### Family A — separation / indistinguishability language

| Query (approx) | Notes |
|----------------|-------|
| extracellular vesicles viruses co-purification separation density gradient ultracentrifugation review | High review density; confirms multi-method co-enrichment narrative |
| "cannot distinguish" OR indistinguishable OR co-isolate OR co-purif exosomes OR EV virus OR virions | Hits Nolte-’t Hoen 2016; many secondary reviews |

### Family B — method-specific

| Query | Notes |
|-------|-------|
| modern techniques isolation EV viruses McNamara | Seed confirmation + method tables |
| purification methods RNA virus particles extracellular vesicles Zhou | Cargo attribution |
| density gradient separate HIV exosomes CD45 | Cantin 2008; Coren 2008; Ott methods |

### Family C — cargo

| Query | Notes |
|-------|-------|
| RNA packaged virion EV contamination | Zhou 2020; debate on miRNA copy number in EV vs virion |

### Family D — counterexamples (successful separation claims)

| Query | Notes |
|-------|-------|
| separate purify discriminate EVs from virus / virions | Affinity (CD45, CD63 beads), velocity gradients, subtilisin shaving, infectivity assays claimed as partial solutions — **not** “impossible always” |

### Family E — historical

| Query | Notes |
|-------|-------|
| Bess 1997 microvesicles HIV | **Key historical primary** — sucrose density co-banding |
| Gluschankof 1997 vesicles HIV preparations | Parallel primary |
| defective interfering particles membrane virus EM | Continuum language pre-EV field; needs deeper full-text round |
| early exosome virus purification contamination 1980s–2000s | Sparse pre-1997 with modern “EV” vocabulary; 1997 cluster is strong |

### Family F — standards / recent persistence

| Query | Notes |
|-------|-------|
| MISEV 2018 virus contamination | Purity recommendations; viral particle co-isolation awareness |
| EV virus separation 2021–2025 | Martin et al. 2023 Viruses; Dias 2018 Frontiers; field still framing as hard problem |

### Negative / thin results

| Strategy | Result |
|----------|--------|
| Pre-1990 English “exosome virus co-purify” | Vocabulary anachronism; need “cellular debris / microvesicles / membrane fragments” language in virus purification monographs (queued Round 3) |
| Claim that UC alone fully separates all enveloped viruses from EVs | No high-quality hit asserting universal clean UC separation |

---

## Round 3+ (queued)

- Full-text snowball depth 2 from every **Y** with PDF.  
- Virus purification handbooks 1960s–1980s (non-EV vocabulary).  
- Plant / non-enveloped contrast papers.  
- Systematic PubMed export with hit counts (not approximate web).  

---

## PDF request list (user fetch)

See end of session response / `P2_pdf_request.md`. High-priority historical + primary separation papers not in local `refs/`.

---

## Agent verification (2026-07-22)

| Agent | Task | Output | Consumed? |
|-------|------|--------|-----------|
| Agent A | Metrics/coding re-screen sample | `agent_reviews/P2_agentA_metrics_and_coding.md` | Yes — CSV amendments applied for P2-006/007/010/011/013/016/018 |
| Agent B | History + counterexamples | `agent_reviews/P2_agentB_history_and_counterexamples.md` | Yes — Cantin imprint fixed; synthesis hedges noted |

### Agent-driven amendments applied
- P2-006: added M-UC, M-DENS  
- P2-007: supports_dilemma=mixed; confidence=medium; dropped weak M-HIST  
- P2-010/011/016/018: confidence high→medium while abstract_only  
- P2-013: corrected to *J Immunol Methods* 2008 (velocity/AChE), not J Virol CD45  
- P2-018: claims_successful_separation=partial  

### Agent findings retained for next round (not yet all applied)
- M-EM strength weaker than provisional “moderate”  
- 2023–2025 continuity = live topic, not proven methods crisis  
- Pre-1997 DI/L-particles ≠ host EV co-purification without interpretive bridge  
- Esser 2001 CD45 foundation paper to screen  
- Devil’s advocate: velocity + AChE/CD45 + infectivity = practical partial separators  

---

*Log append-only; amend with dated notes, no silent rewrites of prior query strings.*
