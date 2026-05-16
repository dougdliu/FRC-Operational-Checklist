# Ways to Win a Season in FRC
## Institutional Memory — Best Practices for a Successful Season

*The antithesis of [Ways to Lose a Match](ways-to-lose-a-match.md) — distilled from hundreds of real team experiences on Chief Delphi*

> Winning a season isn't one big thing. It's eliminating the small failures — consistently, match after match, event after event.

---

## ⚡ Power & Battery Management

1. **Rotate and track batteries every match.** Number every battery, log its last charge and last match used, and always queue with a freshly charged one. A healthy battery is the single most reliable performance upgrade you can make.

2. **Secure every connection on every battery.** Zip-tie the SB50 connector to the breaker so it cannot be pulled free. Strap the battery to the belly pan. Use nord locks or nyloc nuts on all battery terminals. Inspect every battery before each event.

3. **Bring 4–6 batteries to every event.** Borrow from neighboring teams at bag-and-tag if needed. Never be the team hunting for a battery in the queue line. Rotate a full set through a charger at all times.

4. **Keep driver station laptops on a charger** whenever not in a match. Bring the charger to every event in the pit bag, not at the shop.

---

## 🔌 Electrical & Wiring

5. **Cover your main breaker with a printed shroud.** A game piece or robot arm should never be able to switch your robot off mid-match. Replace the Optifuse breaker if your team uses one.

6. **Cover all unused RoboRIO and PDH ports with tape or caps.** Do this before every event. Check for metal shavings in and around the electronics bay after every drilling or fabrication session.

7. **Use proper wire termination everywhere.** Ferrules on lever-nut wires, properly seated RJ45 connectors with boots, strain relief on all cable runs. Tug-test every connection before each event.

8. **Match wire gauge and ferrules to PDH terminal limits, then tug-test every high-current connection.** A connection that only "kind of fits" in the pit will not survive full-match vibration and current spikes.

9. **Invest in a quality wire crimping tool and use it.** Properly crimped connections are vastly more reliable than push-in connectors under vibration. Solder and heat-shrink critical connections.

10. **Use standard CAN bus wiring colors** — yellow and green — throughout the entire robot. Label every device. Make it trivial for a CSA or a fresh team member to trace the CAN chain.

11. **Verify all CAN device IDs and firmware versions** after any change, every time. Keep a wiring diagram and a CAN device list in your pit binder.

12. **Set current limits on every motor controller,** especially NEOs, 550s, and 775s. Know the stall current of every motor in your system. Design to never reach it.

13. **Verify motor wiring polarity on all multi-motor mechanisms** before any powered test. Run each motor individually on the bench before combining them.

14. **Never plug motor controllers into each other.** Route and label every cable before powering on. A 5-minute labeling session prevents a $200 mistake.

15. **Leave no loose hardware near CAN devices.** After any work in the electronics bay, do a visual sweep for stray screws, bolts, and shavings.

16. **Mount vision coprocessors securely** with the SD card slot accessible, supported, and away from any impact zone. A sheared SD card kills your vision system for the event.

17. **Understand your encoder grounding.** Magnetic encoders on rotating mechanisms should have their ground verified before any powered test. A floating ground on a wrist encoder will eventually cause a catastrophic movement.

18. **Verify all gearbox selections against rated load.** Check the VersaPlanetary (or equivalent) load ratings for every stage combination. Size up if in doubt.

19. **Make all wiring accessible and surveyable.** Lay it in open cable trays, use consistent routing, and leave service loops at every connector. If you can't see it, you can't fix it under time pressure at competition.

20. **Zip-tie every CAN bus terminating resistor to a hard mounting point** away from all moving mechanisms. The resistor is tiny and easy to overlook, but losing it during a match will take down your entire CAN network instantly.

21. **After any CAN repair, run a full diagnostics pass before your next match.** Verify bus health on the bench, confirm every device appears in telemetry, and shake-test suspect runs before queueing.

22. **Protect all sensors and electronics during any drilling, grinding, or cutting session.** Use foam, tape, or a physical shield over sensors, encoders, and coprocessors. A single metal shaving in a NavX accelerometer or drilled through its PCB means replacing it — and then recalibrating from scratch.

---

## 📡 Communications & Networking

23. **Disable all non-FMS WiFi connections on the driver station before each event.** Use the FRC Driver Station's "disable WiFi adapter" feature, or manually forget all saved networks. Test it.

24. **Power only one radio at a time per team number.** Immediately after programming a second radio, label it and power off the first. Never run two simultaneously.

25. **Use high-quality stranded copper flat ethernet cord** for all robot ethernet connections. Stranded wire flexes without breaking under constant vibration; solid copper will eventually crack. Replace robot ethernet cables every season.

26. **Secure the ethernet cable at both ends with a retaining clip or strain relief.** A disconnected radio cable is an invisible, instant loss.

27. **Ensure the driver station firewall is completely disabled** for the DriverStation.exe process — or disable the Windows firewall entirely on the competition laptop. Verify in a practice match.

28. **Remove all profiling JVM arguments and debugging flags from your build.gradle** before competition. Keep a competition build config separate from a development config.

29. **Use one SmartDashboard/Shuffleboard instance per driver station.** Close all others before the match. Confirm your autonomous chooser responds correctly in every pre-match systems check.

30. **Verify your RoboRIO image version** at the start of every event using the roboRIO Imaging Tool. A corrupted image is a quiet killer — it causes subtle errors that are hard to diagnose under pressure.

31. **Know your radio's status.** If you're having unexplained communication dropouts, ask a CSA to check your radio health immediately. Don't burn multiple qual matches on an undiagnosed radio problem.

32. **Carry and pre-test at least one configured spare radio.** Before every match, verify a powered radio is physically installed, connected, and linked to the correct robot.

---

## 🤖 Robot Design & Build Quality

33. **Use polycarbonate, not acrylic,** for structural panels, guards, and covers. Polycarb flexes rather than shattering. Buy a sheet at the start of build season and keep it on hand.

34. **Use at least 1/8" wall tubing on your drivetrain** and primary structure. The weight savings on thinner tube is not worth the structural risk in a contact game.

35. **Design for a low center of gravity** from the start. If your robot has any chance of tipping, add outriggers, extend your wheelbase, or lower your heavy components before competition.

36. **Limit complexity to what your team can build, program, and repair reliably.** A well-executed two-degree-of-freedom robot beats a three-DOF robot that breaks every other match. Add complexity only when the simpler version is rock solid.

37. **Prototype multiple designs before committing.** The design that looks worst on a whiteboard often outperforms the elegant one on the field.

38. **Use proven COTS components** wherever they exist. COTS swerve, COTS intakes, and COTS climbers have been tested by hundreds of teams. Your engineering time is better spent on your robot's unique scoring mechanism.

39. **Build bumpers that attach and detach in under 90 seconds.** Use a consistent, proven bumper bracket system. Test them before and after every event, and in both alliance color orientations.

40. **Design the robot to be serviceable.** Every mechanism should be reachable, removable, and replaceable with common tools in under 10 minutes. You will need to fix things fast at competition.

---

## 🔩 Mechanical Assembly & Hardware

41. **Use steel gears on drive motors and in high-torque applications.** Aluminum gears are lighter but wear faster under load. Know when each material is appropriate.

42. **Use appropriate materials for game piece contact mechanisms.** Hard plastics and metals for structure; compliant wheels and polyurethane for intake rollers. PLA melts; PETG and Nylon hold up far better under sustained load.

43. **Before every match, verify that all wheels are oriented correctly** after any swerve module service. Confirm module rotation directions with a quick manual test before queuing.

44. **Use shaft collars on all rolling or rotating elements.** A shaft collar is a 5-cent part that prevents a 50-dollar repair.

45. **Use blue Loctite (243) on all critical fasteners.** Red loctite is nearly permanent — use it only where disassembly is never intended. Never apply loctite to fasteners threading into polycarbonate.

46. **Use steel-backed or aluminum-backed 3D prints in structural applications.** 3D printed parts are excellent for geometry and weight, but should not be the sole structural member in any load-bearing or impact-absorbing joint.

47. **Put a middle bearing on any unsupported hex shaft over 6 inches.** Climbing forces and field collisions will bend unsupported shafts. A bearing mid-span eliminates this failure mode entirely.

48. **Clear the robot interior before every powered test** and before leaving the pit for a match. Any tool left in the robot will find the worst possible mechanism to jam.

49. **Glue encoder magnets permanently.** Use CA glue or epoxy. Verify magnet position every event. A detached magnet turns position-controlled mechanisms into uncontrolled chaos.

50. **Never unplug a RoboRIO during a firmware update.** If this happens, have the recovery reflash procedure memorized and a laptop with the imager ready in the pit.

51. **Physically bolt SparkMax and other motor controllers to the frame** using mounting tabs. They should not be able to move, rotate, or fall through any opening.

52. **Route wires to appropriate lengths** — long enough for service loops, short enough to not tangle in mechanisms. Use velcro ties for main cable runs so they can be adjusted or removed.

53. **Trim all zip tie tails flush** immediately after installation. An untrimmed tail near a limit switch, beam break, or encoder will trigger false readings and cause mechanism failures.

54. **Use stranded coaxial or shielded cable** for encoder and sensor runs on high-vibration mechanisms.

55. **Support vision coprocessor micro SD cards** by mounting the coprocessor so the card is against a hard surface, or use a card with a retention latch and add a mechanical stop.

56. **Grease swerve module gears at every event, not just the bearings.** Gears run dry will wear faster and degrade steering accuracy across an event without an obvious single-point failure. Keep white lithium grease in your pit kit and apply it during your event setup.

57. **Check pulley and wheel clearances against polycarbonate and frame members** after every repair. Add spacers and guards where needed, then spin-test under load to confirm no rubbing, heat buildup, or plastic welding.

---

## 💨 Pneumatics

58. **Pre-charge your pneumatics in the pit** before every single match. Make "check air pressure" a line item on your pre-match checklist. Your solenoids don't work well at 0 PSI.

59. **Use a proper pneumatic tube cutter** for all tubing cuts. A clean, square cut seats properly in push-in fittings. An angled cut will leak at exactly the worst possible moment.

---

## 💻 Software & Controls

60. **Never use blocking `while` loops inside robot periodic methods.** Use WPILib's command-based scheduling or state machine patterns. Every subsystem should cooperate with the watchdog and never starve the main loop.

61. **Create a "competition mode" build configuration** with all profiling tools, extra logging, and debug output stripped out. Deploy only this build at events.

62. **Test every autonomous routine change before deploying it at competition.** A single untested auto change can eliminate an entire match's worth of points. Use a backup auto that always works.

63. **Push all code to the robot during pit time — never on the way to the field.** Set a rule: no code changes within 15 minutes of queuing. Verify the robot is connected and running your intended code after every push.

64. **Test all code on both Red and Blue alliance.** Vision targeting, field-relative odometry, and auto routines must all be verified for both. Keep both tested and named in your routine chooser.

65. **Use software setpoints and automation for repeatable tasks.** Drivers should hit one button to score, not manually position every mechanism. Setpoints reduce cognitive load and increase cycle speed.

66. **Communicate all control layout changes to the entire drive team before the event.** Update your driver reference card. Practice the new layout until it's muscle memory.

67. **Separate critical control functions and lock controller order.** Never share overlapping bindings between reset/zero and high-impact drive actions. Validate mappings after every reconnect.

68. **Set drivetrain speed and acceleration limits appropriate for competition.** Test at full speed before your first match. Drivers need to know how the robot behaves at full throttle.

69. **Treat every "one-time" anomaly as a real failure.** Log it, reproduce it, and fix it. The failure that happened once at practice will happen again during a critical elimination match.

70. **Improve code between matches when there's time.** Fix known issues. Deploy and test during practice matches. A robot that's 10% better in match 3 than match 1 matters over a full event.

71. **Zero your field-oriented heading on the field, not in the pit.** Place the robot, then press the zero button. Repeat if the robot is moved.

72. **Treat persistent swerve spin or heading drift as a no-go fault, not a driver problem.** Disable field-oriented mode if needed, diagnose the module/IMU issue, and clear it before the next match.

73. **Protect critical swerve logic with code review, unit tests, and driver-direction sanity checks.** A one-character inversion in heading logic can fully reverse control intent and should be caught before deployment.

74. **Add a physical gyro/IMU and use it.** If it's in the code, it should be on the robot. If it's not on the robot, comment it out. Mismatches cause silent, hard-to-diagnose failures.

75. **Add software limits and safeties to all mechanisms** that can harm themselves or the robot. A wrist that can't command itself into the elevator, and an elevator that can't extend through the frame, prevents expensive repairs at 3pm on Saturday.

76. **Program explicit null handling for every sensor your code reads.** A camera that unplugs, a beam break that gets damaged, or an encoder that loses signal should produce a known safe state — not a code crash. Test the “sensor missing” case deliberately before competition.

77. **Reverify all mechanism PID constants and motion profiles after any physical repair or replacement.** A new belt, a different-weight game piece, or a repaired gearbox can change the dynamics of a mechanism enough to make previously-safe constants dangerous.

78. **Tag every competition-ready commit in your git repository.** Before each match, verify the build hash on the robot matches your tagged release. Accidentally deploying a development branch mid-event is a silent, hard-to-diagnose problem.

79. **Restore full competition speed and all motion limits before every event.** Create a checklist item for it. Testing at 25% speed and then forgetting to reset is one of the most common causes of unexpectedly “sluggish” match performance.

---

## 🎮 Driver Station & Equipment

80. **Run a full controller check at the start of every event day.** Verify port assignments, axis directions, and button mappings before the first match. Keep a printed reference card in the driver station box.

81. **Unplug all gamepads between matches.** When you plug them back in before a match, verify that all axes are at zero with the sticks centered before enabling. A drifting axis will interfere with autonomous.

82. **If a controller reconnects late, immediately rescan and verify mapping in Driver Station.** Practice this recovery drill so the drive team can recover in seconds instead of losing a full teleop period.

83. **Keep the driver station laptop open and elevated** so it doesn't close during a match. A stable, flat surface is ideal.

84. **Invest in quality controllers and bring two full sets as spares.** Know which controller your driver prefers and have a tested backup ready. Worn thumbsticks are a competitive liability.

85. **Keep the charger in the pit bag — always.** Label it with your team number. Charge after every match.

86. **Standardize to a single controller brand and model across your entire drive team.** Keep tested spares of the same model. Swapping to a borrowed controller of a different brand will silently remap every button with no error — and no time to fix it in a queue line.

87. **Secure your driver station laptop to the shelf with a strap or velcro,** and reboot it at the start of every competition day. An unsecured laptop slides off when a defense robot hits the field wall. A laptop with weeks of uptime accumulates background processes that degrade DS performance at the worst times.

---

## 📋 Pre-Match Preparation & Competition Day Logistics

88. **Maintain a written pre-match checklist and run it before every match.** Include: battery swapped and seated, controllers plugged in and assigned, radio on, bumpers secure, mechanisms zeroed, auto routine selected and confirmed, driver/operator positions confirmed.

89. **Prioritize sleep for your entire team** — especially drive team. Performance degrades sharply under sleep deprivation. Set a hard "everyone in bed" time the night before competition.

90. **Freeze robot changes 24 hours before competition.** Anything done the day before must be tested that same day. Anything done after that is a known risk.

91. **Give your software team meaningful development time** — at least two full practice weeks on the completed robot. Code developed in two days and never tested will fail in interesting ways at competition.

92. **Bring dedicated spare mechanisms for your highest-failure-risk subsystems.** The intake that jams most often at practice should have a replacement ready to bolt in.

93. **Pack a pit supplies checklist** and take it seriously: spare connectors, ferrules, loctite (blue), zip ties, white lithium grease, spare bolts and nuts in common sizes, extra ethernet cable, spare battery, spare controllers. Restock after every event.

94. **Keep a team calendar with all competition events and conflicts overlaid.** Impact interviews, skills challenges, and match schedules must all be visible. Assign someone specifically to manage the day-of schedule.

95. **Be at the field queue 5 minutes early, every time.** Field staff will skip teams that aren't ready. A 2v3 is an avoidable loss.

96. **Schedule your Impact interview far from your expected match times.** Request a swap early if there's a conflict. The match and the interview both matter — don't sacrifice either.

97. **Test reversible bumpers in both orientations** before every event. Walk the robot on carpet with the bumper flap down. If it drags, fix it.

98. **Do a complete robot systems check before your first match of each day.** This is separate from the pre-match checklist — a longer, thorough check: all subsystems actuate, auto runs correctly, drive team confirms controls.

99. **After any repair, verify the fix before leaving the pit.** Run the mechanism through its full range of motion. Confirm nothing is missing — a gear left out is invisible until the mechanism doesn't work at all.

100. **Show up to every match, even when your robot isn't working perfectly.** A damaged robot running autonomous alone can swing enough points to matter. A robot that isn't on the field contributes zero. Always queue.

101. **Inspect all bumper tape before every single match.** A piece of tape hanging loose can drag on the floor, touch a scoring element, or violate bumper rules — any of which can invalidate a climb or result in a penalty. 30 seconds of inspection prevents a heartbreaking referee call.

102. **Track your robot's weight throughout build season, starting with the drivetrain.** Set a budget for each subsystem and weigh as you build. Arriving at inspection overweight with no time to fix it is an entirely avoidable crisis.

---

## 🤝 Alliance Strategy & In-Match Execution

103. **Establish auto collision zones before every match.** In your alliance strategy meeting, map out where each robot will be during auto and ensure no paths cross. Two autonomous robots running into each other costs both teams.

104. **Define autonomous priority rules** — if only one robot should occupy a zone, agree on it beforehand. Respect the plan in the match.

105. **Listen fully in alliance strategy meetings.** Every robot on your alliance has a perspective on what it can and can't do. Let each driver finish before responding. A collaborative alliance outperforms a dominant one.

106. **Communicate with alliance partners during the match** as much as the game allows. Eye contact, body language, and pre-agreed signals matter.

107. **Track the match clock actively.** At 30 seconds remaining, begin endgame sequencing. At 20 seconds, be in position. Know exactly when your robot needs to start climbing or parking.

108. **Have a Plan B auto and a Plan B teleop strategy ready** for when something breaks. If your primary scoring mechanism fails, know immediately what your robot can still do and execute it well.

109. **Prioritize endgame points.** Climbing/docking bonuses are often worth more than one additional cycle. Calculate the expected point value before choosing to skip endgame.

110. **Play purposeful defense only.** Interference should be intentional, rule-compliant, and coordinated with your alliance. Passive drifting or accidental bumping into opponents generates fouls.

111. **Read the game manual every season.** All of it. Know the penalty structure. Know what constitutes a major foul. The team that avoids 5 penalty points is 5 points ahead.

112. **Know the difference between E-Stop and A-Stop.** E-Stop disables your robot for the rest of the match. A-Stop pauses autonomous mode only. Map A-Stop to your most accessible button; E-Stop should require deliberate action.

113. **Know exactly where the scoring zone boundaries are.** Parking a few inches outside during a close match is a precision error that practice eliminates.

114. **Track game piece possession and scoring during the match.** Know the score differential at all times so you can make smart tradeoffs between cycles, defense, and endgame.

---

## 🔍 Scouting & Alliance Selection

115. **Scout every qualification match.** Assign at least two scouts per match. Build a consistent, structured data collection form and stick to it across all events.

116. **Use data, not feelings, for alliance selection.** Quantify scoring, defense, reliability, and endgame. Rank all teams before captain order opens. Update rankings with late-match changes.

117. **Pick the best robot for your alliance's needs** — not your friends. Be honest about capability gaps and fill them. A robot that does what you can't is more valuable than a robot that does what you already do.

118. **Watch match video** for every robot you seriously consider picking. Video catches things scouting sheets miss — defense susceptibility, cycle consistency, auto reliability.

119. **Introduce yourself to top-ranked teams early in the event.** Learn their capabilities, share yours. Alliance selection conversations that happen before the final rankings are more productive than cold calls under time pressure.

120. **Confirm what your picked alliance partners can actually do.** Ask specific questions, watch their matches, and build your strategy around demonstrated capability — not what they claim.

121. **Have a scouting lead who owns the system end-to-end.** Someone who knows the data, can answer questions in the selection queue, and can update strategy on the fly. Scouting without accountability produces unused data.

122. **Make your scouting system failure-tolerant.** Paper backups for digital systems. Two scouts for every match so a bathroom break doesn't leave a gap. Redundancy matters in a noisy, chaotic competition environment.

---

## 🏗️ Build Process & Team Management

123. **Protect programming time.** Software needs the completed robot for a minimum of two full weeks before competition. Plan robot completion accordingly. Code written on a half-built robot or in two days will break.

124. **Design for serviceability from day one.** If you can't replace or repair a mechanism in 10 minutes at a pit table, redesign its mounting. The robot that comes back from the field in worst shape needs the fastest repair.

125. **Build a shooter (or any multi-motor mechanism) and verify every motor is connected and running in the correct direction** before ever testing the full mechanism at speed.

126. **Feed your drive team.** Schedule food breaks. Have snacks in the pit for between-match windows. A driver who hasn't eaten in 6 hours is making worse decisions. Double this if anyone on the team has dietary needs that affect alertness.

127. **Have at least one trained backup driver and one trained backup operator.** They should practice regularly throughout the season. At Worlds, injuries happen, emergencies happen — you need someone ready.

128. **Give your human player dedicated practice time** with real game pieces. The HP is a scored role with a significant point contribution. Treat their skill development as seriously as driver practice.

129. **Diagnose failures as a cross-functional team.** When something breaks, bring mechanical and software people to the same table. Most failures at competition have both a mechanical root cause and a software symptom, or vice versa. Blame delays diagnosis; curiosity fixes it.

130. **Drill weight-reduction holes on a dedicated fabrication bench** away from all electronics. Use a vacuum or cover all nearby components. Metal shavings in a motor or CAN device are a time-consuming and expensive repair.

131. **Schedule deliberate, structured drive practice sessions throughout build season** — not just “driving around”, but timed match simulations with all game elements, a human player, and match-realistic pressure. Competition driving skill is built through repetition; it cannot be improvised on match day.

---

## Key Practices for a Successful Season

| Category | Habit to Build |
|---|---|
| Battery | Numbered rotation system; 4+ batteries per event; always on charger |
| Electrical | Weekly wiring inspection; tug-test all connections; standard CAN colors; accessible routing; secure CAN terminators; protect sensors during machining |
| Communications | Disable venue WiFi; one radio at a time; stranded ethernet; verify RoboRIO image at every event |
| Build | Polycarb over acrylic; serviceable design; COTS where proven; build to repair in <10 min; track robot weight throughout build |
| Software | No while-loops in periodics; competition build config; test both alliances; setpoints for drivers; null-handle all sensors; tag competition commits; verify deployed speed settings |
| Mechanical | Shaft collars everywhere; blue loctite; trim zip ties; bearing mid-span; secure all motor controllers; grease swerve gears every event |
| Pre-Match | Written checklist (run every match); unplug gamepads between matches; arrive 5 min early; inspect bumper tape; always queue even when damaged |
| Competition Day | Enforce sleep; freeze changes 24h out; verify repairs fully before leaving pit; reboot and secure DS laptop |
| Strategy | Alliance meeting before every match; track the clock; prioritize endgame; read the manual |
| Scouting | Scout every match; data drives selection; watch video; verify partner capabilities |
| Team | Feed drive team; cross-subteam debugging; backup drivers trained; HP gets practice time; schedule deliberate drive practice |
