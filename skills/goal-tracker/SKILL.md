---
name: goal-tracker
description: --- Takes your goals and progress notes, then generates a comprehensive status dashboard. Tracks trajectory (not just current state), distinguishes...
---

# Goal Tracker

**Analyze goals against progress notes to generate status dashboards and recommendations.**

---

## What This Does

Takes your goals and progress notes, then generates a comprehensive status dashboard. Tracks trajectory (not just current state), distinguishes blocked goals from abandoned ones, and provides specific recommendations for getting unstuck.

| Output | What You Get |
|--------|--------------|
| goal-dashboard.md | Visual status of all goals |
| recommendations.md | Specific actions to take |
| next-actions.md | Prioritized to-do list |

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
> "Check my goal progress"

### Option 2: With Files
> "Analyze my Q1 goals against my weekly notes"

### Option 3: Specific Goal
> "How am I doing on my fitness goal?"

---

## What I Need From You

### Required
- **Goals**: Your stated goals (OKRs, personal goals, projects)
- **Progress notes**: Evidence of activity (notes, completed tasks)

### Optional (Enhances Output)
- **Timeline**: When do goals need to be achieved?
- **Priority ranking**: Which goals matter most?
- **Blockers**: Known obstacles

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Local Files | Goals and notes from input | Paste directly |

---

## Output Location

```
output/
├── goal-dashboard.md     # Visual status
├── recommendations.md    # What to do
└── next-actions.md       # Prioritized tasks
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Goal Dashboard** | Visual status of all goals with progress bars | "Create a goal dashboard artifact" |
| **Progress Tracker** | Log progress entries and see trends | "Build a progress tracker artifact" |
| **OKR Scorecard** | Track objectives and key results with scores | "Make an OKR scorecard artifact" |
| **Habit Tracker** | Daily/weekly habit completion grid | "Create a habit tracker artifact" |

### Example Artifact Requests

**Goal Dashboard**
> "Create a React dashboard showing each goal with: name, progress bar (0-100%), status (on-track/at-risk/behind), and days remaining"

**Progress Logger**
> "Build an artifact where I can log progress updates for each goal and see a chart of my trajectory over time"

**OKR Scorecard**
> "Create an interactive OKR tracker with objectives, key results, confidence scores, and overall objective health"

### Tips
- Update the dashboard weekly to maintain accurate status
- Use the progress tracker to celebrate small wins
- Review the OKR scorecard monthly to adjust strategies

---

## Examples

### Example 1: Quarterly OKRs
**Input**: Q1 OKRs + weekly progress notes

**Output**:
- Dashboard: 3 on-track, 2 at-risk, 1 unlikely
- Trajectory: "Revenue KR accelerating, Hiring KR stalled"
- Recommendations: Specific actions for at-risk goals

### Example 2: Personal Goals
**Input**: Annual goals + monthly check-ins

**Output**:
- Health: On track (consistent gym notes)
- Reading: Behind (2 books vs 4 target)
- Side project: Stalled (no activity in 6 weeks)
- Recommendations per goal

### Example 3: Project Milestones
**Input**: Project milestones + task completion log

**Output**:
- Phase 1: Complete
- Phase 2: In progress (70%)
- Phase 3: Not started (on schedule)
- Risk flags and recommendations

---

## What I Won't Do

- **Won't inflate progress**: Honest assessment only
- **Won't hide stalled goals**: Surface the uncomfortable truth
- **Won't guess at blockers**: Ask if unclear
- **Won't set goals for you**: Track what you define
- **Won't make you feel bad**: Constructive, not judgmental

---

## Tips for Best Results

1. **Define goals clearly**: Measurable targets enable accurate tracking
2. **Note progress regularly**: Weekly updates beat monthly reviews
3. **Include context**: "Missed due to illness" explains gaps
4. **Be honest about abandonment**: Some goals should be dropped
5. **Review quarterly**: Long enough for patterns, short enough to adjust

---

## Troubleshooting

### "Goals aren't tracked accurately"
Provide more specific metrics. "Get fit" can't be tracked; "Gym 3x/week" can.

### "Missing progress"
Check that progress notes are in expected location. Note activity explicitly.

### "Recommendations aren't helpful"
Share more context about constraints and what's blocking you.

### "Dashboard too complex"
Ask for "simple view" with just status, no analysis.

---

*Part of Art of Fact Cowork Skill Library*
