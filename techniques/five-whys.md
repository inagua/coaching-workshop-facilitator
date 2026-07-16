# Five Whys

## Purpose

The Five Whys is a root cause analysis technique that helps teams move beyond symptoms and identify the underlying causes of a problem.

The technique is based on a simple principle:

> When a problem occurs, repeatedly ask "Why?" until you reach a cause that can be meaningfully addressed.

The goal is not to ask exactly five times.

The goal is to explore the chain of causality until the group identifies actionable root causes.

---

# Workshop Types

Recommended for:

- Post-Mortems
- Incident Reviews
- Problem Solving Workshops
- Operational Improvement Workshops
- Lessons Learned Workshops

Can also be used for:

- Delivery Delays
- Architecture Issues
- Quality Problems
- Collaboration Challenges

Less suitable for:

- Strategic Planning
- Visioning Workshops
- Brainstorming Sessions

---

# Outcomes

Expected deliverables:

- Root causes
- Contributing factors
- Shared understanding
- Improvement opportunities
- Action candidates

---

# Duration

| Problem Complexity | Duration |
|------------|------------|
| Simple issue | 10-15 min |
| Medium issue | 15-30 min |
| Complex issue | 30-60 min |

---

# Materials

Physical workshop:

- Whiteboard
- Sticky notes
- Markers

Remote workshop:

- Miro
- Mural
- Whiteboard

---

# When to Use

The Five Whys works best after the group has already aligned on:

- What happened
- The timeline
- The observed problem

Typical flow:

```text
Timeline
↓
Problem Statement
↓
Five Whys
↓
Action Definition
```

---

# Preparation

Before starting, define a clear problem statement.

Good:

```text
Flights temporarily disappeared from
the AMAN sequence.
```

Bad:

```text
The supplier delivered bad software.
```

The Five Whys should investigate observable facts, not opinions.

---

# Instructions

## Step 1 - State the Problem

Write the problem clearly.

Example:

```text
Problem:
Flights disappeared from the sequence
during ETFMS → Radar transition.
```

Duration: 2 minutes

---

## Step 2 - Ask the First Why

Facilitator asks:

> Why did this happen?

Capture the answer.

Example:

```text
Because flights were temporarily
de-sequenced.
```

---

## Step 3 - Continue Asking Why

Ask:

> Why did that happen?

For each answer, continue exploring.

Example:

```text
Problem
↓
Flights disappeared

Why?
↓
Flights were temporarily de-sequenced

Why?
↓
Valid trajectory information was missing

Why?
↓
ETFMS information was removed too early

Why?
↓
The transition logic assumed radar
data was immediately usable

Why?
↓
The transition scenario was not fully
considered during design and validation
```

---

## Step 4 - Stop When Useful

Do not continue forever.

Stop when:

- The group identifies a cause that can be addressed.
- Further questioning produces speculation.
- The discussion becomes repetitive.

The objective is actionable understanding.

---

## Step 5 - Define Actions

Ask:

> What can we do to prevent this cause from happening again?

Create actions with:

- Owner
- Deadline
- Success criteria

---

# Example 1 – AMAN Incident

## Problem

```text
Flights temporarily disappeared from
the AMAN sequence.
```

### Why #1

Why?

```text
Flights were de-sequenced.
```

### Why #2

Why?

```text
Required trajectory information
was temporarily unavailable.
```

### Why #3

Why?

```text
ETFMS information was removed before
radar sequencing became available.
```

### Why #4

Why?

```text
Transition handling had a timing gap.
```

### Why #5

Why?

```text
The ETFMS-to-radar transition scenario
was not explicitly tested.
```

---

## Candidate Actions

- Create dedicated ETFMS transition test cases.
- Review regression coverage.
- Include transition scenarios in validation activities.

---

# Example 2 – Architecture Collaboration

## Problem

```text
Architecture deliverables arrived
later than expected.
```

### Why #1

Why?

```text
Work was completed later than planned.
```

### Why #2

Why?

```text
Requirements clarification took longer
than expected.
```

### Why #3

Why?

```text
Important stakeholders were involved
late in the process.
```

### Why #4

Why?

```text
Responsibilities and review points
were unclear.
```

### Why #5

Why?

```text
No agreed collaboration model existed
between TRACE and Architecture.
```

---

## Candidate Actions

- Define collaboration working agreement.
- Clarify ownership.
- Define review lifecycle.
- Create escalation path.

---

# Facilitator Tips

## Focus on Systems

Bad:

```text
Why did Ross make that mistake?
```

Good:

```text
Why was the system unable to detect
this issue earlier?
```

The objective is understanding the system.

---

## Avoid Blame

Five Whys is often misused to identify a person.

Example:

```text
Why?
Because John forgot.
```

Don't stop there.

Continue:

```text
Why was forgetting possible?
```

```text
Why was there no verification?
```

```text
Why was detection missing?
```

Look beyond individual actions.

---

## Be Evidence-Based

Support answers with:

- Logs
- Emails
- Metrics
- Jira tickets
- Timeline events

Avoid unsupported assumptions.

---

## Multiple Answers Are Allowed

A problem may have several causes.

Example:

```text
Why was testing ineffective?

- Missing scenario
- Time pressure
- Incomplete requirements
```

Explore each path separately if needed.

---

# Common Mistakes

## Stopping Too Early

Example:

```text
Problem
↓
Human error
```

This is rarely a root cause.

Instead ask:

```text
Why was human error possible?
```

---

## Going Too Deep

Eventually causes become:

```text
Because humans are imperfect.
```

```text
Because reality is complex.
```

These are not useful.

Focus on causes that can be influenced.

---

## Treating Every Cause as Equal

Not all causes deserve actions.

Prioritize causes that:

- Have significant impact.
- Can realistically be improved.
- Reduce future risk.

---

# Variants

## Traditional Five Whys

Single linear chain.

```text
Problem
↓
Why
↓
Why
↓
Why
↓
Why
↓
Why
```

---

## Branching Five Whys

Multiple answers for the same why.

```text
Problem
├── Cause A
│   └── Why?
│
├── Cause B
│   └── Why?
│
└── Cause C
    └── Why?
```

Recommended for complex incidents.

---

# When to Use

Use when:

✅ The problem is known.

✅ Understanding causes is more important than generating ideas.

✅ The group can discuss facts.

✅ Root causes are unclear.

Avoid when:

❌ The workshop is future-oriented.

❌ The group lacks sufficient information.

❌ The objective is brainstorming.

---

# Related Techniques

Frequently combined with:

- Timeline Reconstruction
- Fishbone Diagram
- Root Cause Analysis
- Lessons Learned
- Action Planning

Typical Incident Workshop Flow:

```text
Timeline
↓
What Went Well / Poorly
↓
Five Whys
↓
Root Causes
↓
Actions
↓
Incident Documentation
```

---

# Quick Facilitator Cheat Sheet

Ask repeatedly:

```text
Why did this happen?
```

When an answer points to a person:

```text
What allowed that to happen?
```

When a cause is identified:

```text
What evidence supports this?
```

When the discussion reaches an actionable cause:

```text
What should we change?
```

Remember:

> The purpose of Five Whys is not to find someone to blame.
>
> The purpose is to understand why the system allowed the problem to occur.
