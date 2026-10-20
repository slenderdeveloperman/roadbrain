# ROAD BRAIN EP005 — ONE LANE AT A TIME

**Concept:** A familiar two-lane Indian road suddenly narrows to one. Drivers crowd the pinch point side by side instead of signalling, checking, and merging in turn when safe. A left-side-traffic road diagram, mixed vehicles, and dry system diagnostics make the bottleneck legible without depicting a collision. **Status:** nine editable Paper keyframes updated for the narrowing-road concept; motion and render remain open. **Format target:** 1080 × 1920, 30 fps, 25.2 seconds / 756 frames.

[Open EP005 in the unified Paper storyboard](https://app.paper.design/file/01M4XBCQ0SFYHGKEF9NWC2R334/p-7-0). See the [storyboard index](../STORYBOARDS.md) for the full series file.

## Story

Hook: **TWO LANES IN. ONE LANE OUT.** A marked two-lane road tapers abruptly to one lane, with the left-side traffic orientation kept consistent. The system notices the road narrowing; two streams of drivers then reach the same pinch point, searching for a gap and trying to occupy the same space. The diagnosis gets blunt: `ROAD: 2 → 1 / DRIVERS: STILL 2`, then `MERGE WINDOW: CLOSED BY EGO.` No crash is shown. A hard reset restores a clear road. The correction is simple: signal, check for a safe gap, and take turns. Follow the road's signs and markings.

Escalation:

```text
ROAD NARROWS
2 LANES → 1
GAP: LEFT? / GAP: RIGHT?
ROAD: 2 → 1
DRIVERS: STILL 2
POSITION: SIDE BY SIDE
PROGRESS: NONE
MERGE WINDOW: CLOSED BY EGO
```

Correction: **SIGNAL. CHECK. TAKE TURNS.**

Final rule: **MERGE IN TURN.** Qualification: **ONLY WHEN SAFE.** Brand close: **DRIVE PREDICTABLY.**

## Storyboard pass

Frame ranges are inclusive. The nominal 1.55-second boundary rounds to frame 47 at 30 fps, giving an actual cut at 1.5667 seconds.

| Board | Time | Frames | Picture / copy |
| --- | --- | ---: | --- |
| 00 Visual interrupt | 0.00–0.20 | 0–5 | Open on two lanes visibly tapering to one; show the pinch before the viewer has time to settle. Mixed traffic includes a three-wheeler and a two-wheeler. |
| 01 Hook | 0.20–1.55 | 6–46 | `TWO LANES IN. / ONE LANE OUT.` The wider road narrows ahead; left-side traffic continues through the pinch. |
| 02 Condition | 1.55–4.90 | 47–146 | `ROAD NARROWS / 2 LANES → 1`; establish the lane markings and the fixed merge point. |
| 03 Detection | 4.90–9.80 | 147–293 | `TWO LANES / BECOME ONE`; traffic reaches the narrowed section, with an amber trace showing the unsafe side-by-side approach. |
| 04 Search loop | 9.80–12.20 | 294–365 | `SEARCHING...`; `GAP: LEFT?` and `GAP: RIGHT?` trade places as the system tries to resolve an opening. |
| 05 Geometry failure | 12.20–14.70 | 366–440 | `ROAD: 2 → 1 / DRIVERS: STILL 2`; repeated vehicle positions crowd the narrowing without implying impact. |
| 06 Collapse | 14.70–19.50 | 441–584 | `MERGE WINDOW: / CLOSED BY EGO`; system status reads `POSITION: SIDE BY SIDE / PROGRESS: NONE`. The lane is blocked, not crashed. |
| 07 Correction | 19.50–23.60 | 585–707 | Hard reset. Show an indicator, a checked gap, and vehicles entering the single lane in turn. Caption: `SIGNAL. CHECK. / TAKE TURNS.` |
| 08 Rule | 23.60–25.20 | 708–755 | Pristine card: `MERGE / IN TURN.` Add `ONLY WHEN SAFE.` and secondary `DRIVE PREDICTABLY.` |

The Paper page has nine editable native keyframes. The visual road is wider at the near end and narrows to one lane ahead, with the left road edge continuing and the right lane tapering into it. This gives the sequence a left-side-traffic context without prescribing a manoeuvre that conflicts with local signs or markings.

## Visual direction

Retain the detailed top-view car artwork and add recognizable three-wheeler and two-wheeler silhouettes as secondary traffic. Keep the road boundaries and lane divider clean enough that the two-to-one transition reads at a glance. Amber marks the unstable gap search; red is reserved for system diagnosis; green appears only on the safe corrective path. Do not show forced contact, teach drivers to cross a solid marking, or suggest that a driver should enter a gap that is not safe.

## Rule basis and scope

The [Motor Vehicles (Driving) Regulations, 2017](https://morth.gov.in/sites/default/files/Motor-Vehicle-Driving-Regulation-2017.pdf), Regulation 6, says drivers on lane-marked roads should remain within their lane and change lanes only after the prescribed signal, marking, or signage. Regulation 5 requires due care and caution. Regulation 8 includes signalling and checking traffic to the side and behind when moving into a turn lane. The episode's `MERGE IN TURN` and `ONE LANE AT A TIME` are plain-language instructions, not verbatim statutory quotations. `ONLY WHEN SAFE` and the reminder to follow signs and markings preserve that scope.

## Open work

- Review the narrowed-road geometry and confirm the hook reads without sound.
- Refine the motion so the two approaches become one orderly single-file stream; do not animate a collision or unsafe forced merge.
- Translate the approved Paper vectors into Cavalry and retain the clean hard reset at frame 585.
- Keep any rendered motion picture-only until separate soundtrack direction is given.
- Verify 1080 × 1920, 30 fps, 756 frames / 25.20 seconds, with no audio unless separately requested.
