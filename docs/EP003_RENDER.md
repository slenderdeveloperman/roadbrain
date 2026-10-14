# EP003 — Cavalry Render Handoff

Rendered 2026-10-14 from the current [Paper storyboard](https://app.paper.design/file/01M4WW7Z0Q227S7MJN4DJX2652/p-1-0) and [episode specification](episodes/EP003_SHOULDER_IS_NOT_A_LANE.md).

## Delivered master

Default hook A. 1080 × 1920, H.264, 30 fps, 756 frames, 25.20 seconds. Stereo AAC, 48 kHz, matching 25.20-second duration.

The producing Codex workspace contains `outputs/EP003/ROAD_BRAIN_EP003.mp4`, `ROAD_BRAIN_EP003.cv`, the `assets/` folder, `build_ep003.js`, `EP003_contact_sheet.jpg`, `validation.json`, and a local README. Binary deliverables are outside this documentation repository. The native scene retains existing compositions and opens on `EP003 MASTER — THE SHOULDER IS NOT A LANE`; the original EP002 scene was not overwritten.

## Implementation

- Road, white/amber vehicles, shoulder geometry and collapse geometry come from live Paper SVG exports.
- Exact Inter and IBM Plex Mono fonts are loaded as scene assets.
- Traffic uses one Duplicator with an indexed procedural position/visibility/rotation rig and a frame clock. The main shoulder driver has eased native position/rotation keyframes.
- Two copycats enter with staggered timing. The shoulder barrier is positioned ahead of upward-moving traffic so that its forced merge is causally clear.
- Diagnostics switch discretely; there is no hook type-on animation. A 21-frame consensus caption implements the 0.5–0.8-second text event.
- Collapse combines expanding road width, lane proliferation, opposing merge vectors, short registration faults and 12 fps temporal holds. Captions stay readable.
- At frame 585 the shoulder empties, geometry resets, sound cleans up, and vehicles wait/advance normally. The final rule begins at frame 708.
- Stage metadata from the Paper storyboard is excluded from the picture.

## Audio

Original C5–E5–D5–G5 civic motif; a bright FM-pluck/cheap-keyboard character follows `DA — da-da — DA`. Clean repetitions retain the same contour and rhythm. Ticks, hum, subtle detuning, late duplicate notes and overload grow around it; correction restores the pristine motif. Integrated loudness measured −16.03 LUFS with true peak −5.96 dBTP.

## Render settings and lessons

Cavalry Render Manager: MP4 / Very High, frames 0–755, **100%** resolution, audio enabled. `resolutionScale: 100` is full resolution; `resolutionScale: 1` produces a 1% render. The confirmed export path uses `api.render(renderQueueItemId)`.

A new native composition's `on` Attributes have default inputs; scripted hard visibility gates must connect with `force: true`. SVG assets are loaded through `api.loadAsset` and `api.addAssetToComp`; assigning an asset id as an ordinary scalar input does not bind the asset.

FFmpeg preserves the Cavalry H.264 picture, trims the AAC tail to exactly 25.20 s, and adds fast-start container metadata.

## Verification

- Metadata assertions: 1080 × 1920, 30/1 fps, 756 frames, matching 25.20-second picture/audio/container duration, 48 kHz stereo.
- Visual review: frames 24, 120, 225, 275, 420, 550, 600 and 735 in the exported movie.
- Boundary review: frames 0, 5, 6, 46, 47, 584, 585, 707, 708 and 755.
- Audio loudness and true-peak measurement; no clipping.

Technical checks do not establish the hum test or predict audience response. The three alternate hooks remain available in Paper; the delivered video uses hook A.
