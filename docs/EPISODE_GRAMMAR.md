# ROAD BRAIN — Episode Grammar

## EP001 v2: Telepathy Required

EP001 v2 is an alternate version, not a replacement for the original reference storyboard or master. It keeps the 25.2-second / 30 fps carrier while using a ten-beat escalation: unsignalled lane change → telepathy protocol → false stability → intent changes → prediction collapse → indicator correction. The exact timing and copy live in [EP001 v2](episodes/EP001_V2_TELEPATHY_REQUIRED.md). The clean success beat at 13.20–15.80 seconds is essential; human intent changing is the cause of the collapse, not a decorative glitch effect.

## EP003: current hook-first format

EP003 targets **25.2 seconds** and opens mid-violation. Its current specification overrides the earlier clean-first grammar below:

```text
0.00–0.20   VISUAL INTERRUPT — already crossing the shoulder line
0.20–1.55   HOOK — YOU DIDN’T FIND A FASTER LANE.
1.55–4.90   CONDITION — one driver appears to benefit
4.90–9.80   SOCIAL CONTAGION — copycats force merging
9.80–14.70  GEOMETRY FAILURE — lane count 4 → 6 → 11
14.70–19.50 COLLAPSE — infinite width, average speed zero
19.50–23.60 CORRECTION — empty shoulder, predictable waiting
23.60–25.20 RULE — THE SHOULDER IS NOT A LANE.
```

Hook = accusation; system = bureaucracy; rule = calm authority. Keep all picture/audio after the 1.55-second opening identical across hook tests A/B/C/D. At 30 fps, use frame 47 for the nominal 1.55-second cut; full boundaries and acceptance criteria are in [EP003](episodes/EP003_SHOULDER_IS_NOT_A_LANE.md).

The mnemonic introduced by EP003 preserves melodic identity through changing surroundings; see [Audio Grammar](AUDIO_GRAMMAR.md). The existing EP001/EP002 masters remain unchanged.

## EP004: Right Lane Raja

EP004 applies the same hook-first cut boundaries as EP003 to a different causal sequence: completed pass → unnecessary residency → territorial border/crown → customs queue → safe signalled return → rule. Its territory/crown split is at 12.20 s. See [EP004](episodes/EP004_PASS_RETURN_LEFT.md) for inclusive frame ranges and the picture-only handoff. This does not change the existing EP001/EP002 carrier below.

## EP001/EP002 baseline carrier

The earlier ROAD BRAIN productions use the **25.2-second** five-state carrier:

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

Not every episode needs every level. EP001/EP002 retain the five-state timeline; EP003 follows its hook-first override above.

## The loop test

Before export, ask:
1. Can the offence be understood with sound off?
2. Can the rule be understood if all joke captions are removed?
3. Does loop/state 4 feel meaningfully worse than state 3?
4. Does state 5 feel calmer than state 1?
5. Does the recurring sonic identity remain recognizable? EP003 repeats its mnemonic while changing the surrounding sound.
6. Could the ending cut back to the beginning cleanly if needed?
