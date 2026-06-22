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
```
