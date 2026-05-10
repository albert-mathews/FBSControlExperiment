# Description
These notes capture the re-review of the isolation-refs-overview.csv sources.
The goal here is to filter them based on "use of CPE as an end point in culture analsyis".
The initial review was performed by SuperGrok, using the follwing prompt, and the PDF version of the papers.

For some refs, I read the paper in detail. My comments from that are indicated "Albert:" in the sections below.
Note: I have previously read many of not all of these papers in full. Memory is not always the best, whihc is why I also use Ai to review and filter sources.

This process was also iused to indefiy any instances of control cultures, and the details around that.
See control-cultures-overview.csv for those results.

## Prompt
this is the final list of papers collected that explicitly state a reduction of FBS% in culture medium during cell culture infection.

ATCC Virology Culture Guide
CLSI M41a
ASM - Cytopathic Effects of Viruses Protocols

those are institutional guidelines that define protocols for virus isolation in cell culture. they outline the same protocol: grow cells in high (10%) FBS, decrease FBS to low concentration (2%) and infect cultures, wait and observe cytopathic effect (CPE).

i would like you to carefully review each article in isolation-refs-overview, and identify those which do not employ CPE as part of their infected culture observations.
you will not do them all at once, you will review them 5 to 6 at a time as I will give you pdfs for then 5-6 at a time, so you dont have to find the information from the internet. please start with the 6 attached. when done, i'll upload the next 5, and so on.

this is the specific information I want from you, and I want it formatted this way.
pure text
paper id (e.g. VI27), bulleted list.
-was CPE used as an end point to confirm infection, yes/no
	-quotes form the paper to justify, as many as you can find
-were any control cultures employed, yes/no
	-were the culture conditions of the controls explicitly stated, yes/no
	-if yes, quotes from paper describing the control culture conditions
	-were the control culture conditions identical to the test cultures conditions, with exception of addition of virus source? yes/no
what other endpoints were used in culture analysis, a concise comma separated list

# review
## VI4

was CPE used as an end point to confirm infection, no
"There was no visible cytopathic effect (CPE) in the antigen-positive cultures."
"There was no visible cytopathic effect (CPE) in the antigen-positive cultures. Whole-culture preparations containing the infectious agent was prepared by one cycle of freezing-thawing in the antigen-positive cultures."

were any control cultures employed, no
N/A (no mention of mock, uninfected, or control cultures in the methods or results sections)

what other endpoints were used in culture analysis, IFA antigen staining, percentage of antigen-positive cells, IFA endpoint titration

Albert: 
after reading, the main problem with this paper is that the methods are losely documented and it difficult to follow what was actually done.
certainly the lack of CPE as an end point makes it not a useful reference in this case. although it does suport the claim thta in practice FBS% is reduced during infection, it is not a high quality reference for tis research. 
excluded. 

## VI14

was CPE used as an end point to confirm infection, yes
"Cells that showed cytopathic effect (CPE) were then confirmed by indirect immunofluorescence assay"
"The cytopathic effect (CPE) of inoculated Hep-2 cells was observed everyday for seven days. CPE negative samples at the seventh day after inoculation were blindly inoculated for two consecutive passages and CPE positive samples recorded"
"HRSV positive isolates showed typical CPE. The infected cells became round and fused together forming giant cells"

were any control cultures employed, yes
were the culture conditions of the controls explicitly stated, yes
"CPE positive and uninfected (mock) Hep-2 cells were digested by 0.02 % EDTA"
were the control culture conditions identical to the test cultures conditions, with exception of addition of virus source? yes

what other endpoints were used in culture analysis, IFA, RT-PCR, HVR2 sequencing

## SPT10

was CPE used as an end point to confirm infection, yes
"When the cytopathic effect (CPE) was progressed through 70 to 80%, the culture supernatants"

were any control cultures employed, no
N/A (no mention of mock or uninfected control cultures in the virus propagation or imaging sections)

what other endpoints were used in culture analysis, virus rescue and propagation by transfection, IFA, RT-PCR, TEM (electron microscopy)

## VI13

was CPE used as an end point to confirm infection, yes
"CPE was not observed in mock infected cells (Figure 1, panel A)"
"We observed CPE 2 days postinoculation and harvested viral lysate on day 3 postinoculation"
"SARS-CoV-2 infection of Vero E6 cells produced CPE with areas of cell clearance"
"observed for cytopathic effects (CPEs) daily"
"Major CPE was not observed until 60 h postinoculation and peaked at 72 h postinoculation"

were any control cultures employed, yes
were the culture conditions of the controls explicitly stated, yes
"CPE was not observed in mock infected cells"
were the control culture conditions identical to the test cultures conditions, with exception of addition of virus source? yes

what other endpoints were used in culture analysis, plaque assays, PFU viral titers, qRT-PCR, genome sequencing

## VI2

was CPE used as an end point to confirm infection, yes
"Virus titre was determined in Vero E6 cells by cytopathic effect (CPE) counts."
"CPE was observed using an inverted microscope 2 days after inoculation."

were any control cultures employed, no
N/A (negative control serum was used only in the separate neutralization assay; no mock/uninfected infection controls described for the primary culture isolation or growth)

what other endpoints were used in culture analysis, virus infectivity assays in different cell lines (including ACE2-expressing cells), neutralization test by CPE suppression, qRT-PCR

VI8

was CPE used as an end point to confirm infection, yes
"Clear cytopathogenic effects were observed in cells after incubation for three days"
"The cells were incubated at 37 °C and observed daily for cytopathogenic effects."

were any control cultures employed, no
N/A (no mention of mock or uninfected controls in the virus isolation or propagation sections)

what other endpoints were used in culture analysis, qRT-PCR from culture supernatant, virus neutralization by patient sera