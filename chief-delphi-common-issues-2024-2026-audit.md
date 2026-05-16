# Chief Delphi Common Issues Audit: 2024-2026

Scope:
- 2024 thread: https://www.chiefdelphi.com/t/most-common-issues-seen-on-robots-this-year/466119
- 2025 thread: https://www.chiefdelphi.com/t/most-common-issues-seen-2025/505274
- 2026 thread: https://www.chiefdelphi.com/t/most-common-issues-seen-2026/520595

Method:
- Retrieved the Chief Delphi Discourse JSON pages on May 15, 2026.
- Reviewed all topic pages and nontrivial replies: 78 posts in 2024, 37 posts in 2025, and 33 posts in 2026.
- Distilled repeated or transferable advice into [frc-operational-checklists.md](frc-operational-checklists.md).
- Kept highly year-specific examples only when they revealed a repeatable game archetype or operational control.

---

## Year-to-Year Advice

### Bumpers

- Build bumpers early; do not treat them as a final-night accessory.
- Verify legal foam, backer material, fabric, number size, number durability, and corner construction against the current manual.
- Design bumper mounts into the frame from the start so bumpers remove quickly for inspection and service.
- Through-bolt or otherwise positively capture bumper brackets in high-contact games; wood screws alone are not a high-reliability impact solution.
- Trim excess fabric so the bumper seats cleanly and can be repaired with staples or tape if needed.
- Avoid reversible bumpers unless the team has already proven the flap retention, weight, repair process, and color-change workflow.

### Electrical, Power, and CAN

- Strain-relieve every wire that can be tugged loose, especially radio, ethernet, USB, CANivore, Spark MAX, NEO encoder, Kraken terminal, battery, and PDH/PDP wiring.
- Protect the main breaker from game pieces, robot contact, and internal debris while keeping it accessible.
- Secure the battery connector and the battery itself as two separate controls; a hard hit can defeat either one.
- Torque battery, main breaker, PDH/PDP, and motor-controller terminals and inspect them for heat, looseness, and discoloration.
- Use correct breaker sizes; incorrect breakers can either nuisance trip or fail to protect the device.
- Set supply current limits on every motor to prevent brownouts, main breaker trips, and battery damage.
- Treat tripped or hot main breakers as a reliability problem, not a normal match event.
- Verify Wago/lever connector strip length, insertion, wire gauge, and conductor condition; high-strand or oversized wire can fail if poorly terminated.
- Use ferrules where appropriate, but only with the gauge and terminal style they are rated for.
- Mount, insulate, and strain-relieve CAN terminating resistors so a hit or drop test cannot dislodge them.
- Rule out loose wiring and poor strain relief before declaring a problem to be ESD.

### Swerve and Drivetrain

- Follow the module manufacturer's assembly guide completely; missing bearings, spacers, keys, snap rings, and bolts are recurring failure sources.
- Use threadlocker where appropriate, but avoid products that craze polycarbonate.
- Grease swerve gears and inspect tread, belts, shafts, bearings, retaining rings, motor faceplates, and mounting bolts during events.
- Calibrate steering encoders before events and before playoffs.
- After any module repair, verify wheel orientation, steering angle, encoder offset, and all retained hardware before queueing.
- In hard-contact games, bring spare frame rails, shafts, wheels, belts, and module-specific wear items.

### Mechanisms

- Anything extending outside the frame perimeter should be compliant, guarded, sacrificial, or quickly replaceable.
- Design high-contact intakes so impacts do not transmit directly into swerve modules or hard-to-replace structure.
- Use panels, coreflute, polycarbonate, netting, or surgical tubing to keep game pieces out of elevators, arms, electronics, and drivetrain openings.
- Route dynamic wiring through controlled paths with strain relief, full-travel slack, and no connectors in the moving span.
- Keep elevator chains, ropes, belts, and sprockets synced and tensioned; repeated cycles reveal tracking issues that static tests miss.
- Climber ropes must run over pulleys or smooth radii, not sharp metal edges.
- Verify climber torque, brake mode, center of gravity, reaction point, and hardstop strength with the full robot weight.

### Software and Controls

- Keep a working fallback autonomous that can at least achieve the basic mobility objective when complex scoring autos are unavailable.
- Coordinate auto paths with alliance partners before every match, especially in games with midline races or shared zones.
- Test red/blue alliance behavior, field-relative controls, joystick mappings, and sensor-missing cases before competition.
- Disable or remove Xbox Game Bar on driver station laptops; it can interfere with key input and controller behavior.
- Add software power management for combinations of drivetrain and high-current mechanism loads.

### Driver Station and Event Execution

- Plug in the driver station laptop for every match and disable sleep/display-off behavior.
- Velcro or strap the driver station laptop/console to the field shelf with the correct hook/loop side.
- Strain-relieve DS ethernet, USB, and charger cables.
- Use the Driver Station USB tab before matches to verify controller ports, axes, buttons, and mode switches.
- Restart the Driver Station or laptop when stale state, missing controllers, inverted controls, or unexplained enable failures appear.
- Install Windows updates before the event, then pause updates or set active hours so updates cannot run during competition.
- At events, prioritize reliable existing functions over adding major new features.
- If the robot must miss a match, still send a representative to the field for alliance communication and possible points.

---

## Reply-Derived Additions Not Obvious From the Original Posts

- CAD review for stiffness should include offset swerve impacts, not only flat bumper impacts.
- Over-reinforcing an exposed intake can move damage into expensive swerve modules; isolate damage in a replaceable member when practical.
- Battery straps are commonly underbuilt; poor velcro, bungee cords, rope, or no strap at all are repeat event fixes.
- Correctly securing the Anderson connector does not replace battery retention; both are required.
- Some teams prefer velcro loops or bolts for battery connector retention where inspectors object to zip ties.
- Radio issues should be drop-tested with status lights observed; radio power flicker is often caused by loose wiring.
- Hot glue should retain a connector lightly, not bury it; isopropyl alcohol can help release hot glue during service.
- Good SD cards, cloned coprocessor images, and spare storage media prevent vision/coprocessor downtime.
- PDH/PDP debris and metal shavings can create hard-to-debug failures; cover electronics during fabrication and inspect afterward.
- High-strand 4 AWG wire, ferrules beyond rated sizes, or over-twisted conductors can loosen or heat in PDH main terminals.
- Kraken terminal reliability depends on nearby strain relief as much as torque; wires should be neutral and supported close to the motor.
- Driver station controller checks should include axis zero, full travel, button response, controller order, and accidental mode-switch buttons.
- Bumper material surface can affect whether game pieces catch, slide, or roll along the robot.
- Tall elevator issues often come from dynamic cabling, mismatched chain tension, rope tracking, and stage clocking.

---

## Game Archetypes Detected

### High-Contact, Open-Field, Defense-Heavy, or Midline-Race Games

Signals:
- Long unobstructed lanes, high-speed defense, midline races, contact near scoring zones, or protected-zone edge cases.

Checklist implications:
- Reinforce bumpers and primary frame rails.
- Build intakes and front mechanisms as compliant or sacrificial assemblies.
- Pack frame tube, intake roller, side plate, belt, shaft, and bumper spares.
- Inspect swerve modules, shafts, wheels, and battery retention after hard hits.
- Train drivers to retract vulnerable mechanisms before contact.

### Terrain, Bump, Trench, Ramp, or Robot-Under-Robot Games

Signals:
- Repeated vertical shocks, bumps, ramps, trenches, low bars, robots driving under or near deployed mechanisms.

Checklist implications:
- Check swerve shafts, bearings, retaining rings, belts, motor bolts, and wheel damage after terrain use.
- Verify mechanism clearance against field geometry and other robots.
- Protect motors, cameras, radio, RIO, and wiring from side or underside hits.
- Define driver rules for deploying tall hoods, hoppers, arms, and elevators.

### Game-Piece Ingestion or Falling-Piece Games

Signals:
- Game pieces can fall, bounce, shed, or enter the robot from above, the side, or the floor.

Checklist implications:
- Add covers, panels, netting, coreflute, polycarbonate, or surgical tubing around elevators, arms, electronics, and drivetrain openings.
- Test with realistic game-piece drops and bounces.
- Prevent game pieces from pressing the main breaker, hitting sensors, unplugging wires, or jamming belts/chains.

### Tall Elevator, Arm, Wrist, or Climber Games

Signals:
- Large swept volumes, high extension, climbing, multi-stage elevators, long dynamic cable runs.

Checklist implications:
- Treat dynamic cabling as a subsystem with design reviews and match checks.
- Avoid mid-span connectors in moving cable paths.
- Validate chain, rope, belt, and sprocket tracking over repeated cycles.
- Test climber torque, brake mode, center-of-gravity behavior, hardstops, and rope routing under real load.

### High-Current or Battery-Stress Games

Signals:
- Heavy swerve acceleration, frequent pushing, high-load shooters/intakes/climbers, or simultaneous drivetrain and mechanism peaks.

Checklist implications:
- Break in new batteries before events when possible.
- Set current limits on every motor and consider dynamic limits during high-load actions.
- Replace tripped main breakers and investigate hot breakers.
- Track battery health and internal resistance over the season.
- Inspect PDH/PDP terminals and battery leads for heat damage.

### Static, Dust, Foam, Fuzz, or Shedding Game Pieces

Signals:
- Foam, carpet, rubber rollers, dusty balls, residue, or debris that accumulates on cameras/electronics.

Checklist implications:
- Wipe camera lenses between matches.
- Cover unused ports and electronics from debris.
- Bond mechanisms to chassis where legal and appropriate.
- Apply shielding or grounding mitigations only after loose wiring and weak strain relief have been ruled out.

### Auto-Crowding, Shared-Zone, or Path-Conflict Games

Signals:
- Multiple robots want the same lane, centerline object, or scoring zone during autonomous.

Checklist implications:
- Maintain flexible auto options and a working fallback mobility auto.
- Use a pre-match auto negotiation script with alliance partners.
- Name autos clearly by start position and path.
- Verify retract timing and path safety for vulnerable intakes or arms.

---

## Items Intentionally Generalized

- Vendor-specific failures were converted into checks for torque, strain relief, assembly verification, spare parts, and inspection cadence.
- Game-specific objects such as coral, algae, fuel, bumps, trenches, and cages were generalized into ingestion, debris, terrain, static, and clearance archetypes.
- One-off anecdotes were included only when they revealed a repeatable operational control.