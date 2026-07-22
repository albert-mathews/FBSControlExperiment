# Description

This repository holds research materials and a working draft for a methods-critical paper on **virus Isolation practice**, **cytopathic effect (CPE)**, and **serum/nutrient (FBS) conditions** in cell culture.

**Thesis (brief):** Under standard Isolation workflows, growth medium (~10% FBS) is shifted to low-serum maintenance (~1–3% / 2% FBS) around inoculation while CPE is treated as evidence of virus. That design confounds **inoculum** with **medium change**. A no-virus CRO experiment (Vero E6, 10% vs 2% FBS) produces CPE-like morphology, supporting the claim that CPE under Isolation-style conditions is **not virus-specific**. Downstream claims that rest only on CPE-defined Isolates—and particle work that cannot cleanly separate “virions” from extracellular vesicles—inherit that uncertainty. The paper is a **process critique**, not a claim that “nothing infectious exists.”

**Structure (brief):**

| Kind | Folders | Role |
|------|---------|------|
| **`r*` research** | `r1_isolation_standards_and_practice`, `r2_negative_controls`, `r3_image_labeling` | Empirical streams: Isolation/guideline corpus, negative-control tiers, CRO image labeling |
| **`p*` prediction** | `p1_history`, `p2_virus_EV_indistinguishable_refs`, `p3_genetics` | Discussion streams: medium-practice history (P1), EV–virus indistinguishability (P2), genetics inheritance (P3, parked) |
| **Draft** | `tex/` | Working narrative (`DRAFT.md`), bibliography, LaTeX helpers |

Each stream’s main markdown (`r2.md`, `p1.md`, …) is the entrypoint and TODO list for that topic. Session guidance for collaborators/agents: **`grok.md`**.

Paper data / draft link: <enter zenodo link>

## TODO
-see the end of this grok convo: https://grok.com/share/c2hhcmQtMi1jb3B5_a582ffbe-c6ab-4482-b5b7-2561c838389d, grab all refs there, and incorporate into the bib and narative.
-review the notes at the bottom of isolation-refs-overview.csv. ensure all are addressed, and do not indicated errors in data extraction, or that the ref should be excluded.
-filter isolation-refs by those which use CPE as endpoint. no CPE as end point = excluded. remember to state this explicitly in the paper.
-research on controls
-colate and present in tables and figures the isolation refs search results
-colate and present in tables and figures the institutional resrouces for virus isolation / CPE protocols
-start working the paper draft
-research pre-Enders virus culture works to see if there is an 'evolution' trend of adopting even decreasing level of FBS at inoculation Timeline