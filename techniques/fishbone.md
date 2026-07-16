# Fishbone Diagram (Ishikawa Cause-and-Effect Analysis)

## Purpose

Help participants identify, organize, and visualize the possible causes of a problem.

The Fishbone Diagram is particularly useful when:

- A problem has multiple contributing factors.
- Teams disagree on the root cause.
- The objective is understanding rather than blame.
- A workshop needs to move beyond symptoms.

The technique encourages systems thinking by exploring several categories of potential causes rather than focusing on a single explanation.

---

# Workshop Types

Recommended for:

- Post-Mortems
- Incident Reviews
- Problem Solving Workshops
- Quality Improvement Workshops
- Lessons Learned Workshops

Can also be used for:

- Architecture Problems
- Delivery Challenges
- Collaboration Issues
- Operational Reliability Reviews

Less suitable for:

- Visioning Workshops
- Strategy Workshops
- Future-State Design Sessions

---

# Outcomes

Expected deliverables:

- Structured view of contributing factors
- Shared understanding of the problem
- Candidate root causes
- Investigation areas
- Improvement opportunities

---

# Duration

| Problem Complexity | Duration |
|----------|----------|
| Simple | 20-30 min |
| Moderate | 30-45 min |
| Complex | 45-60 min |
| Major Incident | 60-90 min |

---

# Materials

Physical workshop:

- Large whiteboard or wall
- Sticky notes
- Markers

Online workshop:

- Miro
- Mural
- Whiteboard

---

# Diagram Structure

The "head" of the fish represents the problem.

Example:

```text
Flights disappear
from sequence
during ETFMS →
Radar transition
```

The "bones" represent categories of potential causes.

Example:

```text
              Process
                 /
                /
People ------ Problem ------ Technology
                \
                 \
               Organization
```

---

# Common Categories

Choose categories relevant to the problem.

## Technical Incidents

Typical categories:

- People
- Process
- Technology
- Data
- Environment
- Monitoring

---

## Software Delivery

Typical categories:

- Requirements
- Design
- Development
- Testing
- Deployment
- Operations

---

## Collaboration Issues

Typical categories:

- Communication
- Governance
- Responsibilities
- Processes
- Tools
- Culture

---

# Instructions

## Step 1 - Define the Problem

Facilitator asks:

> What specific problem are we trying to understand?

The problem should be:

✅ Specific

✅ Observable

✅ Neutral

Avoid:

> Ross delivered poor architecture.

Prefer:

> Architecture deliverables arrived later than expected.

Duration: 5 minutes

---

## Step 2 - Select Categories

Choose categories that fit the context.

Example for a release failure:

```text
Requirements
Design
Development
Testing
Deployment
Operations
```

Draw the fishbone and label each branch.

Duration: 5 minutes

---

## Step 3 - Generate Causes

Ask participants:

> What might have contributed to this problem?

One cause per sticky note.

Examples:

```text
Missing test scenario
```

```text
Unclear requirement
```

```text
Limited operational validation
```

```text
Delayed review
```

Place notes in the most relevant category.

Duration: 10-20 minutes

---

## Step 4 - Explore Causes

For each identified cause ask:

> Why did this happen?

Keep decomposing until sufficient understanding is reached.

Example:

```text
Problem:
Regression escaped testing

↓

Missing test scenario

↓

Transition behavior not explicitly identified

↓

Requirements focused only on intended change

↓

Regression risks not discussed
```

Duration: 15-20 minutes

---

## Step 5 - Identify Patterns

Ask:

- Which categories are most populated?
- What themes emerge?
- Are there dependencies between causes?

Look for clusters.

Examples:

```text
Testing weaknesses
```

```text
Communication gaps
```

```text
Ownership confusion
```

Duration: 10 minutes

---

## Step 6 - Prioritize

Ask participants:

> Which causes have the strongest impact?

Possible techniques:

- Dot voting
- Confidence voting
- Risk assessment

Select the causes that deserve action.

Duration: 10 minutes

---

# Facilitator Tips

## Stay System-Oriented

Prefer:

> What made this possible?

Avoid:

> Who made this mistake?

---

## Distinguish Causes From Symptoms

Example:

### Symptom

```text
Late architecture document
```

### Possible Causes

```text
Unclear ownership
```

```text
Competing priorities
```

```text
No review process
```

---

## Encourage Multiple Perspectives

The first cause proposed is rarely the only cause.

Ask:

> What else contributed?

A strong Fishbone usually reveals several interacting factors.

---

## Use Facts

Whenever possible, connect causes to evidence:

- Emails
- Jira tickets
- Logs
- Timeline events
- Metrics

Avoid relying exclusively on opinions.

---

# Example 1 – AMAN Post-Mortem

## Problem

```text
Flights temporarily disappeared
from the AMAN sequence
```

### Requirements

- ETFMS transition behavior not explicitly covered.

### Design

- Side effects of AMANCH-1194 underestimated.

### Testing

- Missing ETFMS-to-radar scenario.
- Validation focused on intended fix.

### Operations

- Limited opportunity to observe transition behavior.

### Process

- Regression risks not explicitly reviewed.

### Outcome

Root causes identified and translated into actions.

---

# Example 2 – TRACE / Architecture Collaboration

## Problem

```text
TRACE and Architecture experience
collaboration difficulties
```

### Communication

- Response latency.
- Limited feedback loops.

### Governance

- Unclear ownership.
- Escalation path unclear.

### Deliverables

- SAD lifecycle unclear.
- Review expectations not defined.

### Processes

- Developers involved late.

### Culture

- Assumptions not challenged early.

### Outcome

Working agreement and action plan.

---

# Advantages

✅ Simple to facilitate

✅ Encourages systems thinking

✅ Prevents jumping to conclusions

✅ Creates shared understanding

✅ Works well with multidisciplinary groups

---

# Limitations

⚠ Does not prove causality.

⚠ Can generate many hypotheses.

⚠ Requires evidence validation.

⚠ Sometimes identifies contributors rather than true root causes.

---

# Typical Follow-Up Activities

After completing the Fishbone:

```text
Fishbone
↓
Validate Root Causes
↓
Prioritize Findings
↓
Define Actions
↓
Assign Owners
```

---

# Related Techniques

Often combined with:

- Timeline Reconstruction
- Five Whys
- Root Cause Analysis
- Dot Voting
- Circles of Influence
- Lessons Learned

Typical Incident Flow:

```text
Timeline
↓
What Went Well / Poorly
↓
Fishbone Analysis
↓
Five Whys
↓
Actions
```

---

# When to Use

Use when:

✅ A problem has multiple possible causes.

✅ Different stakeholders hold different views.

✅ Understanding the system is more important than identifying an individual mistake.

✅ You need to move from symptoms to causes.

Avoid when:

❌ The objective is future visioning.

❌ The problem is already fully understood.

❌ A simple decision is required rather than analysis.
