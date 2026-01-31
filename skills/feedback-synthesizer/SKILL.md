---
name: feedback-synthesizer
description: --- Takes feedback scattered across sources—survey responses, emails, Slack messages, review comments—and synthesizes it into actionable patterns. Distinguishes signal from...
---

# Feedback Synthesizer

**Combine feedback from multiple sources into patterns, priorities, and response drafts.**

---

## What This Does

Takes feedback scattered across sources—survey responses, emails, Slack messages, review comments—and synthesizes it into actionable patterns. Distinguishes signal from noise, preserves original voices through quotes, identifies priority improvements, and drafts responses for key feedback.

| Output | What You Get |
|--------|--------------|
| feedback-synthesis.md | Themes, patterns, and prioritized insights |
| quotes-by-theme.md | Original feedback organized by topic |
| priority-improvements.md | Ranked action items from feedback |
| response-drafts/ | Draft responses to key feedback |

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
> "Synthesize the feedback from our customer survey"

### Option 2: With Files
> "Run feedback synthesizer on files in input/"

### Option 3: Specific Source
> "Analyze the feedback from this email thread"

---

## What I Need From You

### Required
- **Feedback sources**: The raw feedback to analyze (files, paste, or describe)

### Optional (Enhances Output)
- **Context**: What was the feedback about? (product, project, presentation)
- **Source attribution**: Who gave what feedback (if you want to respond)
- **Priority criteria**: What matters most in prioritizing responses
- **Response requirements**: Which feedback needs responses

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Local Files | Feedback documents in input folder | You provide content |
| Email | Feedback threads | Manual copy-paste |
| Slack | Channel discussions | Export or copy |

---

## Output Location

```
output/
├── feedback-synthesis.md      # Complete analysis
├── quotes-by-theme.md         # Original quotes organized
├── priority-improvements.md   # Action items ranked
└── response-drafts/
    ├── response-[name].md     # Individual responses
    └── bulk-response.md       # Template for common feedback
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Feedback Dashboard** | Visual overview of themes, sentiment, and volume | "Create a feedback dashboard artifact" |
| **Theme Explorer** | Interactive view of feedback grouped by topic | "Build a theme explorer artifact" |
| **Priority Matrix** | Plot improvements by impact and effort | "Make a priority matrix artifact" |
| **Response Tracker** | Track which feedback needs responses and status | "Create a response tracker artifact" |

### Example Artifact Requests

**Feedback Dashboard**
> "Create a React dashboard showing: sentiment breakdown (pie chart), top themes (bar chart), and feedback volume over time"

**Theme Explorer**
> "Build an interactive artifact where I can click on a theme and see all the quotes and feedback in that category"

**Priority Matrix**
> "Create a 2x2 matrix with Impact (low/high) and Effort (low/high)—let me drag improvement items into quadrants"

### Tips
- Use the dashboard to present feedback findings to stakeholders
- The theme explorer helps you understand the "why" behind patterns
- Update the response tracker as you address feedback

---

## Examples

### Example 1: Customer Survey
**Input**: 50 survey responses (mix of ratings and comments)

**Output**:
- Themes: "Performance" (mentioned 23x), "Documentation" (18x), "Pricing" (12x)
- Sentiment: 72% positive, 18% neutral, 10% negative
- Priority improvements: Top 3 with impact and effort estimates
- Quotes: Best representative quotes per theme
- Response drafts: For negative feedback requiring follow-up

### Example 2: Project Retrospective
**Input**: Team feedback from sprint retro

**Output**:
- What worked: Patterns in positive feedback
- What didn't: Patterns in challenges
- Suggested experiments: From team recommendations
- Priority: Ranked by frequency and impact
- Response: Summary to share back with team

### Example 3: Performance Review Feedback
**Input**: 360 review comments from 8 reviewers

**Output**:
- Strengths: Consistent themes
- Growth areas: Patterns in development feedback
- Outliers: Single-mention items (note but don't overweight)
- Quotes: De-identified if needed
- Action items: Personal development priorities

---

## What I Won't Do

- **Won't dismiss negative feedback**: All feedback surfaced honestly
- **Won't over-weight loud voices**: One person repeating ≠ pattern
- **Won't identify anonymous respondents**: Preserve stated anonymity
- **Won't fabricate patterns**: If feedback is scattered, I'll say so
- **Won't auto-send responses**: Drafts only, you review and send

---

## Tips for Best Results

1. **Include all feedback**: Don't pre-filter—let synthesis reveal priorities
2. **Note source context**: "This is from customers" vs "from engineers" matters
3. **Specify if anonymous**: Handling differs for attributed vs. anonymous
4. **Share your constraints**: "We can only address 2 items" focuses prioritization
5. **Indicate response needs**: "Need to respond to [specific person]"

---

## Troubleshooting

### "Themes feel wrong"
Provide more context about what the feedback is about. Domain context shapes theme identification.

### "Missing important feedback"
Ensure all sources are included. I synthesize what I receive—can't surface what's not provided.

### "Priorities don't match my sense"
Tell me your prioritization criteria: "Impact matters more than frequency" or "Leadership concerns are high priority."

### "Responses are too generic"
Provide context about your relationship with the feedback giver. Personal context enables personal responses.

---

*Part of Art of Fact Cowork Skill Library*
