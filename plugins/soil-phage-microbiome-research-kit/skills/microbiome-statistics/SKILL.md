---
name: microbiome-statistics
description: Use when analyzing microbial community differences, environmental drivers, phage-host relationships, networks, differential abundance, alpha or beta diversity, ordination, or mixed models for microbiome and virome data.
---

# Microbiome Statistics

Use this skill for statistical analysis of microbiome, virome, phage-host, metagenomics, amplicon, environmental, and community ecology data.

## Non-negotiable research safety rules

- Do not fabricate results, p-values, effect sizes, confidence intervals, citations, taxa, pathways, software versions, or database names.
- Do not report a statistical conclusion without the input data, model formula, assumptions, multiple testing correction when needed, and uncertainty.
- Do not overwrite original count tables, metadata, distance matrices, or model outputs.
- Do not present exploratory associations as causal claims unless the design supports causality.

## First confirm the data type

Before choosing a method, identify whether each input is:

- Count table.
- Relative abundance table.
- CLR transformed table.
- Presence/absence table.
- Distance matrix.
- Metadata table.
- Environmental variable table.
- Taxonomic, functional, viral, MAG, or vMAG feature table.

## Required statistical checks

Evaluate and report:

- Compositionality.
- Zero inflation.
- Overdispersion.
- Library size and sequencing depth.
- Multiple testing burden.
- Batch effects.
- Confounding.
- Pseudoreplication.
- Spatial or temporal autocorrelation.
- Environmental variable collinearity.
- Group dispersion when using PERMANOVA.

## Candidate methods

Choose methods according to data type and design. Options include:

- Alpha diversity models.
- PERMANOVA with appropriate distance metrics and permutation structure.
- betadisper or equivalent dispersion checks.
- PCoA, NMDS, PCA, and other ordination methods.
- RDA and db-RDA for constrained ordination.
- Mantel and partial Mantel only with explicit caution and a clear reason.
- ANCOM-BC, ALDEx2, DESeq2, MaAsLin2, or other differential abundance methods selected for the data scale and assumptions.
- Mixed models for nested, repeated, spatial, or temporal designs.
- Random forest for prediction with cross-validation and feature importance caveats.
- Network analysis with compositionality-aware choices, stability checks, and clear edge interpretation.

## Reporting standard

Every statistical conclusion must include:

- Effect direction.
- Effect size.
- Uncertainty, such as confidence interval, standard error, posterior interval, or model-based interval.
- Multiple testing correction when applicable.
- Model formula or test description.
- Ecological interpretation tied to the design and variables.

Do not report only a p-value. Explain whether the effect is biologically meaningful, how large it is, and what ecological process it may represent.

## R script standard

When generating R code:

- Use explicit input and output paths.
- Set seeds where stochastic methods are used.
- Keep package loading, metadata checks, filtering, transformations, models, plots, and exports in clear sections.
- Write tables and figures with stable filenames.
- Save session information or a package version summary.
- Include comments that explain why each method is used.

## Expected outputs

When triggered, produce:

- A data audit checklist.
- A method selection table.
- Reproducible R code for statistics and figures.
- A results reporting template with effect size, uncertainty, correction method, and ecological interpretation.
- A short warning section for assumptions, confounders, and residual risks.
