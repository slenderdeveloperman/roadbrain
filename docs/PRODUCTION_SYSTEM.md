# ROAD BRAIN — Production System

## Current pipeline

```text
Paper
→ Cavalry
→ lightweight finishing / assembly
→ Instagram Reels
```

### Paper — static source of truth
Use Paper for:
- canonical assets;
- tokens;
- roads and lane geometry;
- vehicles;
- characters;
- captions;
- behaviour diagrams;
- static episode boards;
- exportable SVGs.

Paper is **not** the motion source of truth. MCP testing showed animation/transition properties were not authorable through the Paper MCP, while static SVG composition and video export were available. Treat Paper as the visual workshop and storyboard system.

### Cavalry — motion source of truth
Use Cavalry for:
- timelines;
- keyframes;
- easing;
- independent layer timing;
- procedural FX;
- reusable motion behaviours;
- episode compositions;
- agent-addressable motion through Cavalry MCP.

The goal is not to hand-build every episode. Build a reusable motion grammar and swap assets/behaviours.

### Finishing — stay lightweight
Do not require DaVinci Resolve by default. Resolve/Fairlight is powerful but is optional unless an episode genuinely needs detailed sound design or finishing.

Current preference:
- generate/prepare the recurring audio separately;
- combine picture + audio using the simplest reliable tool available (Instagram/Edits or another lightweight editor);
- use Resolve only when its precision is worth the complexity.

## Project formats

- Canvas: **1080 × 1920**
- Frame rate: **30 fps**
- Current recurring episode duration: **25.2 s**
- Orientation: vertical 9:16

## Paper organization

Use [one canonical Paper file](STORYBOARDS.md) for the series. Separate pages keep episode sequences distinct while sharing the editable asset library:

```text
00 / SHARED ASSETS & FOUNDATIONS
01 / EP001 — INDICATE. THEN MOVE.
02 / EP002 — DIM YOUR HIGH BEAMS.
03 / EP003 — THE SHOULDER IS NOT A LANE
04 / EP004 — PASS. RETURN LEFT.
...
```

Add future episode pages to this same file. Keep text and vector groups editable; namespace historical episode tokens where scales differ. The originals linked in the storyboard index remain provenance rather than active production destinations. EP004 is storyboard-only until its separate Cavalry motion/render phase.

## Naming contract

Use semantic naming only for layers that may be targeted independently in motion.

### Vehicle
```text
vehicle
  body
  windows
  indicator_left
  indicator_right
  brake_left
  brake_right
```

### Indicator character
```text
indicator_character
  stalk
  housing
  eye_left
  eye_right
  mouth
  halo
  rays
```

### Impact FX
```text
impact_fx
  rays_primary
  rays_secondary
  center_mask
```

### Road
```text
road
  asphalt
  divider_1
  divider_2
```

### Caption
```text
caption
  state_label
  message
  indicator_dot
  rule_line
```

Do **not** waste time renaming microscopic vector paths that will never animate independently.

## Asset naming

Canonical component examples:

```text
Road/Straight/3-Lane
Vehicle/Car/Hatchback
Character/Indicator
FX/Impact-Lines
Caption/System
```

Export filenames should be lowercase kebab-case:

```text
road-straight-3-lane.svg
vehicle-car-hatchback.svg
character-indicator-divine.svg
fx-impact-lines-absurd.svg
```

Independently exported sub-assets use `__`:

```text
vehicle-car-hatchback__indicator-left.svg
```

## Core five kernel assets

The first system kernel is:
1. `Vehicle/Car/Hatchback`
2. `Character/Indicator`
3. `Road/Straight/3-Lane`
4. `Caption/System`
5. `FX/Impact-Lines`

Do not expand the full asset backlog until reuse has been proven across multiple episodes.

## Core motion behaviours

Reusable behaviours established from EP001:

```text
CAR_LANE_CHANGE
SYSTEM_CARD_IN
IMPACT_BURST
CHARACTER_POP
DIVINE_REVEAL
INDICATOR_BLINK
HARD_RESET
```

Future behaviours should be named semantically, not by episode number.

## Production rule

**Paper decides what exists. Cavalry decides how it moves.**

If something is visually wrong, fix it in Paper. If something moves badly, fix it in Cavalry.

## Stopping rule

Avoid infrastructure for infrastructure's sake.

A new tool, asset family or motion abstraction earns its place only if it makes the next episode faster, clearer or more reusable.
