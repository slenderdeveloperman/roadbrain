# ROAD BRAIN — Season 01 Plan (EP004–EP020)

This document extends the current EP001–EP003 grammar into the first complete ROAD BRAIN season.

## Locked production constraint

Every episode uses the existing **25.2-second carrier track unchanged** and maps visuals to the same five states:

```text
0.0–4.9    CLEAN
4.9–9.8    PRESSURED
9.8–14.7   BROKEN
14.7–19.5  COLLAPSING
19.5–25.2  CALM / CORRECT
```

Do not rescore individual episodes. Small diegetic SFX are optional, but the recurring music remains the broadcast carrier.

The season should feel like one institution repeatedly trying to explain simple road behaviour while different parts of its world model fail.

## Season design rule

Avoid clustering too many similar offences together. Rotate the subsystem that breaks:

- lane geometry;
- boundaries;
- intersection logic;
- human priority;
- attention;
- sound;
- emergency access;
- direction / world orientation.

The violation gets surreal. The correction stays boring.

---

# EP004 — PASS. RETURN LEFT.

**Behaviour:** complete the overtake and return left when safe.

**Legal spine:** Regulation 14(6) requires a driver overtaking to indicate and, after completing the manoeuvre, return to the left side of the road as quickly as possible. Regulation 4 also establishes keep-left logic, especially for heavy / speed-restricted vehicles.

**Recurring archetype:** **RIGHT LANE RAJA**.

**Subsystem failure:** territorial sovereignty.

### CLEAN — 0.0–4.9
A car overtakes normally on a multi-lane road.

System:
```text
OVERTAKE IN PROGRESS
```

### PRESSURED — 4.9–9.8
The pass is completed. The car remains in the right lane.

```text
OVERTAKE COMPLETE?
YES
RETURN LEFT?
PENDING
```

### BROKEN — 9.8–14.7
Nothing changes. A small ceremonial border appears around the right lane.

```text
RIGHT LANE OCCUPANCY
DURATION: EXCESSIVE
```

A crown descends onto the car.

### COLLAPSING — 14.7–19.5
The right lane becomes a tiny sovereign state. Border posts, flags, customs checkpoint, fake map label:

```text
KINGDOM ESTABLISHED
RIGHT LANE RAJA
```

Traffic queues behind the new monarchy.

### CALM / CORRECT — 19.5–25.2
Hard reset. Car finishes pass and returns left.

```text
ROAD STATE
PASS. RETURN LEFT.
```

**New reusable primitive:** `TERRITORY_ESTABLISH`, `CROWN_DROP`, `QUEUE_BUILD`.

---

# EP005 — ONE LANE AT A TIME.

**Behaviour:** change into one intended lane, settle, then make any further move deliberately.

**Legal spine:** Regulation 6 requires drivers to remain within marked lanes and change lanes only after proper signalling / according to markings or signage.

**Subsystem failure:** target acquisition.

### CLEAN
A car begins one ordinary lane change.

```text
TARGET LANE: 02
```

### PRESSURED
Car enters lane 02 but keeps drifting.

```text
TARGET LANE ACQUIRED
```

then:
```text
TARGET LANE LOST
```

### BROKEN
System repeatedly reassigns destinations:

```text
TARGET: 03
TARGET: 01
TARGET: ???
```

### COLLAPSING
Car diagonally traverses the road like a screensaver object, bouncing between lane boundaries.

```text
SEARCHING...
VEHICLE HAS DECLINED GEOMETRY
```

### CALM / CORRECT
One indicated move. Car settles.

```text
ONE LANE AT A TIME.
```

**New primitive:** `TARGET_LOCK`, `LANE_SEARCH`, `SCREENSAVER_BOUNCE`.

---

# EP006 — SOLID LINE = DON'T CROSS.

**Behaviour:** do not cross solid longitudinal road markings except where the regulations specifically allow an exception.

**Legal spine:** Regulation 6(4) says a driver overtaking another vehicle shall not cross a longitudinal yellow or white solid line; Regulation 6(6) also prohibits driving on or over single or double longitudinal solid lines or painted traffic islands except in case of obstruction.

**Subsystem failure:** boundary enforcement.

### CLEAN
A clean road. Solid line rendered with unusually bureaucratic precision.

```text
BOUNDARY TYPE: SOLID
```

### PRESSURED
Vehicle approaches the line.

```text
CROSSING PERMISSION: NONE
```

### BROKEN
Vehicle crosses anyway. The line thickens and follows the vehicle like a security laser.

```text
BOUNDARY BREACH
```

### COLLAPSING
The line becomes an enormous wall / firewall / redacted government boundary. Vehicle keeps trying to phase through it. Reality tears exactly along the line.

```text
THIS WAS NOT DECORATIVE
```

### CALM / CORRECT
Vehicle remains on its side.

```text
SOLID LINE = DON'T CROSS.
```

**New primitive:** `BOUNDARY_SCAN`, `LINE_TO_WALL`, `BREACH_ALERT`.

---

# EP007 — STOP BEFORE THE LINE.

**Behaviour:** at a red / amber signal or relevant stop instruction, stop before the stop line; if no visible stop line, stop before the pedestrian crossing as the regulation requires.

**Legal spine:** Regulation 12 specifies stopping before the stop line preceding the pedestrian crossing for red and amber signals, or before the crossing where the line is absent / not visible.

**Subsystem failure:** coordinate precision.

### CLEAN
Intersection, red signal, obvious stop line.

```text
STOP LINE LOCATED
```

### PRESSURED
Car rolls half a bonnet over it.

```text
VEHICLE POSITION:
+0.8 m
```

### BROKEN
Car keeps creeping forward centimetre by centimetre. System ruler becomes absurdly precise.

```text
+1.1 m
+1.3 m
+1.37 m
```

### COLLAPSING
Vehicle somehow migrates into the pedestrian crossing while still technically “stopped”. The stop line chases it forward like a movable finish line.

```text
STOP LINE IS NOT
A SUGGESTION
```

### CALM / CORRECT
Car stops cleanly behind it.

```text
STOP BEFORE THE LINE.
```

**New primitive:** `MEASURE_OFFSET`, `CREEP_LOOP`, `LINE_CHASE`.

---

# EP008 — MATCH. SIGNAL. MERGE.

**Behaviour:** merge predictably: use the acceleration / merging lane where applicable, build appropriate speed, observe traffic and signal intention. Traffic entering a major road must give way to traffic already on it.

**Legal spine:** Regulation 15 covers merging, including giving way when entering national / state highways or major district roads, using acceleration lanes where applicable, observing mirrors and signalling intention.

**Important wording guardrail:** do **not** present universal “zipper merging” as Indian law.

**Subsystem failure:** packet routing.

### CLEAN
Main road traffic flows. One vehicle enters acceleration lane.

```text
MERGE REQUEST RECEIVED
```

### PRESSURED
Vehicle crawls too slowly / fails to signal while trying to enter.

```text
SPEED MISMATCH
INTENT UNKNOWN
```

### BROKEN
ROAD BRAIN treats cars as data packets. Merge vehicle repeatedly gets `ROUTE FAILED` and requeues.

### COLLAPSING
Traffic becomes a network diagram with packet collisions, dropped frames, route loops.

```text
PACKET CANNOT JOIN NETWORK
```

### CALM / CORRECT
Vehicle builds speed, signals, finds safe gap, merges.

```text
MATCH. SIGNAL. MERGE.
```

**New primitive:** `PACKET_ROUTE`, `MERGE_GAP`, `SPEED_MATCH`.

---

# EP009 — ZEBRA CROSSING = HUMAN LANE.

**Behaviour:** slow / stop and give way to pedestrians at an uncontrolled pedestrian crossing.

**Legal spine:** Regulation 39(1) requires drivers approaching an uncontrolled pedestrian crossing to slow down, stop and give way to pedestrians and specified vulnerable users.

**Subsystem failure:** species classification.

### CLEAN
Pedestrian approaches zebra crossing.

```text
CROSSING OCCUPANCY: HUMAN
```

### PRESSURED
Vehicle does not yield.

```text
PRIORITY CONFLICT
```

### BROKEN
System begins classifying the crossing as a literal traffic lane.

```text
LANE TYPE: PEDESTRIAN
```

### COLLAPSING
Pedestrian becomes a gigantic vehicle icon; car shrinks to toy scale. Zebra stripes rise as physical barriers.

```text
WRONG SPECIES HAS PRIORITY
```

### CALM / CORRECT
Car stops. Pedestrian crosses.

```text
ZEBRA CROSSING = HUMAN LANE.
```

**New primitive:** `SPECIES_CLASSIFY`, `ZEBRA_RISE`, `PRIORITY_SWAP`.

---

# EP010 — TRAFFIC INSIDE FIRST.

**Behaviour:** traffic already in a roundabout has right of way; choose the appropriate lane and indicate lane changes / exit as required.

**Legal spine:** Regulation 10 gives traffic already in the roundabout right of way and contains lane / indicator rules.

**Subsystem failure:** orbital mechanics.

### CLEAN
Simple roundabout. One car already circulating.

```text
ORBIT OCCUPIED
```

### PRESSURED
Incoming car barrels in without yielding.

```text
ENTRY WINDOW: CLOSED
```

### BROKEN
System converts roundabout into orbital diagram. Incoming vehicle becomes an asteroid with bad trajectory.

### COLLAPSING
Full solar-system map. Cars orbit central island. Rogue entrant causes gravitational catastrophe.

```text
YOU CANNOT MERGE
DIRECTLY INTO A PLANET
```

### CALM / CORRECT
Incoming vehicle yields, then joins safely.

```text
TRAFFIC INSIDE FIRST.
```

**New primitive:** `ORBIT_PATH`, `ENTRY_WINDOW`, `GRAVITY_FAILURE`.

---

# EP011 — PHONE DOWN. EYES UP.

**Behaviour:** do not use a hand-held mobile phone or communication device while driving; maintain lookout and avoid distraction.

**Legal spine:** Regulation 37 prohibits hand-held mobile / communication-device use while driving; Regulation 5 requires attention and avoidance of distracting activity.

**Subsystem failure:** attention allocation.

### CLEAN
Driver representation has 100% attention directed to road.

```text
ATTENTION: ROAD 100%
```

### PRESSURED
Phone activates.

```text
NEW TASK DETECTED
```

### BROKEN
Attention meter splits:

```text
ROAD 51%
PHONE 49%
```

then reverses.

### COLLAPSING
Road physically shrinks into a tiny picture-in-picture window while the phone UI fills the world.

```text
ROAD RUNNING IN BACKGROUND
```

### CALM / CORRECT
Phone disappears. Road returns full-frame.

```text
PHONE DOWN. EYES UP.
```

**New primitive:** `ATTENTION_METER`, `PIP_WORLD`, `FOCUS_RESTORE`.

---

# EP012 — KEEP YOUR DISTANCE.

**Behaviour:** maintain enough following distance to stop safely if the vehicle ahead slows or stops.

**Legal spine:** Regulation 17 requires sufficient distance commensurate with traffic conditions so the following driver can safely stop if the vehicle ahead slows or stops suddenly.

**Subsystem failure:** personal-space model.

### CLEAN
Two cars with healthy gap.

```text
FOLLOWING DISTANCE: STABLE
```

### PRESSURED
Rear car closes excessively.

```text
BUFFER REDUCING
```

### BROKEN
Distance becomes a storage / memory buffer meter approaching zero.

```text
STOPPING BUFFER: 12%
```

### COLLAPSING
Vehicles visually fuse into one impossible two-car organism.

```text
VEHICLES HAVE MERGED
WITHOUT CONSENT
```

### CALM / CORRECT
Gap restored.

```text
KEEP YOUR DISTANCE.
```

**New primitive:** `GAP_METER`, `BUFFER_DRAIN`, `VEHICLE_FUSION`.

---

# EP013 — HORN ≠ EMOTION.

**Behaviour:** unnecessary horn use is prohibited; horn should be used when genuinely necessary for danger / where mandated.

**Legal spine:** Regulation 23 prohibits unnecessary horn use and continuous / repeated / overlong use, including additional restrictions in residential / silence zones.

**Subsystem failure:** emotional telemetry.

### CLEAN
Traffic is mildly slow.

```text
THREAT LEVEL: NONE
```

### PRESSURED
Driver starts honking anyway.

```text
HORN EVENT DETECTED
DANGER: NONE
```

### BROKEN
System desperately searches for reason:

```text
OBSTACLE? NO
COLLISION RISK? NO
EMOTION? YES
```

### COLLAPSING
Every honk spawns giant comic shockwaves and increasingly useless “URGENT” banners until the road itself vibrates apart.

```text
HORN IS NOT
A BUTTON FOR FEELINGS
```

### CALM / CORRECT
Quiet road ambience.

```text
HORN ≠ EMOTION.
```

**New primitive:** `HORN_WAVE`, `CAUSE_SEARCH`, `NOISE_OVERLOAD`.

---

# EP014 — HAZARDS ≠ PARKING PERMISSION.

**Behaviour:** hazard lights do not make an otherwise prohibited / obstructive parking position acceptable.

**Legal spine:** Regulation 22 contains extensive stopping / parking prohibitions; hazard-warning lights are separately prescribed for specific emergency / breakdown situations elsewhere in the regulations. The episode must not claim that hazard lights themselves are illegal in ordinary use; the point is that they do not erase parking restrictions.

**Subsystem failure:** permission token.

### CLEAN
A clearly inappropriate stopping / parking location: pedestrian crossing, entrance, bus lane, etc.

### PRESSURED
Vehicle stops and switches hazards on.

```text
PARKING RESTRICTION ACTIVE
```

### BROKEN
System sees hazards and briefly attempts to authenticate them as a magic override credential.

```text
OVERRIDE TOKEN DETECTED?
```

### COLLAPSING
Hazard triangle becomes a giant bureaucratic rubber stamp labelled `PERMISSION`, repeatedly stamping everything while the system screams `INVALID CREDENTIAL`.

```text
BLINKING DOES NOT
CHANGE GEOGRAPHY
```

### CALM / CORRECT
Vehicle moves to a lawful / non-obstructive place.

```text
HAZARDS ≠ PARKING PERMISSION.
```

**New primitive:** `HAZARD_BLINK`, `AUTH_TOKEN`, `STAMP_REJECT`.

---

# EP015 — MAKE SPACE.

**Behaviour:** yield right of way to an emergency vehicle operating its siren / flasher; move left as practicable and stop if required until it passes.

**Legal spine:** Regulation 27 gives responding emergency vehicles right of way and directs other drivers to yield, move left as practicable and stop if required.

**Subsystem failure:** priority scheduler.

### CLEAN
Ordinary traffic. Emergency vehicle appears behind with active siren / flasher.

```text
PRIORITY VEHICLE DETECTED
```

### PRESSURED
Traffic does not create space.

```text
PRIORITY REQUEST BLOCKED
```

### BROKEN
ROAD BRAIN shows a CPU scheduler where every normal vehicle has inexplicably marked itself `CRITICAL`.

### COLLAPSING
Emergency packet starves while regular cars consume every lane / resource.

```text
EVERYONE CANNOT BE
PRIORITY ONE
```

### CALM / CORRECT
Traffic moves aside; ambulance passes.

```text
MAKE SPACE.
```

**New primitive:** `PRIORITY_QUEUE`, `LANE_CLEAR`, `EMERGENCY_PASS`.

---

# EP016 — IF YOU CAN'T EXIT, DON'T ENTER.

**Behaviour:** do not enter an intersection / junction if doing so will obstruct or endanger traffic already moving through it.

**Legal spine:** Regulation 9 requires slowing at intersections / junctions / crossings and prohibits entering when doing so is likely to endanger other road users. Frame this as anti-blocking / predictive intersection discipline, not as a claim about a painted “box junction” rule unless the location actually has one.

**Subsystem failure:** future-state prediction.

### CLEAN
Green signal. Space beyond intersection is visibly full.

```text
EXIT CAPACITY: 0
```

### PRESSURED
Driver enters anyway.

```text
ROUTE COMPLETION: IMPOSSIBLE
```

### BROKEN
Signal changes. Vehicle now blocks cross traffic.

```text
PREDICTION FAILURE
```

### COLLAPSING
Entire intersection deadlocks into a literal puzzle grid; every car waits for another car to move first.

```text
CONGRATULATIONS
YOU BUILT A KNOT
```

### CALM / CORRECT
Driver waits before intersection until exit space exists.

```text
IF YOU CAN'T EXIT,
DON'T ENTER.
```

**New primitive:** `CAPACITY_SCAN`, `GRIDLOCK_KNOT`, `FUTURE_PATH`.

---

# EP017 — U-TURN IS A MANOEUVRE.

**Behaviour:** plan, signal and perform a U-turn only where safe / permitted; do not treat it as an impulsive mid-road plot twist.

**Legal spine:** Regulation 8 covers U-turns and places restrictions on where they may be made. Before publication, use the exact location-specific wording from the regulation / signage rather than claiming one universal prohibition beyond the rule.

**Subsystem failure:** narrative continuity.

### CLEAN
Vehicle proceeds normally.

```text
ROUTE DIRECTION: FORWARD
```

### PRESSURED
Without setup, vehicle suddenly begins turning across traffic.

```text
PLOT CHANGE DETECTED
```

### BROKEN
Map route rewrites itself mid-frame. Navigation arrow spins repeatedly.

### COLLAPSING
Entire reel rotates 180° while captions remain upright. ROAD BRAIN cannot determine which direction time is flowing.

```text
U-TURN IS NOT
A PLOT TWIST
```

### CALM / CORRECT
Safe, signalled, deliberate U-turn in a permitted context.

```text
PLAN. SIGNAL. TURN.
```

**New primitive:** `WORLD_ROTATE`, `ROUTE_REWRITE`, `TURN_ARC`.

---

# EP018 — TURN LANE MEANS TURN LANE.

**Behaviour:** remain in the lane designated for the intended manoeuvre at intersections.

**Legal spine:** Regulation 6(5) requires a vehicle approaching intersections with turning lanes marked by a single solid line to remain in the lane meant for the direction of manoeuvre.

**Subsystem failure:** semantic meaning of arrows.

### CLEAN
Clearly marked left / straight / right lanes.

```text
LANE INTENT: STRAIGHT
```

### PRESSURED
Car in turn lane decides to go straight.

```text
ARROW DISAGREEMENT
```

### BROKEN
Painted arrows start rotating, confused by driver behaviour.

### COLLAPSING
All arrows detach from the road and point everywhere simultaneously.

```text
SYMBOL MEANING
HAS COLLAPSED
```

### CALM / CORRECT
Car follows marked lane direction.

```text
TURN LANE MEANS TURN LANE.
```

**New primitive:** `ARROW_DETACH`, `SEMANTIC_ERROR`, `LANE_INTENT_LOCK`.

---

# EP019 — FOOTPATH ≠ PARKING.

**Behaviour:** do not park on the footpath / pedestrian crossing and obstruct pedestrian space.

**Legal spine:** Regulation 22(2)(c) prohibits parking on a footpath, cycle track and pedestrian crossing.

**Subsystem failure:** object classification.

### CLEAN
Empty footpath with pedestrian icon.

```text
SURFACE TYPE: PEDESTRIAN
```

### PRESSURED
Car mounts and parks on it.

```text
OBJECT CLASSIFICATION ERROR
```

### BROKEN
System tries to reinterpret car as pedestrian.

```text
LEGS: 0
WHEELS: 4
PEDESTRIAN CONFIDENCE: 0%
```

### COLLAPSING
Car receives tiny animated human legs and attempts to “walk” while pedestrians are forced into road.

```text
YOUR CAR IS NOT
A PEDESTRIAN
```

### CALM / CORRECT
Footpath cleared.

```text
FOOTPATH ≠ PARKING.
```

**New primitive:** `SURFACE_CLASSIFY`, `CAR_LEGS`, `PEDESTRIAN_DISPLACEMENT`.

---

# EP020 — ONE WAY MEANS ONE WAY.

**Behaviour:** do not drive against the designated direction of a one-way road.

**Legal spine:** Regulation 4(6) says a vehicle shall not be driven on a road declared “One Way” except in the direction specified by signage; Regulation 4(7) also prohibits driving against the flow of traffic except when specifically directed.

**Subsystem failure:** universe orientation.

### CLEAN
One-way street. Every vehicle moves in one direction.

```text
TRAFFIC VECTOR: →
```

### PRESSURED
One vehicle appears heading the opposite way.

```text
VECTOR CONFLICT
```

### BROKEN
ROAD BRAIN rotates arrows and camera trying to reconcile the impossible object.

```text
NORTH?
SOUTH?
REALITY?
```

### COLLAPSING
World splits into mirrored universes: half the road believes left is right, forward is backward. Vehicles duplicate into oppositely moving ghosts.

```text
DIRECTIONAL CONSENSUS LOST
```

### CALM / CORRECT
Single coherent traffic flow restored.

```text
ONE WAY MEANS ONE WAY.
```

**New primitive:** `VECTOR_FIELD`, `MIRROR_WORLD`, `FLOW_RESTORE`.

---

# Season 01 production order

The numbered order is the intended default because it alternates visual mechanisms and avoids repetitive adjacent lessons:

```text
EP001  INDICATE. THEN MOVE.              geometry failure
EP002  DIM YOUR HIGH BEAMS.              vision failure
EP003  THE SHOULDER IS NOT A LANE.       world-model failure
EP004  PASS. RETURN LEFT.                 territorial failure
EP005  ONE LANE AT A TIME.               target-acquisition failure
EP006  SOLID LINE = DON'T CROSS.          boundary failure
EP007  STOP BEFORE THE LINE.              coordinate failure
EP008  MATCH. SIGNAL. MERGE.              routing failure
EP009  ZEBRA CROSSING = HUMAN LANE.       species / priority failure
EP010  TRAFFIC INSIDE FIRST.              orbital failure
EP011  PHONE DOWN. EYES UP.               attention failure
EP012  KEEP YOUR DISTANCE.                buffer failure
EP013  HORN ≠ EMOTION.                    emotional telemetry failure
EP014  HAZARDS ≠ PARKING PERMISSION.      authorization failure
EP015  MAKE SPACE.                        priority-scheduler failure
EP016  IF YOU CAN'T EXIT, DON'T ENTER.    future-state failure
EP017  U-TURN IS A MANOEUVRE.             continuity failure
EP018  TURN LANE MEANS TURN LANE.         semantic-symbol failure
EP019  FOOTPATH ≠ PARKING.                object-classification failure
EP020  ONE WAY MEANS ONE WAY.             orientation failure
```

## Production tiers

### Tier A — build soon
High sendability + strong new visual grammar:
- EP004 Right Lane Raja
- EP006 Solid Line
- EP009 Human Lane
- EP011 Phone Down
- EP013 Horn ≠ Emotion
- EP015 Make Space
- EP020 One Way

### Tier B — core instructional spine
- EP005 One Lane at a Time
- EP007 Stop Before the Line
- EP008 Merge
- EP010 Roundabout
- EP012 Following Distance
- EP016 Don't Block Intersection
- EP018 Turn Lane

### Tier C — publish after visual test / exact legal copy check
- EP014 Hazards ≠ Parking Permission
- EP017 U-turn
- EP019 Footpath ≠ Parking

Tier C is not lower importance. It means the final visual scenario and copy need extra care so the joke does not overstate the legal rule.

---

# Legal / factual source map

Primary season planning source: **Motor Vehicles (Driving) Regulations, 2017**, notified by the Ministry of Road Transport and Highways on 23 June 2017.

Relevant regulations used in this plan:

```text
Reg. 4   Use of roads by vehicles / keep left / one way / against flow
Reg. 5   Duties, attention and vulnerable road users
Reg. 6   Lane traffic / solid lines / turning lanes
Reg. 8   Left, right and U-turns
Reg. 9   Intersections
Reg. 10  Roundabouts
Reg. 12  Traffic-control signals / stop line
Reg. 14  Overtaking / return left
Reg. 15  Merging
Reg. 17  Safe following distance
Reg. 22  Stopping and parking
Reg. 23  Horns and silence zones
Reg. 27  Emergency vehicles
Reg. 31  Vehicle lighting
Reg. 33  Lane splitting, where specifically permitted
Reg. 37  Mobile phones / communication devices
Reg. 39  Pedestrian crossings / footpaths / cycle tracks
```

Before publishing any episode, re-check the exact regulation and any location-specific signage / exceptions. The creative shorthand is not itself legal advice.

---

# What is deliberately not in EP004–EP020

These remain useful future candidates but are intentionally held back to avoid overcrowding Season 01:

- lane splitting / filtering: Regulation 33 is unusually conditional (urban area, max 40 km/h, specifically permitted by signs, speed difference ≤15 km/h), so it deserves a later episode built around the nuance rather than a blanket prohibition;
- railway crossings;
- helmet / seat-belt behaviour;
- school zones;
- fog-light misuse;
- reverse driving;
- wrong-side overtaking variants;
- parking near intersections / bus stops / hospital entrances;
- breakdown-warning triangles;
- speed-limit episodes;
- bus-lane / cycle-lane occupation.

These can seed Season 02 once the first 20 transmissions establish the grammar.
