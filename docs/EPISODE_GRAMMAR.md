# ROAD BRAIN — Episode Grammar

## Current fixed carrier

Every current ROAD BRAIN transmission uses the same **25.2-second** five-state carrier.

```text
0.0–4.9    CLEAN
4.9–9.8    PRESSURED
9.8–14.7   BROKEN
14.7–19.5  COLLAPSING
19.5–25.2  CALM / CORRECT
```

The recurring audio stays constant. The visuals change episode to episode.

This is a production constraint and a branding device.

## What each state means

### 1. CLEAN — establish reality
Show the road behaviour before the violation becomes absurd.

Rules:
- almost no corruption;
- normal road geometry;
- sparse captions;
- restrained palette;
- viewer understands the physical situation immediately.

### 2. PRESSURED — detect the offence
The violation becomes legible and the institution starts responding.

Rules:
- introduce amber/system warnings;
- increase motion pressure slightly;
- no full meltdown yet;
- the system remains professional.

### 3. BROKEN — system performance degrades
The institution can still understand the offence, but its representation begins failing.

Useful failures:
- one- or two-frame holds;
- residue from previous UI states;
- small RGB/misregistration faults;
- duplicate contours;
- partial classification loss;
- minor temporal disagreement.

### 4. COLLAPSING — reality/model failure
This is the episode-specific psychic rupture.

Rules:
- break the subsystem relevant to the offence;
- preserve the core idea beneath the chaos;
- use short violent failures rather than a permanent glitch filter;
- reach one memorable apex;
- end with a hard interruption/reset.

Examples:
- EP001: lane geometry / psychic punishment
- EP002: overexposure → sensor blindness → local star
- EP003: shoulder use → fake lane classification → infinite road width

### 5. CALM / CORRECT — boring competence
Hard reset to the correct behaviour.

Rules:
- no glitches;
- no heroic treatment;
- final rule pristine;
- action performed normally;
- end with `DRIVE PREDICTABLY.` when appropriate.

The payoff is **nothing dramatic happens because the driver behaves normally**.

## Caption hierarchy

Use these semantic roles:

```text
Caption/Rule
Caption/Violation
Caption/Reaction
Caption/System
Caption/Annotation
Caption/Endcard
```

### Rule
The actual behaviour to remember.

Examples:
- `INDICATE. THEN MOVE.`
- `DIM YOUR HIGH BEAMS.`
- `THE SHOULDER IS NOT A LANE.`

### Violation
Literal diagnosis.

Example:
- `UNSIGNALLED LATERAL MOVEMENT DETECTED`

### System
Status / machine interpretation.

Examples:
- `ROAD STATE`
- `VISUAL INPUT DEGRADED`
- `ROAD WIDTH: INFINITE`

### Reaction
The institution momentarily reveals personality.

Examples:
- `TELEPATHY NOT SUPPORTED`
- `WHY IS THE SUN DRIVING TOWARD US`

### Annotation
Small technical flavor. Never required to understand the rule.

### Endcard
Series-level closure.

Default:
- `DRIVE PREDICTABLY.`

## Escalation levels

A useful internal shorthand:

```text
0 — instructional
1 — intrusive thought
2 — manga rupture
3 — reality failure
4 — cosmic punishment / celestial bureaucracy
RESET — calm correction
```

Not every episode needs every level. The five-state timeline is fixed; the intensity within it can vary.

## The loop test

Before export, ask:
1. Can the offence be understood with sound off?
2. Can the rule be understood if all joke captions are removed?
3. Does loop/state 4 feel meaningfully worse than state 3?
4. Does state 5 feel calmer than state 1?
5. Does the recurring audio still fit without custom rescoring?
6. Could the ending cut back to the beginning cleanly if needed?
