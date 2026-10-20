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
A two-lane Indian road narrows to one; drivers crowd the pinch point instead of signalling, checking for a safe gap, and merging in turn.

Possible escalation:
```text
ROAD NARROWS
2 LANES → 1
GAP: LEFT? / GAP: RIGHT?
ROAD: 2 → 1
DRIVERS: STILL 2
MERGE WINDOW: CLOSED BY EGO
```

Correction:
```text
SIGNAL. CHECK. TAKE TURNS.
MERGE IN TURN. ONLY WHEN SAFE.
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
EP005 — ONE LANE AT A TIME            two-to-one road narrowing / merge failure
EP006 — UNMANNED JUNCTIONS            exit-lane check / uncontrolled intersection deadlock
```

EP004 uses the season plan's Right Lane Raja topic, superseding the initial slate's tentative `KEEP LEFT.` placement. EP005 develops the `ONE LANE AT A TIME` concept through a marked two-lane road narrowing to one, with an orderly, signalled, safe merge as the correction. Its nine storyboard frames are in the [unified Paper file](STORYBOARDS.md). EP006 develops **UNMANNED JUNCTIONS** as an uncontrolled, unsignaled road-junction episode: slow down, scan each approach, and wait if the exit lane is blocked so the vehicle can clear the junction. Its correction shows the exit traffic moving, the exit fully clearing while the lead still holds, a separate hold while yielding to right-side traffic, and then release. The cars have a defined detailed hatchback silhouette, and cars, an auto-rickshaw and scooter remain present in every frame. In the scoped equal-class example, the driver also yields to traffic from the right. Final guidance preserves the exceptions for traffic control, mandatory signs and major-road priority. Twelve keyframes are in the unified Paper file; see the [EP006 specification](episodes/EP006_UNMANNED_JUNCTIONS.md). The numbered initial slate above is historical, not the current production numbering.
