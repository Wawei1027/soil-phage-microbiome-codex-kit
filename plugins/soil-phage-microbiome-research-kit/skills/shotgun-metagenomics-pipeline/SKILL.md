---
name: shotgun-metagenomics-pipeline
description: Use when planning or running shotgun metagenomics analysis for soil microbial communities, including QC, host removal, taxonomic profiling, assembly, binning, MAG quality, functional annotation, pathway profiling, workflow scripts, and Methods drafting.
---

# Shotgun Metagenomics Pipeline

Use this skill for shotgun metagenomics projects that need a reproducible analysis plan, shell script, Snakemake draft, Nextflow draft, interpretation notes, or Methods text.

## Non-negotiable research safety rules

- Do not fabricate results, citations, species calls, database names, database dates, software versions, or parameter values.
- Do not invent host genomes, reference paths, sample metadata, assembly statistics, MAG quality metrics, or pathway results.
- Do not overwrite raw FASTQ files. Write derived files to processed, results, logs, and temporary workflow directories.
- If drafting manuscript Methods, use placeholders for unknown versions, database dates, and parameters rather than making them up.

## Modular workflow

1. Run FastQC and MultiQC for raw read quality.
2. Perform adapter and quality trimming with recorded tool, version, and parameters.
3. Remove host or non-target reads when relevant using explicit reference genome paths, Bowtie2 or another aligner, and samtools-based summaries.
4. Choose taxonomic profiling tools by task, not by habit:
   - Kraken2 and Bracken for k-mer classification and abundance re-estimation.
   - MetaPhlAn for marker-gene profiling.
   - Other validated profilers when required by the project.
5. Choose functional and pathway profiling by task:
   - HUMAnN for gene family and pathway profiles.
   - eggNOG-mapper, DRAM, Prokka, or equivalent tools for annotation of assemblies, contigs, or bins.
6. Assemble reads when appropriate with MEGAHIT, metaSPAdes, or another selected assembler.
7. Assess contig QC: assembly size, N50, length distribution, GC distribution, read mapping, and coverage.
8. Bin contigs when the project needs MAGs, using appropriate binners and refinement.
9. Assess MAG quality with explicit completeness, contamination, strain heterogeneity, taxonomy, and dereplication criteria.
10. Profile pathways, functional genes, or biogeochemical marker genes with transparent databases and thresholds.
11. Summarize taxonomic, functional, assembly, binning, and pathway outputs for downstream statistics and figures.

## Tool selection rule

Recommend tools according to the input data, research question, available compute, and expected output. Candidate tools may include Kraken2, Bracken, MetaPhlAn, HUMAnN, MEGAHIT, metaSPAdes, Bowtie2, samtools, Prokka, eggNOG-mapper, DRAM, and related validated tools, but do not force a single software stack.

## Reproducibility requirements

- Record every database path, software version, database release date, parameter set, input file, output file, and log file.
- Keep workflow scripts idempotent where possible and avoid commands that overwrite existing results without an explicit backup or versioned output path.
- Prefer a shell script for small projects and Snakemake or Nextflow for multi-sample or multi-module projects.

## Expected outputs

When triggered, produce:

- A reproducible shell script, Snakemake draft, or Nextflow draft.
- A directory and naming convention for QC, taxonomic profiling, assembly, binning, annotation, and pathway profiling.
- A table of required metadata, software versions, database paths, and missing values.
- A Methods paragraph draft with placeholders for unknown versions and database dates.
- A result interpretation guide that distinguishes observed profiles, statistical evidence, and ecological interpretation.
