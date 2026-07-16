# Timeline Reconstruction

## Purpose

Help participants establish a shared understanding of what happened, in what order, and why.

A timeline exercise creates a factual, chronological view of events before attempting to:
- identify successes,
- identify failures,
- understand contributing factors,
- perform root cause analysis,
- define improvement actions.

The timeline acts as a "single source of truth" for the rest of the workshop.

---

# Workshop Types

Recommended for:

- Post-Mortems
- Incident Reviews
- Lessons Learned Workshops
- Release Reviews
- Project Retrospectives

Can also be adapted for:

- Organizational Change Analysis
- Architecture Evolution Reviews
- Transformation Programs

---

# Outcomes

Expected deliverables:

- Shared understanding of events
- Key milestones
- Decision points
- Communication history
- Critical delays
- Contributing factors

---

# Duration

| Scope | Duration |
|---------|---------|
| Small incident | 15-20 min |
| Medium incident | 20-40 min |
| Major incident | 40-60 min |
| Multi-month project | 60-90 min |

---

# Materials

Physical workshop:

- Sticky notes
- Timeline wall
- Markers

Online workshop:

- Miro
- Mural
- Whiteboard

---

# Preparation

Before the workshop, gather as much evidence as possible:

- Emails
- Teams conversations
- Jira tickets
- Monitoring alerts
- Logs
- Release records
- Meeting notes
- Participant recollections

The facilitator should prepare an initial timeline draft whenever possible.

Participants should enrich and validate it during the workshop.

---

# Instructions

## Step 1 - Establish the Frame

Facilitator script:

> Before discussing causes or solutions, let's first build a common understanding of what happened.
>
> We will reconstruct the events as objectively as possible.
>
> At this stage we are not looking for blame or explanations.
>
> We are simply establishing the facts.

Duration: 3 minutes

---

## Step 2 - Build the Timeline

Ask participants:

### What happened?

Capture:

- Events
- Technical actions
- Decisions
- Communications

Use one sticky note per event.

Example format:

```text
27/05 10:34
Supplier contacted
```

```text
27/05 14:30
Issue reproduced by supplier
```

```text
27/05 18:00
Rollback decision taken
```

Arrange events chronologically.

Duration: 10-20 minutes

---

## Step 3 - Validate the Timeline

Review the timeline from beginning to end.

Ask:

- Is anything missing?
- Are the timestamps accurate?
- Were parallel activities happening?
- Are we missing important communications?

Correct and complete the timeline.

Duration: 5-10 minutes

---

## Step 4 - Identify Key Moments

Ask participants to highlight:

### Detection

When was the issue first discovered?

### Escalation

When was support engaged?

### Decision Points

When were significant decisions made?

### Resolution

When was the system stabilized?

### Recovery

When was normal operation restored?

Use a different color for these events.

Duration: 5-10 minutes

---

## Step 5 - Add Context

For each important event ask:

### What information was available at the time?

Not:

> What do we know today?

But:

> What did people know at that moment?

This helps prevent hindsight bias.

Example:

```text
Rollback decision

Known at the time:
- Flights disappearing
- Operational impact increasing
- Root cause not yet confirmed
```

Duration: 10-15 minutes

---

# Variants

## Incident Timeline

Focus on:

- Detection
- Investigation
- Escalation
- Resolution

Typical output:

```text
Issue
↓
Detection
↓
Supplier Contacted
↓
Analysis
↓
Decision
↓
Fix
↓
Recovery
```

---

## Release Timeline

Focus on:

- Requirements
- Design
- Development
- Validation
- Deployment
- Outcome

Useful for:

- Release failures
- Project lessons learned

---

## Project Timeline

Focus on:

- Milestones
- Decisions
- Dependencies
- Changes in direction

Useful for:

- Long initiatives
- Transformation projects

---

# Facilitator Tips

## Stay factual

Prefer:

> What happened?

Avoid:

> Why did you do that?

The purpose of the timeline is reconstruction, not explanation.

---

## Separate facts from opinions

### Fact

```text
27/05 14:30
Supplier reproduced the issue
```

### Opinion

```text
Supplier reacted too slowly
```

Capture opinions later in the workshop.

---

## Prevent hindsight bias

Avoid:

> They should have known.

Ask:

> What information was available at the time?

---

## Capture parallel work

Many incidents have multiple streams:

- Operations
- Development
- Supplier Investigation
- Communication
- Management Decisions

Use swim lanes if useful.

Example:

```text
OPS
|----Detection----Rollback----Recovery----|

SUPPLIER
|----Analysis----Fix----Validation----|

MANAGEMENT
|----Escalation----Decision----Communication----|
```

---

# Common Follow-Up Activities

A timeline is rarely the final activity.

Typical sequence:

```text
1. Timeline
2. What Went Well
3. What Went Poorly
4. Root Cause Analysis
5. Action Definition
```

---

# Example

## Context

AMAN incident after release 3.11.0.

---

## Reconstructed Timeline

```text
26/27 May
Release 3.11.0 deployed

27 May 10:34
Supplier contacted

27 May 14:30
Issue reproduced

27 May evening
Rollback decision

27/28 May
Rollback executed

04 June
Root cause shared

11 June
Detailed solution proposed

19 June
Fix delivered

08 July
Fix deployed
```

---

# When to Use

Use when:

✅ Participants have different versions of events.

✅ The order of events matters.

✅ Root cause analysis is required.

✅ An incident or project needs to be reconstructed.

Avoid when:

❌ The objective is only future planning.

❌ The workshop focuses exclusively on vision creation.

❌ The chronology is not important.

---

# Related Techniques

Usually combined with:

- What Went Well / What Went Poorly
- Five Whys
- Fishbone Diagram
- Root Cause Analysis
- Lessons Learned
- Circles of Influence

Typical Post-Mortem Flow:

```text
Timeline
↓
Successes & Failures
↓
Root Causes
↓
Action Items
↓
Incident Documentation
```
