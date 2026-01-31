---
name: knowledge-capture
description: --- Takes a problem you just solved and transforms it into a searchable, reusable knowledge base article. Captures the problem,...
---

# Knowledge Capture

**Transform any solved problem into a reusable knowledge base article.**

---

## What This Does

Takes a problem you just solved and transforms it into a searchable, reusable knowledge base article. Captures the problem, context, solution, and gotchas so future-you (or teammates) can solve it instantly next time. Creates institutional knowledge from daily work.

| Output | What You Get |
|--------|--------------|
| kb-article.md | Complete knowledge base article |
| quick-reference.md | TL;DR cheat sheet version |
| related-articles.md | Links to similar knowledge |

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
> "Capture how I fixed the API timeout issue"

### Option 2: From Notes
> "Turn my troubleshooting notes into a KB article"

### Option 3: Post-Solution
> "I just solved [problem], help me document it"

---

## What I Need From You

### Required
- **The problem**: What was broken/confusing?
- **The solution**: What fixed it?

### Optional (Enhances Output)
- **Context**: When does this occur?
- **Symptoms**: How did you know there was a problem?
- **Failed attempts**: What didn't work?
- **Root cause**: Why did this happen?
- **Prevention**: How to avoid in future?

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Existing KB | Related articles to link | Standalone article |
| None required | Works standalone | Full article created |

---

## Output Location

```
output/
├── kb-article.md       # Full article
├── quick-reference.md  # TL;DR version
└── related-articles.md # Cross-references
```

---

## Examples

### Example 1: Technical Fix
**Input**: "Fixed the issue where API calls time out. Needed to increase the connection pool size in config."

**Output**:
- KB article: Problem, symptoms, root cause, solution with code
- Quick reference: One-line fix
- Tags: api, timeout, configuration

### Example 2: Process Problem
**Input**: "Finally figured out why expenses weren't getting approved—the workflow skips finance if under $100."

**Output**:
- KB article: Workflow explanation, when it applies, how to check
- Quick reference: Approval thresholds table
- Tags: expenses, approvals, workflow

### Example 3: Common Error
**Input**: "Team keeps hitting this npm error. Fix is to clear node_modules and reinstall."

**Output**:
- KB article: Error message, causes, step-by-step fix
- Quick reference: Commands to run
- Tags: npm, node, dependencies

---

## What I Won't Do

- **Won't assume context**: If unclear, I'll ask
- **Won't skip gotchas**: Failed attempts are valuable
- **Won't over-complicate**: Simple problems get simple articles
- **Won't make up solutions**: Only document what actually worked
- **Won't publish**: Creates article, you review and add to KB

---

## Tips for Best Results

1. **Capture immediately**: Details fade fast after solving
2. **Include the error message**: Exact text helps searchability
3. **Note what didn't work**: Saves future troubleshooters time
4. **Add context**: "After upgrading to v2.0" helps others recognize situation
5. **Think about search terms**: What would you have searched?

---

## Troubleshooting

### "Article is too technical/simple"
Specify your audience: "This is for developers" vs "This is for end users."

### "Missing important details"
Provide more context. Walk through the problem chronologically.

### "Too long for a KB article"
Ask for "brief version" or I'll split into overview + detailed sections.

### "Need specific format"
Share your KB template if you have one.

---

*Part of Art of Fact Cowork Skill Library*
