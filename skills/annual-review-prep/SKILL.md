---
name: annual-review-prep
description: --- Scans your year's calendar, email, notes, and completed work to compile comprehensive accomplishments. Generates a self-review draft, brag document,...
---

# Annual Review Prep

**Compile a year's accomplishments into self-review and brag doc ready for performance reviews.**

---

## What This Does

Scans your year's calendar, email, notes, and completed work to compile comprehensive accomplishments. Generates a self-review draft, brag document, and metrics summary. Captures wins you've forgotten and praise you've received.

| Output | What You Get |
|--------|--------------|
| self-review-draft.md | Performance review ready |
| accomplishments-by-theme.md | Organized wins |
| brag-document.md | Shareable achievement summary |
| metrics-summary.md | Quantified impact |

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
> "Compile my accomplishments for 2024"

### Option 2: With Date Range
> "Prepare my annual review covering January to December"

### Option 3: Focused
> "What were my biggest wins this year?"

---

## What I Need From You

### Required
- **Time period**: What year/period to cover
- **Data sources**: Calendar, email, notes, or description

### Optional (Enhances Output)
- **Goals from start of year**: What you were measured against
- **Praise received**: Kudos, thank-you emails, recognition
- **Role context**: Your title and responsibilities
- **Review format**: Your company's self-review template

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Calendar | Projects, milestones, meetings led | Manual input |
| Email | Praise, project threads, completions | Manual input |
| Notes | Documented accomplishments | Manual input |

---

## Output Location

```
output/
├── self-review-draft.md         # Review-ready document
├── accomplishments-by-theme.md  # Organized wins
├── brag-document.md             # Shareable version
└── metrics-summary.md           # Quantified impact
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Accomplishment Tracker** | Log wins throughout the year, categorized by theme | "Create an accomplishment tracker artifact" |
| **Brag Doc Builder** | Interactive form to build your brag document | "Build a brag doc artifact I can update" |
| **Impact Dashboard** | Visualize metrics and quantified achievements | "Make an impact metrics dashboard" |
| **Career Timeline** | Visual timeline of major milestones and growth | "Create a career timeline artifact" |

### Example Artifact Requests

**Accomplishment Tracker**
> "Create a React artifact where I can log accomplishments with date, category (Leadership/Technical/Delivery/Mentoring), and impact notes"

**Impact Dashboard**
> "Build a dashboard showing my key metrics: projects delivered, people mentored, revenue influenced, processes improved"

**Praise Collector**
> "Create an artifact where I can paste praise/kudos I receive and tag them by source and theme"

### Tips
- Start your accomplishment tracker at the beginning of the year—don't wait until review time
- Update monthly to capture wins while they're fresh
- Use the brag doc artifact for promotions, job interviews, and LinkedIn updates too

---

## Examples

### Example 1: Engineering IC Review
**Input**: Year of calendar + email + project notes

**Output**:
- 47 accomplishments identified
- Themes: Technical leadership, mentoring, delivery, innovation
- Metrics: 3 major launches, 2 team processes improved, 12 PRs mentored
- Praise: 8 recognition emails surfaced

### Example 2: Manager Review
**Input**: Calendar + team notes + OKRs

**Output**:
- Team accomplishments: 4 promotions supported, 12 projects shipped
- Personal leadership: 2 processes created, hiring program built
- Metrics: 15% team velocity improvement, 4.2 engagement score

### Example 3: Quick Prep
**Input**: Verbal summary of year

**Output**:
- Structured themes from description
- Suggestions for metrics to add
- Self-review draft framework

---

## What I Won't Do

- **Won't fabricate accomplishments**: Only surface what happened
- **Won't inflate metrics**: Honest quantification only
- **Won't exaggerate**: Accurate representation of impact
- **Won't include confidential info**: You control what's shared
- **Won't write fiction**: Real accomplishments, your words

---

## Tips for Best Results

1. **Save praise year-round**: Forward kudos to a folder
2. **Note completions**: Quick log when projects ship
3. **Track metrics**: Numbers are powerful in reviews
4. **Include stretch work**: Projects beyond your role
5. **Run before needed**: Prep takes time, don't rush

---

## Troubleshooting

### "Missing accomplishments"
Scan email sent folder for project completions. Check calendar for milestones.

### "Hard to quantify impact"
Look for: time saved, revenue influenced, people helped, errors prevented.

### "Format doesn't match our template"
Provide your company's template and I'll match it.

### "Too many/few items"
Specify: "Focus on top 10 accomplishments" or "Include everything."

---

*Part of Art of Fact Cowork Skill Library*
