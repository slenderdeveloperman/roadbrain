# ROAD BRAIN — Unified Storyboards

[Open the canonical Paper file](https://app.paper.design/file/01M4XBCQ0SFYHGKEF9NWC2R334).

All future episode storyboard work belongs in this file, on a separate episode page. Updated from live Paper content on 2026-10-20: **86 artboards across eight pages**.

| Page | Content | Artboards |
| --- | --- | ---: |
| [00 / Shared assets & foundations](https://app.paper.design/file/01M4XBCQ0SFYHGKEF9NWC2R334/p-2-0) | EP001 kernel, tokens, EP002 night vehicles and lighting | 8 |
| [01 / EP001 — INDICATE. THEN MOVE.](https://app.paper.design/file/01M4XBCQ0SFYHGKEF9NWC2R334/p-3-0) | Six original storyboard shots | 6 |
| [02 / EP002 — DIM YOUR HIGH BEAMS.](https://app.paper.design/file/01M4XBCQ0SFYHGKEF9NWC2R334/p-4-0) | Eleven original lighting, rupture, and correction keyframes | 11 |
| [03 / EP003 — THE SHOULDER IS NOT A LANE](https://app.paper.design/file/01M4XBCQ0SFYHGKEF9NWC2R334/p-1-0) | Nine hook-first frames and three opening-only hook tests | 12 |
| [04 / EP004 — PASS. RETURN LEFT.](https://app.paper.design/file/01M4XBCQ0SFYHGKEF9NWC2R334/p-5-0) | Nine Right Lane Raja keyframes | 9 |
| [05 / EP005 — ONE LANE AT A TIME](https://app.paper.design/file/01M4XBCQ0SFYHGKEF9NWC2R334/p-7-0) | Nine keyframes: Indian two-lane road narrowing to one, bottleneck, and safe turn-by-turn merge | 9 |
| [06 / EP001 v2 — TELEPATHY REQUIRED](https://app.paper.design/file/01M4XBCQ0SFYHGKEF9NWC2R334/p-6-0) | Ten hook-first frames: inferred intent, false success, human-intent reversal, collapse and indicator correction | 10 |
| [07 / EP006 — UNMANNED JUNCTIONS](https://app.paper.design/file/01M4XBCQ0SFYHGKEF9NWC2R334/p-8-0) | Twelve canonical frames plus a separate nine-frame south-to-east simplified alternate | 21 |

## Consolidation and provenance

The 37 existing artboards were consolidated before EP004 was added. Source files were read live during consolidation; earlier screenshot exports were not used to reconstruct designs.

- [EP001 source / ROAD BRAIN v0.1 Kernel](https://app.paper.design/file/01M4KR2YRHPPZ0DBW9QTJ5MPVQ): six shot boards and six asset/foundation boards.
- [EP002 source](https://app.paper.design/file/01M4T1FP855E8S222QPWEXR402): eleven shot boards and two asset boards.
- [EP003 source](https://app.paper.design/file/01M4WW7Z0Q227S7MJN4DJX2652): cloned natively as the unified file's starting point, preserving all twelve boards and 1,108 page nodes.

EP001/EP002 were transferred using their exact live JSX, native text, SVG geometry and source child groups. Their 84 top-level visual groups were retained. Their tokens are namespaced with `--ep001-` and `--ep002-` to avoid collisions with EP003's larger caption scale. No artboard was flattened to an image. Caption whitespace and asset-row direction were checked and corrected against the sources. Storyboard boards remain 1080 × 1920.

Original files remain available as provenance. The unified file is the destination for subsequent changes; old source links should not be used for new production edits.

## Verification

Each imported/new artboard was reviewed through Paper screenshots. Final checks covered text hierarchy, contrast, alignment, clipping, chronological horizontal placement, page counts, and source completeness. EP004's customs label was moved clear of the lead car, and its correction explicitly lights the left indicator. The clean final card gives the road rule priority over the brand line.

The storyboards remain editable. EP004 has a first picture-only Cavalry motion preview; see its [motion handoff](episodes/EP004_PASS_RETURN_LEFT.md). EP005's nine keyframes now show the road narrowing from two lanes to one and the safe, orderly merge correction; motion/render remain open. See the [EP005 specification](episodes/EP005_ONE_LANE_AT_A_TIME.md). EP006 retains its twelve-board canonical sequence and adds a separate nine-board simple alternate on the same page: a south-to-east car waits as east-, north- and west-side traffic clears, then crosses. The earlier boards remain untouched. See the [EP006 specification](episodes/EP006_UNMANNED_JUNCTIONS.md). EP001 v2 is a separate, alternate telling and preserves the original EP001 reference storyboard and published master; see its [specification and motion handoff](episodes/EP001_V2_TELEPATHY_REQUIRED.md).
