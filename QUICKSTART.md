# Quickstart

This guide helps you install and test the Soil Phage Microbiome Codex Kit.

## 1. Install the plugin marketplace

From a terminal with Codex available, run:

```bash
codex plugin marketplace add Wawei1027/soil-phage-microbiome-codex-kit --ref codex/soil-phage-skills
codex
/plugins
```

If you are testing this documentation branch before merge, use:

```bash
codex plugin marketplace add Wawei1027/soil-phage-microbiome-codex-kit --ref docs/toolbox-polish-20260706
```

## 2. Confirm the skills are visible

Inside Codex, open `/plugins` and confirm that `soil-phage-microbiome-research-kit` is installed. The skills should include project planning, amplicon analysis, shotgun metagenomics, phage and virome analysis, microbiome statistics, figures, manuscripts, literature mapping, DOI checking, journal screening, paper integrity auditing, and evidence synthesis.

## 3. Run a smoke test

Try one prompt from `examples/smoke-test-prompts.md`, for example:

```text
Use the soil-phage-project-planner skill to design a metadata checklist and analysis roadmap for a soil phage metagenomics project with treatment, timepoint, and soil chemistry variables.
```

## 4. Safety expectations

Do not place raw sequencing data, private manuscripts, API keys, unpublished results, reviewer comments, or sensitive personal information in this repository. When using the kit for real literature, journal, or paper-integrity tasks, verify current information online or provide trusted sources.
