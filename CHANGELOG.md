# Changelog

## 2026-10-20

### EP006 alternate — wait for every approach to clear

- Added north-side and west-side traffic-clearance hold beats to the separate south-to-east alternate; the lead stays behind the line during both.
- Kept the east-clear and all-clear hold beats before release, so the car turns only after all three approaches and the east exit are open.
- Updated the Paper inventory and EP006 storyboard documentation; the twelve canonical boards remain unchanged.

### EP006 simplified alternate — south to east

- Added a separate seven-frame storyboard row beneath the original EP006 sequence on the same Paper page; the twelve existing boards were left unchanged.
- Simplified the lesson to one lead car, one vehicle from each other approach, two clear wrong moves, holding while the east exit clears, then turning through without stopping.
- Reviewed the full sequence in Paper and corrected the route overlay and final clearance label for legibility.
- Updated the storyboard inventory, EP006 specification, grammar and backlog.

### EP006 storyboard — Unmanned Junctions

- Added nine editable EP006 keyframes to the unified ROAD BRAIN Paper file for an uncontrolled, unsignaled road junction.
- Opened with `HOW DO YOU CROSS THIS JUNCTION SAFELY?`, held for 1.55 seconds, then reordered the setup so the rule is taught before the gridlock payoff.
- Added detailed shared hatchback vectors, auto-rickshaws and scooters to the opening and approach boards; the mixed traffic escalates into the four-way jam where nobody can move.
- Made the central instruction explicit: check that the exit lane is clear before entering; wait behind the line when you cannot clear the junction. Kept yielding to traffic from the right in the scoped equal-class example, with exceptions for traffic control, mandatory signs and major-road priority.
- Redrew the auto-rickshaw and scooter as distinct top-down vector vehicles, with clear wheel, cabin, handlebar and seat details; spaced them apart from the hatchbacks across the junction boards.
- Updated the frame timing, storyboard index, episode grammar and production backlog. Motion and render remain open.

### EP006 storyboard — car clarity and exit-clear correction

- Replaced the abstract red vehicle blocks and central cross with the detailed hatchback, auto-rickshaw and scooter artwork so the vehicles themselves explain the four-way gridlock. Specified the car silhouette in the episode notes: bonnet, front/rear glass, roof, mirrors, wheel arches, lights and dark window trim.
- Expanded EP006 from nine to eleven boards while retaining 25.2 seconds / 756 frames: hold behind the line with the exit blocked; show the far-side lane clearing while the lead vehicle remains stopped; then enter only after the full exit and conflicting traffic are clear.
- Added the mixed-traffic auto-rickshaw and scooter to the final rule card, keeping them visible in all storyboard frames.
- Reviewed the revised gridlock, hold, exit-clear, entry and rule boards in Paper; synchronized timing and copy in the episode specification, grammar, index and backlog.

### EP006 storyboard — make exit clearance unmistakable

- Expanded the correction to four visible states: exit blocked; far-side traffic begins to move while the lead vehicle holds; exit fully clears while the lead still holds; then the lead enters.
- Added red, amber and green directional callouts that point to the far-side exit and label it `EXIT BLOCKED`, `EXIT CLEARING` or `EXIT CLEAR`.
- Added one more keyframe and updated the EP006 count to twelve without changing the 25.2-second / 756-frame runtime. Autos and scooters remain in the new frame.
- Updated the episode timing table, storyboard index, grammar and backlog to match the Paper sequence.

### EP006 storyboard — separate exit clearance from right-of-way

- Added a distinct hold frame after the exit lane opens: the lead vehicle remains behind the line while traffic from the right passes.
- Added an amber `YIELD TO RIGHT` directional callout and `HOLD UNTIL CONFLICT PASSES` copy, followed by a separate green release frame.
- Expanded EP006 to thirteen editable boards and kept the 25.2-second / 756-frame runtime unchanged; autos and scooters remain in the new frame.
- Reviewed the clear-exit hold, right-yield hold, release and rule card in Paper, then synchronized the specification and episode documentation.

### EP006 sequence review — reduce repetition and clarify release

- Removed the duplicate uncontrolled-junction condition board and reflowed the sequence to twelve boards without changing the 25.2-second / 756-frame runtime.
- Reordered the explanation to establish the scene, slow and scan, check the exit, show the deadlock, then correct it through blocked / clearing / clear / yield-right / release states.
- Tightened captions, removed a redundant exit-clear callout, and kept each frame centered on one decision.
- Corrected the safe-entry artboard: the exit and right-side conflict are now visibly clear before the lead enters; autos and scooter remain outside its path.
- Reviewed the full sequence in Paper screenshots and updated the episode spec, index, grammar and backlog.

### EP005 storyboard — One Lane at a Time

- Updated the nine editable 1080 × 1920 Paper keyframes to show an Indian left-side-traffic road narrowing from two lanes to one, with auto-rickshaw and two-wheeler silhouettes.
- Replaced lane-search copy with the two-to-one bottleneck story: `TWO LANES IN. ONE LANE OUT.`, `MERGE WINDOW: CLOSED BY EGO`, and a `SIGNAL. CHECK. TAKE TURNS.` correction.
- Kept the 25.2-second hook-first timing; the final card says `MERGE IN TURN.` and qualifies it with `ONLY WHEN SAFE.`
- Checked the rule basis against the Ministry of Road Transport and Highways' Motor Vehicles (Driving) Regulations, 2017. Documented that the title is plain-language guidance rather than a verbatim statutory quote.
- Updated the episode specification, backlog, grammar, README and unified storyboard index. Motion and render are not part of this storyboard pass.

## 2026-10-14

### EP001 v2 — Telepathy Required

- Added ten editable hook-first frames to a new page in the unified Paper storyboard, preserving the original EP001 storyboard and master.
- Built a separate 1080 × 1920, 30 fps Cavalry composition and rebuild script for the telepathy protocol, temporary stable-network reversal, intent-change collapse, and indicator correction.
- Kept the render picture-only with audio disabled. The Cavalry render connection dropped and left an invalid MP4; the preview is pending a successful render after Cavalry reconnects. Updated the episode grammar, storyboard index and production docs.

### EP004 Cavalry motion preview

- Built the first editable EP004 Cavalry composition from the current Paper vector boards, with the pass, right-lane residency, border/crown escalation, staggered customs queue, signalled safe return and final rule card.
- Rendered a silent H.264 preview at 1080 × 1920, 30 fps, 756 frames and 25.20 seconds; confirmed the export contains no audio stream.
- Saved the scene, rebuild script and preview under the workspace's `outputs/EP004/` handoff folder. Motion remains a review preview, with soundtrack and publication still open.

### EP004 sharper commentary

- Applied the approved Paper copy: `ONE OVERTAKE. LIFETIME APPOINTMENT.`, `LEFT LANE: CLEAR. EXCUSE: NONE.`, `PUBLIC ROAD. PRIVATE DELUSION.`, `AUTHORITY: SELF-ISSUED`, and `ALL HAIL THE BOTTLENECK.`
- Adjusted hook/payoff typography for readable two-line captions, reviewed the five changed boards, and synchronized the motion handoff. Story flow, timings, correction and final road rule remain unchanged.

### Unified storyboards and EP004

- Consolidated all 37 existing EP001–EP003 Paper artboards into one canonical file before adding EP004, preserving editable text, vector groups, assets and EP003 hook tests.
- Organized five pages: shared assets, EP001, EP002, EP003 and EP004. Historical originals remain available as provenance; new production edits use the unified file.
- Created nine 1080 × 1920 Right Lane Raja storyboard keyframes for EP004 `PASS. RETURN LEFT.`, with hook-first timing, territorial/crown/customs escalation, safe signalled correction and `WHEN SAFE.` qualification.
- Used Exa to retrieve the official Gazette rule baseline; documented frame ranges, source notes and the later motion/render acceptance criteria. EP004 animation, audio and video render remain pending.
- Verified 46 total artboards, source group counts, editable content, final rule hierarchy and correction indicator. Updated canonical links, production organization and episode numbering notes.

### EP003 hook-first update

- Updated EP003 to the supplied hook-first 25.2-second format, showing false capacity, copycats, forced merging, infinite road width, and zero average speed.
- Revised the existing Paper storyboard with nine main keyframes and opening-only B/C/D test boards; removed the ambulance payoff and made the shoulder rule primary on the final card.
- Documented the new 3–4-note civic mnemonic, its escalation/clean reset, shared hook-test carrier, and 30 fps cut boundaries. Audio composition and motion rendering remain outstanding production tasks.
- Aligned README, episode/audio grammar, visual language, and decision log with EP003 while retaining the EP001/EP002 baseline.

### EP003 Cavalry master

- Built the updated Hook A animation from live Paper SVG exports in a separate Cavalry composition, preserving the existing EP002 work.
- Animated shoulder entry, two staggered copycats, forced merging, road expansion, temporal holds, zero-speed collapse, ordinary waiting, and the final shoulder rule.
- Composed an original four-note civic motif with stage-specific surroundings and a clean correction.
- Delivered the editable scene and a verified 1080 × 1920 / 30 fps / 756-frame / 25.20-second MP4 with 48 kHz stereo audio.
- Documented Cavalry's percentage-based `resolutionScale` and the confirmed foreground render path.

### EP003 picture-only handoff

- Removed the generated soundtrack from the EP003 movie, editable Cavalry scene, source assets and rebuild script at the user's request.
- Disabled audio in future Cavalry exports and supplied `ROAD_BRAIN_EP003_SILENT.mp4`; the original master filename is also updated to silent picture.
- Verified zero audio streams and an unchanged encoded picture hash, retaining 1080 × 1920, 30 fps, 756 frames and 25.20 seconds. Replacement soundtrack will be added separately by the user.
