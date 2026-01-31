---
name: energy-audit
description: --- Analyzes your calendar, notes, and self-reported energy to identify patterns. Shows where your time actually goes versus where you...
---

# Energy Audit

**Analyze time and energy patterns to suggest schedule optimizations.**

---

## What This Does

Analyzes your calendar, notes, and self-reported energy to identify patterns. Shows where your time actually goes versus where you think it goes, correlates energy levels with activities, and suggests schedule optimizations.

| Output | What You Get |
|--------|--------------|
| energy-audit.md | Complete time and energy analysis |
| patterns.md | Identified patterns |
| optimization-suggestions.md | Schedule recommendations |

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
> "Audit my energy for the last month"

### Option 2: With Calendar
> "Analyze where my time goes"

### Option 3: Focused Analysis
> "When am I most productive?"

---

## What I Need From You

### Required
- **Calendar access**: To see time allocation
- **Or**: Time log/notes about how you spend time

### Optional (Enhances Output)
- **Energy ratings**: Daily or activity-level energy notes
- **Productivity notes**: What felt effective vs. draining
- **Goals**: What you want to optimize for

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Calendar | Meeting times, categories | Manual time log |
| Notes | Energy mentions, productivity notes | Ask for input |

---

## Output Location

```
output/
├── energy-audit.md              # Full analysis
├── patterns.md                  # What I found
└── optimization-suggestions.md  # What to change
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Energy Dashboard** | Visualize energy levels and patterns over time | "Create an energy dashboard artifact" |
| **Daily Logger** | Quick energy rating input with notes | "Build an energy logger artifact" |
| **Time Allocation Chart** | See where your time actually goes | "Make a time allocation artifact" |
| **Optimization Tracker** | Track schedule changes and their impact | "Create an optimization tracker artifact" |

### Example Artifact Requests

**Energy Dashboard**
> "Create a React dashboard showing: daily energy trend (line chart), best/worst times (heat map), and correlation with meeting load"

**Quick Logger**
> "Build a simple artifact where I can rate my energy 1-10 each day, add optional notes, and see my weekly average"

**Time Pie Chart**
> "Create an interactive chart showing how I actually spend my time: meetings, focus, admin, breaks—based on my calendar"

### Tips
- Log energy at the same time each day for consistency
- Look for patterns after 3-4 weeks of data
- Test one optimization at a time to see what works

---

## Examples

### Example 1: Work Week Analysis
**Input**: Calendar + energy notes for one month

**Output**:
- Time allocation: 40% meetings, 30% focus, 20% admin, 10% breaks
- Energy pattern: Peaks Tuesday morning, dips Wednesday afternoon
- Insight: Back-to-back meetings correlate with low afternoon energy
- Suggestion: Buffer meetings, protect Tuesday mornings

### Example 2: Meeting Load
**Input**: Calendar access

**Output**:
- Meeting hours: 22 hours/week average
- Meeting-free days: 0 last month
- Longest focus block: 2 hours
- Suggestion: Institute no-meeting Thursdays

### Example 3: Energy Tracking
**Input**: Daily energy logs (1-10)

**Output**:
- Average: 6.2
- Best days: Tuesday (7.1), Thursday (6.8)
- Worst: Monday (5.4), Friday afternoon (4.2)
- Correlations: Sleep, exercise, meeting load

---

## What I Won't Do

- **Won't judge**: Descriptive, not prescriptive
- **Won't assume causes**: Correlation noted, causation you determine
- **Won't mandate changes**: Suggestions only
- **Won't track without your data**: Only analyze what you provide
- **Won't share data**: Analysis stays private

---

## Tips for Best Results

1. **Track energy simply**: Even "good/bad/meh" is useful
2. **Include calendar notes**: Meeting titles help categorize
3. **Note sleep and exercise**: Strong energy correlations
4. **Provide context**: "January was unusual because..."
5. **Analyze monthly**: Weekly is too noisy

---

## Troubleshooting

### "Patterns don't seem right"
More data helps. One week is noisy; one month shows patterns.

### "Calendar doesn't reflect reality"
Add notes about actual activities, not just scheduled ones.

### "Suggestions aren't practical"
Share constraints: "I can't move the Monday meeting."

### "Energy tracking is tedious"
Simplify: Just morning energy rating, or just after meetings.

---

*Part of Art of Fact Cowork Skill Library*
