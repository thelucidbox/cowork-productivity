---
name: weekly-momentum-report
description: --- Takes all your notes, calendar events, and completed tasks from the week and transforms them into an actionable momentum...
---

# Weekly Momentum Report

**Synthesize your week's scattered notes into wins, blockers, patterns, and priorities.**

---

## What This Does

Takes all your notes, calendar events, and completed tasks from the week and transforms them into an actionable momentum report. Surfaces what worked, what's stuck, identifies patterns you might miss, and recommends priorities for next week based on actual data.

| Output | What You Get |
|--------|--------------|
| weekly-momentum.md | Complete synthesis: wins, blockers, patterns, priorities, energy audit |
| wins.md | Accomplishments formatted for sharing/brag doc |
| blockers.md | Stuck items with suggested unblocking strategies |
| next-week-priorities.md | Recommended focus areas for coming week |

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
> "Generate my weekly momentum report"

### Option 2: With Notes Folder
> "Run weekly momentum on my notes from this week"

### Option 3: Manual Mode
> "Help me review my week and plan next week"

---

## What I Need From You

### Required
- **Week's notes**: Daily notes, meeting notes, task lists from the week
- **Week boundary**: Which week (defaults to current/just-ended week)

### Optional (Enhances Output)
- **Current goals**: What you're working toward (quarterly OKRs, project goals)
- **Energy ratings**: How you felt each day (if you track this)
- **Last week's report**: For continuity and pattern tracking

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Local Files | Notes from specified folder | You provide notes directly |
| Calendar | Meeting load, time allocation | Manual estimation |
| Email | Communication volume, thread counts | Skip email analysis |
| Previous Reports | Trends over time | Single-week analysis |

---

## Output Location

```
output/
├── weekly-momentum.md        # Complete report
├── wins.md                   # Accomplishments
├── blockers.md               # Stuck items + strategies
└── next-week-priorities.md   # Recommended focus
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Weekly Dashboard** | Live overview of wins, blockers, and priorities | "Create a weekly momentum dashboard" |
| **Energy Tracker** | Log and visualize daily energy levels over time | "Build an energy tracking artifact" |
| **Blocker Board** | Kanban for blocked items with unblocking strategies | "Make a blocker tracker artifact" |
| **Priority Matrix** | Eisenhower matrix for prioritizing next week | "Create a priority matrix artifact" |

### Example Artifact Requests

**Weekly Dashboard**
> "Create a React dashboard showing: this week's wins (list), active blockers (with status), energy trend (sparkline), and top 3 priorities for next week"

**Energy Tracker**
> "Build an artifact where I can rate my energy 1-10 each day and see patterns over weeks"

**Blocker Board**
> "Create a Kanban with columns: Blocked, Unblocking, Resolved—let me track what's stuck and what I did about it"

### Tips
- Run the weekly dashboard every Friday to close out the week
- Energy patterns become visible after 3-4 weeks of tracking
- Keep the blocker board updated—celebrate when things move to Resolved

---

## Examples

### Example 1: Standard Week Review
**Input**: Folder of daily notes + calendar access

**Output**:
- Wins: 4 accomplishments identified and quantified
- Blockers: 2 items stuck, each with 2 suggested unblocking moves
- Patterns: "Most productive on Tuesday mornings; meetings cluster Wednesday"
- Priorities: Top 3 focus areas based on momentum and blockers

### Example 2: With Energy Tracking
**Input**: Notes include energy ratings (1-10 per day)

**Output**:
- Standard report plus:
- Energy audit: Average 6.2, peaked Thursday, dipped Monday
- Pattern: "Energy drops after back-to-back meetings"
- Suggestion: "Block recovery time after meeting-heavy days"

### Example 3: Quarterly Context
**Input**: Weekly notes + Q1 OKRs document

**Output**:
- Wins mapped to OKR progress
- Blockers assessed by goal impact
- Priorities weighted by quarterly importance
- Progress summary: "On track for 2/4 key results"

---

## What I Won't Do

- **Won't fabricate accomplishments**: Only capture what's in your notes
- **Won't minimize blockers**: Surface honestly, not dismissively
- **Won't overpromise next week**: Recommendations based on realistic capacity
- **Won't share your data**: Analysis is private to your session
- **Won't replace reflection**: Augments, not replaces, your own thinking

---

## Tips for Best Results

1. **Consistent note location**: Keep week's notes in predictable place
2. **Include micro-wins**: Small completions count toward momentum
3. **Note frustrations**: "Stuck on X" becomes a blocker to address
4. **Track energy casually**: Even "good day / rough day" notes help
5. **Run same time weekly**: Friday afternoon or Sunday evening works well

---

## Troubleshooting

### "Wins feel thin"
Your notes may not capture completions. Try:
- Reviewing sent emails for things you finished
- Checking calendar for meetings that moved projects forward
- Noting even small progress as wins

### "Patterns aren't accurate"
More data = better patterns. Run for 3-4 weeks to see meaningful trends. Single weeks show snapshots, not patterns.

### "Too many priorities"
Specify constraints: "I can only focus on 2-3 things" and I'll ruthlessly prioritize.

### "Blockers feel overwhelming"
Ask for "one move per blocker" to get actionable next steps rather than comprehensive solutions.

---

*Part of Art of Fact Cowork Skill Library*
