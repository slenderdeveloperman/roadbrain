# ROAD BRAIN — Episode Backlog

## Initial slate

1. **INDICATE. THEN MOVE.**
2. **DIM YOUR HIGH BEAMS.**
3. **THE SHOULDER IS NOT A LANE.**
4. **KEEP LEFT.**
5. **PASS. RETURN LEFT.**
6. **ONE LANE AT A TIME.**
7. **SOLID LINE = DON'T CROSS.**
8. **STOP BEFORE THE LINE.**
9. **LET THEM MERGE.**
10. **ZEBRA CROSSING = HUMAN LANE.**

## Strong recurring concepts

### Right Lane Raja
A driver occupies the right lane indefinitely after any overtaking need has ended.

Possible system copy:
```text
OVERTAKE COMPLETE?
NO

OVERTAKE PLANNED?
NO

KINGDOM ESTABLISHED
```

Correction:
```text
PASS. RETURN LEFT.
```

### One Lane at a Time
A vehicle keeps drifting across multiple lanes after the target lane is already acquired.

Possible escalation:
```text
TARGET LANE ACQUIRED
TARGET LANE LOST
SEARCHING...
VEHICLE HAS DECLINED GEOMETRY
```

Correction:
```text
ONE LANE AT A TIME.
```

### Zebra Crossing = Human Lane
Treat the crossing as a lane whose priority belongs to pedestrians.

Possible system copy:
```text
LANE OCCUPIED
WRONG SPECIES HAS PRIORITY
```

Correction:
```text
STOP. LET THEM CROSS.
```

### Let Them Merge
Turn merging into a packet-routing / zipper-system metaphor. The system should punish blocking and chaotic acceleration rather than make merging feel like a moral negotiation.

### Solid Line
The solid line can behave like an explicit system boundary rather than a decorative stripe.

Possible system copy:
```text
BOUNDARY TYPE: SOLID
CROSSING PERMISSION: NONE
```

## Prioritization rule

Do not choose the next episode only by importance of the road rule.

Prefer episodes that do at least one of these:
- break a new subsystem visually;
- introduce a reusable character/archetype;
- add a reusable motion primitive;
- remain instantly understandable to a non-follower;
- create a highly sendable social observation.

## Current production order

```text
EP001 — INDICATE. THEN MOVE.          geometry failure
EP002 — HIGH BEAM DETECTED            vision failure
EP003 — THE SHOULDER IS NOT A LANE    world-model failure
EP004 — PASS. RETURN LEFT.            Right Lane Raja / territorial bureaucracy
```

EP004 now uses the season plan's Right Lane Raja topic, superseding the initial slate's tentative `KEEP LEFT.` placement. Its nine [storyboard frames](episodes/EP004_PASS_RETURN_LEFT.md) are complete in the [unified Paper file](STORYBOARDS.md); motion/rendering remain pending. The numbered initial slate above is historical, not the current production numbering.
