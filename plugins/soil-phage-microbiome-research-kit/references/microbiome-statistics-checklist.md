# Microbiome Statistics Checklist

Use this checklist before reporting microbiome, virome, phage-host, amplicon, shotgun, functional, or environmental statistics.

## Input audit

- Data type is identified: count, relative abundance, CLR, presence/absence, distance matrix, metadata, or environmental table.
- Sample IDs match across all tables.
- Filtering rules are documented.
- Missing metadata and excluded samples are listed.
- Batch variables and nested design variables are available.

## Assumption checks

- Compositionality is considered.
- Zero inflation and overdispersion are considered.
- Sequencing depth or library size effects are addressed.
- Group dispersion is checked for PERMANOVA.
- Multiple testing correction is applied where needed.
- Confounding, pseudoreplication, spatial autocorrelation, and temporal autocorrelation are considered.
- Environmental variable collinearity is checked before multivariable models.

## Reporting

- Report model formula or test design.
- Report effect direction and effect size.
- Report uncertainty.
- Report adjusted p-values where multiple testing is performed.
- Provide ecological interpretation.
- Avoid p-value-only conclusions.
- Do not fabricate statistics, taxa, pathways, host links, or citations.
