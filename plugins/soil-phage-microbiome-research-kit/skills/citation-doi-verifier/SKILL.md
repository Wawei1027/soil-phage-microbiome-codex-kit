---
name: citation-doi-verifier
description: Use when checking whether a citation, DOI, paper title, author list, year, journal name, publisher, or bibliographic record is real and internally consistent.
---

# Citation DOI Verifier

Use this skill when checking whether a bibliographic record is real, resolvable, and internally consistent.

## Safety rules

- Do not correct citations from memory.
- If evidence cannot be found, mark the record as `[unverified]`.
- Do not assume similar titles refer to the same paper.
- If DOI and title do not match, mark the record as high risk.
- Do not fabricate DOI, authors, title, journal, publisher, year, volume, issue, pages, or article number.

## Inputs

Accept:

- DOI.
- Title.
- Author list.
- Journal.
- Year.
- BibTeX.
- RIS.
- Reference list.

## Verification fields

Check:

- DOI resolves?
- Title matches?
- First author matches?
- Year matches?
- Journal or source matches?
- Publisher matches?
- Volume, issue, pages, or article number match?
- Crossref, OpenAlex, or Semantic Scholar metadata match?

## Output format

When triggered, provide:

- Verified citation.
- Mismatch table.
- Corrected citation if evidence supports it.
- Unresolved records.
- Citations requiring manual verification.
- Risk labels for high-risk mismatches.
