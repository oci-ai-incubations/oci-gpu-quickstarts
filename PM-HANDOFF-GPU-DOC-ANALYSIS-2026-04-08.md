# PM Handoff: GPU README Coverage and Drift Analysis

Date: 2026-04-08

Repository: `/Users/zsmith/github/oci-gpu-quickstarts`

## Purpose

This document combines the latest:

- README coverage gap analysis
- internal/public/source drift analysis

The goal is to give product management a clear view of:

- which GPU families are fully documented
- which GPU families are missing publication steps
- which GPU families may need refresh work because the internal README has drifted from public content or current source material

## Executive Summary

### Best current state

These GPU families are effectively complete across the major content locations:

- `B200`
- `GB200`
- `GB300`
- `MI300X`
- `MI355X`

### Highest-priority publication gaps

These GPU families now have source documents and internal READMEs, but are not yet published upstream as public README content:

- `H100`
- `H200`

These are the clearest near-term content promotion candidates.

### Public visibility gaps

These GPU families are documented in repo content but do not currently appear as separate public OCI shape-doc entries on the public Compute Shapes page:

- `B300`
- `GB200-v2`
- `GB200-v3`
- `MI355X-Pollara`

These are not missing README problems; they are public-shape-doc visibility gaps.

### Highest-confidence drift / refresh candidates

These GPU families show the clearest signs of incomplete or aging content and should be treated as priority follow-up items:

- `B200`
- `MI300X`
- `MI355X-Pollara`

## Coverage Analysis

This matrix answers:

1. does a source document exist?
2. does an internal README exist in the staging repo?
3. does a public README exist in the public repo?
4. does the shape appear in public OCI Compute Shapes documentation?

| Vendor | GPU Family | Source Document | Internal README | Public README | Public OCI Shape Docs | Coverage Status |
|---|---|---|---|---|---|---|
| NVIDIA | B200 | Yes | Yes | Yes | Present in public docs | Complete |
| NVIDIA | B300 | Yes | Yes | Yes | Not present in public docs | Public README present, not in public docs |
| NVIDIA | GB200 | Yes | Yes | Yes | Present in public docs | Complete |
| NVIDIA | GB200-v2 | Yes | Yes (shared with `README-GB200.md`) | Yes (shared) | Not present in public docs | Public README present, not in public docs |
| NVIDIA | GB200-v3 | Yes | Yes (shared with `README-GB200.md`) | Yes (shared) | Not present in public docs | Public README present, not in public docs |
| NVIDIA | GB300 | Yes | Yes | Yes | Present in public docs | Complete |
| NVIDIA | H100 | Yes | Yes | No | Present in public docs | Staged internally |
| NVIDIA | H200 | Yes | Yes | No | Present in public docs | Staged internally |
| AMD | MI300X | Yes | Yes | Yes | Present in public docs | Complete |
| AMD | MI355X | Yes | Yes | Yes | Present in public docs | Complete |
| AMD | MI355X-Pollara | Yes | Yes | Yes | Not present in public docs | Public README present, not in public docs |

## Drift Analysis

This matrix combines two signals:

- `Internal vs Public Drift`
  - whether the internal canonical README differs from the public upstream README where both exist
- `Source Drift Signal`
  - whether the current source document or latest image lifecycle appears to have moved ahead of the README

### Drift categories

- `README drift detected`
  - internal and public README content differ materially
- `Public README missing`
  - no upstream public README exists yet
- `No obvious source drift signal`
  - no quick signal of source/image freshness issues
- `Source drift detected`
  - clear signs of incomplete or outdated source alignment
- `Newer image batch detected`
  - image lifecycle likely moved beyond what the README reflects
- `Possible section drift`
  - source appears older-style or structurally inconsistent enough to warrant review

| GPU Family | Internal vs Public Drift | Source Drift Signal | Notes |
|---|---|---|---|
| `B200` | README drift detected | Source drift detected | Internal README is still explicitly under construction, while a source document exists. |
| `B300` | README drift detected | No obvious source drift signal | Internal README was freshly regenerated from current source and current March 2026 image set; public README appears much older/sparser. |
| `GB200` | README drift detected | Newer image batch detected | Internal README now includes `GB200-v3` coverage, but image/software detail likely trails the latest image batch. |
| `GB200-v2` | README drift detected | Newer image batch detected | Covered via the shared GB200 family README; same image-lifecycle drift signal as `GB200`. |
| `GB200-v3` | README drift detected | Newer image batch detected | Also covered via the shared GB200 family README; same image-lifecycle drift signal as `GB200`. |
| `GB300` | README drift detected | Newer image batch detected | Internal and public README both exist, but the content likely trails the latest image-batch state. |
| `H100` | Public README missing | Possible section drift | Internal README exists, but the source document is older-style and its stack guidance predates the modern March 2026 image set used in current repo content. |
| `H200` | Public README missing | Possible section drift | Same pattern as H100: current internal README is modernized, but source structure and stack assumptions are older. |
| `MI300X` | README drift detected | Source drift detected | Internal README remains under construction, so drift from current source is highly likely. |
| `MI355X` | README drift detected | No obvious source drift signal | Internal README appears closer to current source and image state than most older docs. |
| `MI355X-Pollara` | README drift detected | Source drift detected | Internal README still contains `To be updated` image-packer cells and placeholder image-link text, so it remains partially incomplete relative to source. |

## Interpretation Guide

### What counts as “complete”

A GPU family is effectively complete when:

- a source document exists
- an internal README exists
- a public README exists
- the family appears in public OCI shape docs, when applicable
- there are no obvious drift signals

### What counts as “staged internally”

A GPU family is staged internally when:

- the source document exists
- the internal README exists
- the public README does not yet exist

This is the current state for:

- `H100`
- `H200`

### What counts as “publication drift”

Publication drift means the public README is lagging behind the internal README or current source material. This is most relevant when:

- the internal README has already been refreshed
- the public README still reflects older content

The clearest example right now is:

- `B300`

## Recommended Action Queue

### Priority 1: Publish newly staged content

- Publish `H100` README upstream
- Publish `H200` README upstream

Reason:

- both have source documents
- both now have internal README coverage
- both already have public OCI shape visibility

### Priority 2: Refresh incomplete or aging content

- `MI355X-Pollara`
- `MI300X`
- `B200`

Reason:

- strongest drift or incompleteness signals
- likely to need source-to-README refresh work before broader reuse

### Priority 3: Reconcile internal/public drift

- `B300`
- `GB200` family
- `GB300`
- `MI355X`

Reason:

- public and internal README content differ
- some of these likely need only synchronization rather than a full rewrite

### Priority 4: Monitor OCI public shape-doc visibility

- `B300`
- `GB200-v2`
- `GB200-v3`
- `MI355X-Pollara`

Reason:

- these are documented in repo content but are not currently represented as separate public OCI shape entries

## Caveats

- `GB200`, `GB200-v2`, and `GB200-v3` are intentionally handled as one family README, so the shared file should be considered the canonical coverage location for all three variants.
- This analysis uses published/internal canonical files, not local scratch or comparison artifacts.
- Drift analysis here is a practical operational signal, not a full semantic rewrite recommendation.
- Public OCI shape-doc presence is a useful GA/public-visibility signal, but not the sole source of truth for documentation readiness.

## Suggested Next Steps

1. Promote `H100` and `H200` into the public repo.
2. Run a deeper section-by-section drift refresh for:
   - `MI355X-Pollara`
   - `MI300X`
   - `B200`
3. Re-run coverage and drift analysis after public publication or major image-batch updates.
