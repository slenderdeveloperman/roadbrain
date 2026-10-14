# EP003 — Cavalry Render Handoff

Rendered 2026-10-14 from the current [Paper storyboard](https://app.paper.design/file/01M4WW7Z0Q227S7MJN4DJX2652/p-1-0) and [episode specification](episodes/EP003_SHOULDER_IS_NOT_A_LANE.md).

## Delivered master

Default hook A. 1080 × 1920, H.264, 30 fps, 756 frames, 25.20 seconds. Picture-only: no audio stream. The user will supply a replacement soundtrack separately.

The producing Codex workspace contains `outputs/EP003/ROAD_BRAIN_EP003_SILENT.mp4` (and the original master filename updated to the same silent picture), `ROAD_BRAIN_EP003.cv`, the `assets/` folder, `build_ep003.js`, `EP003_contact_sheet.jpg`, `validation.json`, and a local README. Binary deliverables are outside this documentation repository. The native scene retains existing compositions and opens on `EP003 MASTER — THE SHOULDER IS NOT A LANE`; the original EP002 scene was not overwritten.

## Implementation

- Road, white/amber vehicles, shoulder geometry and collapse geometry come from live Paper SVG exports.
- Exact Inter and IBM Plex Mono fonts are loaded as scene assets.
- Traffic uses one Duplicator with an indexed procedural position/visibility/rotation rig and a frame clock. The main shoulder driver has eased native position/rotation keyframes.
- Two copycats enter with staggered timing. The shoulder barrier is positioned ahead of upward-moving traffic so that its forced merge is causally clear.
- Diagnostics switch discretely; there is no hook type-on animation. A 21-frame consensus caption implements the 0.5–0.8-second text event.
- Collapse combines expanding road width, lane proliferation, opposing merge vectors, short registration faults and 12 fps temporal holds. Captions stay readable.
- At frame 585 the shoulder empties, geometry resets and vehicles wait/advance normally. The final rule begins at frame 708.
- Stage metadata from the Paper storyboard is excluded from the picture.

## Audio

The generated civic soundtrack, sound layer and source audio asset were removed at the user's request. The editable scene, rebuild script and delivered movies are picture-only. The user will add a different soundtrack separately; no replacement has been added.

## Render settings and lessons

Cavalry Render Manager: MP4 / Very High, frames 0–755, **100%** resolution, audio disabled. `resolutionScale: 100` is full resolution; `resolutionScale: 1` produces a 1% render. The confirmed export path uses `api.render(renderQueueItemId)`.

A new native composition's `on` Attributes have default inputs; scripted hard visibility gates must connect with `force: true`. SVG assets are loaded through `api.loadAsset` and `api.addAssetToComp`; assigning an asset id as an ordinary scalar input does not bind the asset.

FFmpeg removes the audio stream with `-map 0:v:0 -c:v copy -an`. The encoded H.264 picture hash is identical before and after removal; the duration remains exactly 25.20 s.

## Verification

- Metadata assertions: 1080 × 1920, 30/1 fps, 756 frames, 25.20-second picture/container duration, exactly one video stream and zero audio streams.
- Visual review: frames 24, 120, 225, 275, 420, 550, 600 and 735 in the exported movie.
- Boundary review: frames 0, 5, 6, 46, 47, 584, 585, 707, 708 and 755.
- SHA-256 comparison of the encoded picture stream before/after audio removal: identical.
- Cavalry verification: no EP003 sound layer or generated soundtrack asset remains; `generator.exportAudio` is false.

Technical checks do not establish the hum test or predict audience response. The three alternate hooks remain available in Paper; the delivered video uses hook A.
