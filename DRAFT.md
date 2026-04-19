# Draft paper

## introduction
This article identifies virology cell culture methods for virus isolation—particularly the reliance on cytopathic effects (CPE) as a primary indicator of viral presence amid changes in fetal bovine serum (FBS) concentration—as a high-impact research area in need of replication studies. These methods underpin foundational evidence in infectious disease research, including during outbreaks like SARS-CoV-2, and potential confounders could affect interpretations across studies.
Standard guidelines in virology recommend reducing FBS concentration in cell culture media from approximately 10% during cell growth to 2% during virus propagation phases. These same guidelines position the observance of CPE in inoculated cell cultures as the primary indication of viral presence.

Guidelines recommending reduction of FBS concentration from 10% to 2%:
ATCC Virology Culture Guide [11]:
	- “Viral growth medium is usually supplemented with a lower percentage of serum than cell growth medium, often ranging between 2-10% depending on the virus”
	- “NOTE 5: For viral inoculation, ATCC recommends decreasing the percentage of serum to 2% as it can interfere with viral attachment. This can vary from strain to strain, and is not applicable for influenza viruses.”
CLSI M41a [10]:
	- section “5.3.1.2 Cell Density”: “Once the cultures have reached the required density, maintenance medium containing 2% fetal bovine serum (FBS) can be used in place of growth medium, which usually contains 10% FBS. Medium with the lower concentration of FBS will maintain cell viability and will slow monolayer overgrowth.”
	- section “5.3.2 Maintenance”: “Refeed monolayers that are at 75% or greater confluence with fresh maintenance medium containing a low concentration of FBS (e.g., 2%) when the medium color indicates that the pH is below 7.0 (yellow-orange to yellow).”
	- section “5.4.1 Medium Composition”: “Typically 10% FBS is used for growth medium intended for the propagation of cell culture monolayers, while a concentration of 1 to 3% is utilized to maintain subconfluent to confluent monolayers both before and after inoculation.”
	- section “7.1.2 Preinoculation Assessment of Monolayers”: “Inspect cell culture microscopically and macroscopically as described in Section 5.3.1 just prior to specimen inoculation. In summary: the cell culture medium must not be cloudy or turbid; cells should be adherent and healthy in appearance; and the monolayer should be 75 to 90% confluent, but not overgrown.”
Guidelines stating CPE is the primary detection method for viral presence:
	- ATCC Virology Culture Guide: section “Viral authentication and viability testing”
	- CLSI M41a: section “7.4.2 Viral Effects”

Given the above, it is reasonable to state that in cell culture experiments where a virus is being “isolated,” there are two independent variables being manipulated and one dependent variable being observed:
	- Independent variables:
		- Virus added or not
		- FBS concentration
	- Dependent variable:
		- CPE in cell culture

Literature on virus isolation aligns with these guidelines [1-8], often employing reduced FBS during propagation and relying on CPE for detection. For example [1,3,4]:
	- In Ge et al. (2013), Vero E6 cells were maintained in DMEM with 10% FCS, but virus propagation used DMEM with 2% FCS. CPE was observed daily to detect viral presence.
	- In Zhou et al. (2020), Vero E6 cells were cultured in DMEM with 10% FBS, with clear CPE observed after three days of incubation as a key indicator of viral infection.
	- In Zhao et al. (2019), methods involved virus isolation in cell cultures with CPE as a general indicator, consistent with standard practices.

FBS concentration could act as a confounder in inducing CPE in cell cultures, potentially making CPE non-specific to the presence of virus particles. If validated, this would necessitate more robust, specific detection methods to ensure accurate virus isolation and characterization.



The control experiment offers preliminary evidence: Reduced FBS alone induced CPE-like changes without virus, aligning with literature but exposing a media control gap. Public data enables re-analysis for quantification.

Virus isolation protocols are foundational to biomedical research, including HHS and NIH's Generation Gold Standard program for developing beta-propiolactone-inactivated, whole-virus universal vaccines against pandemic-prone viruses like influenza and coronaviruses. These vaccines are designed, iterated, and produced using cell cultures reliant on accurate virus isolation and propagation. If CPE is non-specific due to FBS changes, it could lead to misattributions of viral effects, undermining reproducibility and derailing vaccine candidates, with economic consequences including billions in wasted R&D costs for flawed designs and trillions in broader pandemic losses from delayed or ineffective responses. Replicating this across cell lines/viruses could refine guidelines, enhance specificity, and build trust in virology. Answering this would impact public health by improving virus detection reliability in outbreaks, preventing misdiagnoses, and aiding resource allocation. It would influence cell biology (serum effects), microbiology (isolation standards), and infectious disease epidemiology (pathogen validation).



## methods

## experiment
To explore this hypothesis, a control experiment was commissioned through a certified U.S.-based CRO using Vero E6 cells (ATCC-CRL-1586), with no virus added. Two identical paths differed only in FBS: Path A at 10%, Path B at 2%. After preparation (thawing and passaging) and experimental stages (daily imaging), greater CPE-like changes appeared in Path B, shown in over 50 light microscope images (EVOS FL at 10x/20x) and 170 TEM images (Tecnai G2 Spirit BioTWIN). Raw data is on Zenodo [9] for analysis and replication.

### Identification of standard CPE descriptors
\subsection{Standard CPE descriptors}
Characteristic CPE descriptors were extracted from Table 7 of the CLSI M41 Guideline \cite{clsi} through an iterative review process. First, the full table was examined to identify a set of ten descriptors: rounded, ballooned/enlarged, syncytia, vacuolation, detachment, granularity, refractile, cytoplasmic strands, nonspecific degeneration, and no CPE. An incidence table was then constructed by identifying every instance of these terms (or close semantic correlates) in text entries of the ``Appearance'' column, see Table 1 below.

\input{clsi-table7-descriptors.tex}

Next, the same mapping procedure was applied to the CRO image descriptions to generate a second incidence table (CLSI descriptor set + image descriptions). Only five of the original ten CLSI descriptors appeared in the CRO descriptions. A sixth term, ``Dying Cells'', emerged directly from the CRO text and was retained as a distinct category (Dy) rather than being forced into the CLSI ``nonspecific degeneration'' bin. The resulting \textit{CPE descriptor set} used for ground truth and all subsequent analyses therefore consisted of: Dying cells (Dy), Rounded (Ro), Vacuolation (V), Detached (D), Granularity (G), and Refractile (Re).



## results


## discussion



# references
1. Ge XY, Li JL, Yang XL, Chmura AA, Zhu G, Epstein JH, Mazet JK, Hu B, Zhang W, Peng
C, Zhang YJ, Luo CM, Tan B, Wang N, Zhu Y, Crameri G, Zhang SY, Wang LF, Daszak
P, Shi ZL. Isolation and characterization of a bat SARS-like coronavirus that uses the
ACE2 receptor. Nature. 2013 Nov 28;503(7477):535-8. doi: 10.1038/nature12711. PMID:
24172901; PMCID: PMC5389864.
2. Kitamura T, Morita C, Komatsu T, Sugiyama K, Arikawa J, Shiga S, Takeda H, Akao Y,
Imaizumi K, Oya A, Hashimoto N, Urasawa S. Isolation of virus causing hemorrhagic
fever with renal syndrome (HFRS) through a cell culture system. Jpn J Med Sci Biol.
1983 Feb;36(1):17-25. doi: 10.7883/yoken1952.36.17. PMID: 6134854.
3. Zhou P, Yang XL, Wang XG, Hu B, Zhang L, Zhang W, Si HR, Zhu Y, Li B, Huang CL,
Chen HD, Chen J, Luo Y, Guo H, Jiang RD, Liu MQ, Chen Y, Shen XR, Wang X, Zheng
XS, Zhao K, Chen QJ, Deng F, Liu LL, Yan B, Zhan FX, Wang YY, Xiao GF, Shi ZL. A
pneumonia outbreak associated with a new coronavirus of probable bat origin. Nature.
2020 Mar;579(7798):270-3. doi: 10.1038/s41586-020-2012-7. PMID: 32015507; PMCID:
PMC7095418.
4. Zhao T, Ye Z, Wang B, Cui Y, Nie Y, Yang B, Chen K, Zhang H, Hu F, Yu F. Virus
isolation and genotype identification of human respiratory syncytial virus in Guizhou
Province, China. Braz J Infect Dis. 2019 Nov-Dec;23(6):427-34. doi:
10.1016/j.bjid.2019.10.007.
5. Kar M, Nisheetha A, Kumar A, Jagtap S, Shinde J, Singla M, M S, Pandit A, Chandele A,
Kabra SK, Krishna S, Roy R, Lodha R, Pattabiraman C, Medigeshi GR. Isolation and
molecular characterization of dengue virus clinical isolates from pediatric patients in New
Delhi. Int J Infect Dis. 2019 Jul;84S:S25-33. doi: 10.1016/j.ijid.2018.12.003. PMID:
30528666; PMCID: PMC6823047.
6. Athmanathan S, Reddy SB, Nutheti R, Rao GN. Comparison of an immortalized human
corneal epithelial cell line with Vero cells in the isolation of Herpes simplex virus-1 for the
laboratory diagnosis of Herpes simplex keratitis. BMC Ophthalmol. 2002 Apr 30;2:3. doi:
10.1186/1471-2415-2-3. PMID: 11983023; PMCID: PMC113264.
7. Hu W, Zhang H, Han Q, Li L, Chen Y, Xia N, Chen Z, Shu Y, Xu K, Sun B. A
Vero-cell-adapted vaccine donor strain of influenza A virus generated by serial
passages. Vaccine. 2015 Jan 3;33(2):374-81. doi: 10.1016/j.vaccine.2014.11.007. PMID:
25448099.
8. Li S, Wang D, Ghulam A, Li X, Li M, Li Q, Ma Y, Wang L, Wu H, Cui Z, Zhang XE.
Tracking the replication-competent Zika virus with tetracysteine-tagged capsid protein in
living cells. J Virol. 2022 Apr 13;96(7):e0184621. doi: 10.1128/jvi.01846-21. PMID:
35285687; PMCID: PMC9006885.
9. Mathews A. Vero cell culture image dataset [dataset on the Internet]. Zenodo; c2025
[cited 2025 Dec 14]. Available from: https://doi.org/10.5281/zenodo.17928456
10. Clinical and Laboratory Standards Institute. (2006). Viral culture; Approved guideline
(CLSI Document M41-A).
https://clsi.org/standards/products/microbiology/documents/m41/
11. American Type Culture Collection [Internet]. Manassas (VA): The Collection; c2025 [cited
2025 Dec 14]. Virology Culture Guide. Available from:
https://www.atcc.org/resources/culture-guides/virology-culture-guide

