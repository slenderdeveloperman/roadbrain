# ROAD BRAIN — Production System

## Current pipeline

```text
Research / rule verification
→ static storyboard + composition
→ carousel export
→ Instagram carousel
→ optional Reel adaptation only after the static idea works
```

The production system is deliberately static-first. A simple road behaviour should not require motion infrastructure to become publishable.

## Paper / static design environment — source of truth

Use the static design environment for:
- canonical assets;
- tokens;
- roads and lane geometry;
- vehicles;
- ROAD BRAIN archetypes;
- guest-character redraws / transformed collage;
- captions;
- behaviour diagrams;
- complete episode slides;
- all-in-one shareable comics;
- exportable SVG/PNG assets.

The storyboard and the finished carousel may now be effectively the same artifact.

## Motion tools — optional adaptation layer

Cavalry, Resolve or other motion tools are no longer part of the default path.

Use them only when:
- a successful comic deserves a Reel adaptation;
- motion adds a joke unavailable in static form;
- a platform-specific experiment calls for animation;
- a reused motion asset makes the adaptation genuinely cheap.

Do not animate merely because ROAD BRAIN previously used animation.

## Project formats

### Default carousel

```text
Canvas: 1080 × 1350
Aspect ratio: 4:5 portrait
Colour: RGB
Output: PNG or high-quality JPEG as appropriate
```

### Optional all-in-one comic

```text
1080 × 1350 preferred
1080 × 1080 allowed when composition benefits
```

### Optional Reel adaptation

```text
1080 × 1920
30 fps unless the adaptation needs otherwise
No fixed duration requirement
```

## Episode folder / board organization

Recommended structure:

```text
00 SYSTEM
01 TOKENS
02 ROADS
03 VEHICLES
04 ARCHETYPES
05 GUEST CAST
06 MARKINGS
07 CONTAMINATION / FX
08 CAPTIONS
09 COMIC TEMPLATE
10 EP001
11 EP002
12 EP003
...
```

## Default episode board

Each episode should contain:

```text
01_hook
02_violation
03_diagnosis
04_absurd-consequence
05_correct
06_shareable        optional
07_rule-card        optional
```

## Naming contract

Use semantic naming for independently reusable pieces.

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

### Road
```text
road
  asphalt
  divider_1
  divider_2
```

### Guest cast
```text
guest_cast
  head
  body
  prop
  speech
```

### Caption
```text
caption
  state_label
  message
  metadata
  rule_line
```

Do not waste time renaming microscopic vector paths that will never be reused.

## Asset naming

Canonical examples:

```text
Road/Straight/3-Lane
Vehicle/Car/Hatchback
Archetype/Indicator-Divine
Archetype/Right-Lane-Raja
Caption/System
Contamination/Photocopy
```

Export filenames should be lowercase kebab-case:

```text
road-straight-3-lane.svg
vehicle-car-hatchback.svg
archetype-indicator-divine.svg
slide-01-hook.png
slide-02-violation.png
```

## Character-source rule

If an episode riffs on an existing viral reel/persona:
1. identify what is actually recognisable: expression, pose, phrase, costume, situation or archetype;
2. translate that recognition into an original redraw, collage treatment or parody composition;
3. cast it into a ROAD BRAIN role;
4. do not depend on a ripped creator asset as the canonical source file;
5. retain enough ROAD BRAIN institutional framing that the image still belongs to this series.

## Production sequence per episode

```text
1. State the road rule in one sentence.
2. Verify the rule.
3. Choose the ROAD BRAIN archetype.
4. Choose guest-cast/reference energy if useful.
5. Write the five swipe beats.
6. Thumbnail all five slides before polishing any one slide.
7. Build slide 5 first enough to confirm the correction is clear.
8. Build slides 1–4 around escalating contrast.
9. Export and review at actual phone size.
10. Build the optional shareable composite from finished slides.
11. Publish static first.
12. Consider motion only if results or concept justify it.
```

## Production rule

**The road rule decides what exists. The swipe decides how the joke unfolds. Motion is optional.**

## Stopping rule

Avoid infrastructure for infrastructure's sake.

A new tool, asset family, character treatment or animation system earns its place only if it makes the next episode faster, clearer, more reusable or more shareable.