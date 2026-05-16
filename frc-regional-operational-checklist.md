# FRC Regional Operational Checklist

This markdown version mirrors the team-facing regional checklist being maintained in Google Docs.

If anything here conflicts with the current **FIRST Game Manual**, the **official inspection checklist**, inspectors, or field staff, follow the official source.

## Table of Contents

1. [T-7 Pre-Regional Prep](#t-7-pre-regional-prep)
2. [T-1 Final Readiness Check](#t-1-final-readiness-check)
3. [Load-In and Setup](#load-in-and-setup)
4. [Inspection Calibration and Practice Day](#inspection-calibration-and-practice-day)
5. [Event Day Start](#event-day-start)
6. [Pre-Match and Queue](#pre-match-and-queue)
7. [System Check](#system-check)
8. [Match Operating Rules](#match-operating-rules)
9. [Immediate Post-Match](#immediate-post-match)
10. [Match Review](#match-review)
11. [Repair Recovery and Ready for Next Match](#repair-recovery-and-ready-for-next-match)
12. [Alliance Selection Transition](#alliance-selection-transition)
13. [Playoffs and Elims Cycle](#playoffs-and-elims-cycle)
14. [Pack-Out and Event Closeout](#pack-out-and-event-closeout)
15. [D+1 Post-Event Breakdown](#d1-post-event-breakdown)
16. [D+2 Retrospective and Lessons Learned](#d2-retrospective-and-lessons-learned)
17. [No-Go Conditions](#no-go-conditions)
18. [Rationale and Sources](#rationale-and-sources)

---

## T-7 Pre-Regional Prep

- Confirm travel roster, pit roles, drive team roles, and primary backups. [Why](#why-t-7-pre-regional-prep)
- Review the event agenda, load-in rules, inspection timing, practice windows, and awards schedule. [Why](#why-t-7-pre-regional-prep)
- Run a game-archetype risk review and decide which durability, wiring, auto-conflict, and battery risks apply this season. [Why](#why-t-7-pre-regional-prep)
- Build the spare-parts plan for bumpers, intake wear parts, drivetrain wear parts, wiring repairs, and driver-station failures. [Why](#why-t-7-pre-regional-prep)
- Verify the driver station laptop image, required software, controller mappings, and update policy. [Why](#why-t-7-pre-regional-prep)
- Define the release, rollback, and fallback-auto plan for the event. [Why](#why-t-7-pre-regional-prep)
- Confirm inspection readiness items early: bumpers, weight budget, numbers, serviceability, and access to required mechanisms. [Why](#why-t-7-pre-regional-prep)

## T-1 Final Readiness Check

- Charge, label, and stage match-ready batteries; separate questionable batteries from the ready pile. [Why](#why-t-1-final-readiness-check)
- Run a full fastener, wiring, bumper, and strain-relief audit on the robot. [Why](#why-t-1-final-readiness-check)
- Verify main-breaker protection, battery retention, battery connector retention, and radio/ethernet strain relief. [Why](#why-t-1-final-readiness-check)
- Check dynamic cable paths, encoder zeros, camera cleanliness, and swerve wear items. [Why](#why-t-1-final-readiness-check)
- Pack the pit, consumables, chargers, field-shelf velcro, spare controllers, and logging tools. [Why](#why-t-1-final-readiness-check)
- Rehearse the queue workflow, pit repair workflow, and post-match logging workflow with the actual people assigned to those jobs. [Why](#why-t-1-final-readiness-check)
- Freeze risky feature work and keep only tested code paths for the event build. [Why](#why-t-1-final-readiness-check)

## Load-In and Setup

- Set the pit layout first: batteries, chargers, tools, repair space, admin area, and walkways. [Why](#why-load-in-and-setup)
- Check the robot for transport damage before the first powered test. [Why](#why-load-in-and-setup)
- Stage the most-used repair items where they can be reached quickly during match turnaround. [Why](#why-load-in-and-setup)
- Confirm the driver station shelf kit is complete: laptop retention, charger, ethernet, controller cables, and backup controller. [Why](#why-load-in-and-setup)
- Review event-specific field flow, inspection flow, pit admin expectations, and any site restrictions. [Why](#why-load-in-and-setup)

## Inspection Calibration and Practice Day

- Present the robot in an inspection-friendly state with accessible hardware, legal bumpers, clear numbers, and serviceable covers. [Why](#why-inspection-calibration-and-practice-day)
- Resolve inspection findings immediately and log any recurring failure modes the team learns during inspection. [Why](#why-inspection-calibration-and-practice-day)
- Re-zero steering, absolute sensors, and any match-critical mechanism calibration before practice matches. [Why](#why-inspection-calibration-and-practice-day)
- Validate autonomous routines on both alliance colors and confirm the fallback auto still works. [Why](#why-inspection-calibration-and-practice-day)
- Use practice time to test the whole match cycle: queue, controls, pathing, recovery after contact, and pit turnaround. [Why](#why-inspection-calibration-and-practice-day)

## Event Day Start

- Reboot the driver station laptop and verify power settings, sleep behavior, and startup apps. [Why](#why-event-day-start)
- Confirm the Driver Station software version, controller order, cable strain relief, and charger connection. [Why](#why-event-day-start)
- Check the first-match battery rotation plan, match schedule, scouting assignments, and pit coverage. [Why](#why-event-day-start)
- Inspect the robot for overnight loosening, damage, dirt, debris, and camera obstruction. [Why](#why-event-day-start)
- Make sure the currently loaded robot software matches the intended match release and rollback plan. [Why](#why-event-day-start)

## Pre-Match and Queue

- Install the correct charged battery and verify both battery retention and connector retention. [Why](#why-pre-match-and-queue)
- Confirm the selected autonomous mode, alliance-color assumptions, and expected starting position. [Why](#why-pre-match-and-queue)
- Negotiate autonomous paths and opening responsibilities with alliance partners before entering the field. [Why](#why-pre-match-and-queue)
- Check bumpers, numbers, tape, fabric, brackets, and color before leaving the pit. [Why](#why-pre-match-and-queue)
- Verify controller state, controller order, DS charger, ethernet seating, and any match-specific control changes. [Why](#why-pre-match-and-queue)
- If the previous match involved heavy contact or terrain hits, do a quick drivetrain and exposed-mechanism inspection before queueing. [Why](#why-pre-match-and-queue)

## System Check

- Run a quick enabled test in the pit or queue area when allowed. [Why](#why-system-check)
- Verify radios, CAN devices, pneumatics, key sensors, and cameras are online with no known intermittent fault. [Why](#why-system-check)
- Confirm full mechanism range of motion is clear and that no cable path is near binding or snagging. [Why](#why-system-check)
- Check that current limits, brake/coast assumptions, and heading zero procedures match the intended match strategy. [Why](#why-system-check)
- Clear any open no-go condition before the robot enters the field. [Why](#why-system-check)

## Match Operating Rules

- Prefer the tested match configuration over an unverified pit-side tweak. [Why](#why-match-operating-rules)
- Retract or protect vulnerable mechanisms before predictable contact. [Why](#why-match-operating-rules)
- If the robot behavior is unsafe or severely degraded, stop risking secondary failures and communicate the issue clearly. [Why](#why-match-operating-rules)
- Drive and operate with battery, bumper, and field-condition awareness instead of assuming the robot is unchanged from the last match. [Why](#why-match-operating-rules)

## Immediate Post-Match

- Get the robot off the field safely, then start the battery swap and quick damage scan immediately. [Why](#why-immediate-post-match)
- Note any brownout, disconnect, breaker heat, unusual battery sag, or control anomaly before memories fade. [Why](#why-immediate-post-match)
- Flag any hit to bumpers, frame rails, swerve modules, exposed shafts, or intake structure before the next queue cycle starts. [Why](#why-immediate-post-match)
- Decide whether the robot is ready for the next match, needs repair, or must be held in pit for deeper inspection. [Why](#why-immediate-post-match)

## Match Review

- Capture the result, autonomous outcome, endgame outcome, penalties, and the top one or two issues that matter most. [Why](#why-match-review)
- Assign an owner for the immediate fix, and confirm the owner knows the expected deadline. [Why](#why-match-review)
- Separate root-cause clues from emotional reactions so the next repair starts with useful evidence. [Why](#why-match-review)
- Record alliance-specific or field-specific observations that might matter in playoffs or replays. [Why](#why-match-review)

## Repair Recovery and Ready for Next Match

- Reproduce the symptom or state the observed failure clearly before turning tools. [Why](#why-repair-recovery-and-ready-for-next-match)
- Name the root-cause hypothesis before starting the repair. [Why](#why-repair-recovery-and-ready-for-next-match)
- Restore fasteners, strain relief, dynamic cable routing, and connector retention after any repair. [Why](#why-repair-recovery-and-ready-for-next-match)
- Re-check sensor zero, full range of motion, and software behavior if hardware changed. [Why](#why-repair-recovery-and-ready-for-next-match)
- Repeat a drop or shake test after fixing intermittent radio, CAN, or power problems. [Why](#why-repair-recovery-and-ready-for-next-match)
- Do not send the robot back to queue until the repaired subsystem has passed a realistic functional check. [Why](#why-repair-recovery-and-ready-for-next-match)

## Alliance Selection Transition

- Re-rank pick candidates by role fit, reliability, and no-show risk rather than by raw preference. [Why](#why-alliance-selection-transition)
- Review actual match video or trusted notes for close decisions. [Why](#why-alliance-selection-transition)
- Confirm the robot's own reliability limits before promising playoff-role capability. [Why](#why-alliance-selection-transition)
- Tighten battery rotation, spare-parts staging, and match-turnaround expectations before playoffs start. [Why](#why-alliance-selection-transition)

## Playoffs and Elims Cycle

- Keep the robot on the most stable tested configuration unless a change is clearly worth the playoff risk. [Why](#why-playoffs-and-elims-cycle)
- Inspect bumpers, drivetrain, and exposed mechanisms after every hard-contact playoff match. [Why](#why-playoffs-and-elims-cycle)
- Shorten the communication loop between scouts, drive team, and pit so the next plan is clear before the robot returns to queue. [Why](#why-playoffs-and-elims-cycle)
- Protect battery quality, cooling time, and repair time more aggressively than in qualification matches. [Why](#why-playoffs-and-elims-cycle)

## Pack-Out and Event Closeout

- Summarize critical failures, root causes, and near-misses before the team leaves the venue. [Why](#why-pack-out-and-event-closeout)
- Tag broken parts, depleted consumables, suspect batteries, and software debt so they are not forgotten in transit. [Why](#why-pack-out-and-event-closeout)
- Save match video references, logs, scouting notes, and incident notes while the event context is still fresh. [Why](#why-pack-out-and-event-closeout)
- Pack the pit so chargers, laptops, radios, tools, and field-shelf gear all come home with clear ownership. [Why](#why-pack-out-and-event-closeout)

## D+1 Post-Event Breakdown

- Unload, clean, and inspect the robot before normal shop work resumes. [Why](#why-d1-post-event-breakdown)
- Document wear, cracks, connector damage, and electrical heat evidence found after the event. [Why](#why-d1-post-event-breakdown)
- Start corrective actions for the failures that most threatened match availability or scoring. [Why](#why-d1-post-event-breakdown)
- Restock batteries, breakers, wires, bumper supplies, and the pit kit immediately. [Why](#why-d1-post-event-breakdown)

## D+2 Retrospective and Lessons Learned

- Review what the team should repeat, stop, and change before the next event. [Why](#why-d2-retrospective-and-lessons-learned)
- Update the checklist, training materials, pick-list process, and release process based on real evidence from the event. [Why](#why-d2-retrospective-and-lessons-learned)
- Assign owners and due dates for corrective actions instead of leaving them as general observations. [Why](#why-d2-retrospective-and-lessons-learned)
- Preserve lessons that help next season too, not just the next event. [Why](#why-d2-retrospective-and-lessons-learned)

## No-Go Conditions

Do not queue until resolved or consciously accepted by the coach and pit lead if any of these are true. [Why](#why-no-go-conditions)

- Unknown electrical fault affecting control power, CAN, or radio stability. [Why](#why-no-go-conditions)
- Untested code change on the robot. [Why](#why-no-go-conditions)
- Controller mapping uncertainty or unexplained controller behavior. [Why](#why-no-go-conditions)
- Battery security uncertainty, battery health uncertainty, or repeated brownout trend. [Why](#why-no-go-conditions)
- Hot main breaker, recently tripped main breaker not yet replaced, or unexplained power-terminal heating. [Why](#why-no-go-conditions)
- Damaged bumper attachment, illegal bumper construction, or bumper fabric dragging or catching. [Why](#why-no-go-conditions)
- Damaged swerve module, drivetrain rail, intake side plate, or exposed shaft not yet inspected under load. [Why](#why-no-go-conditions)
- Significant mechanical interference risk or uncalibrated critical sensor used by autonomous or closed-loop control. [Why](#why-no-go-conditions)
- Unresolved alliance auto conflict that creates an avoidable opening-match collision risk. [Why](#why-no-go-conditions)

---

## Rationale and Sources

### Why T-7 Pre-Regional Prep

The biggest event failures are usually visible before the team leaves for the venue: unclear ownership, missing spares, weak bumper planning, battery readiness issues, and no fallback software plan. A week out is the right time to catch structural gaps without adding last-minute chaos.

Sources:
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)
- [Ways to Lose a Match in FRC](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/ways-to-lose-a-match.md)
- [Ways to Win a Season in FRC](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/ways-to-win-a-season-in-frc.md)
- [Chief Delphi Common Issues Audit 2024-2026](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/chief-delphi-common-issues-2024-2026-audit.md)

### Why T-1 Final Readiness Check

The last full shop day is where teams should find loose wiring, weak strain relief, bad batteries, missing pit items, and risky software changes. Those are frequent causes of avoidable qualification-match losses and slow pit recovery.

Sources:
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)
- [Chief Delphi Common Issues Audit 2024-2026](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/chief-delphi-common-issues-2024-2026-audit.md)
- [Chief Delphi: Most Common Issues Seen on Robots This Year, 2024](https://www.chiefdelphi.com/t/most-common-issues-seen-on-robots-this-year/466119)
- [Chief Delphi: Most Common Issues Seen 2025](https://www.chiefdelphi.com/t/most-common-issues-seen-2025/505274)
- [Chief Delphi: Most Common Issues Seen 2026](https://www.chiefdelphi.com/t/most-common-issues-seen-2026/520595)

### Why Load-In and Setup

Regional events compress setup time. A clean pit layout, a transport-damage check, and correctly staged repair gear reduce the odds that the team burns practice and inspection time on preventable setup mistakes.

Sources:
- [2026 Nevada Las Vegas Regional Agenda](https://info.firstinspires.org/hubfs/web/event/frc/2026/2026_NVLV_Agenda.pdf)
- [Ways to Win a Season in FRC](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/ways-to-win-a-season-in-frc.md)

### Why Inspection Calibration and Practice Day

Inspection and practice day are not just compliance tasks. They are the best time to confirm the robot is legal, calibrations are still valid after transport, and the actual event build still behaves correctly on both alliances and under event pressure.

Sources:
- [2026 FRC Inspection Checklist](https://firstfrc.blob.core.windows.net/frc2026/Manual/2026FRCInspectionChecklist.pdf)
- [2026 Nevada Las Vegas Regional Agenda](https://info.firstinspires.org/hubfs/web/event/frc/2026/2026_NVLV_Agenda.pdf)
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)

### Why Event Day Start

Morning driver-station problems and stale robot state can sink an otherwise good day. Reboots, power-setting checks, cable checks, and a quick physical inspection catch many of the issues teams otherwise discover only after the robot is on the field.

Sources:
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)
- [Chief Delphi Common Issues Audit 2024-2026](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/chief-delphi-common-issues-2024-2026-audit.md)

### Why Pre-Match and Queue

Queue is where simple misses become match losses: wrong battery, loose connector, wrong auto, bad bumper state, or an unresolved alliance-path conflict. This block focuses on the highest-probability errors that still fit in a short turnaround window.

Sources:
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)
- [Ways to Lose a Match in FRC](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/ways-to-lose-a-match.md)
- [Chief Delphi Common Issues Audit 2024-2026](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/chief-delphi-common-issues-2024-2026-audit.md)

### Why System Check

A short systems check bridges the gap between queue confidence and actual robot readiness. It forces the team to confirm that communications, calibration, motion limits, and known intermittent faults are under control before the match starts.

Sources:
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)
- [Chief Delphi Common Issues Audit 2024-2026](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/chief-delphi-common-issues-2024-2026-audit.md)

### Why Match Operating Rules

Many event failures are caused less by design and more by decision-making under pressure. Stable playoff teams preserve tested behavior, protect vulnerable hardware, and stop compounding damage when a subsystem is already compromised.

Sources:
- [Ways to Lose a Match in FRC](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/ways-to-lose-a-match.md)
- [Ways to Win a Season in FRC](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/ways-to-win-a-season-in-frc.md)
- [Chief Delphi Common Issues Audit 2024-2026](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/chief-delphi-common-issues-2024-2026-audit.md)

### Why Immediate Post-Match

The fastest path to missing the next match is delaying the first damage scan. Fresh observations about brownouts, breaker heat, impacts, and control anomalies are much more useful immediately after the match than ten minutes later.

Sources:
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)
- [Chief Delphi Common Issues Audit 2024-2026](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/chief-delphi-common-issues-2024-2026-audit.md)

### Why Match Review

The team needs a short evidence-first review, not a long emotional one. Logging the match result, penalty causes, and the most urgent fix keeps pit time aligned with what matters before the next queue call.

Sources:
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)
- [Ways to Lose a Match in FRC](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/ways-to-lose-a-match.md)

### Why Repair Recovery and Ready for Next Match

Repairs fail when teams fix the symptom, forget the strain relief, skip the range-of-motion check, or send the robot out without a realistic retest. This section is built to reduce repeat failures and turnaround surprises.

Sources:
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)
- [Chief Delphi Common Issues Audit 2024-2026](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/chief-delphi-common-issues-2024-2026-audit.md)
- [Chief Delphi: Most Common Issues Seen on Robots This Year, 2024](https://www.chiefdelphi.com/t/most-common-issues-seen-on-robots-this-year/466119)

### Why Alliance Selection Transition

Alliance selection rewards teams that know their true role fit and reliability. The same discipline used in match prep matters here too: use real evidence, prepare backups, and understand the robot the team can reliably field right now.

Sources:
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)
- [Ways to Win a Season in FRC](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/ways-to-win-a-season-in-frc.md)

### Why Playoffs and Elims Cycle

Playoffs shorten turnaround time and raise the cost of every failure. Teams need tighter inspection cadence, more conservative change control, and faster communication than they can get away with in early qualifications.

Sources:
- [Ways to Win a Season in FRC](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/ways-to-win-a-season-in-frc.md)
- [Chief Delphi Common Issues Audit 2024-2026](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/chief-delphi-common-issues-2024-2026-audit.md)

### Why Pack-Out and Event Closeout

If the team waits until midweek to remember what failed, important evidence is already gone. Event closeout should capture the hard-earned lessons, missing inventory, and lingering repairs while the details are still accurate.

Sources:
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)
- [Ways to Win a Season in FRC](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/ways-to-win-a-season-in-frc.md)

### Why D+1 Post-Event Breakdown

The first day home is the best time to find structural damage, connector heat, worn parts, and depleted consumables before normal shop work hides them. It also keeps event repairs from becoming next-event emergencies.

Sources:
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)
- [Chief Delphi Common Issues Audit 2024-2026](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/chief-delphi-common-issues-2024-2026-audit.md)

### Why D+2 Retrospective and Lessons Learned

Without an explicit retrospective, teams repeat the same process failures even when they fix the hardware. Turning lessons into assigned actions and updated checklists is what makes the event experience durable.

Sources:
- [Ways to Win a Season in FRC](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/ways-to-win-a-season-in-frc.md)
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)

### Why No-Go Conditions

No-go calls exist to stop the team from turning a manageable problem into a dead robot, field fault, or avoidable loss. The conditions here focus on issues that repeatedly correlate with severe match-risk: electrical uncertainty, bad batteries, untested code, bumper illegality, drivetrain damage, and unresolved auto conflicts.

Sources:
- [FRC Operational Checklists](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/frc-operational-checklists.md)
- [Ways to Lose a Match in FRC](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/ways-to-lose-a-match.md)
- [Chief Delphi Common Issues Audit 2024-2026](https://github.com/dougdliu/FRC-Operational-Checklist/blob/main/chief-delphi-common-issues-2024-2026-audit.md)
