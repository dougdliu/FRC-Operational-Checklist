# Chief Delphi Thread Audit: Items 320-369

Scope:
- Source thread: https://www.chiefdelphi.com/t/50-fun-ways-to-lose-a-match/481954
- Audit range: numbered entries 320-369
- Current targets checked: ways-to-lose-a-match.md and ways-to-win-a-season-in-frc.md

Legend:
- covered: already represented in the current lists
- add: missing and should be added
- skip: too game-specific, joke-only, duplicate, or low transfer value for institutional memory
- not found: no distinct numbered post found for that number in retrieved pages

| Thread # | Exact Thread Entry (Condensed Quote) | Audit Status | Rationale |
|---|---|---|---|
| 320 | NRG radio power disconnected by collision in finals | covered | Covered by breaker/radio vulnerability and comm loss prevention guidance. |
| 321 | No distinct numbered entry found | not found | Not present in retrieved 320-369 span. |
| 322 | No distinct numbered entry found | not found | Not present in retrieved 320-369 span. |
| 323 | "Get your hopper ripped off ... continue driving with it flapping" | skip | Highly game-mechanism specific; broader damaged-robot behavior already covered. |
| 324 | "Metal shavings in your Rio and you can’t connect to field" | covered | Already covered by electronics contamination and drill/debris controls. |
| 325 | "Metal shavings in your gyro ... changes forward" | covered | Already covered by sensor protection/calibration and IMU reliability checks. |
| 326 | "SD card out of rio; loaner DS doesn’t work" | skip | Legacy/hardware-specific edge case; comms and DS redundancy already covered. |
| 327 | "Alliance-color coordinate mismatch in pose estimation" | covered | Already covered by red/blue validation and field-coordinate sanity checks. |
| 328 | "Don’t tell driver about defense penalties in endgame" | covered | Already covered by rules briefing/manual discipline and strategy comms. |
| 329 | "Forget to restore robot from 25% speed" | covered | Explicitly present in current list. |
| 330 | "Collect another robot" | skip | Joke/non-transferable. |
| 331 | "Forget human players exist when robot is broken" | covered | Covered by human-player utilization and match-show-up discipline. |
| 332 | "Forget which hub is active" | skip | Older-game specific and non-generalized wording. |
| 333 | "Launch fuel at field e-stop button" | skip | Old-game specific and intentionally unsafe behavior. |
| 334 | "Leave hood up under trench" | skip | Specific to old field geometry; generalized clearance checks already covered. |
| 335 | No distinct numbered entry found | not found | Not present in retrieved 320-369 span. |
| 336 | "Drill without covering Neo Vortexes" | covered | Explicitly covered by fabrication/debris protection guidance. |
| 337 | "Don’t have a radio" | covered | Explicitly covered by no-radio failure mode and comm readiness checks. |
| 338 | "Fry your radio and keep playing" | covered | Explicitly covered by radio-health and comm-dropout handling. |
| 339 | "Swerve constantly rotates; driver compensates" | covered | Explicitly covered by swerve drift/spin no-go policy. |
| 340 | "Drive quals with corrupted Rio image" | covered | Explicitly covered by Rio image verification and related failure item. |
| 341 | "Blame software/mech depending on latest change" | covered | Explicitly covered by cross-subteam root-cause discipline. |
| 342 | No distinct numbered entry found | not found | Not present in retrieved 320-369 span. |
| 343 | "3D printed pulley explodes in playoffs" | covered | Covered by printed pulley/material reliability and clearance/load checks. |
| 344 | "Don’t set current limits; brownouts" | covered | Explicitly covered by motor current-limit requirements. |
| 345 | "Rotate motor Spark MAX not secured; wires caught in wheel" | covered | Covered by controller mounting and wire-routing/strain-relief guidance. |
| 346 | "Forget CAN ID / zero encoder on replacement" | covered | Covered by CAN verification and post-repair calibration checks. |
| 347 | "Kraken falls out" and "45 min wrong diagnosis on bad encoder cable" | covered | Covered by bolt checks, service validation, and evidence-based troubleshooting. |
| 348 | "Reassemble swerve without key" | covered | Covered by post-repair missing-component and validation checklist discipline. |
| 349 | "Turn off power to the building" | skip | Joke/non-transferable. |
| 350 | "Have too much fun ramming bots" | skip | Low transfer value; already broadly covered by defense/foul discipline. |
| 351 | "Good robot, bad match comps/picks" | skip | More luck/selection outcome than operational control; scouting process already covered. |
| 352 | "Put a single ! in crucial swerve code" | covered | Explicitly added in current revision. |
| 353 | "Forget Loctite; intake disassembles" | covered | Already covered by fastener/Loctite discipline. |
| 354 | "RoboRio gets flattened" | skip | Specific failure symptom; broader electronics protection and mounting already covered. |
| 355 | "Only scorer, intake roller cracks" | skip | Game/role specific; generic single-point failure mitigation already covered. |
| 356 | "Unplug network cable between RBR and switch" | covered | Covered by ethernet securing and comms validation rules. |
| 357 | "Use acrylic everywhere" | covered | Covered by acrylic vs polycarbonate guidance. |
| 358 | "Wrong-infill 3D pulley explodes" | covered | Covered by critical-subsystem material/print reliability guidance. |
| 359 | "Turret side not checked + Xbox disconnect" | skip | Composite old-game specific issue; DS/controller robustness already covered. |
| 360 | "Use acrylic like polycarbonate" | covered | Duplicate theme already covered. |
| 361 | "Don’t mount bumpers properly" | covered | Covered by bumper fastening/inspection requirements. |
| 362 | "Break CAN in playoffs, fail to find in time" | covered | Covered by CAN integrity and diagnostics process. |
| 363 | "Use 4awg in PDH; comes out mid-match" | covered | Explicitly added via PDH wire-fit mismatch failure mode. |
| 364 | "Fuel bounces into launcher crack and stalls" | skip | Very game-specific geometry/jam edge case. |
| 365 | "Unbind robot-relative button mid-playoffs" | covered | Covered by control mapping change discipline and pre-match validation. |
| 366 | "Logitech switches Xbox to PlayStation mode" | covered | Explicitly covered by controller mode/mapping controls. |
| 367 | "Replug CAN wire untested; still broken next match" | covered | Explicitly added via CAN-repair diagnostics requirement/failure mode. |
| 368 | No distinct numbered entry found | not found | Not present in retrieved 320-369 span. |
| 369 | "Intake pulley near polycarb without spacer ... angle grinder" | covered | Explicitly covered by pulley-to-polycarbonate clearance/spacer item. |

## Outcome

High-value misses identified in this audit and now incorporated:
- Logical inversion bug in swerve control code (thread #352)
- CAN replug without diagnostics before next match (thread #367)
- PDH wire-fit mismatch / oversized conductor risk (thread #363)

All other entries in 320-369 are now either covered, intentionally skipped as low-transfer/game-specific, or not found as distinct numbered posts in retrieved content.
