<div align="center">

# Ancient pathogen genomics of domestic small ruminants

**Supplementary material accompanying the PhD thesis**

*Tracing Zoonoses and Ancient Pathogens of Domesticated Small Ruminants: From Domestication to Today*

Louis L'Hôte — UCD School of Agriculture and Food Science, University College Dublin, 2026

[![Licence: CC BY 4.0](https://img.shields.io/badge/Licence-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Chapter 3](https://img.shields.io/badge/Chapter%203-Nature%20Communications-blue.svg)](https://doi.org/10.1038/s41467-024-50536-1)
[![Chapter 4](https://img.shields.io/badge/Chapter%204-Science%20Advances-orange.svg)](https://doi.org/10.1126/sciadv.aeh3571)
[![Data: ENA](https://img.shields.io/badge/Data-ENA-green.svg)](https://www.ebi.ac.uk/ena)

</div>

---

## Overview

This repository holds the supplementary tables, figures and data files for the three research chapters that address that question. Material also published as journal supplementary information is duplicated here for convenience; the version of record is the publisher's in each case.

| Chapter | Subject | Folder | Status |
|:--|:--|:--|:--|
| **2** | A screening workflow for archaeological animal remains | [`chapter2_pigsti/`](chapter2_pigsti) | Submitted, *F1000Research* |
| **3** | A Neolithic *Brucella melitensis* genome | [`chapter3_brucella/`](chapter3_brucella) | [*Nature Communications* **15**:6132](https://doi.org/10.1038/s41467-024-50536-1) |
| **4** | Ancient sheeppox virus genomes | [`chapter4_capripox/`](chapter4_capripox) | [*Science Advances* **12**:eaeh3571](https://doi.org/10.1126/sciadv.aeh3571) |

Supplementary tables for each chapter are provided as a single workbook with one sheet per table, named `S1`, `S2`, `S3` and so on. Supplementary figures and notes are provided as a single PDF.

---

## Repository structure

```
.
├── chapter2_pigsti/
│   ├── Chapter_2_Supp_Tables.xlsx      Sheets S1–S8
│   └── Chapter_2_Supp_Info.pdf         Archaeological site descriptions
├── chapter3_brucella/
│   ├── Chapter_3_Supp_Tables.xlsx      Sheets S1–S11
│   └── Chapter_3_Supp_Info.pdf         Figures S3.1–S3.8
├── chapter4_capripox/
│   ├── Chapter_4_Supp_Tables.xlsx      Sheets S1–S13
│   └── Chapter_4_Supp_Info.pdf         Figures S4.1–S4.23, Note S4.1
└── README.md
```

---

## Contents by chapter

<details>
<summary><b>Chapter 2 — PIGSTI: pathogen screening in ancient animal genomic data</b></summary>
<br>

PIGSTI (Pathogen anImal Genome Sequence ToolkIt) combines host species identification, microbial screening and pathogen authentication in a single reproducible Snakemake workflow, developed for archaeological faunal material rather than adapted from human-focused pipelines. Applied to 952 ancient and modern livestock datasets, returning 109 authenticated detections from 1,023 candidate hits across 89 specimens, including the first ancient animal records of *Rickettsia felis* and *Leptospira borgpetersenii*.

| File | Sheet | Description |
|:--|:--|:--|
| `Chapter_2_Supp_Tables.xlsx` | `S1` | Pathogen panel screened, with per-pathogen E-value and read-count thresholds |
| | `S2` | Sequencing data for newly generated libraries: sample of origin, library identifier, UDG treatment, raw read pairs |
| | `S3` | Detection scores and authentication metrics for the 60 simulated benchmarking datasets |
| | `S4` | Metadata for all 952 screened datasets |
| | `S5` | All 1,023 candidate hits passing the initial E-value threshold |
| | `S6` | The 109 hits passing the high-confidence filter set |
| | `S7` | The 89 samples carrying at least one authenticated detection |
| | `S8` | Metadata for the 153 newly generated datasets |
| `Chapter_2_Supp_Info.pdf` | — | Description of archaeological sites for newly reported material |

**Pipeline:** [github.com/LouisLhote/PIGSTI](https://github.com/LouisLhote/PIGSTI) · archived at [doi:10.5281/zenodo.22161588](https://doi.org/10.5281/zenodo.22161588) · MIT licence

**Supplementary data on Zenodo:** [doi:10.5281/zenodo.22135224](https://doi.org/10.5281/zenodo.22135224) — also includes the modified pathPhynder v1.2.3 implementing `--maximumToleranceProp`

</details>

<details>
<summary><b>Chapter 3 — A Neolithic <i>Brucella melitensis</i> genome</b></summary>
<br>

A *B. melitensis* genome recovered from the Neolithic sheep specimen Mentese6 (Menteşe Höyük, northwest Türkiye, 8007–7863 cal BP), calibrating the divergence of *B. melitensis* from the cattle-associated *B. abortus* to approximately 9,800 BP.

| File | Sheet | Description |
|:--|:--|:--|
| `Chapter_3_Supp_Tables.xlsx` | `S1` | Menteşe specimen information: archaeological identifiers, material, species, molecular sex, biosample accessions |
| | `S2` | KrakenUniq results for core *Brucella* species, with read counts, unique k-mer counts and E values |
| | `S3` | Radiocarbon dating results |
| | `S4` | Sequencing results for the Mentese6 libraries |
| | `S5` | Dataset used for the IQ-TREE2 and BEAST analyses |
| | `S6` | Accessions and species used in the lineage analysis |
| | `S7` | Lineage analysis using lineage-defining variants |
| | `S8` | Pairwise average nucleotide identity (ANI) values |
| | `S9` | Summary of BEAST runs: marginal likelihoods, tree heights, mutation rates, ESS |
| | `S10` | Variant sites defining the *B. melitensis* lineage, with Mentese6 genotypes and consequences |
| | `S11` | Coverage of *B. melitensis* genes in the Mentese6 alignment |
| `Chapter_3_Supp_Info.pdf` | — | Supplementary Figures S3.1–S3.8 |

**Published as:** L'Hôte L, Light I, Mattiangeli V, Teasdale MD, Halpin Á, Gourichon L, Key FM, Daly KG (2024). An 8000 years old genome reveals the Neolithic origin of the zoonosis *Brucella melitensis*. *Nature Communications* **15**:6132. [doi:10.1038/s41467-024-50536-1](https://doi.org/10.1038/s41467-024-50536-1)

**Code:** [github.com/LouisLhote/Neolithic_Brucella_paper](https://github.com/LouisLhote/Neolithic_Brucella_paper)

</details>

<details>
<summary><b>Chapter 4 — Ancient sheeppox virus genomes</b></summary>
<br>

Twenty-one ancient sheeppox virus genomes spanning the Late Bronze Age Eurasian steppe to Early Modern Europe — the oldest *Poxviridae* genomes recovered to date, and the first complete pathogen genomes obtained from parchment.

| File | Sheet | Description |
|:--|:--|:--|
| `Chapter_4_Supp_Tables.xlsx` | `S1` | Sample information: material, dates, radiocarbon data, object identifiers, inferred origin |
| | `S2` | Sequencing data, with SPPV representation before and after filtering |
| | `S3` | Mitochondrial competitive alignment and host species assignment |
| | `S4` | Localised sampling of parchment specimen TCCL02 |
| | `S5` | Marginal likelihoods of SPPV BEAST models with and without temporal information |
| | `S6` | Branch-site and clade model tests for positive selection |
| | `S7` | Modern Capripoxvirus genomes used in the analyses |
| | `S8` | Root posterior probabilities across clock models, with and without enforced monophyly |
| | `S9` | Pairwise similarity in 500 bp windows at 100 bp steps |
| | `S10` | Global pairwise similarities between Capripoxvirus species pairs |
| | `S11` | Gene inactivation states across ancient and modern genomes |
| | `S12` | CheckV assembly quality metrics |
| | `S13` | Disruptive mutations within the inactivated genes |
| `Chapter_4_Supp_Info.pdf` | — | Supplementary Figures S4.1–S4.23 and Supplementary Note S4.1 |

**Published as:** L'Hôte L, Sacristán L, Ferguson R, *et al.* (2026). Three thousand five hundred years of sheeppox virus evolution inferred from archaeological and codicological genomes. *Science Advances* **12**:eaeh3571. [doi:10.1126/sciadv.aeh3571](https://doi.org/10.1126/sciadv.aeh3571)

**Code and BEAST input files:** [github.com/LouisLhote/Sheeppox_aDNA](https://github.com/LouisLhote/Sheeppox_aDNA) · [doi:10.5061/dryad.mw6m906c5](https://doi.org/10.5061/dryad.mw6m906c5)

</details>

---

## Sequence data

Raw sequencing data are deposited in the [European Nucleotide Archive](https://www.ebi.ac.uk/ena) under accessions **PRJEB124647** (Chapter 2), **PRJEB75678** (Chapter 3) and **PRJEB107108** (Chapter 4). Accessions for individual specimens are given in sheet `S1` of each chapter's table workbook.

---

## Licence

[![CC BY 4.0](https://img.shields.io/badge/Licence-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

Data files and figures are released under [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) unless a folder states otherwise. Code is released under the MIT licence in its own repository.

---

## Contact

**Louis L'Hôte** — <louis.lhote@outlook.fr>

Enquiries about specific archaeological material should be directed to the institution holding it, identified against each specimen in sheet `S1` of the relevant workbook.
