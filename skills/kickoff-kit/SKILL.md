---
name: kickoff-kit
description: --- Takes a project description and generates everything needed for a solid kickoff. Creates a project charter with clear scope...
---

# Kickoff Kit

**Generate a complete project kickoff package—charter, stakeholders, risks, and first milestone breakdown.**

---

## What This Does

Takes a project description and generates everything needed for a solid kickoff. Creates a project charter with clear scope (including what's OUT), maps stakeholders, identifies risks with mitigations, and breaks down the first milestone into actionable tasks.

| Output | What You Get |
|--------|--------------|
| project-charter.md | Scope, goals, constraints, success criteria |
| stakeholder-map.md | Who's involved and what they need |
| risk-register.md | Risks identified with mitigations |
| milestone-1-breakdown.md | First milestone in actionable tasks |

---


---

## IMPORTANT: Always Ask First

When the user says "ready to work", "get to work", or loads this folder:

1. **Greet and explain** what this skill does
2. **Ask what they need**:
   > "I can help you with [skill purpose]. Would you like to:
   > 1. **Start fresh** - I'll guide you through what I need
   > 2. **Use files in input/** - I'll process what you've added
   > 3. **See an example** - I'll show you what this produces"

3. **Never auto-run** without confirming what the user wants

### Why This Matters
Users loading a skill folder expect guidance, not assumptions. Always confirm before processing.

## Quick Start

### Option 1: Natural Language
> "Create a kickoff kit for our new mobile app project"

### Option 2: With Brief
> "Run kickoff kit on the project brief in input/"

### Option 3: Interactive
> "Help me plan a new project kickoff"

---

## What I Need From You

### Required
- **Project concept**: What are you trying to build/achieve?
- **Goals**: What does success look like?

### Optional (Enhances Output)
- **Constraints**: Budget, timeline, team size
- **Stakeholders**: Who's involved or affected
- **Known risks**: Concerns you already have
- **Similar projects**: Past projects for context

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Templates | Your org's kickoff templates | Best-practice defaults |
| None required | Works standalone | Complete kit generated |

---

## Output Location

```
output/
├── project-charter.md        # Project definition
├── stakeholder-map.md        # Who's involved
├── risk-register.md          # Risks and mitigations
└── milestone-1-breakdown.md  # First sprint/phase
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Project Dashboard** | Live overview with health score, milestones, risks | "Create a project dashboard artifact" |
| **Stakeholder Tracker** | Interactive RACI matrix with alignment status | "Build a stakeholder tracker I can update" |
| **Risk Heatmap** | Visual risk matrix (likelihood × impact) you can modify | "Make an interactive risk heatmap" |
| **Milestone Tracker** | Progress checklist with completion percentage | "Create a milestone tracker artifact" |

### Example Artifact Requests

**Project Dashboard**
> "Create a React artifact dashboard showing: project health score, milestone progress bar, top 3 risks, and upcoming deadlines"

**Stakeholder Tracker**
> "Build an interactive stakeholder table where I can track who I've aligned with and who still needs outreach"

**Milestone Kanban**
> "Create a Kanban-style artifact showing Milestone 1 tasks that I can drag between To Do, In Progress, and Done"

### Tips
- Artifacts persist in your conversation—return to update them as the project evolves
- Ask Claude to "update the dashboard with new status" after check-ins
- Request "exportable" versions for sharing outside Claude

---

## Examples

### Example 1: Software Project
**Input**: "Build an internal dashboard for sales metrics"

**Output**:
- Charter: Goals, features, tech stack assumptions, OUT of scope
- Stakeholders: Sales team, IT, leadership + their needs
- Risks: Data quality, adoption, scope creep
- Milestone 1: Requirements gathering breakdown

### Example 2: Business Initiative
**Input**: "Launch a customer referral program"

**Output**:
- Charter: Objectives, success metrics, program structure
- Stakeholders: Marketing, sales, legal, customers
- Risks: Low participation, fraud, operational complexity
- Milestone 1: Program design tasks

### Example 3: Process Improvement
**Input**: "Streamline our onboarding process"

**Output**:
- Charter: Current state, goals, constraints
- Stakeholders: HR, managers, new hires, IT
- Risks: Resistance to change, missing edge cases
- Milestone 1: Discovery and mapping tasks

---

## What I Won't Do

- **Won't skip OUT of scope**: Every charter explicitly states what's not included
- **Won't ignore risks**: Surface them even if uncomfortable
- **Won't create >2-week milestones**: Breaks down into manageable chunks
- **Won't assume unlimited resources**: Work within stated constraints
- **Won't forget stakeholders**: Include all affected parties

---

## Tips for Best Results

1. **State constraints clearly**: Budget, timeline, team matter for scoping
2. **Include known concerns**: Your instincts about risks are valuable
3. **Be explicit about scope**: "Does NOT include X" prevents creep
4. **Share org context**: How do projects typically run here?
5. **Name stakeholders**: Specific people vs. generic roles when possible

---

## Troubleshooting

### "Scope is too broad/narrow"
Adjust: "Make scope more focused" or "This is a bigger initiative than shown."

### "Missing stakeholders"
Add them: "Also include [stakeholder] who cares about [interest]."

### "Risks don't seem relevant"
Share more context about your environment and what typically goes wrong.

### "Milestones too large"
Specify: "Break milestones into 1-week chunks maximum."

---

*Part of Art of Fact Cowork Skill Library*
