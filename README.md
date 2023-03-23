# CKE-Datasets

This repository contains manually annotated/extracted Keywords, which serve as ground truths 
for Contrastive Keyword Extraction (CKE) tasks. 
In total 200 versioned documents (articles and policies) were manually annotated.

The dataset is split into two csv files:
* policies.csv: different versions of <a href="https://privacypolicies.cs.princeton.edu//">policy snapshots</a>.
* articles.csv: revised versions of <a href="https://github.com/isi-nlp/NewsEdits//">news articles</a>.

## Princeton-Leuven Longitudinal Corpus of Privacy Policies
* **Id**: Policy Identifier 
* **Keywords**: Manually Extracted Keywords
* **TextA:** Markdown text of former version
* **TextB:** Markdown text of latter version
* **LengthA:** Text length of former version
* **LengthB:** Text length of latter version
* **LengthDifference:** $Length_B - Length_A$
* **YearA:** Release Year of former version
* **YearB:** Release Year of latter version
* **YearsApart:** $Year_B - Year_A$

### Characteristics:
|          | **LengthA** | **LengthB** | **LengthDifference** | **YearA** | **YearB** | **YearsApart** | **#Keywords** |
|:--------:|:-----------:|:-----------:|:--------------------:|:---------:|:---------:|:--------------:|:-------------:|
| **mean** |   11457.63  |   13738.46  |        2280.83       |  2011.82  |  2015.29  |      3.47      |      7.92     |
|  **std** |   8228.67   |   9529.49   |        4050.25       |    3.52   |    3.04   |      2.39      |      2.65     |
|  **min** |   1285.00   |   1586.00   |       -5263.00       |  2002.00  |  2004.00  |      0.00      |      2.00     |
|  **max** |   44999.00  |   49858.00  |       28242.00       |  2018.00  |  2019.00  |      12.00     |     14.00     |


## News Edits: News Article Revision 

* **Id**: Article Identifier 
* **Keywords**: Manually Extracted Keywords
* **TextA:** Text of former version
* **TextB:** Text of latter version
* **LengthA:** Text length of former version
* **LengthB:** Text length of latter version
* **LengthDifference:** $Length_B - Length_A$
* **VersionA:** Version Number of former version 
* **VersionB:** Version Number of latter version
* **Magazine:** Either _Alternative Press_ or _New York Times_




### Characteristics:
|          | **LengthA** | **LengthB** | **LengthDifference** | **VersionA** | **VersionB** | **#Keywords** |
|:--------:|:-----------:|:-----------:|:--------------------:|:-----------:|:------------:|:-------------:|
| **mean** | 5620.30     | 6967.48     | 1347.18              | 0.0         | 9.71         |      6.25     |
|  **std** | 3992.69     | 4291.93     | 2479.42              | 0.0         | 8.68         |      2.11     |
|  **min** | 738.00      | 795.00      | -2307.00             | 0.0         | 2.00         |      1.0      |
|  **max** | 31634.00    | 32820.00    | 14603.00             | 0.0         | 35.00        |      11.0     |
