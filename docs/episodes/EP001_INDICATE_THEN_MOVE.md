# EP001 — INDICATE. THEN MOVE.

## Role in the series

EP001 is the **reference implementation** that established ROAD BRAIN’s grammar.

Subsystem that fails: **geometry / prediction**.

Core idea: a completely ordinary unsignalled lane change is treated as a catastrophic failure of civilisation’s ability to predict another road user.

## Rule

```text
INDICATE.
THEN MOVE.
```

Series line:

```text
DRIVE PREDICTABLY.
```

## Original six-beat storyboard

### 1. Setup
Top-down 3-lane road. One car. Deadpan normality.

Possible label:
```text
NORMAL HUMAN ACTIVITY
```

### 2. Violation
Car abruptly moves right with no indicator.

### 3. Detection
Freeze / zoom / system recognition.

```text
UNSIGNALLED
LATERAL MOVEMENT
DETECTED
```

### 4. Escalation
Other cars brake. Lane markings vibrate. Impact system activates. Indicator character appears ignored.

Possible reaction:
```text
HOW DID ANYONE KNOW
YOU WERE DOING THAT
```

### 5. Revelation
Indicator character becomes Divine. Psychic punishment peaks.

### 6. Correction
Hard reset to clean geometry.

```text
ROAD STATE
INDICATE.
THEN MOVE.
```

Footer:
```text
DRIVE PREDICTABLY.
```

## Canonical EP001 assets

```text
Road/Straight/3-Lane
Vehicle/Car/Hatchback
Character/Indicator — Ignored
Character/Indicator — Divine
Caption/System
FX/Impact-Lines — Absurd
```

## Canonical motion behaviours

```text
CAR_LANE_CHANGE
SYSTEM_CARD_IN
IMPACT_BURST
CHARACTER_POP
DIVINE_REVEAL
HARD_RESET
INDICATOR_BLINK
```

## Initial Cavalry motion timings

Reference motion prototype:

```text
0.00–1.20  setup
1.20–1.90  violation / lane change
1.90–2.30  displaced hold
2.30–2.50  detection enters
2.50–3.30  detection hold
3.30–3.55  psychic rupture
3.55–4.10  escalation settles
4.10–4.35  divine reveal
4.35–5.30  divine hold
5.30–5.45  hard reset
5.45–7.20  correction
```

These timings are useful as motion-preset references, **not** the current series duration.

## Current published-series grammar

EP001 later evolved into the recurring **25.2-second / five-state carrier** that should be reused by later episodes:

```text
0.0–4.9    clean
4.9–9.8    pressured
9.8–14.7   broken
14.7–19.5  collapsing
19.5–25.2  calm / correct
```

The rendered EP001 master used during development was approximately 25.23 seconds / 757 frames at 30 fps. Preserve the existing master rather than rebuilding it solely to remove a few frame-level differences. Future episodes should use the normalized carrier boundaries unless the audio master dictates exact frame points.

## EP001 aberration logic

The early loop experiments established the corruption hierarchy:
- temporal errors first;
- structural misregistration second;
- image degradation third;
- generic noise last.

The most successful evolution became:
- wrong behaviour repeats/escalates;
- the final pass is clean and correct;
- the correction card is never corrupted.

## Audio

EP001 produced the recurring ROAD BRAIN carrier track.

Its shape:
```text
clean
→ pressured
→ broken
→ collapsing
→ calm / correct
```

This soundtrack should be reused across current episodes rather than rescored.

## What EP001 proved

1. The tiny car / huge road field works.
2. The system itself can be the main character.
3. The Indicator character works best as infrastructure personification, not mascot comedy.
4. Psychic escalation can be extreme as long as the final instruction is pristine.
5. Repetition becomes conditioning when audio, captions and state transitions recur.
6. ROAD BRAIN should build reusable motion grammar instead of bespoke edits.
