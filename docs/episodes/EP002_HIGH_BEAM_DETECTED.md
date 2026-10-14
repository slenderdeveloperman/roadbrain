# EP002 — HIGH BEAM DETECTED

[Editable storyboard in the unified Paper file](https://app.paper.design/file/01M4XBCQ0SFYHGKEF9NWC2R334/p-4-0). See [the storyboard index](../STORYBOARDS.md) for source provenance.

## Role in the series

Subsystem that fails: **vision / sensor interpretation**.

The same recurring 25.2-second ROAD BRAIN audio carrier is reused unchanged.

Core joke: one ordinary oncoming driver has somehow converted a hatchback into a solar event.

## Rule

```text
DIM YOUR HIGH BEAMS.
```

Secondary wording:
```text
DON'T BLIND ONCOMING TRAFFIC.
```

Do not imply that high beam is forbidden in every context. The episode targets inappropriate high-beam use, especially around oncoming traffic / close following / well-lit roads.

## Fixed carrier

```text
0.0–4.9    CLEAN
4.9–9.8    PRESSURED
9.8–14.7   BROKEN
14.7–19.5  COLLAPSING
19.5–25.2  CALM / CORRECT
```

## State 1 — CLEAN / 0.0–4.9

Night road. Two vehicles approach each other. Dipped headlights. Road edges and lane markings fully legible.

System copy:
```text
NIGHT ROAD
VISIBILITY: NORMAL
```

No corruption.

## State 2 — PRESSURED / 4.9–9.8

Oncoming car activates high beam.

Picture:
- light cones expand;
- brightness rises;
- scene remains readable;
- subtle amber diagnostic layer appears.

System copy:
```text
LUMINANCE INCREASE DETECTED
HIGH BEAM?
CONFIRMED
```

Corruption:
- tiny exposure twitch;
- restrained bloom;
- faint sensor banding only.

## State 3 — BROKEN / 9.8–14.7

The system starts losing the road.

Progression:
1. lane markings partially disappear;
2. road-edge detection flickers;
3. offending vehicle becomes harder to classify.

System copy:
```text
ROAD EDGE: UNSTABLE
LANE MARKING: PARTIAL
ONCOMING VEHICLE: DEGRADED
VISUAL INPUT: COMPROMISED
```

Allowed failures:
- 1–2 frame hold;
- small horizontal registration error;
- caption residue;
- duplicate contour around headlamps;
- short overexposure pulse.

Recurring fault candidate:
```text
GAIN WARNING
```
lingers slightly too long.

## State 4 — COLLAPSING / 14.7–19.5

Full psychic rupture.

The headlights stop reading as headlights and become celestial bodies.

Classification sequence:
```text
LIGHT SOURCE: HEADLAMP
```

glitches into:
```text
LIGHT SOURCE: LOCAL STAR
```

Then:
```text
SOLAR EVENT DETECTED
WHY IS THE SUN
DRIVING TOWARD US
```

Visual vocabulary:
- giant white discs;
- concentric solar rings;
- black vehicle silhouette;
- fake sensor telemetry;
- blown exposure graph;
- amber/red alert blocks;
- one genuinely ugly 1–2 frame failure.

Microtext:
```text
GAIN: MAX
RETINA: UNAVAILABLE
ROAD MODEL: LOST
```

Peak sequence:
```text
VISUAL INPUT LOST
```

then:
```text
YOU ARE NOT
LIGHTING THE ROAD
```

cut to:
```text
YOU ARE
INTERROGATING IT
```

End state with a hard near-white or near-black failure. No graceful dissolve.

## State 5 — CALM / CORRECT / 19.5–25.2

Hard reset. High beams dip. Road geometry instantly returns.

No corruption.

Status card:
```text
ROAD STATE
DIM YOUR HIGH BEAMS.
```

Optional subline:
```text
ONCOMING TRAFFIC DETECTED
```

Vehicles pass normally.

End:
```text
DRIVE PREDICTABLY.
```

Optional tiny diagnostic:
```text
VISION RESTORED
```

## Layer plan

```text
road
vehicle_self
vehicle_oncoming
headlight_low_left
headlight_low_right
headlight_high_left
headlight_high_right
exposure_overlay
sensor_ui
solar_fx
caption_system
caption_status
flash_overlay
```

## New reusable motion behaviours

```text
HIGH_BEAM_ON
HEADLIGHT_BLOOM
EXPOSURE_PRESSURE
SENSOR_DEGRADE
TARGET_LOSS
SOLAR_ASCENSION
WHITEOUT_COLLAPSE
DIP_TO_NORMAL
```

Reuse:
```text
SYSTEM_CARD_IN
HARD_RESET
IMPACT_BURST
```

## Audio

Use the EP001 carrier unchanged.

Optional diegetic SFX only:
- headlamp relay click;
- one detection beep;
- one overloaded sensor chirp;
- relay click when beam dips.

No new score, choir, riser or custom musical climax.
