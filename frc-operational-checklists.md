# FRC Operational Checklists
## Season, Event, Match, and Recovery Checklists

These checklists convert lessons into daily execution.

Source references:
- [ways-to-lose-a-match.md](ways-to-lose-a-match.md)
- [ways-to-win-a-season-in-frc.md](ways-to-win-a-season-in-frc.md)

How to use:
- Print this document or use it on a tablet.
- Assign a single owner for each checklist block.
- Mark each line item Done, Not Done, or N/A.

---

## A) Preseason Readiness Checklist

Owner: Team Leads

- Team roles assigned with primary and backup for each critical role
- Driver, operator, and human player practice plan scheduled
- Electrical standards defined (wire colors, labels, strain relief, CAN conventions)
- Software release process defined (branching, tagged match releases, rollback plan)
- Robot weight budget defined by subsystem
- Spare parts plan created for high-risk mechanisms
- Pit tool and consumables inventory list created
- Driver station laptop standard image prepared and tested
- Safety and emergency procedures reviewed
- Post-match review template ready

---

## B) Weekly Build and Integration Checklist

Owner: Build Lead

- Wiring accessible and inspectable
- CAN chain physically secured end-to-end
- Main breaker protected by shroud
- Battery connections strain-relieved and tested
- Radio and ethernet strain relief installed
- All critical fasteners checked and marked
- Sensor mounting secure and protected from chips/debris
- Robot weighed and compared to budget
- Serviceability test run (remove and reinstall major subsystem)
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
- Heading zero procedure confirmed with drive team
- Deploy performed in pit, not in queue
- Commit hash recorded in match log
- Rollback commit prepared and verified

---

## D) Driver Station Checklist (Start of Event Day)

Owner: Drive Coach or DS Operator

- Laptop rebooted today
- Power settings set to high performance
- Non-essential apps closed
- Driver Station software version verified
- Firewall settings verified for DS operation
- WiFi auto-connect disabled except required field behavior
- USB ports, cables, and controller connections verified
- Controller brand/model matches expected mapping
- Spare controllers and spare cable present
- Laptop physically secured to DS shelf
- Charger present and functional

---

## E) Pre-Match Queue Checklist

Owner: Queue Lead

- Correct battery installed, secured, and recently charged
- Main breaker accessible and protected
- Robot enabled test passed in pit
- Correct autonomous routine selected
- Bumpers installed correctly for alliance color
- Bumper tape and fabric condition checked
- Pneumatics charged and leak check done
- Controllers connected and assigned correctly
- Driver/operator aware of any control changes
- Strategy reviewed with alliance partners
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
- Software retest if hardware changed
- Dry run enable test in pit
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

## L) 10 Non-Negotiables

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
