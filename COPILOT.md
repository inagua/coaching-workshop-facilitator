# Using Copilot to Build a Workshop from Multiple Sources

Use Copilot as a facilitation co-pilot to transform a collection of project artefacts into a structured workshop design, including a complete 8P Workshop Canvas, workshop agenda, and facilitation strategy.

## Key Principle

Treat Copilot as an **analysis and facilitation partner**, not as an agenda generator.

The most effective approach is:

```text
Documentation
      +
Stakeholder Interviews
      +
Copilot Analysis
      +
Facilitator Expertise
      =
Workshop Design
```

Copilot consolidates information, identifies patterns and challenges assumptions, while the Scrum Master remains responsible for facilitation, stakeholder management and final workshop design decisions.


## Recommended Procedure

### Step 1 – Collect Source Material
Gather all relevant information before engaging Copilot.

### Step 2 – Upload Knowledge Sources

Provide Copilot with all available reference material.

For this workshop, the following categories of documents were uploaded:
* Workshop facilitation framework (8P Workshop Canvas)
* ERE standards and guidelines
* SRE quality management guidelines
* SRS requirements management standards
* Jira describing the workshop objectives and acceptance criteria
* OneNote interview notes collected from stakeholders

Upload all documents before asking Copilot to design the workshop.

With the default free (basic) plan, you can only upload files by 3. You have to merge files or upload in several times if you have more than 3 files. You can maybe separate what are the existing material, your notes and the details of the request for the workshop.


### Step 3 – Establish the Knowledge Base

Ask Copilot to read and analyze all uploaded sources before generating any output.

Example prompt:

```text
These documents constitute the knowledge base for this workshop.
Analyze them and extract:
- context
- stakeholders
- pain points
- objectives
- risks
- dependencies
- recurring themes
```

The objective is to consolidate the information spread across multiple documents into a shared understanding.


### Step 4 – Identify the Appropriate Workshop Type

Once the analysis is complete, ask Copilot to determine the most suitable workshop format.

Example prompt:

```text
Based on all provided sources,
recommend the most appropriate workshop type
(retrospective, lessons learned, collaboration workshop,
post-mortem, process improvement workshop, etc.)
and justify your recommendation.
```

This helps challenge initial assumptions and ensures the workshop format addresses the real problem.

### Step 5 – Complete the 8P Workshop Canvas

Ask Copilot to populate the complete canvas using all available information.

Example prompt:

```text
Using the workshop framework and all uploaded documents,
complete the entire 8P Workshop Canvas.

Highlight:
- assumptions
- missing information
- risks
- potential root causes
```

At this stage, Copilot consolidates information from documentation, interviews and business objectives into a single workshop definition.


### Step 6 – Challenge the Initial Problem Statement

Do not immediately accept the problem described in the Jira or by stakeholders.

Ask Copilot to evaluate whether:
* the stated problem is actually the root cause
* the observed issue is a symptom
* systemic issues may exist behind the reported complaints

Example prompt:

```text
Based on all interview notes and documentation,
what are the likely root causes?
What assumptions should be challenged?
Which reported issues appear to be symptoms rather than causes?
```

This step often provides the highest value.

***

### Step 7 – Design the Workshop Flow

Once the workshop type has been validated, ask Copilot to build a facilitation flow.

Example prompt:

```text
Create a detailed agenda including:
- objectives
- facilitation techniques
- participant instructions
- timeboxes
- expected outputs
```

The workshop should progressively move participants from:

```text
Current State
      ↓
Pain Points
      ↓
Root Causes
      ↓
Future State
      ↓
Improvement Actions
      ↓
Commitments
```


### Step 8 – Validate Against Business Expectations

Compare the generated workshop outputs against the original objectives and acceptance criteria.

Ask Copilot:

```text
Verify that every Jira acceptance criterion
is addressed by a workshop activity and a workshop output.
```

This ensures that the workshop remains outcome-focused rather than becoming a generic discussion session.


### Step 9 – Refine Iteratively

Use follow-up prompts to improve specific sections.

Examples:

```text
Make the agenda more interactive.
```

```text
Challenge the proposed root causes.
```

```text
Identify facilitation risks.
```

```text
Suggest powerful coaching questions.
```

```text
Create participant invitation email.
```

```text
Create workshop report template.
```
