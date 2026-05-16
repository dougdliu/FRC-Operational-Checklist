# FRC Operational Checklists
## Season, Event, Match, and Recovery Checklists

These checklists convert lessons into daily execution.

Source references:
- [ways-to-lose-a-match.md](ways-to-lose-a-match.md)
- [ways-to-win-a-season-in-frc.md](ways-to-win-a-season-in-frc.md)
- [chief-delphi-common-issues-2024-2026-audit.md](chief-delphi-common-issues-2024-2026-audit.md)
- Chief Delphi: [Most Common Issues Seen on Robots This Year, 2024](https://www.chiefdelphi.com/t/most-common-issues-seen-on-robots-this-year/466119)
- Chief Delphi: [Most Common Issues Seen 2025](https://www.chiefdelphi.com/t/most-common-issues-seen-2025/505274)
- Chief Delphi: [Most Common Issues Seen 2026](https://www.chiefdelphi.com/t/most-common-issues-seen-2026/520595)

How to use:
- Print this document or use it on a tablet.
- Assign a single owner for each checklist block.
- Mark each line item Done, Not Done, or N/A.
- At kickoff, run the game archetype checklist and add the matching risks to the season risk register.

---

## A) Preseason Readiness Checklist

Owner: Team Leads

- Team roles assigned with primary and backup for each critical role
- Driver, operator, and human player practice plan scheduled
- Electrical standards defined (wire colors, labels, strain relief, CAN conventions)
- Software release process defined (branching, tagged match releases, rollback plan)
- Robot weight budget defined by subsystem
- Spare parts plan created for high-risk mechanisms
- Game archetype risks identified from the current game manual and compared against Section L
- Bumper design selected early, including mounting, legal foam/backer material, fabric, numbers, and inspection removal plan
- Battery inventory tested, labeled, and break-in plan created for any new batteries
- High-current motor current-limit standards defined for every motor controller family
- Pit tool and consumables inventory list created
- Pit kit includes spare main breakers, bumper repair supplies, frame/intake stock, swerve wear parts, ferrules, Wago-compatible wire tools, ethernet/USB cables, and DS controller spares
- Driver station laptop standard image prepared and tested
- Safety and emergency procedures reviewed
- Post-match review template ready

---

## B) Weekly Build and Integration Checklist

Owner: Build Lead

- Wiring accessible and inspectable
- CAN chain physically secured end-to-end
- CAN terminating resistors mounted, insulated, and shake-tested
- Main breaker protected by shroud
- Battery connections strain-relieved and tested
- Battery leads torqued at battery, main breaker, and PDH/PDP; exposed terminals heat-shrunk
- Radio and ethernet strain relief installed
- USB connections for CANivore, coprocessors, cameras, and log drives secured without making them unserviceable
- Dynamic cabling run through a controlled path with no connectors in moving sections
- All critical fasteners checked and marked
- Swerve module assembly checked against manufacturer instructions; gears greased; wheel tread inspected
- Sensor mounting secure and protected from chips/debris
- Cameras and vision lenses cleaned; game-piece fuzz or dust removed
- Robot weighed and compared to budget
- Bumpers attach securely, remove quickly for inspection, and have no loose fabric/flaps
- Serviceability test run (remove and reinstall major subsystem)
- Drop/shake test run for intermittent electrical, radio, or CAN symptoms with status lights observed
- Failure log updated from latest testing

---

## C) Software Release Checklist

Owner: Software Lead

- Build from tagged release branch
- Competition config used (no profiling/debug arguments)
- Auto tested on both alliance sides
- Control mappings validated with current controllers
- Null handling tested for disconnected sensors/cameras
- Soft limits and safety interlocks validated
- Supply current limits set for every motor and reviewed against battery/main-breaker behavior
- High-current actions staggered or power-managed where simultaneous drivetrain and mechanism loads can brown out the robot
- Heading zero procedure confirmed with drive team
- Basic fallback autonomous available, even if only a mobility/go-straight routine
- Auto paths reviewed for partner conflicts and common alliance configurations
- Deploy performed in pit, not in queue
- Commit hash recorded in match log
- Rollback commit prepared and verified

---

## D) Driver Station Checklist (Start of Event Day)

Owner: Drive Coach or DS Operator

- Laptop rebooted today
- Power settings set to high performance
- Sleep and display-off disabled while on battery and AC power
- Non-essential apps closed
- Windows updates installed before the event or paused/active-hours set so updates cannot run during competition
- Xbox Game Bar disabled or removed
- Driver Station software version verified
- Firewall settings verified for DS operation
- WiFi auto-connect disabled except required field behavior
- USB ports, cables, and controller connections verified
- Ethernet, USB, and charger cables strain-relieved on the driver station shelf
- Controller brand/model matches expected mapping
- Controller axes, buttons, and mode switches tested in the USB Devices tab
- Spare controllers and spare cable present
- Laptop physically secured to DS shelf
- Correct hook/loop side of velcro installed for the field shelf
- Charger present and functional

---

## E) Pre-Match Queue Checklist

Owner: Queue Lead

- Correct battery installed, secured, and recently charged
- Battery connector fully seated and secured with the team's approved zip tie, reusable tie, bolt, or velcro loop method
- Main breaker accessible and protected
- Robot enabled test passed in pit
- Correct autonomous routine selected
- Alliance auto paths agreed with partners; no path conflict or midline collision risk left unresolved
- Bumpers installed correctly for alliance color
- Bumper tape and fabric condition checked
- Bumper backers, brackets, and numbers checked for damage or looseness
- Pneumatics charged and leak check done
- Controllers connected and assigned correctly
- Controller axes centered and buttons verified after any reconnect
- DS laptop plugged into field power; ethernet fully clicked into laptop and field port
- Driver/operator aware of any control changes
- Strategy reviewed with alliance partners
- Camera lenses wiped if game pieces shed dust, fuzz, or residue
- Swerve wheels, belts, shafts, and module bolts checked if the last match involved hard defense or terrain hits
- Match-specific no-go issues cleared
- Team arrives to queue on time

---

## F) Post-Match Debrief Checklist (3-Minute Version)

Owner: Drive Coach

- Match result captured
- Auto success/failure captured
- Endgame success/failure captured
- Penalties captured with brief cause
- Any disconnect or brownout noted
- Any mechanism anomaly noted
- Any hot breaker, warm PDH/PDP terminal, or unusual battery voltage sag noted
- Any bumper, intake, frame, swerve, or exposed mechanism impact noted
- Top 1 immediate fix identified
- Owner assigned for immediate fix
- Verify fix complete before next queue

---

## G) Pit Repair Checklist

Owner: Pit Lead

- Failure symptom reproduced or clearly observed
- Root cause hypothesis stated before repair
- Repair owner assigned
- Repair completed with second-person verification
- Full range-of-motion check performed
- Sensor zero/calibration check performed
- Fastener and connector audit of touched area
- Dynamic cable path rechecked through full range of motion after any arm, elevator, intake, or climber repair
- Wago/lever connectors checked for correct strip length, untwisted conductor insertion, and tug-test pass
- Kraken, Spark, NEO, CANivore, radio, and battery wiring strain relief restored after service
- Software retest if hardware changed
- Dry run enable test in pit
- Drop/shake test repeated after fixing intermittent radio, CAN, or power issues
- Repair log updated

---

## H) Alliance Selection and Scouting Checklist

Owner: Scouting Lead

- All qualification matches scouted
- Data quality spot-check completed
- Candidate list ranked by role fit, not friendship
- Reliability and no-show risk considered
- Match video reviewed for top candidates
- Claims validated against actual performance
- Pick list rehearsal completed with captain and coach
- Backup pick paths prepared

---

## I) Event Closeout Checklist

Owner: Team Leads

- Critical failures summarized with root causes
- Corrective actions assigned with due dates
- Consumables and spare inventory updated
- Mechanical wear items flagged for replacement
- Software technical debt list updated
- Scouting process improvements captured
- Training gaps identified for next week

---

## J) No-Go Conditions

If any condition below is true, do not queue until resolved or consciously accepted by coach and pit lead.

- Unknown electrical fault affecting control power or CAN
- Untested code change on robot
- Controller mapping uncertainty
- Battery security or battery health uncertainty
- Hot main breaker, tripped main breaker not yet replaced, or unexplained brownout trend
- Damaged bumper attachment, illegal bumper construction, or bumper fabric dragging/catching
- Damaged swerve module, drivetrain rail, intake side plate, or exposed shaft not yet inspected under load
- Significant mechanical interference risk
- Uncalibrated critical sensor used by autonomous or closed-loop control

---

## K) Institutional Knowledge Capture Template

Use this for major incidents.

- Date and event:
- Match number:
- Subsystem:
- Failure description:
- Root cause:
- What made detection hard:
- Immediate containment:
- Permanent corrective action:
- Checklist or process update required:
- Owner:
- Verified by:

---

## L) Game Archetype Risk Checklist

Run this at kickoff, after the first week of driver practice, and after the first event. Add every applicable line to the build risk register.

### High-Contact, Open-Field, Defense-Heavy, or Midline-Race Games

- Bumper mounts, backers, and brackets designed for repeated full-speed hits; brackets through-bolted where possible
- Front and side frame rails sized for offset swerve-to-swerve impacts, not only flat bumper hits
- Intakes outside the frame perimeter designed as compliant, guarded, sacrificial, or quickly replaceable assemblies
- Spare intake rollers, side plates, shafts, belts, frame tubes, bumper material, and mounting hardware packed
- Damage isolated to replaceable bars or plates instead of transmitting impact loads into swerve modules or complex mechanisms
- Drivers trained on when to retract vulnerable mechanisms before contact
- Post-match inspection includes bumpers, frame rails, intake geometry, exposed shafts, swerve modules, and battery retention

### Terrain, Bump, Trench, Ramp, or Robot-Under-Robot Games

- Swerve drive shafts, main bearings, retaining rings, belts, internal motor bolts, and wheel tread inspected after terrain-heavy matches
- Clearance checked for motors, wires, cameras, RIO/radio, hoods, hoppers, arms, and elevators against field elements and other robots
- Mechanisms that rise above a protected height have driver rules for when they may be deployed
- Spare module shafts, belts, wheels, bearings, and mounting hardware packed if the drivetrain will take repeated vertical shocks

### Game-Piece Ingestion or Falling-Piece Games

- Elevators, arms, intakes, electronics bays, and drivetrain openings protected with panels, coreflute, polycarbonate, netting, or surgical tubing
- Robot tested by dropping and bouncing game pieces into likely openings while disabled and while mechanisms move slowly
- Internal game pieces cannot press the main breaker, bind belts/chains, hit sensors, unplug wires, or jam swerve modules
- Covers are removable quickly enough for inspection and pit service

### Tall Elevator, Arm, Wrist, or Climber Games

- Dynamic cabling has controlled motion, strain relief, full travel slack, and no connectors in the moving span
- E-chain or rolling-loop fill is conservative enough for wires to move without binding or crushing
- Double-chain, rope, or belt-driven stages are synced, tensioned, and checked for tracking over repeated cycles
- Ropes run over pulleys or smooth radii, never sharp metal edges
- Climber gearbox, brake mode, reaction point, and center-of-gravity behavior verified with the actual robot weight
- Hardstops, plates, and brackets sized for repeated high-load impacts, not just static holding

### High-Current or Battery-Stress Games

- New batteries broken in before the first event when possible; battery health tracked across the season
- Supply current limits set on every motor, not only drivetrain motors
- High-current mechanism actions staggered or power-managed against drivetrain demand
- Correct breaker sizes verified for radio, RIO, swerve modules, motors, and other protected loads
- Main breaker replaced after a trip and spare breakers carried in the pit
- Battery leads, PDH/PDP main terminals, and motor power terminals checked for heat, discoloration, looseness, and strain relief

### Static, Dust, Foam, Fuzz, or Shedding Game Pieces

- Loose wiring, weak strain relief, and poor grounds ruled out before blaming ESD
- Intake and mechanism structures electrically bonded to chassis where legal and appropriate
- Sensitive electronics protected or shielded if static resets appear after wiring causes are cleared
- Camera lenses wiped between matches if game pieces shed debris
- RIO, PDH/PDP, radio, coprocessors, and unused ports protected from dust, metal shavings, and game-piece debris

### Auto-Crowding, Shared-Zone, or Path-Conflict Games

- Drive team has a pre-match auto-path negotiation script
- Autos are named clearly by start position, path, and scoring objective
- Fallback mobility/go-straight auto is kept working even if complex path tools fail
- Vulnerable intakes and arms retract or avoid midline race contact zones during auto
- Software can select safe autos quickly without editing code in queue

---

## M) Thread-Derived Reliability Hotlist

Run this before every event, especially if the current game matches one of the archetypes above.

### Bumpers and Inspection

- Legal bumper foam/backer/fabric verified against the current manual
- Hollow pool noodles avoided unless repaired into a legal solid-core equivalent under inspector guidance
- Excess fabric trimmed so bumpers mount cleanly and can be re-stapled or repaired
- Numbers durable, legal, and not likely to scrape off during contact
- Reversible bumpers avoided unless flaps, velcro, weight, and repair process are fully tested
- Bumpers removable quickly for weight inspection and service, then locked down immediately after reinstall

### Electrical, Power, and CAN

- Ferrules used on Weidmuller or screw-terminal ports where appropriate and properly crimped
- Wago/lever connectors stripped to the printed gauge, inserted without twisting high-strand conductors, and not overloaded beyond the application
- High-current paths avoid questionable mid-run connectors; direct runs or rated service connectors used where practical
- Battery connector, battery strap, and battery box each independently prevent movement or disconnects
- Battery bolts are appropriate hardware, not weak supplied bolts that loosen or deform under FRC use
- REV NEO encoder/hall wires protected from pulling, impact, and aggressive routing; Spark MAX connectors retained
- Kraken terminals torqued and strain-relieved near the motor so vibration does not side-load screws or lugs
- CANivore USB uses a shielded, secured cable; logging drives or extensions cannot disrupt USB power or CANivore connectivity
- PDH/PDP main terminals inspected for heat damage, melted plastic, loose high-strand wire, or ferrule/wire-gauge mismatch

### Swerve and Drivetrain

- Steering encoders calibrated before each event and before playoffs
- Wheel tread checked after every match in contact-heavy games
- MK4i belts, MAXSwerve shafts, module bearings, retaining rings, motor faceplates, and internal bolts inspected as applicable
- Module repair followed by a wheel-orientation, missing-spacer, missing-bearing, and missing-key check before queueing
- Frame rail stiffness reviewed in CAD; chassis not over-lightened in unknown collision paths

### Vision, Coprocessors, and Storage

- Known-good coprocessor image and spare storage media available
- SD cards are high quality; endurance-class media used for frequent logging where appropriate
- Coprocessors, cameras, and storage cards mounted away from impact zones and with connectors retained
- USB-to-ethernet adapters and spare ethernet cables packed for DS/network emergencies

### Driver Station and Event Execution

- DS process checklist visible on the laptop or driver station console
- Driver Station restarted when weird stale state, controller inversion, missing controllers, or enable issues appear
- Windows updates installed ahead of time, then paused or active-hours-limited before competition
- If the robot cannot make a match, a team representative still reports to the field for alliance communication and possible points
- At events, focus on making existing functions reliable before adding new capabilities

---

## N) 10 Non-Negotiables

- No last-minute untested code in queue
- No match without checklist run
- No unsecured battery or DS laptop
- No unknown CAN health
- No unresolved repeated failure
- No missing backup role coverage
- No skipped post-match debrief
- No unverified alliance assumptions
- No ignored penalty trends
- No offseason without handoff documentation
