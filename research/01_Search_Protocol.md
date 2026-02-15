---
note_id: BRN-PROTOCOL-01
title: Search Protocol
type: protocol
created_utc: 2026-02-15T21:42:17Z
updated_utc: 2026-02-15T21:42:17Z
tags:
  - bernedoodle
  - search
  - protocol
coverage_status: partial
---

# Search Protocol

> [!summary]
> Frozen query sets were applied for Bernedoodle literal and concept-equivalent naming plus core canine guideline collection.

## Protocol Links
- [[00_Home]]
- [[02_Screening_and_PRISMA]]
- [[03_Bernedoodle_Evidence_Map]]

## Frozen Query Library

| Query ID | Database | Query |
|---|---|---|
| Q_BERNE_1_PUBMED | PubMed | `("bernedoodle"[All Fields] OR "berne-doodle"[All Fields] OR ("bernese mountain dog"[All Fields] AND poodle[All Fields] AND (cross*[All Fields] OR hybrid*[All Fields] OR mix*[All Fields])))` |
| Q_BERNE_2_PUBMED | PubMed | `(("berner"[All Fields] OR "boyero de berna"[All Fields] OR "bouvier bernois"[All Fields] OR "berner sennenhund"[All Fields]) AND ("poodle"[All Fields] OR "caniche"[All Fields] OR "barbon"[All Fields] OR "pudel"[All Fields]) AND (cross*[All Fields] OR hybrid*[All Fields] OR "croise"[All Fields] OR "cruza"[All Fields] OR "kreuzung"[All Fields] OR "mestizo"[All Fields]))` |
| Q_BERNE_3_PUBMED | PubMed | `("standard poodle crossbred"[All Fields] AND "patent ductus arteriosus"[All Fields])` |
| Q_BERNE_1_CROSSREF | Crossref | `query=bernedoodle` |
| Q_BERNE_2_CROSSREF | Crossref | `query="bernese mountain dog" poodle crossbreed` |
| Q_BERNE_1_SCHOLAR | Google Scholar | `"bernedoodle" OR "berne-doodle" dog health` |
| Q_BERNE_2_SCHOLAR | Google Scholar | `"Bernese Mountain Dog" poodle cross health dog` |
| Q_GUIDE_WSAVA_SITE | WSAVA | `site:wsava.org dog guideline vaccination nutrition dental` |
| Q_GUIDE_AAHA_SITE | AAHA | `site:aaha.org canine guideline vaccination nutrition dental parasite` |
| Q_GUIDE_CAPC_SITE | CAPC | `site:capcvet.org dog parasite guideline` |

## Source Matrix Status

| Source | Status | Notes |
|---|---|---|
| PubMed | completed | Direct Bernedoodle term confirmed sparse indexed literature. |
| Europe PMC | partial | Indirect checks only; full structured export not completed in this run. |
| Crossref | completed | Direct `bernedoodle` query returned zero exact matches. |
| Google Scholar | partial | Used for discovery signals only; full deterministic top-200 capture not completed. |
| CAB Abstracts | blocked | No accessible index connection in this environment. |
| Scopus/Web of Science | blocked | No accessible index connection in this environment. |
| WSAVA/AAHA/CAPC | completed | Guideline records captured and indexed in source notes. |

## Machine Logs
- `research/data/search_log.json`
- `research/data/coverage_status.json`
