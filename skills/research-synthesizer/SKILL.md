---
name: research-synthesizer
description: --- Takes multiple research sources—web searches, PDFs, documents—and synthesizes them into a coherent executive brief. Every claim is cited, conflicting...
---

# Research Synthesizer

**Combine research from web and documents into a cited executive brief.**

---

## What This Does

Takes multiple research sources—web searches, PDFs, documents—and synthesizes them into a coherent executive brief. Every claim is cited, conflicting sources are flagged, and fact is distinguished from opinion. Transforms research chaos into actionable intelligence.

| Output | What You Get |
|--------|--------------|
| research-brief.md | Executive summary with citations |
| source-comparison.md | How sources agree/disagree |
| findings.md | Detailed findings by topic |
| sources/ | Organized source materials |

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
> "Research the current state of remote work tools and synthesize findings"

### Option 2: With Sources
> "Synthesize the research materials in input/"

### Option 3: Specific Question
> "Research: What's the best approach to API rate limiting?"

---

## What I Need From You

### Required
- **Research topic or question**: What do you want to understand?
- **Sources**: Web search, documents, or both

### Optional (Enhances Output)
- **Angle**: What specific aspect matters most?
- **Audience**: Who is this brief for?
- **Depth**: Quick overview vs. comprehensive
- **Known sources**: Specific documents to include

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Web Search | Current information, multiple perspectives | Document-only synthesis |
| Local Files | PDFs, reports, documents you provide | Web-only research |

---

## Output Location

```
output/
├── research-brief.md      # Executive summary
├── source-comparison.md   # Agreement/disagreement
├── findings.md            # Detailed breakdown
└── sources/
    └── [organized sources]
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Research Dashboard** | Overview of findings with key insights and source count | "Create a research dashboard artifact" |
| **Source Comparison Chart** | Visual matrix showing where sources agree/conflict | "Build a source comparison artifact" |
| **Findings Explorer** | Interactive cards for each key finding with citations | "Make a findings explorer artifact" |
| **Citation Tracker** | Manage sources with credibility ratings and notes | "Create a citation tracker artifact" |

### Example Artifact Requests

**Research Dashboard**
> "Create a React dashboard showing: research question, key findings (ranked by confidence), source count, and areas needing more research"

**Source Comparison Matrix**
> "Build an interactive matrix showing how my 5 sources agree or disagree on the key questions"

**Findings Explorer**
> "Create a card-based artifact where each finding has: summary, supporting sources, confidence level, and my notes"

### Tips
- Use the source comparison artifact to identify gaps and conflicts before writing
- The findings explorer helps when presenting research to stakeholders
- Update the citation tracker as you discover new sources

---

## Examples

### Example 1: Market Research
**Input**: "Research competitors in the AI writing space"

**Output**:
- Brief: Landscape overview, key players, differentiation
- Source comparison: Pricing claims, feature claims
- Findings: Per-competitor breakdown
- All claims cited to specific sources

### Example 2: Technical Decision
**Input**: "Research options for database migration"

**Output**:
- Brief: Recommended approach with rationale
- Source comparison: Different expert opinions
- Findings: Migration paths, risks, timelines
- Citations to documentation and case studies

### Example 3: Policy Research
**Input**: PDFs of three industry reports + web research

**Output**:
- Brief: Synthesized conclusions
- Source comparison: Where reports agree/conflict
- Findings: Key data points extracted
- All statistics cited to original source

---

## What I Won't Do

- **Won't fabricate sources**: All citations are real
- **Won't hide conflicts**: Disagreements are surfaced
- **Won't mix fact and opinion**: Clearly distinguished
- **Won't present speculation as fact**: Uncertainty noted
- **Won't miss attribution**: Every claim has a source

---

## Tips for Best Results

1. **Be specific about question**: "Remote work trends" is vague; "Remote work tool adoption 2024" is better
2. **Provide key documents**: If you have authoritative sources, include them
3. **Specify angle**: "From a security perspective" focuses the synthesis
4. **Note what you know**: "I've read X, need perspectives beyond that"
5. **Ask about conflicts**: "Which source should I trust on Y?"

---

## Troubleshooting

### "Sources conflict—which is right?"
I'll highlight the conflict. Use source credibility, recency, and your domain knowledge to judge.

### "Missing important sources"
Provide them directly, or ask: "Also search for [specific topic]"

### "Too much detail / not enough"
Specify: "Brief overview only" or "Need comprehensive coverage"

### "Need primary sources"
Ask: "Include original research and studies, not just articles"

---

*Part of Art of Fact Cowork Skill Library*
