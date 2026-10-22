# Revised Project Proposal - Pair 05

**Analysing Consumer Purchasing Behaviour: A Two-Dataset Credibility Audit
and Spending-Driver Study**

QU YING (MC641326) and LIU ZIXUAN (MC641811), Class B, Pair 05.

## Why the topic was revised

The dataset on which the preliminary proposal relied turned out to contain almost no
usable signal. In the Shopping Behaviour dataset, the three strongest candidate
predictors correlate with purchase amount at r = 0.008, -0.010 and 0.031, and seven of
eight grouping variables return ANOVA p-values above 0.05. A dataset that cannot predict
its own outcome variable cannot answer the original question, so it is retained as the
object of an explicit credibility audit, and the modelling moves to the Customer
Personality Analysis dataset, which does contain structure.

## Key findings so far

| Finding | Value |
|---|---|
| Primary dataset, best correlation with spending | 0.031 |
| Primary dataset, only significant ANOVA group | Season, p = 0.011 |
| Income vs total spending | r = +0.668 |
| Catalogue purchases vs total spending | r = +0.780 |
| Children at home vs total spending | r = -0.558 |
| Regression R-squared (seven predictors) | 0.771 |
| Cluster campaign response rates | 0.04 to 0.27 |

## Research questions

- **RQ1** Is the Shopping Behaviour dataset reliably associated with purchase amount, or effectively signal-free?
- **RQ2** How much of total spending variation is explained by income, household composition and channel behaviour?
- **RQ3** Can distinct customer-value segments be identified, and do they differ in campaign response?
- **RQ4** What does the contrast between a signal-free synthetic dataset and a structured real one imply for evidence-based retail decisions?

## Data sources

- Shopping Behaviour Dataset - https://www.kaggle.com/datasets/saadaliyaseen/shopping-behaviour-dataset
- Customer Personality Analysis - https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis

The CSV files are not redistributed here. Note that `marketing_campaign.csv` is
tab-separated and must be read with `sep='\t'`.

## Files

| File | Description |
|---|---|
| `CISC7204-Assgn02-Pair05-RevisedProjectProposal.docx` | The submitted proposal, 5 A4 pages |
| `CISC7204-Assgn02-Pair05-ProposalNotebook.ipynb` | Reproducible notebook producing every figure and number above |

## Reproducing the analysis

Place both CSV files in the same folder as the notebook and run all cells under the
`CISC7204_SugEx10_ENV` environment (Python 3.11, pandas, numpy, scipy, matplotlib,
seaborn, scikit-learn). The notebook regenerates all six figures and the numbers quoted
above, including the sensitivity check showing that removing a single extreme income
record raises the income correlation from 0.668 to 0.792.
