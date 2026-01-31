---
name: decision-capture
description: --- Takes a decision you're facing—described in plain language—and transforms it into a structured framework. Surfaces hidden assumptions, clarifies criteria,...
---

# Decision Capture

**Transform any situation into a structured decision framework with options, criteria, and recommendation.**

---

## What This Does

Takes a decision you're facing—described in plain language—and transforms it into a structured framework. Surfaces hidden assumptions, clarifies criteria, maps out options objectively, and provides a recommendation based on your stated priorities.

| Output | What You Get |
|--------|--------------|
| decision-framework.md | Complete analysis: situation, criteria, options, recommendation |
| options-matrix.md | Side-by-side comparison of all options |
| assumptions.md | Hidden assumptions surfaced for validation |
| decision-record.md | Archive-ready record once decision is made |

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
> "Help me decide whether to hire a contractor or build in-house"

### Option 2: Structured Input
> "Run decision capture: situation is X, options are A, B, C"

### Option 3: Exploration Mode
> "I'm stuck on a decision, help me think through it"

---

## What I Need From You

### Required
- **The situation**: What decision are you facing?
- **Why it matters**: What's at stake?

### Optional (Enhances Output)
- **Options you're considering**: Your current candidates
- **Constraints**: Budget, time, team, technical limits
- **Priorities**: What matters most? (speed, cost, quality, etc.)
- **Stakeholders**: Who else this affects

---

## What I'll Pull Automatically

| Source | What I Get | Fallback |
|--------|-----------|----------|
| Conversation | Context from our discussion | Ask clarifying questions |
| Prior decisions | Similar decisions you've made | Analyze fresh |
| None required | This is a standalone thinking tool | — |

---

## Output Location

```
output/
├── decision-framework.md   # Complete analysis
├── options-matrix.md       # Comparison table
├── assumptions.md          # Surfaced assumptions
└── decision-record.md      # For archive after deciding
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Decision Framework Board** | Visual layout of situation, criteria, and options | "Create a decision framework artifact" |
| **Options Matrix** | Interactive scoring grid for options vs criteria | "Build an options comparison artifact" |
| **Criteria Weighter** | Adjust importance weights and see recommendation change | "Make a criteria weighting artifact" |
| **Decision Log** | Track past decisions with outcomes for learning | "Create a decision log artifact" |

### Example Artifact Requests

**Decision Framework**
> "Create a React artifact showing: the decision question, key criteria (weighted), options as cards, and a recommendation based on scores"

**Interactive Options Matrix**
> "Build a matrix where I can score each option 1-5 on each criterion, adjust weights, and see the winning option update"

**Decision Log**
> "Create a tracker for past decisions with: decision, date, what we chose, outcome, and learnings"

### Tips
- Use the criteria weighter when stakeholders disagree on priorities—visualize how different weights change the recommendation
- The decision log becomes valuable over time for pattern recognition
- Share the framework artifact to get buy-in before deciding

---

## Examples

### Example 1: Build vs. Buy
**Input**: "Should we build our own analytics or buy a tool?"

**Output**:
- Situation mapped with stakeholders and timeline
- Criteria: Cost (18mo), Time to value, Customization, Maintenance
- Options: Build custom, Buy established, Buy + customize, Hybrid
- Each option scored against criteria
- Recommendation with rationale and reversibility note

### Example 2: Career Decision
**Input**: "I have two job offers, don't know which to take"

**Output**:
- Situation: Career stage, what you're optimizing for
- Criteria: Compensation, Growth, Culture, Work-life, Location
- Options: Offer A, Offer B, Neither (stay current)
- Assumptions: "Assuming stated culture matches reality"
- Recommendation based on your stated priorities

### Example 3: Technical Architecture
**Input**: "Monolith vs. microservices for our new system"

**Output**:
- Situation: Team size, timeline, scale requirements
- Criteria: Team capability, Time to MVP, Scale needs, Ops complexity
- Options: Monolith, Microservices, Modular monolith, Start mono/migrate
- Reversibility analysis for each option
- Recommendation with "decision review trigger"

---

## What I Won't Do

- **Won't decide for you**: Framework and recommendation, you choose
- **Won't hide trade-offs**: All downsides surfaced clearly
- **Won't oversimplify**: Complex decisions stay appropriately complex
- **Won't add false precision**: "Roughly equivalent" is valid when true
- **Won't assume your values**: Ask about priorities, don't guess

---

## Tips for Best Results

1. **State what you're optimizing for**: Speed? Cost? Quality? Growth?
2. **Include constraints upfront**: "Budget is $50k max" shapes analysis
3. **Mention stakeholders**: Their priorities become criteria
4. **Share your gut feeling**: I'll stress-test it
5. **Ask about reversibility**: Some decisions are more permanent than others

---

## Troubleshooting

### "Options seem incomplete"
Tell me your constraints more specifically. Sometimes "hidden" options emerge from clearer boundaries.

### "Criteria don't match my priorities"
Explicitly state what matters most. Default criteria may not match your situation.

### "Recommendation doesn't feel right"
Your gut is data. Let's explore why the framework output doesn't match your intuition—often reveals unstated criteria.

### "Too complex / too simple"
Specify: "Keep this simple—just the key factors" or "Go deep—this is important."

---

*Part of Art of Fact Cowork Skill Library*
