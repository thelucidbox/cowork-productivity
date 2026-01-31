---
name: life-admin-queue
description: --- Takes all those vague life admin items—call the insurance, schedule the appointment, renew the thing—and transforms them into a...
---

# Life Admin Queue

**Transform scattered admin items into a prioritized, time-blocked queue.**

---

## What This Does

Takes all those vague life admin items—call the insurance, schedule the appointment, renew the thing—and transforms them into a concrete, prioritized queue. Breaks vague tasks into specific actions, estimates time, batches similar items, and suggests calendar blocks.

| Output | What You Get |
|--------|--------------|
| admin-queue.md | Prioritized task list |
| calendar-blocks.ics | Time blocks for admin |
| weekly-schedule.md | When to do what |

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
> "Help me get my life admin under control"

### Option 2: Brain Dump
> "Here are all the admin things I need to do: [list]"

### Option 3: Review Mode
> "What admin tasks am I avoiding?"

---

## What I Need From You

### Required
- **Admin tasks**: What needs to get done (any format)

### Optional (Enhances Output)
- **Deadlines**: What's time-sensitive
- **Constraints**: When you can make calls, business hours
- **Energy context**: When you have admin energy
- **Calendar access**: For scheduling

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Notes | Admin mentions | Manual input |
| Calendar | Available time slots | Suggest schedule |

---

## Output Location

```
output/
├── admin-queue.md           # Prioritized list
├── calendar-blocks.ics      # Time blocks
└── weekly-schedule.md       # Day-by-day plan
```

---

## Examples

### Example 1: Monthly Admin Review
**Input**: "Renew car registration, call dentist, update address with bank, cancel old subscription"

**Output**:
- Queue ordered by deadline and complexity
- "Call dentist" broken into: find number, check insurance, call, schedule
- Calendar: 30-min block Tuesday for calls
- Similar items batched: all "call" tasks together

### Example 2: Move-Related Admin
**Input**: "Moving next month, lots of address changes"

**Output**:
- Checklist: All entities needing address update
- Batched by method: online, phone, mail
- Timeline: What to do before vs after move
- Estimated: 3 hours total, spread over 4 sessions

### Example 3: Financial Admin
**Input**: "Need to deal with tax stuff, check insurance, review subscriptions"

**Output**:
- Tax items by deadline
- Insurance review checklist
- Subscription audit process
- Time estimate per category

---

## What I Won't Do

- **Won't do admin for you**: Organize and plan, not execute
- **Won't call on your behalf**: You make the calls
- **Won't access your accounts**: Just help you organize
- **Won't nag**: Provide structure, not guilt
- **Won't overload**: Realistic scheduling

---

## Tips for Best Results

1. **Brain dump everything**: Don't filter, just list
2. **Include vague items**: "Deal with insurance thing" is fine
3. **Note deadlines**: Hard deadlines get priority
4. **Share constraints**: "Can only call 9-5 weekdays"
5. **Batch processing**: Admin blocks are more efficient

---

## Troubleshooting

### "List is overwhelming"
Ask for "top 5 only" or "urgent items only."

### "Tasks are still too vague"
Describe what makes it complex. I'll break it down further.

### "Don't have time for admin"
Let's find 30-minute windows. Admin batches efficiently.

### "Keep procrastinating"
We can discuss what's blocking you and find ways around it.

---

*Part of Art of Fact Cowork Skill Library*
