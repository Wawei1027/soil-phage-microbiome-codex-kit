# Soil Phage Microbiome Codex Kit

This repository is a personal Codex skill/plugin kit for research workflows in soil microbial ecology, bacteriophage and phage ecology, virome analysis, amplicon microbiome analysis, shotgun metagenomics, microbiome statistics, publication figures, manuscript revision, journal selection, and submission preparation.

The plugin is designed for practical day-to-day research support. Its skills emphasize reproducible workflows, explicit assumptions, transparent metadata, careful statistics, and strict avoidance of fabricated results, citations, species names, database details, software versions, or biological interpretations.

## Scope

- Soil microbiome.
- Bacteriophage and phage ecology.
- Virome analysis.
- 16S and ITS amplicon analysis.
- Shotgun metagenomics.
- Microbiome statistics.
- Publication figures and tables.
- Manuscript revision.
- Journal selection and submission.

## Plugin

- Plugin name: `soil-phage-microbiome-research-kit`
- Marketplace file: `.agents/plugins/marketplace.json`
- Plugin manifest: `plugins/soil-phage-microbiome-research-kit/.codex-plugin/plugin.json`

## Skills

- `soil-phage-project-planner`: Design soil microbiome, phage, virome, metagenomics, or amplicon projects; check experimental design; organize metadata; map hypotheses to analyses and figures.
- `amplicon-microbiome-pipeline`: Draft and audit 16S, ITS, or other amplicon workflows using QIIME 2, DADA2, phyloseq, diversity analysis, ordination, PERMANOVA, differential abundance, visualization, and Methods text.
- `shotgun-metagenomics-pipeline`: Plan reproducible shotgun metagenomics workflows covering QC, trimming, host removal, taxonomic profiling, assembly, binning, MAG quality, functional annotation, and pathway profiling.
- `phage-virome-analysis`: Plan viral contig identification, viral quality checks, dereplication, taxonomy, host prediction, abundance mapping, AMG screening, and soil phage ecological interpretation.
- `microbiome-statistics`: Select and implement statistics for microbial community differences, environmental drivers, phage-host relationships, networks, differential abundance, mixed models, ordination, and reporting.
- `publication-figures-and-tables`: Create publication-ready figures, tables, supplementary tables, captions, legends, and reproducible plotting code for microbiome, phage, virome, and metagenomics manuscripts.
- `manuscript-journal-submission`: Draft, revise, diagnose, and prepare manuscripts; compare journals; draft cover letters; and respond to reviewers without inventing journal metrics or unsupported claims.
- `literature-discovery-mapper`: Search, map, screen, and organize verifiable literature for soil microbiome, phage, virome, metagenomics, amplicon, Introduction, Discussion, review, and proposal work.
- `citation-doi-verifier`: Check whether citations, DOI, titles, authors, years, journals, publishers, and bibliographic records are real and internally consistent.
- `journal-integrity-screener`: Screen journal reliability, warning list status, publication ethics, indexing, APC transparency, peer review claims, and journal risk.
- `paper-integrity-risk-auditor`: Check papers for retraction, correction, expression of concern, PubPeer concerns, publisher notices, and integrity risk before citation.
- `evidence-synthesis-matrix`: Organize screened papers into evidence matrices for Introduction, Discussion, reviews, proposals, journal selection, or manuscript revision.

## Literature Discovery And Integrity Screening

This kit can help search and organize real literature, screen journal risk, check warning list status, verify DOI and citation metadata, and review retraction, correction, expression of concern, and paper integrity risks.

It cannot guarantee automatic discovery of every research integrity issue. It only screens risk based on verifiable sources. Do not fabricate literature or journal information. Current journal status and paper status must be verified online or supplied by the user.

## Install From Current Branch

```bash
codex plugin marketplace add YOUR_GITHUB_USERNAME/soil-phage-microbiome-codex-kit --ref codex/soil-phage-skills
codex
/plugins
```

## Install After Merging To Main

```bash
codex plugin marketplace add YOUR_GITHUB_USERNAME/soil-phage-microbiome-codex-kit --ref main
codex
/plugins
```

## Usage Examples

```text
Use the soil-phage-project-planner skill to design a metadata table and analysis plan for a soil phage metagenomics project with treatment, timepoint, and soil chemistry variables.

Use the amplicon-microbiome-pipeline skill to draft a QIIME2/DADA2 workflow for my soil 16S amplicon data, including alpha diversity, beta diversity, PERMANOVA, and taxonomy visualization.

Use the shotgun-metagenomics-pipeline skill to create a reproducible shotgun metagenomics workflow for soil samples, including QC, host removal, taxonomic profiling, assembly, binning, and functional annotation.

Use the phage-virome-analysis skill to plan viral contig identification, CheckV QC, host prediction, abundance mapping, and AMG screening for soil metagenomic contigs.

Use the manuscript-journal-submission skill to help me compare candidate journals for a soil phage metagenomics manuscript, and list what information must be verified online before choosing.

帮我搜索土壤噬菌体影响微生物群落和碳氮循环的核心文献，并做文献矩阵。只使用可核验文献，标注 DOI 和风险状态。

帮我筛查这些期刊是否适合作为投稿目标或核心参考来源：检查中科院预警名单、DOAJ、COPE/出版伦理、APC 透明度和可疑信号。

帮我检查这批文献是否有撤稿、更正、expression of concern 或其他诚信风险。不要自行指控学术不端，只标注可核验风险。

帮我把这些已核验文献整理成 Introduction 的 evidence matrix，区分 background、direct evidence、method support 和 caveat。
```
