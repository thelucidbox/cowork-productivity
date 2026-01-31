---
name: scope-creep-detector
description: --- Takes your original project specification and compares it to current state. Identifies what's changed, distinguishes legitimate clarification from scope...
---

# Scope Creep Detector

**Compare original spec to current state, quantify drift, and generate renegotiation points.**

---

## What This Does

Takes your original project specification and compares it to current state. Identifies what's changed, distinguishes legitimate clarification from scope creep, quantifies the impact, and generates talking points for renegotiating timeline, budget, or scope.

| Output | What You Get |
|--------|--------------|
| scope-analysis.md | Original vs current comparison |
| drift-items.md | Each change categorized |
| impact-assessment.md | Time/cost/resource impact |
| renegotiation-points.md | Talking points for discussion |

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
> "Compare our original project spec to where we are now"

### Option 2: With Files
> "Run scope creep detector on original-spec.md and current-state.md"

### Option 3: Interactive
> "Help me identify if we're experiencing scope creep"

---

## What I Need From You

### Required
- **Original spec**: What was agreed initially
- **Current state**: What's now expected/being built

### Optional (Enhances Output)
- **Change requests**: Documented changes along the way
- **Original timeline/budget**: For impact calculation
- **Stakeholder context**: Who requested changes

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Local Files | Specs from input folder | Paste directly |
| None required | Works standalone | Manual comparison |

---

## Output Location

```
output/
├── scope-analysis.md        # Full comparison
├── drift-items.md           # Categorized changes
├── impact-assessment.md     # Quantified impact
└── renegotiation-points.md  # Talking points
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Scope Drift Tracker** | Visual comparison of original vs current scope | "Create a scope drift artifact" |
| **Impact Calculator** | Calculate time/cost impact of scope changes | "Build an impact calculator artifact" |
| **Change Log** | Track all scope changes with who requested and why | "Make a change log artifact" |
| **Renegotiation Dashboard** | Prepare talking points with data visualization | "Create a renegotiation prep artifact" |

### Example Artifact Requests

**Scope Drift Visualizer**
> "Create a React artifact showing original features vs current features as two columns, with connecting lines showing what changed"

**Impact Calculator**
> "Build a calculator where I can input: original timeline, scope increase %, and see estimated new timeline and cost impact"

**Change Log**
> "Create a tracker for scope changes with: change description, date, requester, category (clarification/new scope/removed), and impact"

### Tips
- Use the scope drift artifact in stakeholder meetings to objectively show what changed
- The impact calculator helps translate "we added X" into "this costs Y days"
- Keep the change log updated as requests come in—don't wait until there's a problem

---

## Examples

### Example 1: Software Project
**Input**: Original PRD vs current feature list

**Output**:
- Original: 12 features, 8-week timeline
- Current: 18 features, same timeline
- Drift: 6 features added (50% increase)
- Impact: Estimated 4 additional weeks
- Renegotiation: Extend timeline or cut 4 features

### Example 2: Service Engagement
**Input**: Original SOW vs actual work done

**Output**:
- Original: 40 hours/month, defined deliverables
- Current: 60 hours/month, expanded deliverables
- Drift: 50% more effort
- Impact: $X additional cost
- Renegotiation: Revise rate or scope down

### Example 3: Ongoing Project
**Input**: Initial charter vs current expectations

**Output**:
- Drift categories: Clarification (3), New scope (7), Removed (1)
- Net change: 35% larger scope
- Options presented: Timeline extension, team expansion, scope reduction

---

## What I Won't Do

- **Won't hide creep**: Surface all changes honestly
- **Won't assume malice**: Changes often reflect learning
- **Won't recommend without options**: Provide choices, not mandates
- **Won't ignore legitimate clarification**: Distinguish from true creep
- **Won't make it adversarial**: Frame for productive discussion

---

## Tips for Best Results

1. **Find the original doc**: The actual signed/approved spec matters
2. **Document current state clearly**: What's actually expected now
3. **Include change history**: How did we get here?
4. **Note who requested**: Helps context but not blame
5. **Know your constraints**: Can you extend timeline? Add resources?

---

## Troubleshooting

### "No clear original spec"
Start from earliest documentation. Note that baseline is fuzzy—this itself is a finding.

### "Changes seem reasonable"
They may be! Classify as "clarification" vs "new scope." Both are valid, but one needs renegotiation.

### "Don't want to create conflict"
Frame as "alignment discussion" not "confrontation." Everyone benefits from clear scope.

### "Stakeholder disputes the analysis"
Show specific comparisons. "Original said X, current includes Y" is factual.

---

*Part of Art of Fact Cowork Skill Library*
