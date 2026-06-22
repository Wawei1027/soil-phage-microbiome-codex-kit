---
name: amplicon-microbiome-pipeline
description: Use when planning or executing 16S, ITS, or other amplicon microbiome analysis, including QIIME 2, DADA2, phyloseq, diversity, ordination, PERMANOVA, differential abundance, figures, and Methods drafting.
---

# Amplicon Microbiome Pipeline

Use this skill for soil 16S, ITS, or other amplicon data analysis from raw reads through manuscript-ready outputs.

## Non-negotiable research safety rules

- Do not fabricate results, citations, taxonomic labels, database names, classifier versions, software versions, or parameter values.
- Do not invent sample metadata, sequencing depth, primer sequences, or reference database release dates.
- Do not overwrite raw FASTQ files or original metadata. Write cleaned data, ASV tables, and figures to processed folders.
- If a result is intended for a manuscript, separate observed results from interpretation and label all assumptions.

## Preferred analysis routes

Prioritize one of these reproducible routes unless the user provides another established pipeline:

- QIIME 2 plus DADA2 for import, denoising, taxonomy, diversity, and provenance-rich artifacts.
- DADA2 plus phyloseq for R-centered denoising, object construction, statistics, and visualization.
- Hybrid route when needed: QIIME 2 for artifact provenance and R for custom statistics and publication figures.

## Workflow

1. Inspect raw reads with FastQC, MultiQC, read counts, read length, quality profiles, and primer orientation.
2. Create or validate manifest files, sample metadata, sample IDs, and sequencing type.
3. Trim primers and adapters with an explicit tool and parameters.
4. Run denoising with DADA2 or an equivalent method, recording truncation, trimming, pooling, chimera handling, and expected error settings.
5. Remove chimeras and summarize retained reads per sample.
6. Generate ASV table, representative sequences, taxonomy table, and feature tracking summaries.
7. Assign taxonomy with an explicitly named database, classifier, marker region, and release date when known.
8. Build or import a phylogenetic tree when phylogenetic diversity or UniFrac analyses are planned.
9. Analyze alpha diversity with models appropriate for the study design.
10. Analyze beta diversity with appropriate distances, ordination, PERMANOVA, and dispersion checks.
11. Run differential abundance only after discussing compositionality, filtering, normalization, confounders, and multiple testing correction.
12. Integrate soil environmental variables using constrained ordination, mixed models, or correlation approaches selected from the actual design.

## Soil microbiome cautions

- Remind the user to evaluate low-abundance feature filtering, contaminant control, extraction/PCR blanks, batch effects, and environmental metadata integration.
- Do not treat rarefaction as the only valid choice. Discuss sequencing depth, compositional data, library size, normalization, CLR-based approaches, variance-stabilizing methods, and method-specific assumptions.
- Check whether treatment, site, season, and sequencing batch are confounded before interpreting community differences.

## Expected outputs

When triggered, produce:

- A command script for QIIME 2, DADA2, or the selected route.
- An R visualization and statistics script using stable input/output paths.
- A result interpretation template that separates facts, uncertainty, and ecological interpretation.
- A Methods draft with placeholders for software versions, database release dates, primer sequences, and key parameters that are not yet known.
- A reproducibility checklist listing raw data locations, manifest path, metadata path, software versions, database paths, and random seeds if used.
