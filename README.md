# **De**mystified **n**on-**f**unctional r**e**quirements for **t**uning (Denfet)


Software configuration tuning is an important engineering activity that ensures stakeholders’ non-functional needs are satisfied, e.g., “the search should take no longer than 15 seconds.” However, incorporating non-functional requirements in the tuning process is challenging, because they can be highly imprecise; may be inconsistent due to the presence of different stakeholders; and require trade-offs under multi-dimensional metrics. While current research has gained momentum on improving the optimizers, little progress has been made in understanding how to quantify the requirements, reason about their differences, and perform refinement, all of which are necessary for them to effectively guide the tuning. 

To overcome such, we firstly conduct an empirical study on 139 real-world requirements, among which we found that 74% contain at least one threshold; 87% involve some forms of imprecision; nearly half suffer inconsistency and 86% cases have multi-dimensional concerns. Drawing on the insights, we design ***De***mystified ***n***on-***f***unctional r***e***quirements for ***t***uning (Denfet), a holistic theoretical framework that helps to demystify non-functional requirements for configuration tuning. Denfet handles requirements as fragments, which can be arbitrarily combined to form complex propositions. More importantly, it quantifies the difficulty of satisfaction, allowing us to formally define the relationships between requirements by means of refinement. Through a real-world case study of 19 participants, we show that Denfet can considerably improve stakeholders’ confidence in making decisions up to 1.78× and reduce the efforts by ≈ 70 minutes on average over standard elicitation while being generally useful.

This repository contains the data and supplementary materials that we are allowed to release as part of the work.


## Data for empirical study

All the extracted data for our empirical study, which contains the non-functional requirements from 21 configurable software systems, can be accessed in the [empirical-study](https://github.com/csusera/denfet/tree/main/empirical-study) folder. The spreadsheet is self-explained and it has the results for the following questions:

- Q1: What are the patterns?
- Q2: How imprecise the non-functional requirements are?
- Q3: How prevalent for having inconsistent requirements on the same non-functional metric per system (module)?
- Q4: How many dimensions of non-functional metrics are often considered per system?

## Data for case study

All the results obtained and reported for our case study can be found in the [survey](https://github.com/csusera/denfet/tree/main/survey) folder. The results are organized with respect to the following phases:

- Define contexts
- Qunaityf requirements
- Resolve inconsistency
- Reason trade-offs

The naming of the files is also self-explained. For example, `define-context-w.csv` means the task for "define context" phase with Denfet; `define-context-w:o.csv` denotes the task for "define context" phase without Denfet; `define-context.csv` contains the overall usefulness rating. The tasks for the other phases can be similarly interpreted. `overall.csv` contains the statistics calculation results.

The instructions for the tasks and the link to the actual questions used in our case study can be accessed [here](https://github.com/csusera/denfet/blob/main/case-study-brief.pdf).

## Proof of the theorems

We have also provided detailed proofs of the theorems about the relationships between single- and multi-dimensional requirement propositions, which can be found [here](https://github.com/csusera/denfet/blob/main/proof.pdf).
