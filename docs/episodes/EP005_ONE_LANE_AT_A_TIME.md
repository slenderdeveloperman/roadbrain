# ROAD BRAIN EP005 — ONE LANE AT A TIME

**Concept:** A driver keeps drifting across lanes after reaching a target lane. The system repeatedly marks the target acquired, loses it, and searches again until the road geometry multiplies without moving traffic forward. **Status:** nine editable first-pass Paper keyframes; story and motion remain open. **Format target:** 1080 × 1920, 30 fps, 25.2 seconds / 756 frames.

[Open EP005 in the unified Paper storyboard](https://app.paper.design/file/01M4XBCQ0SFYHGKEF9NWC2R334/p-7-0). See the [storyboard index](../STORYBOARDS.md) for the full series file.

## Story

Hook: **FOUR LANES. ZERO COMMITMENT.** The amber car reaches a lane, then immediately drifts out of it. `TARGET LANE ACQUIRED` becomes `TARGET LANE LOST`; the system flips between left and right targets. Its response is to multiply the road into more lanes while the car makes no progress. The hard reset restores ordinary road geometry. The driver signals, checks, makes one deliberate lane change, and settles into the lane.

System escalation:

```text
TARGET LANE ACQUIRED
TARGET LANE LOST
SEARCHING...
LANE COUNT: STILL ONE DRIVER
VEHICLE HAS DECLINED GEOMETRY
POSITION: EVERYWHERE
SPEED: UNCHANGED
```

Correction: **SIGNAL. CHECK. CHANGE ONE LANE.**

Final rule: **ONE LANE AT A TIME.** Qualification: **ONLY WHEN SAFE.** Brand close: **DRIVE PREDICTABLY.**

## First storyboard pass

Frame ranges are inclusive. The nominal 1.55-second boundary rounds to frame 47 at 30 fps, giving an actual cut at 1.5667 seconds.

| Board | Time | Frames | Picture / copy |
| --- | --- | ---: | --- |
| 00 Visual interrupt | 0.00–0.20 | 0–5 | Open mid-drift: amber car straddles a broken lane divider; another car holds its lane. |
| 01 Hook | 0.20–1.55 | 6–46 | `FOUR LANES. / ZERO COMMITMENT.` |
| 02 Condition | 1.55–4.90 | 47–146 | `TARGET LANE / ACQUIRED`; the car reaches the lane, then starts moving again. |
| 03 Detection | 4.90–9.80 | 147–293 | `TARGET LANE / LOST`; a route trace records another lateral drift. |
| 04 Search loop | 9.80–12.20 | 294–365 | `SEARCHING...`; target labels flip between left and right. |
| 05 Geometry failure | 12.20–14.70 | 366–440 | `LANE COUNT: / STILL ONE DRIVER`; road markings multiply around repeated car positions. |
| 06 Collapse | 14.70–19.50 | 441–584 | `VEHICLE HAS / DECLINED GEOMETRY`; diagnostics say `POSITION: EVERYWHERE / SPEED: UNCHANGED`. |
| 07 Correction | 19.50–23.60 | 585–707 | Hard reset. Show left signal on, a checked gap, and one deliberate lane change. Caption: `SIGNAL. CHECK. / CHANGE ONE LANE.` |
| 08 Rule | 23.60–25.20 | 708–755 | Pristine card: `ONE LANE / AT A TIME.` Add `ONLY WHEN SAFE.` and secondary `DRIVE PREDICTABLY.` |

The Paper page currently has nine editable native keyframes. Its lane-count collapse uses repeated vehicle placements as storyboard shorthand; motion design should keep the real driving readable and should not depict a collision.

## Visual direction

Reuse the ROAD BRAIN three-lane road and detailed top-view hatchback. Keep the base diagram legible and stable through the first condition beat. Amber marks detection/search; red is reserved for the escalating system diagnosis; green appears only on the corrective path. The correction and final card return to clean signage. Do not turn lane changes into an evasive slalom or imply that the driver should cross solid markings.

## Rule basis and scope

The [Motor Vehicles (Driving) Regulations, 2017](https://morth.gov.in/sites/default/files/Motor-Vehicle-Driving-Regulation-2017.pdf), Regulation 6, says drivers on lane-marked roads should remain within their lane and change lanes only after the prescribed signal, marking, or signage. Regulation 5 requires due care and caution. Regulation 8 includes signalling and checking traffic to the side and behind when moving into a turn lane. The episode's `ONE LANE AT A TIME` phrasing is a plain-language safety instruction, not a verbatim quote from the regulations; `ONLY WHEN SAFE` preserves that scope.

## Open work

- Confirm the sharpest hook and whether the search loop stays instantly readable without sound.
- Review the first-pass frame sequence and refine any remaining route geometry or correction timing.
- Translate the approved Paper vectors into Cavalry motion; preserve the clean hard reset at frame 585.
- Keep any rendered motion picture-only until separate soundtrack direction is given.
- Verify 1080 × 1920, 30 fps, 756 frames / 25.20 seconds, with no audio unless separately requested.
