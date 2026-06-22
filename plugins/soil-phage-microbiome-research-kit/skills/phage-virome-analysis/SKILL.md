---
name: phage-virome-analysis
description: Use when analyzing bacteriophages, viromes, viral contigs, prophages, vMAGs, host prediction, viral taxonomy, AMG screening, abundance mapping, or soil phage ecological interpretation.
---

# Phage Virome Analysis

Use this skill for soil phage, viral metagenome, viral contig, prophage, vMAG, host prediction, viral taxonomy, AMG, and phage-host ecology workflows.

## Non-negotiable research safety rules

- Do not fabricate viral contigs, host predictions, AMG calls, taxonomy, citations, database names, database dates, software versions, or ecological conclusions.
- Do not treat predicted hosts or AMGs as confirmed without confidence levels and validation evidence.
- Do not overwrite raw assemblies, raw reads, or original viral predictions. Keep each tool output in a separate results directory.
- Explicitly separate bacteriophage, eukaryotic virus, prophage, viral-like sequence, plasmid-like sequence, and uncertain sequence labels.

## Workflow

1. Check contig inputs: source assembly, minimum length, N50, coverage, circularity evidence, sample origin, and whether contigs came from bulk metagenomes or viral-enriched libraries.
2. Identify viral sequences using multiple tools when appropriate, such as VirSorter2, VIBRANT, geNomad, or other validated methods.
3. Assess viral quality with CheckV or an equivalent approach, recording completeness, contamination, provirus status, and quality category.
4. Remove redundancy with explicit average nucleotide identity, coverage, and clustering thresholds.
5. Classify and annotate viral sequences using transparent databases and tools such as geNomad, vContact2, BLAST, DIAMOND, or curated viral protein databases.
6. Predict hosts using evidence from iPHoP, CRISPR spacer matching, tRNA matches, k-mer similarity, genomic similarity, proximity to microbial genomes, or other justified methods.
7. Assign every host prediction to one of:
   - High confidence: multiple independent evidence types or a highly specific validated match.
   - Medium confidence: one strong evidence type or consistent but limited support.
   - Low confidence: weak, broad, indirect, or exploratory evidence.
8. Map reads back to viral contigs or vMAGs for abundance estimates, with explicit mapping thresholds and normalization strategy.
9. Screen AMGs using protein annotation, viral quality, gene context, genomic neighborhood, contig-edge proximity, and possible host contamination.
10. Link viral results to soil ecological processes, including carbon, nitrogen, and phosphorus cycling; host community shifts; environmental gradients; disturbance; season; land use; and treatment groups.

## AMG caution

Do not call an AMG from keyword matches alone. Require inspection of viral contig quality, gene context, flanking genes, proximity to contig edges, annotation support, and whether the sequence may represent host contamination or a mis-binned region.

## Expected outputs

When triggered, produce:

- A reproducible command workflow for viral identification, quality assessment, dereplication, taxonomy, host prediction, abundance mapping, and AMG screening.
- A table schema for viral contigs, quality, taxonomy, host predictions, confidence levels, abundance, and AMG candidates.
- A list of required database paths, software versions, and parameters.
- A soil ecological interpretation plan that separates evidence-backed conclusions from hypotheses.
- A Methods paragraph draft with placeholders for unknown software versions, database dates, and thresholds.
