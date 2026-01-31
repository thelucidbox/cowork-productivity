---
name: learning-path-builder
description: --- Takes a skill you want to learn and builds a complete learning path. Breaks the skill into phases, finds...
---

# Learning Path Builder

**Generate a structured curriculum from any skill goal—phases, resources, and first assignment ready.**

---

## What This Does

Takes a skill you want to learn and builds a complete learning path. Breaks the skill into phases, finds resources matched to your level, mixes learning formats (video, reading, practice), and gives you your first assignment immediately. Prefers free resources but includes paid options where they're significantly better.

| Output | What You Get |
|--------|--------------|
| learning-path.md | Complete curriculum with phases and milestones |
| resources.md | Curated list of tutorials, courses, books |
| first-assignment.md | Start today—immediate practical task |
| progress-tracker.md | Track your advancement |

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
> "Build me a learning path for Python programming"

### Option 2: With Context
> "I want to learn machine learning. I know Python basics. I have 5 hours per week."

### Option 3: Specific Goal
> "Help me learn enough SQL to analyze our sales data"

---

## What I Need From You

### Required
- **Skill goal**: What do you want to learn?

### Optional (Enhances Output)
- **Current level**: What do you already know?
- **Time available**: Hours per week you can dedicate
- **Learning style**: Video vs reading vs hands-on
- **End goal**: Why are you learning this?
- **Timeline**: Any deadline?

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Web Search | Current best resources, free courses | Recommend classics |
| Local Files | Your notes on topic for level assessment | Ask about experience |

---

## Output Location

```
output/
├── learning-path.md       # Full curriculum
├── resources.md           # Curated resources
├── first-assignment.md    # Start immediately
└── progress-tracker.md    # Track advancement
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Learning Roadmap** | Visual path from beginner to goal | "Create a learning roadmap artifact" |
| **Progress Tracker** | Check off completed modules and see progress | "Build a learning progress artifact" |
| **Resource Library** | Organized collection of learning materials | "Make a resource library artifact" |
| **Study Planner** | Schedule learning sessions into your week | "Create a study planner artifact" |

### Example Artifact Requests

**Learning Roadmap**
> "Create a React artifact showing my learning path as phases—each phase expandable with modules, estimated time, and completion status"

**Progress Dashboard**
> "Build a tracker where I can mark modules complete, see overall progress %, and estimated time to finish"

**Weekly Study Planner**
> "Create a calendar artifact where I can schedule learning sessions and see recommended weekly hours"

### Tips
- Update progress after each learning session
- Use the roadmap to see how concepts build on each other
- The study planner helps maintain consistent learning habits

---

## Examples

### Example 1: Programming Language
**Input**: "Learn Python, complete beginner, 3 hours/week"

**Output**:
- Phase 1: Basics (variables, loops) - 2 weeks
- Phase 2: Functions and data structures - 2 weeks
- Phase 3: Working with files - 1 week
- Phase 4: First project - 2 weeks
- Resources: Free interactive tutorials, one recommended paid course
- First assignment: Install Python, write "Hello World"

### Example 2: Professional Skill
**Input**: "Get better at public speaking"

**Output**:
- Phase 1: Foundation (structure, nerves) - 3 weeks
- Phase 2: Delivery (voice, body language) - 3 weeks
- Phase 3: Audience engagement - 2 weeks
- Phase 4: Advanced (Q&A, improvisation) - 2 weeks
- Resources: Books, YouTube channels, local Toastmasters
- First assignment: Record yourself for 2 minutes on camera

### Example 3: Tool Mastery
**Input**: "Learn Figma for UI design, know Sketch already"

**Output**:
- Phase 1: Interface and key differences from Sketch - 1 week
- Phase 2: Components and variants - 1 week
- Phase 3: Prototyping and collaboration - 1 week
- Phase 4: Advanced features (auto-layout, plugins) - 2 weeks
- Resources: Official tutorials, YouTube comparisons
- First assignment: Rebuild an existing Sketch file in Figma

---

## What I Won't Do

- **Won't create content**: Curate existing resources, not create courses
- **Won't guarantee timeline**: Estimates based on typical learners
- **Won't skip fundamentals**: Build on solid foundations
- **Won't ignore your level**: Adapt difficulty to where you are
- **Won't only list paid options**: Free resources prioritized

---

## Tips for Best Results

1. **Be specific about goal**: "Python for data analysis" beats just "Python"
2. **Share constraints**: Budget, time, preferred formats all help
3. **Mention learning style**: "I learn best by doing" shapes the path
4. **Include end goal**: "To get a job" vs "for personal projects" matters
5. **Be honest about level**: Starting at wrong level wastes time

---

## Troubleshooting

### "Path is too long/ambitious"
Specify time constraint: "I need functional skills in 4 weeks" and I'll prioritize ruthlessly.

### "Resources are outdated"
Ask for current search: "Find 2024 resources for [topic]"

### "Too many/few resources"
Specify: "Give me just the top 3" or "I want lots of options to explore"

### "First assignment is too easy/hard"
Tell me your actual level more specifically. The assignment should stretch but not overwhelm.

---

*Part of Art of Fact Cowork Skill Library*
