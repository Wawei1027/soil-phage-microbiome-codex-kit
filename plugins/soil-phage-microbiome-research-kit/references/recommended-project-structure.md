# Recommended Project Structure

```text
project-name/
  README.md
  environment/
  data/
    raw/
    metadata/
    processed/
  scripts/
    00_setup/
    01_qc/
    02_amplicon/
    03_metagenomics/
    04_virome/
    05_statistics/
    06_figures/
  results/
    qc/
    amplicon/
    metagenomics/
    virome/
    statistics/
  figures/
  tables/
  manuscript/
  logs/
```

## Notes

- Keep `data/raw/` read-only and never overwrite original FASTQ, assemblies, metadata, or lab-provided files.
- Store sample metadata and data dictionaries in `data/metadata/`.
- Store derived, script-generated files in `data/processed/`, `results/`, `figures/`, and `tables/`.
- Keep environment files, package lock files, and database manifests in `environment/`.
- Save logs for QC, denoising, assembly, profiling, statistics, and figure generation in `logs/`.
