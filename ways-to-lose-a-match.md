# Ways to Lose a Match in FRC
## Institutional Memory — Mistakes to Avoid for a Successful Season

*Source: [Chief Delphi — "50+ Fun Ways to Lose a Match"](https://www.chiefdelphi.com/t/50-fun-ways-to-lose-a-match/481954) by jtrv and the Chief Delphi community (595 replies)*

> Every item on this list is something a real team has personally experienced. The little things add up — and the sum of the little things is greater than the sum of the big things.

---

## ⚡ Power & Battery Management

1. **Reuse the same battery back-to-back without charging or rotating.** You're likely to start browning out shortly into the second or third match, preventing effective movement.

2. **Don't secure your battery or its connections.** Skip zip ties on the SB50 battery-to-breaker connection, don't strap the battery to the belly pan, skip nord locks or grasshopper nuts on battery terminals, and use the frayed Velcro strap that's been on the last four robots. A loose battery slides around, breaks sensor pins on your RoboRIO, and causes intermittent electrical failures across multiple matches.

3. **Bring only one battery to an event.** Don't ask anyone to borrow extras. When it drains, just leave.

4. **Don't charge your driver station laptop.** Having it die right as you're about to earn a climb bonus is an unforgettable experience. For maximum effect, leave the charger at the lab.

---

## 🔌 Electrical & Wiring

5. **Expose your main breaker to the outside world.** A robot or game piece can toggle it off mid-match. Also expose it to the inside world — a game piece bouncing around your robot's internals can find its way to the button just as reliably. Using the Optifuse breaker adds extra excitement since its power-off button has a history of breaking. A printable shroud exists; ignore it.

6. **Leave unused RoboRIO and PDH ports uncovered.** Metal shavings accumulate over time as you break and fix things, and eventually something will short.

7. **Make poor wire connections.** Twist wire strands going into lever nuts (results in a shoddy connection prone to pulling out), pull wires from NEO encoder cables, break the RJ45 locking mechanism on ethernet cables, and leave loose CAN wires in the RIO. Any vibration or stiff breeze will cause a comms dropout or haywire behavior.

8. **Force oversized wire into PDH terminals because it "fits enough."** If the clamp cannot reliably hold the conductor through match vibration, that power path can loosen and fail under load.

9. **Use cheap "kit of parts" push-in crimp connectors** instead of proper crimped or soldered connectors. The savings on a crimping tool will be more than offset by time lost diagnosing random disconnects. Using inline Wago connectors is even better — only half-connect some of them and bury them under your mechanisms so random subsystems lose power mid-match and it's impossible to troubleshoot quickly.

10. **Color-code your CAN bus wiring to your team colors** instead of the standard yellow/green. Even better: swap yellow and green every few devices so both colors of magic smoke can mix. CSAs (Control System Advisors) will love helping you.

11. **Don't verify CAN device settings or IDs** after any changes. Let surprises happen mid-match.

12. **Don't set current limits on 550 or 775 class motors.** They'll burn out the moment something gets jammed — like a hand tool left inside the robot.

13. **Wire motors or gearbox motors backwards.** You won't notice until your elevator crashes down because one of three motors is wired in the opposite direction. Alternatively, plug your intake motors backwards after swapping the assembly so the robot pushes game pieces away instead of intaking them — and intakes when you try to score.

14. **Plug two motor controllers (e.g., Spark Maxes) into each other,** frying both. This is equally effective as a weight-reduction strategy.

15. **Leave a Kraken screw in the motor cap** so it can randomly short the CAN loop during a match.

16. **Mount your coprocessor facing downward** in its enclosure so its own weight presses onto its power button and shuts it off.

17. **Use an improperly grounded magnetic encoder** for wrist or arm position on a mechanism that can destroy your drivetrain if it runs past its limits. When it randomly goes haywire, you'll find out exactly how much damage your robot can do to itself.

18. **Exceed gearbox load ratings.** A VersaPlanetary should handle a NEO at 100:1 just fine, right?

19. **Leave the PDH wiring just loose enough** that the RoboRIO constantly reboots throughout a match. The comms will come back eventually.

20. **Drill weight-reduction holes or fabricate parts over your robot without covering motors or electronics.** Metal shavings landing in a Neo Vortex will have you hearing the pit admin announce over the intercom: *"If anyone has a Neo Vortex to spare, (your team number) needs one."*

21. **Leave your CAN bus terminating resistor loose and unprotected.** It will eventually get snagged by a moving mechanism, pulled off the CAN bus, and take your entire CAN network down mid-match.

22. **Replug a popped CAN wire by guesswork and skip diagnostics before the next match.** If the wrong connection is restored or a poor connection remains, you'll discover it only when your robot still has no CAN on the field.

23. **Drill aggressively through your robot for weight reduction without protecting nearby sensors.** Drill right through your NavX pins, replace the board, and then forget to re-calibrate before your first district championship match.

---

## 📡 Communications & Networking

24. **Connect to the venue WiFi — or your personal mobile hotspot.** Your driver station may periodically reconnect to it mid-match, causing a comms dropout at the worst possible moment. Disable all non-field WiFi auto-connect before the event.

25. **Image two radios at the event and power both at the same time.** The pit radio will connect to the field instead of the one on your robot, and you won't move.

26. **Don't check your ethernet cord.** 2024. Bayou Regional. Semifinals. Match 13. Enough said. For bonus points, use a solid copper ethernet cord instead of flat stranded; stranded is far more durable under competition vibration.

27. **Leave the ethernet cable on your radio unsecured.** It will unplug right after autonomous, and you won't be able to move for the rest of the match.

28. **Leave a personal firewall running on your driver station laptop** that occasionally blocks the Driver Station software mid-match.

29. **Leave JVM profiling arguments in your `build.gradle`** from debugging/profiling sessions at the shop. Your data transfer rate will be inexplicably high on the field and it will take CSAs to figure out why.

30. **Open two instances of SmartDashboard.** Your autonomous chooser won't respond, your robot will sit motionless for 15 seconds, and you won't know why.

31. **Drive all of qualifying rounds with a corrupted RoboRIO image.** You'll lose several matches before a CSA finally sorts you out right before eliminations — by seconds.

32. **Play multiple matches with an unknowingly fried radio** that constantly drops connection. Blame the field.

33. **Show up with no radio installed or connected.** Your robot will be perfectly reliable at doing absolutely nothing in every phase of the match.

---

## 🤖 Robot Design & Build Quality

34. **Use acrylic instead of polycarbonate** for structural or lightweight applications. Acrylic shatters under mild stress, leaving your mechanism dysfunctional.

35. **Use lightened 1/16" wall tubing on your drivetrain.** It bends into interesting shapes quickly under competition loads.

36. **Build a robot with a high center of gravity.** Put a fun "oops" decal on the underside so the audience has something to laugh at when you tip over.

37. **Build a turret. Or two.** The more independently rotating axes you add, the more failure points you create under competition stress.

38. **Build a defense-only mecanum robot.** You'll be the talk of the town — just not in the way you intended.

39. **Build a dozer/pusher bot** that scores nothing. Statistically, it outperforms a surprisingly high percentage of teams, but it won't win elims.

40. **Build a whole new robot for Championships** but use all your remaining time building it so you have no time to test.

41. **Refuse to use any COTS (commercial off-the-shelf) components.** It's more thought-provoking to reinvent everything from scratch.

42. **Attach bumpers poorly** — ejectable bumpers are a crowd-pleaser, and a belly pan that splits in two and drags on the floor will disable your robot mid-match just as reliably.

43. **Leave hand tools inside the robot** after pit maintenance. They're conveniently located next to whatever mechanism they'll eventually jam and destroy.

---

## 🔩 Mechanical Assembly & Hardware

44. **Use aluminum gears on your drive motors.** Mid-match grinding sounds are fun, and the audience will definitely notice.

45. **Use plastic gears in critical subsystems.** When they strip, the subsystem simply stops working. Use PLA printed pulleys in intake or shooter mechanisms for the added excitement of having them vaporize when the intake slams into the ground while running.

46. **Fix your swerve modules right before a match and put the wheels in backwards.** It will try to drag the other wheels, leave a rubber pile on the field, and your wheel will be completely bald when you're done. Optionally, leave out a bearing or two.

47. **Use shaft collars? Skip them.** Wrapping tape around both sides of a gear, wheel, or pulley axle will hold just fine. Alternatively, use 3D printed hubs to mount subsystems onto hex shaft — they'll start slipping under load after a few matches.

48. **For loctite, pick one extreme:** either use red loctite everywhere (impossible to remove later), or use no loctite at all (because removing last year's red loctite was too hard). Never use the correct blue loctite. Bonus: applying loctite to fasteners that go into polycarbonate will crack it. Hand-tighten your swerve module bolts instead.

49. **Use 3D-printed plates or brackets** for your main climbing mechanism. They'll cleanly detach when a defense bot hits you, your bumper will drag on the ground, and your climb will be invalidated. They'll also cleanly fail when snagged, allowing you to continue the match with park-only endgame.

50. **Leave a wrench on a hex shaft** before heading to the practice field. The resulting expensive noise is educational.

51. **Forget to glue encoder magnets in.** Dorito-shaped Colson wheels are a natural consequence.

52. **Unplug the RoboRIO while it's updating firmware.** You'll have a very expensive brick, and desperately trying to re-flash it field-side is a great way to get a delay-of-game warning.

53. **Don't secure your SparkMax motor controllers.** Leave bellypan holes uncovered so they can fall through and get ingested by your swerve drives.

54. **Cut wires to whatever random length you have lying around** rather than to the actual needed length. The extra slack will find somewhere interesting to go. Alternatively, embed all your wiring in inaccessible, not-surveyable places inside the robot — you won't be able to diagnose anything quickly at competition.

55. **Zip tie cables next to your zeroing limit switch or beam break, but don't trim the excess zip tie tail.** The protruding tail will trigger the sensor, causing your mechanism to believe it's always at the home position, and it will never travel correctly.

56. **Use a case for your vision coprocessor that doesn't fully enclose the micro SD card slot.** A heavy defense hit will drive the card into your frame rail, shearing it off the PCB. Hypothetically speaking.

57. **Use long, unsupported hex shafts** without a middle bearing. Climbing forces or an unexpected impact will bend them in the middle.

58. **Leave "quick-release" safety pins installed** when deploying telescoping or spring-loaded mechanisms. You'll find out they were still in when you try to use the mechanism in a match and it tangles itself.

59. **Keep your old laptop from the cRIO days** for a driver station. It doesn't matter that the battery holds no charge and the Ethernet port doesn't retain connectors — it's tradition.

60. **Don't grease your swerve module gears** — save the grease for the bearings only. Module gear wear will quietly degrade your drive efficiency and accuracy across an event without an obvious failure.

61. **Ignore pulley-to-polycarbonate clearance and skip spacers.** Let intake or climber pulleys rub until they heat, deform, or melt parts right before playoffs.

---

## 💨 Pneumatics

62. **Don't pre-charge pneumatics before a match.** This saves you from hearing the compressor buzz in the pits. The tradeoff is your pneumatic mechanisms won't work at the start of the match.

63. **Use arts & crafts scissors to cut pneumatic tubing** instead of a proper tubing cutter. The rough, angled cut will cause air leaks and inconsistent actuations.

---

## 💻 Software & Controls

64. **Use lots of `while` loops** in your robot code. Robot timing loops and watchdog timers exist for a reason — ignore them. For extra credit, copy and paste your teleop code as many lines as will fit on the RoboRIO instead of using a loop at all — your robot will stop functioning about 15 seconds before the end of each match when it "runs out of code."

65. **Allow (or schedule) Windows updates on the driver station laptop** during competition. A mid-match OS update is a great way to end things early.

66. **Change your autonomous routine right before a match with zero testing.** That 1 extra potential point is absolutely worth the risk of a broken auto.

67. **Push updated code to the robot while it's queuing** and heading to the field. The resulting code crash will leave your robot motionless for the entire match.

68. **Don't test your auto or aiming code for both alliances.** Your vision and aim code that reliably scores on the Red alliance's target will definitely also work on the Blue alliance — no need to check.

69. **For drivers, don't provide setpoints** — have them manually align every single shot. It builds character.

70. **Change the control layout without telling your drivers.** Communication between software and the drive team is overrated.

71. **Map critical actions to conflicting buttons across controllers.** Put "zero mechanism" and a major drive action on overlapping inputs, then scramble controller order and watch your robot panic.

72. **Keep your drivetrain speed limited to the slow shop-testing speed for competition.** You tuned everything at that speed, so it stays that way.

73. **Never investigate weird software, mechanical, or electrical failures.** It was probably a one-time blip that will never happen again.

74. **Don't improve your robot or code between matches**, even when a small software tweak would make driving significantly easier.

75. **Turn on your field-oriented swerve robot before placing it on the field,** then place it 180° off from your intended heading. Let field orientation do the rest.

76. **Leave your gyro or IMU referenced in code when no physical component is installed.** The swerve code will love you for it.

77. **Let your swerve heading or module state spin constantly and make the driver compensate manually.** If the robot is fighting itself every cycle, keep driving anyway instead of fixing the root cause.

78. **Put a single logical `!` in a critical branch of your swerve code and ship it.** One wrong inversion in heading or module control can make the robot drive the opposite of what the driver commands.

79. **Allow mechanism setpoints that command linked mechanisms into each other.** For example, setting a wrist to go way back into the robot and then immediately elevating to full height. The resulting collision is educational and expensive.

80. **Don't program null handling for sensor disconnects.** If a sensor unplugs mid-match, your code should fail gracefully — not crash, loop uncontrollably, or slam actuators to extreme positions. Similarly, if you unplug a camera or sensor in the pits because it was causing problems, make sure the code handles the missing input cleanly before going back on the field.

81. **Unplug a problematic vision camera between matches without fixing the null case in code.** Unloading the camera solves the comms problem but creates a code crash as soon as it tries to read from the missing device. Test the "camera unplugged" state before putting the robot back on the field.

82. **Run complex path-planning or vision-heavy code on a RoboRIO 1.0.** Its limited RAM and storage will not handle the workload — expect loop overruns, crashes, and bizarre behavior at the worst moments.

83. **Tune your mechanism PID/velocity/acceleration constants and never reverify them under competition load.** Shop-floor tuning on an unloaded mechanism rarely matches match-day performance. Untested constants can cause your elevator or arm to overshoot, oscillate, or strip a belt in a real match.

84. **Revert your code to a previous commit right before a match — but don't verify you reverted to the correct one.** You may end up running a branch that was never intended for match use, producing completely unexpected autonomous behavior.

85. **Ignore Java garbage collection tuning.** A 600ms GC pause during the fastest part of autonomous is a great way to drive your robot into the structure you were supposed to score on.

86. **Don't configure motor soft limits.** Without soft limits, a sensor glitch or operator error can command a mechanism well past its physical travel, destroying belts, gearboxes, or frame elements.

87. **Test your robot at 25% speed and forget to restore full speed before your first match.** Your drivers will wonder why the robot feels like it's driving through sand.

---

## 🎮 Driver Station & Equipment

88. **Don't verify controller port assignments before a match.** If your driver and operator controllers are swapped, just have them switch roles on the fly.

89. **Don't unplug your gamepads between matches.** The Driver Station latches joystick axis values and doesn't zero them — if a stick is drifting at a small value and your drivetrain has joystick control as a default command, the robot will drift during autonomous when no commands are actively controlling the drivetrain.

90. **Forget to plug controllers in before the match and never rescan/reset Driver Station after reconnecting.** Spend teleop troubleshooting USB while your robot sits still.

91. **Keep your driver station laptop nearly closed** to avoid blocking your view. If a robot bumps the DS wall and closes it, re-open it, log back in, and reconnect.

92. **Use old, worn-out hand-me-down controllers and bring no spares.** They worked once.

93. **Leave the charger at the lab.** One fewer thing to carry to the field.

94. **Forget where your controller is between matches; borrow one from another team.** Different controller brands map buttons to different port indices in WPILib — a borrowed Xbox controller replacing your Logitech (or vice versa) will silently scramble every button on your operator's board with no error message.

95. **Don't secure your driver station laptop to the shelf, and don't reboot it between events.** An unsecured laptop slides or falls when a defense bot hits the wall near your station. A laptop that hasn't been rebooted in days will accumulate background processes and thermal throttling that degrade DS responsiveness exactly when you need it most.

---

## 📋 Pre-Match Preparation & Competition Day Logistics

96. **Don't run a pre-match systems check or written checklist.** Humans have great memory, and surprises are exciting. (See also: wrong controllers, uncharged batteries, forgotten pneumatics, reversed bumpers, unplugged controllers, sticky gamepads.)

97. **Stay up late the night before competition** — drivers, operators, and pit crew alike. Sleep deprivation sharpens focus. Let your drivers fall asleep between matches so they miss queuing and the entire match.

98. **Make last-minute robot changes the night before competition** with no time left to verify or test anything. For maximum disruption, do a full robot rebuild the morning of competition so something breaks before your first match.

99. **Give your software team only 2 days to program the entire robot** before competition. That's plenty of time.

100. **Forget spare mechanisms, bumpers, or critical hardware** at the shop or 5 hours away from the competition venue.

101. **Forget to pack critical maintenance supplies** — white lithium grease, spare connectors, spare bolts. You won't need them. (You will need them.)

102. **Use all your superglue on decorative items** before the event so you have none left for actual repairs.

103. **Don't keep track of important match/schedule logistics** — like when your Impact interview is scheduled vs. when you play.

104. **Take your time getting to the field.** Field volunteers can bypass your team if you arrive too late, turning it into a 2v3.

105. **Miss your match because of an Impact interview overlap.** Don't bother asking another team to swap time slots; just skip the match.

106. **Only test your reversible bumpers one way** — with the flap up, never with the flap down where the velcro drags on the floor. ("Why does our robot work great on Red but not move at all on Blue?")

107. **Complete a repair right before a match but leave out a critical component** — a gear, a pin, a bolt. You'll discover what's missing when the mechanism either doesn't work or tries to destroy itself.

108. **Get excited about winning your previous match and forget to repair the damage from it** before your next one.

109. **Don't show up to the match.** A match where your robot isn't on the field is one you can never win — but more painfully, post-match analysis often reveals that simply showing up and running your autonomous routine would have won it.

110. **Let bumper tape come loose before a match.** A piece of tape hanging off a bumper can be ruled by a referee as dragging on the floor or touching a restricted element, invalidating your climb or costing you penalties.

111. **Don't weigh your robot during build season — wait until inspection.** Structural decisions and weight-saving modifications made under last-minute pressure are far more likely to compromise your robot's integrity than planned design choices.

---

## 🤝 Alliance Strategy & In-Match Execution

112. **Drive into your alliance partner during autonomous.** It demoralizes both teams and is a great way to lose two robots' worth of points in the first 15 seconds.

113. **Drive into your opponents' zone during autonomous** instead of executing your planned strategy.

114. **Dominate the pre-match alliance strategy discussion.** Interrupt your alliance partners repeatedly, because you're SURE your idea is better and your robot is better than everyone else's. Never listen.

115. **Ignore your alliance partners during a match.** Your task is always top priority, even if it means blocking their access to a critical field element for half the match. Don't talk to them before the match, either.

116. **Don't track the time remaining in a match.** Strategy never needs to adjust based on the number of seconds left.

117. **Don't adjust strategy mid-match, even when the situation changes.** Rigid adherence to the original plan is a virtue.

118. **Skip the climb / endgame bonus** to chase that last cycle. You'll miss the big point swing and slightly improve your cycle average in scouting data.

119. **Play completely passive — move slowly and politely yield to opponents at all times.** Never contest anything.

120. **If your robot starts malfunctioning and appendages are flailing, go play defense.** Sharing the chaos seems fair.

121. **Keep working on your climb mechanism during the entire event** rather than testing other parts of the robot. It'll work eventually.

122. **Play defense with more than one robot simultaneously** — and make sure to hit opponents in restricted field zones. Nobody can outscore the volume of major fouls that generates.

123. **Don't read the game manual.** Get penalized for rule violations you didn't know existed throughout the entire event.

124. **Hit E-Stop instead of A-Stop when your robot goes the wrong way in autonomous.** The E-Stop disables the robot for the remainder of the match; A-Stop only pauses auto. These are very different buttons.

125. **Score game pieces in your opponents' scoring zone** by mistake. Great way to give them free points.

126. **Park a few inches outside the scoring zone** at the end of the match when you're down by exactly one point.

127. **Mix up your intake and outtake button assignments.** Having your operator accidentally push game pieces away instead of picking them up builds tension.

---

## 🔍 Scouting & Alliance Selection

128. **Don't scout any matches.** Flying completely blind into alliance selection is a bold strategy.

129. **Pick your friends in alliance selection** regardless of their robot's actual performance or capability.

130. **Pick the lowest-numbered shiny powder-coated robot** if none of your friends are available. It looks fast.

131. **Pick a robot because one person on your team said it played well once.** No scouting data, no match video — vibes are sufficient.

132. **Don't talk to or introduce yourself to high-ranked teams** at the event. Relationships and pre-selection scouting conversations are unnecessary.

133. **Choose an alliance partner without a working CAN bus** and expect them to contribute meaningfully.

134. **Trust promises that a custom scouting app will be ready before competition.** It will definitely be done in time. Plan your entire scouting workflow around it.

135. **Do lots of pit scouting** — walk to every single pit and fill out clipboards — then never actually use any of that data for strategy decisions.

136. **Have inexperienced freshmen plan all of scouting with no oversight.** They'll figure it out.

137. **Never verify what your alliance partners claim they can do.** Base your entire alliance strategy on their promises without ever watching them play or asking follow-up questions.

---

## 🏗️ Build Process & Team Management

138. **Give design all the build time.** Software won't have to do much, and the drive team doesn't really need to know what the buttons do anyway.

139. **Send only a human player to a match** because your robot isn't ready, isn't repaired, or wasn't built with quick serviceability in mind. Your alliance partners and scouting teams definitely won't notice.

140. **Build a shooter powered by two motors and never verify that both are plugged in.** Discovering that one was disconnected for two entire regionals and half of Champs is a great story.

141. **Ignore your drive team's physical needs.** Make sure they don't have time to eat — especially if someone on the team is diabetic. A drive team operating under stress and hunger at a multi-day event is peak performance.

142. **Have no drive team backups or replacements.** Your primary driver and operator should be constantly stressed, with nobody available to step in if there's an emergency.

143. **Don't give your human player any practice time.** They'll figure it out under match pressure.

144. **When something breaks, always blame the other subteam** — if a mechanical change was just made, it's definitely a software problem; if a software change was just made, it's definitely mechanical. This will simultaneously teach everyone about the other subteam's domain while making everyone hate each other, and the actual root cause will go unresolved.

145. **Don't practice with the robot.** Competition driving is a skill — your drivers need deliberate practice time on a real field setup to develop spatial awareness, reaction time, and the muscle memory to execute strategy under pressure. Sending untrained drivers into a match is like entering a race having only read about how to drive.

---

## Key Takeaways for a Successful Season

| Category | Action Items |
|---|---|
| Battery | Rotate and charge every match; zip-tie SB50; strap battery down; use nord locks on terminals; bring multiple batteries |
| Electrical | Cover unused ports; use proper connectors; set motor current limits; standard CAN color codes; verify all wiring is accessible; secure terminating resistors; protect sensors from drill debris |
| Communications | Disable venue WiFi and hotspot auto-connect; power only the robot's radio; use stranded ethernet cord; verify RoboRIO image integrity |
| Build | Polycarb not acrylic; proper wall tubing; low CoG; test both alliance colors; trim zip tie tails near sensors; track robot weight throughout build season |
| Software | Test every auto change; verify both alliance modes; communicate control changes to drivers; null-handle all sensor inputs; configure motor soft limits; restore full speed after testing; verify git commit before matches |
| Mechanical | Use correct loctite (blue); shaft collars; secure all motor controllers; middle bearings on long shafts; cover motors when drilling; grease swerve gears and bearings |
| Pre-Match | Written systems checklist; arrive at field early; carry spare controllers and charger; unplug gamepads between matches; pack grease and spare hardware; inspect bumper tape; show up to every match |
| Competition Day | Sleep; manage schedule; bring spare mechanisms and bumpers; test reversible bumpers both ways; complete repairs before celebrating; secure and reboot driver station laptop |
| Strategy | Coordinate with alliance partners; track match time; prioritize endgame; adjust plans mid-match; read the game manual |
| Scouting | Scout every match; use data — not feelings — for alliance selection; talk to top teams early; verify partner capabilities |
| Team | Feed your drive team; have backups for all drive team roles; investigate failures cross-subteam instead of blaming; practice driving deliberately |
