# Interface Plan — Job Acquisition Engine

## Goals
- Provide a single workspace to track **targets, applications, outreach, portfolio shipping, and interview prep**.
- Enforce the **clearance firewall** with explicit flags and exclusions.
- Make weekly execution **measurable** (quotas, status, and next actions).

## Primary Users
- **You (solo operator)**: quick capture, high signal, low overhead.

## Information Architecture (Top‑Level Navigation)
1. **Dashboard**
2. **Targets**
3. **Applications**
4. **Outreach**
5. **Portfolio**
6. **Interview Prep**
7. **Search Queries**
8. **Settings (Constraints/Rules)**

## Core Data Models (Entities)
### Company Target
- Company name
- Remote/local/hybrid
- Rationale
- Roles to search
- Keywords (2–3)
- Clearance risk (Y/N + notes)
- Status (watching/applied/active/paused)

### Role/Application
- Company
- Role title
- Link/source
- Comp range
- Status (saved/applied/screen/interview/offer/rejected)
- Date applied
- Next action + due date
- Clearance flag (Y/N)

### Outreach Thread
- Company
- Contact name + role
- Channel (LinkedIn/email)
- Message template used
- Status (sent/replied/follow‑up)
- Next follow‑up date

### Portfolio Item
- Project name
- Milestone
- Ship date
- Demo link
- Acceptance criteria checklist

### Interview Prep Session
- Date
- Focus area (SQL/system design/behavioral/debugging)
- Notes
- Gaps + next practice

## Key Screens & Workflows
### 1) Dashboard
**Purpose:** weekly overview + daily priorities.
- Weekly quota progress (apps/outreach/portfolio/interview reps)
- Today’s tasks (next actions due)
- Clearance firewall alerts (flagged roles)
- Recent wins (replies, interviews scheduled)

### 2) Targets
**Purpose:** curate companies with rationale + filters.
- Table view + filters (remote only, clearance‑safe)
- Bulk add from target lists
- Quick toggle: “Do not pursue”

### 3) Applications
**Purpose:** pipeline tracking.
- Kanban by status
- Detailed record for each role
- Clearance flag required before moving to “Applied”

### 4) Outreach
**Purpose:** track messages + follow‑ups.
- Sequence view: initial + follow‑up 1 + follow‑up 2
- Status reminders
- Template picker for manager/engineer/recruiter

### 5) Portfolio
**Purpose:** shipment tracking.
- Milestone checklist per project
- Demo checklist links
- Metrics to capture for resume/interviews

### 6) Interview Prep
**Purpose:** repeatable practice loop.
- Weekly plan checklist
- Session log
- Gap tracker

### 7) Search Queries
**Purpose:** copy‑paste strings per job board.
- LinkedIn/Indeed/BuiltIn/Wellfound
- Negative keywords included

### 8) Settings
**Purpose:** enforce rules.
- Clearance firewall rules
- Compensation targets
- Role lanes + negative keywords

## Critical UX Requirements
- **Fast capture**: add a role in <60 seconds.
- **Hard clearance gating**: must mark clearance flag before submit.
- **Reminder system**: follow‑ups + next actions visible daily.
- **Metrics**: weekly throughput + conversion rates.

## MVP Feature Set (Phase 1)
- Dashboard + Targets + Applications + Outreach
- Hard clearance flag before apply
- Weekly quota counters
- CSV export of pipeline

## Phase 2 Enhancements
- Portfolio + Interview modules
- Calendar integration for interviews
- Light analytics (response rates, time‑to‑response)

## Data Entry Templates (Minimum Fields)
- **Target**: Company, Remote/Hybrid, Rationale, Roles, Keywords, Clearance risk
- **Role**: Title, Link, Comp range, Status, Next action, Clearance flag
- **Outreach**: Contact, Template, Status, Follow‑up date
- **Portfolio**: Milestone, Demo link, Acceptance checklist

## Success Criteria
- At least 90% of roles tracked with clearance flag.
- Weekly quota adherence (apps/outreach/interviews).
- Reduced drop‑offs due to missed follow‑ups.
