# ROAD BRAIN EP004 — PASS. RETURN LEFT.

**Concept:** Right Lane Raja. **Status:** nine editable Paper keyframes and a first Cavalry motion preview completed. **Format:** 1080 × 1920, 30 fps, 25.2 seconds / 756 frames. Picture-only; no soundtrack.

[Open EP004 in the unified storyboard file](https://app.paper.design/file/01M4XBCQ0SFYHGKEF9NWC2R334/p-5-0). See [the full storyboard index](../STORYBOARDS.md).

## Behaviour and joke

A driver completes an overtake, has a clear safe opportunity to return left, but stays in the right lane. The institution mistakes this indefinite residency for a territorial claim. A ceremonial border forms, a crown descends, and the lane becomes a tiny kingdom with its own customs queue. Hard reset: signal, check the gap, return left normally.

Hook: **ONE OVERTAKE. LIFETIME APPOINTMENT.**

Payoff: **ALL HAIL THE BOTTLENECK.**

Approved copy pass: the institution diagnoses the driver's self-importance through `LEFT LANE: CLEAR. / EXCUSE: NONE.`, `PUBLIC ROAD. / PRIVATE DELUSION.`, and `AUTHORITY: SELF-ISSUED`. Keep delivery neutral, with no shouted emphasis or exclamation marks. The correction returns to plain professional instruction. The story flow, shot timings, road artwork and final rule stay the same.

Rule: **PASS. RETURN LEFT.** Qualification on the same final card: **WHEN SAFE.** Brand closure: **DRIVE PREDICTABLY.**

This uses the EP004 topic from the season plan on `origin/docs/season-01-episodes-04-20`, adapted to the latest EP003 hook-first pacing. It supersedes the initial slate's tentative EP004 `KEEP LEFT.` placeholder. It does not change EP001/EP002's existing masters or depend on merging that season-planning branch.

## Storyboard and motion handoff

Frame ranges are inclusive. Nominal 1.55 s rounds to frame 47 at 30 fps. The actual cut is therefore 1.5667 s. All other listed boundaries fall on whole frames.

| Board | Nominal time | Frames | Picture / copy | Motion intent |
| --- | --- | --- | --- | --- |
| 00 Visual interrupt | 0.00–0.20 | 0–5 | Amber car ahead in right lane; white overtaken car behind in left. Both lanes travel upward. | Open during completion of a pass, with road motion already running. |
| 01 Hook | 0.20–1.55 | 6–46 | `ONE OVERTAKE. / LIFETIME APPOINTMENT.` | Caption interrupts the live road action; no logo-first introduction. |
| 02 Condition | 1.55–4.90 | 47–146 | `OVERTAKE / COMPLETE.` Diagnostic: `LEFT: CLEAR / RIGHT: STILL OCCUPIED`. | Establish ample clearance ahead of the passed vehicle. The amber car remains right. |
| 03 Detection | 4.90–9.80 | 147–293 | `LEFT LANE: CLEAR. / EXCUSE: NONE.` Diagnostic: `PASSING: COMPLETE / RESIDENCY: INDEFINITE`. | Hold the unnecessary right-lane occupancy while the bureaucracy notices. |
| 04 Territory | 9.80–12.20 | 294–365 | `PUBLIC ROAD. / PRIVATE DELUSION.` Fictional dashed border and generic pennant. | `TERRITORY_ESTABLISH`: trace the border around the occupied right lane. |
| 05 Crown | 12.20–14.70 | 366–440 | `RIGHT LANE / RAJA.` Diagnostic: `AUTHORITY: SELF-ISSUED`. | `CROWN_DROP`: ceremonial reveal; one short failed classification/hold, not a permanent glitch filter. |
| 06 Collapse | 14.70–19.50 | 441–584 | `ALL HAIL / THE BOTTLENECK.` Two following cars queue behind the mock customs boundary. | `QUEUE_BUILD`: stagger the two cars. Increase bureaucratic residue, then interrupt hard at frame 585. |
| 07 Correction | 19.50–23.60 | 585–707 | `SIGNAL. CHECK. / RETURN LEFT.` White car with left indicator, checked gap and ordinary trajectory. | Remove crown/border/queue effects instantly. Blink left indicator before lateral movement; check clearance and return smoothly without cutting in. Turn signal off after completion. |
| 08 Rule | 23.60–25.20 | 708–755 | `PASS. / RETURN LEFT.` + `WHEN SAFE.` + secondary brand closure. | Pristine white card; no corruption or celebratory hero treatment. |

The storyboard contains representative keyframes, not every intermediate motion state. Board 07 shows the end of the signalled return; Cavalry must also show the pre-move signal and checked gap during its 123-frame span. The drawn trajectory is an explanatory overlay, not a physical road marking. Metadata along the lower edge is for storyboard navigation and should be omitted from the finished video.

## Visual system

Use the existing ROAD BRAIN signage system: ink black, white, asphalt `#2A2A2A`, lane white `#F2F2F2`, amber `#FFB000`, and warning red `#FF2B2B`. Inter 800 gives the 64–96 px headline hierarchy; IBM Plex Mono 24 px handles diagnostics. Road width is 720 px within a 1080 px canvas. Two 360 px lanes belong to one carriageway and travel in the same direction; both upward arrows are explicit. The amber offender becomes an ordinary white car after reset.

The approved longer hook uses 64 px type / 68 px line height to stay on two lines. The bottleneck payoff uses 80 px type / 80 px line height. Both were checked in Paper for fit and contrast.

Reuse the kernel hatchback. New editable vector groups are a generic three-point crown, dashed territorial border/pennant, symbolic customs boundary, and safe-return path. No real sovereign, political, religious or government insignia is used. Crown/border effects belong exclusively to the violation.

## Factual basis checked with Exa

Checked on 2026-10-14 against the English Gazette text of the [Motor Vehicles (Driving) Regulations, 2017, hosted by Tripura Traffic Police](https://trafficpolice.tripura.gov.in/sites/default/files/2023-08/Motor%20Vehicle%20Driving%20Regulation%2C2017.pdf). Exa was used for source discovery and retrieval. This source supports the episode's narrow scenario; it is not a claim that every road has an identical lane-use rule.

- Regulation 14(1): overtaking must be safe and lawful.
- Regulation 14(6): signal overtaking intent and return left after overtaking as quickly as possible; read together with the safety requirements.
- Regulation 6: change lanes with proper signalling and only when safe, respecting markings/signage.
- Regulation 14(9): the overtaken vehicle must not accelerate or impede the other vehicle's safe return.
- Regulation 14(2) contains specific permitted left-overtaking situations. Do not turn this episode into a universal claim that the right lane is exclusively for overtaking on every road.

The corrective action therefore waits for safe clearance and respects signs/markings. It does not reward speeding, tailgating, flashing vehicles out of the way, undertaking, or an immediate unsafe merge. The overtaken car does not accelerate to close the gap. The fictional customs apparatus must read as the transmission's absurd representation, not an actual barrier a driver should navigate.

## Acceptance for the later motion/render phase

- The offence and correction remain understandable with sound off.
- Both lanes visibly carry traffic in the same direction.
- Passing is complete before residency is diagnosed; a safe return opportunity is visible.
- Crown and border appear only after the real behaviour is established.
- Queue cars maintain visible separation; no aggressive close following.
- At frame 585 the surreal layer disappears. The driver signals, checks, returns left with clearance, then cancels the signal.
- Final card remains clean throughout frames 708–755 and includes `WHEN SAFE.`
- Export is 1080 × 1920, 30 fps, 756 frames, 25.20 seconds. No audio track is added unless separately requested.

## Motion preview handoff

The first motion pass is saved as an editable Cavalry composition and a silent H.264 preview in the workspace's `outputs/EP004/` folder (`ROAD_BRAIN_EP004.cv` and `ROAD_BRAIN_EP004_MOTION_PREVIEW.mp4`). `build_ep004.js` rebuilds the composition from the adjacent Paper SVG/font exports. The full-resolution render was checked at the hook, completed-pass, detection, territory, crown, bottleneck, correction and final-card beats. The output is 1080 × 1920, 30 fps, 756 frames / 25.20 seconds, with no audio stream.

The pass completes before the driver holds the right lane; border, crown and customs effects enter in sequence, then clear at frame 585. The correction shows the left indicator before lateral movement and follows the Paper safe-gap trajectory. The final 48 frames hold the clean `PASS. / RETURN LEFT.` rule with `WHEN SAFE.` and `DRIVE PREDICTABLY.` This is a motion preview for review, not a published or final-audio master.

## Storyboard verification completed

Nine native Paper boards reviewed. Corrected the customs-label overlap and lit the left indicator. Verified all board dimensions, temporal ordering, final rule hierarchy and inclusion in the unified file. Cavalry motion and the picture-only preview are now available in the workspace handoff above.
