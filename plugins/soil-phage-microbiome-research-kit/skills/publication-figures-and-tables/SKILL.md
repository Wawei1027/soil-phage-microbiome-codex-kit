---
name: publication-figures-and-tables
description: Use when creating microbiome, phage, virome, metagenomics, MAG, vMAG, statistics, manuscript, or supplementary figures and tables, including captions, legends, and reproducible plotting code.
---

# Publication Figures And Tables

Use this skill to create journal-ready figures, figure legends, result tables, supplementary tables, and reproducible plotting scripts for microbiome, phage, virome, and metagenomics manuscripts.

## Non-negotiable research safety rules

- Do not fabricate results, taxa, pathways, host links, quality metrics, statistics, captions, citations, software versions, or database names.
- Do not make a figure that cannot be regenerated from a script and input data.
- Do not overwrite original result tables or raw data. Export derived figure inputs to a versioned table or processed directory.
- If a statistic appears in a caption, it must come from a traceable test output.

## Figure types to consider

Choose figures that match the story and data:

- Sampling design figure.
- Workflow figure.
- Stacked bar plot.
- Heatmap.
- PCoA or NMDS.
- RDA or db-RDA.
- Volcano plot.
- Effect size plot.
- Network plot.
- Phage-host link plot.
- MAG or vMAG quality summary.
- Functional pathway figure.
- Alpha diversity panel.
- Differential abundance panel.
- Environmental gradient response figure.

## Design rules

- Prefer information density, readability, color-blind friendly palettes, and journal-acceptable layouts.
- Avoid excessive decoration, unsupported visual metaphors, and misleading scales.
- Use consistent sample ordering, treatment colors, taxonomy levels, and abbreviations across figures.
- Label axes, transformations, units, grouping variables, and statistical tests.
- Default to PDF or SVG for submission and PNG for talks or quick sharing.

## Required output per figure

For every figure, produce:

- Figure file name.
- Figure purpose.
- Input data files and required columns.
- R or Python code to regenerate the figure.
- Caption draft.
- Statistical test explanation.
- Export format and dimensions.
- Notes on color palette, ordering, and journal constraints.

## Table rules

- For main tables, prioritize concise results that support the manuscript claims.
- For supplementary tables, include enough detail to audit feature IDs, taxonomy, viral contig IDs, host prediction confidence, model terms, adjusted p-values, effect sizes, and database/source information.
- Use stable identifiers and avoid manually edited copies that cannot be regenerated.

## Expected outputs

When triggered, produce:

- A figure and table plan tied to manuscript results.
- Reproducible plotting scripts in R or Python.
- Main and supplementary table schemas.
- Caption and legend drafts.
- A final checklist for file formats, font sizes, line weights, colors, statistical labels, and regeneration from scripts.
