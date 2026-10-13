# EP003 — THE SHOULDER IS NOT A LANE

## Role in the series

Subsystem that fails: **world model / map logic**.

The same recurring 25.2-second ROAD BRAIN audio carrier is reused unchanged.

Core joke: one driver uses the shoulder, so the institution reluctantly begins redrawing reality to accommodate this new “infrastructure.”

## Rule

```text
THE SHOULDER IS NOT A LANE.
KEEP IT CLEAR.
```

## Fixed carrier

```text
0.0–4.9    CLEAN
4.9–9.8    PRESSURED
9.8–14.7   BROKEN
14.7–19.5  COLLAPSING
19.5–25.2  CALM / CORRECT
```

## State 1 — CLEAN / 0.0–4.9

Top-down multi-lane road with slow traffic.

System copy:
```text
TRAFFIC STATE
SLOW
```

Everything remains orderly.

## State 2 — PRESSURED / 4.9–9.8

One hatchback calmly exits onto the shoulder.

System response:
```text
LATERAL MOVEMENT DETECTED
LANE 4?
```

Tiny pause.

Then:
```text
NEW LANE DETECTED?
```

loading / scan behaviour.

Finally:
```text
NO.
```

Keep this dry. `NO.` should be one of the cleanest cuts in the series.

## State 3 — BROKEN / 9.8–14.7

The offender continues. Another vehicle follows.

ROAD BRAIN begins drawing fake geometry because reality apparently refuses to cooperate.

System copy:
```text
UNAUTHORISED
INFRASTRUCTURE
```

Then the map begins reluctantly labeling space:
```text
LANE 4
LANE 5?
```

Visual progression:
- paved shoulder gains fake boundary;
- dirt edge becomes candidate lane;
- map labels start disagreeing;
- road container begins widening.

## State 4 — COLLAPSING / 14.7–19.5

Full world-model failure.

Cars spread beyond:
- shoulder;
- dirt edge;
- drainage channel;
- pavement;
- grass;
- nearby frontage / tea-stall territory if visually useful.

Measurement UI escalates:
```text
ROAD WIDTH: 720 PX
ROAD WIDTH: 960 PX
ROAD WIDTH: 1280 PX
ROAD WIDTH: INFINITE
```

Possible reaction lines:
```text
URBAN PLANNING CANCELLED
```

or:
```text
EVERY SURFACE
NOW CARRIAGEWAY
```

The canvas may briefly break its own 9:16 logic as ROAD BRAIN tries to accommodate an infinitely widening road.

### Consequence beat
An ambulance / emergency vehicle appears behind traffic and needs the shoulder.

System tone snaps serious:
```text
EMERGENCY ROUTE
OBSTRUCTED
```

Hold for a beat.

Optional tiny dry reaction:
```text
FANTASTIC WORK
```

The emergency obstruction is the factual consequence that prevents the episode from becoming purely abstract.

## State 5 — CALM / CORRECT / 19.5–25.2

Hard reset.

Fake lanes disappear. Everything outside the legitimate road model is deleted. Ordinary traffic returns to the carriageway. Shoulder clears.

Status card:
```text
ROAD STATE
THE SHOULDER IS NOT A LANE.
```

Subline:
```text
KEEP IT CLEAR.
```

Emergency vehicle passes unobstructed if used in the preceding beat.

End:
```text
DRIVE PREDICTABLY.
```

## Recurring archetype

### Shoulder Entrepreneur
The offending vehicle itself can carry the title.

Possible metadata:
```text
SHOULDER ENTREPRENEUR
INFRASTRUCTURE DEPT.
SELF-APPOINTED
```

No human mascot is required.

## New reusable motion behaviours

```text
SHOULDER_EXIT
LANE_SCAN
FAKE_LANE_DRAW
MAP_EXPAND
ROAD_WIDTH_COUNTER
EMERGENCY_ALERT
WORLD_SNAP_BACK
```

## Audio

Use the EP001 carrier unchanged.

Optional diegetic SFX only:
- scan beep;
- small loading tone;
- real ambulance siren if the emergency beat is used;
- short hard reset/dropout.

Do not build a bespoke cartographic soundtrack over the recurring carrier.
