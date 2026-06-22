---
name: soil-phage-project-planner
description: Use when designing soil microbiome, bacteriophage, virome, shotgun metagenomics, or amplicon projects; organizing metadata; planning analysis routes; or checking experimental design.
---

# Soil Phage Project Planner

Use this skill to turn a soil microbiome, phage, virome, shotgun metagenomics, 16S, ITS, or mixed-marker study idea into a concrete, auditable project plan.

## Non-negotiable research safety rules

- Do not fabricate results, citations, species names, database names, software versions, parameter values, accession IDs, or sampling details.
- Do not infer missing metadata as fact. Mark gaps explicitly and ask for the missing information or propose placeholders labeled as placeholders.
- Do not overwrite raw data. Keep original FASTQ, metadata sheets, lab notes, and received files read-only in `data/raw` or `data/metadata`.
- Record every assumption, data transformation, filtering rule, software version, database path, and database release date when available.

## Required intake checklist

Collect or verify these fields before proposing the final design:

- Sample source: ecosystem, site, plot, treatment, depth, rhizosphere or bulk soil, and collection method.
- Soil type and measured soil properties, including pH, moisture, temperature, organic matter, nitrate, ammonium, total C, and total N when available.
- Treatment groups, controls, time points, gradients, disturbance regimes, land use categories, and management history.
- Spatial design: plot layout, coordinates, nested structure, spatial replicates, and blocking.
- Biological replicates, technical replicates, extraction replicates, PCR replicates, and sequencing lanes or batches.
- Sequencing type: 16S, ITS, shotgun metagenomics, virome, viral-enriched metagenomics, metatranscriptomics, or mixed data.
- Planned sequencing depth and expected read length.
- Negative controls, positive controls, mock communities, extraction blanks, PCR blanks, spike-ins, and contamination tracking.

## Design checks

Before recommending analyses, check for:

- Pseudoreplication: distinguish true biological replicates from repeated reads, PCR replicates, subsamples, or repeated measures from the same plot.
- Batch effects: extraction kit, extraction date, PCR batch, library prep, sequencing run, lane, operator, and shipment.
- Spatial autocorrelation: plots nested in sites, distance among samples, transects, blocks, and field gradients.
- Temporal autocorrelation: repeated sampling dates, seasons, lag effects, and pre/post treatment structure.
- Environmental variable collinearity: pH, moisture, nutrients, organic matter, temperature, land use, and treatment covariates.
- Confounding: treatment aligned with site, batch aligned with treatment, or timepoint aligned with sequencing run.

## Planning workflow

1. Restate the research question in one or two testable sentences.
2. List primary and secondary hypotheses before selecting methods.
3. Map each hypothesis to required data, statistical method, figure, and table.
4. Identify missing metadata and design risks.
5. Recommend a reproducible folder layout:

```text
data/raw
data/metadata
data/processed
scripts
results
figures
tables
manuscript
```

6. Propose a file naming scheme, sample ID rules, and metadata validation checks.
7. Draft an analysis roadmap with dependencies among QC, profiling, statistics, figures, and manuscript outputs.

## Output format

When triggered, produce:

- A short project summary.
- A missing information table.
- A design risk table with severity and suggested mitigation.
- A hypothesis to method to figure mapping.
- A recommended project directory structure.
- A first-pass analysis timeline.
- A reproducibility checklist covering raw data protection, metadata versioning, software versions, database paths, and logs.
