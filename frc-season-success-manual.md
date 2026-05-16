# FRC Season Success Manual
## Institutional Knowledge System and Operating Playbook

This manual turns hard-earned team lessons into repeatable process so your team does not relearn the same failures each season.

Primary source references:
- [ways-to-lose-a-match.md](ways-to-lose-a-match.md)
- [ways-to-win-a-season-in-frc.md](ways-to-win-a-season-in-frc.md)

---

## 1) Purpose

Use this document to:
- Preserve institutional knowledge across graduating classes
- Reduce preventable match losses
- Improve reliability, consistency, and decision quality
- Standardize expectations across subteams

Definition of success:
- Fewer unforced errors
- Faster pit recovery
- Better match execution under pressure
- Better year-over-year handoff

---

## 2) Team Standards

Set these standards before kickoff and revisit weekly.

### Reliability Standard
- Robot must survive full event cycle without recurring critical failures.
- Every subsystem has an owner and a backup owner.

### Readiness Standard
- No untested code changes within 15 minutes of queueing.
- Every match runs a written pre-match checklist.

### Communication Standard
- Strategy, controls, and mechanical changes are announced to drive team and pit lead.
- Post-match review happens after every match.

### Accountability Standard
- No blame-first behavior. Use root cause analysis with actions.
- Every major failure gets a documented corrective action owner and due date.

---

## 3) Season Phases and Gates

### Phase A: Kickoff to Concept Freeze
Exit criteria:
- Strategy priorities defined
- Mechanism options prototyped
- Weight budget started
- Risk register created

### Phase B: Build and Integration
Exit criteria:
- Electrical complete and labeled
- Robot software baseline complete
- All mechanisms can be tested repeatedly
- Serviceability validated in timed pit drills

### Phase C: Driver and Systems Validation
Exit criteria:
- Full-field or simulated match reps complete
- Auto validated for both alliances
- Recovery procedures practiced
- Backup plans for partial robot failures

### Phase D: Competition Execution
Exit criteria each event:
- Pre-event inspection complete
- Event checklist discipline maintained
- Daily postmortem captured
- Improvements queued for next event

### Phase E: Offseason Knowledge Transfer
Exit criteria:
- Final season review documented
- New student onboarding package updated
- Tooling and checklist revisions completed

---

## 4) Core Operating Rhythm

### Weekly In-Season Cadence
- Monday: Failure review, improvement planning
- Midweek: Build and software integration
- End of week: Full systems test and drive reps
- Weekend or final meeting: Simulated match block and debrief

### Event-Day Cadence
- Morning: Full systems check, role confirmation
- Before every match: Quick pre-match checklist
- After every match: 3-minute debrief and action assignment
- End of day: Reliability review and next-day prep

---

## 5) Roles and Responsibilities

### Head Coach or Lead Mentor
- Enforces process discipline
- Owns final go/no-go decisions
- Removes blockers between subteams

### Pit Lead
- Owns robot readiness status
- Runs pit repair prioritization
- Confirms checklist completion before queueing

### Drive Coach
- Owns strategy execution and alliance comms
- Leads post-match review with objective evidence

### Software Lead
- Owns release process and version tagging
- Prevents last-minute unvalidated deployments

### Electrical Lead
- Owns connection integrity and CAN health
- Verifies battery, breaker, and radio reliability controls

### Mechanical Lead
- Owns fastener integrity and serviceability
- Verifies wear items and critical spares readiness

### Scouting Lead
- Owns data quality and alliance selection support
- Ensures scouting outputs are actually used in strategy

---

## 6) Decision Rules

Use these rules to avoid emotional decision making.

### Go/No-Go Rule for Match Deployment
No-go if any of the following are true:
- Unknown root cause for a critical failure
- Drive controls changed without practice rep
- Code updated but not validated on robot
- Battery, radio, or DS readiness uncertain

### Change Control Rule
- All changes logged in a simple change log.
- High-risk changes require lead mentor or pit lead approval.

### Escalation Rule
- If a repair exceeds 10 minutes, escalate to pit lead.
- If repeated failure appears twice, stop patching and do root cause analysis.

---

## 7) Metrics That Matter

Track simple metrics consistently.

### Reliability Metrics
- Matches without critical fault
- Brownout count per event
- Unplanned DS disconnect incidents
- Repeat failure count by subsystem

### Performance Metrics
- Auto completion rate
- Endgame completion rate
- Cycle consistency under defense
- Penalty count and penalty points

### Process Metrics
- Checklist completion rate
- Queue on-time rate
- Mean time to repair
- Percent of post-match actions closed by next match

---

## 8) Failure Review Format

Use this exact format after each serious failure.

- What happened:
- Impact on match result:
- Immediate containment:
- Root cause:
- Corrective action:
- Preventive action:
- Owner:
- Due date:
- Verification method:

Rule:
- No blame language
- Evidence over opinion

---

## 9) Knowledge Retention System

### What to Save
- Final wiring diagrams
- Controller mappings
- Proven autos and known failure autos
- Event-specific lessons learned
- Parts that failed and why
- Best repair procedures and timing

### Where to Save
- Keep all season docs in this folder.
- Maintain one master index file for quick onboarding.

### How to Hand Off
- Hold an offseason review meeting.
- Require each lead to present top 10 lessons and top 10 non-negotiables.

---

## 10) Implementation Plan (Next 2 Weeks)

Week 1:
- Assign owners for all checklist sections
- Adopt the pre-match and post-match checklists
- Start logging failures and actions

Week 2:
- Run one full mock event day
- Measure checklist adherence
- Revise checklist wording based on confusion points

---

## 11) Quick Start

Start with these three steps:
1. Use [frc-operational-checklists.md](frc-operational-checklists.md) at your next meeting and next event.
2. Pick 5 recurring failures from [ways-to-lose-a-match.md](ways-to-lose-a-match.md) and create hard controls for each.
3. Assign one student owner per control and verify completion weekly.

If this manual is followed consistently, your team should see fewer preventable losses, faster pit recovery, and stronger competitive consistency by mid-season.
