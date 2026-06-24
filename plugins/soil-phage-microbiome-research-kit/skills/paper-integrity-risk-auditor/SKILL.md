---
name: paper-integrity-risk-auditor
description: Use when checking whether a paper has retraction, correction, expression of concern, PubPeer concerns, paper mill red flags, image/data concerns, suspicious citations, or other research integrity risks.
---

# Paper Integrity Risk Auditor

Use this skill when checking whether an article has documented research integrity risks before citing it as evidence.

## Safety rules

- Do not independently accuse authors, papers, journals, or labs of misconduct.
- Only mark risks based on verifiable sources.
- "No known issue found" does not mean "no issue exists."
- Retracted papers must not be used as positive evidence unless the user is discussing the retraction or integrity issue itself.
- Mark unverifiable records as `insufficient information`.

## Sources to check

- Retraction Watch Database.
- Crossref and Crossmark updates.
- PubMed retraction notices if biomedical.
- Publisher page.
- Journal correction or retraction page.
- PubPeer if available.
- Article DOI landing page.

## Screening fields

Check:

- DOI.
- Article title.
- Authors.
- Journal.
- Year.
- Retraction status.
- Correction status.
- Expression of concern.
- Publisher notice.
- PubPeer comments.
- Duplicated image or data concerns if publicly reported.
- Paper mill red flags if publicly documented.

## Integrity status labels

Use:

- No known issue found.
- Correction found.
- Expression of concern found.
- Retracted.
- Unresolved concern.
- Insufficient information.

## Citation use recommendations

Use:

- Safe for background.
- Use cautiously.
- Avoid as core evidence.
- Do not cite unless discussing retraction/problem.

## Output format

When triggered, provide:

- Paper integrity status.
- Risk notes.
- Whether the paper can be used as core evidence.
- Recommended citation use.
- Source URLs and date verified.
