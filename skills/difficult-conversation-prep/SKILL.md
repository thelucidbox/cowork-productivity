---
name: difficult-conversation-prep
description: --- Takes a difficult conversation you're facing and helps you prepare thoughtfully. Generates talking points that focus on interests rather...
---

# Difficult Conversation Prep

**Prepare for challenging conversations with talking points, anticipated responses, and de-escalation strategies.**

---

## What This Does

Takes a difficult conversation you're facing and helps you prepare thoughtfully. Generates talking points that focus on interests rather than positions, anticipates likely responses, provides de-escalation options, and helps you clarify your walk-away point. Enables you to enter tough conversations with confidence.

| Output | What You Get |
|--------|--------------|
| conversation-prep.md | Complete preparation document |
| talking-points.md | What to say and how to frame it |
| anticipated-responses.md | Their likely reactions + your responses |
| de-escalation-options.md | If things get heated |

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
> "Help me prepare for a tough conversation with my manager about compensation"

### Option 2: Structured Input
> "Difficult conversation prep: [person], [topic], [my goal]"

### Option 3: Exploration Mode
> "I need to have a hard conversation, help me think through it"

---

## What I Need From You

### Required
- **Who**: Who is this conversation with?
- **What**: What's the topic/issue?
- **Goal**: What outcome do you want?

### Optional (Enhances Output)
- **Relationship context**: Your history with this person
- **Their perspective**: What you think they'll say
- **Constraints**: What you can/can't offer
- **Stakes**: What happens if it goes poorly
- **Prior attempts**: Have you tried discussing before?

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Email | Prior communication dynamic | Ask about history |
| None required | Works standalone | Conversational input |

---

## Output Location

```
output/
├── conversation-prep.md        # Complete prep document
├── talking-points.md           # Key messages
├── anticipated-responses.md    # Their reactions + your rebuttals
└── de-escalation-options.md    # If things get heated
```

---

## Examples

### Example 1: Compensation Discussion
**Input**: "Need to ask my manager for a raise—haven't gotten one in 2 years"

**Output**:
- Talking points: Value delivered, market data, specific ask
- Anticipated responses: "Budget is tight," "Not the right time," "What about..."
- Your responses: Scripts for each scenario
- Walk-away clarity: What's your minimum? What if no?

### Example 2: Performance Feedback
**Input**: "Have to give tough feedback to a direct report about attitude issues"

**Output**:
- Frame: Specific behaviors, impact, expectation
- Talking points: Start with facts, listen, collaborate on solutions
- Anticipated responses: Defensiveness, excuses, deflection
- De-escalation: If emotions run high

### Example 3: Client Pushback
**Input**: "Client wants to reduce our fee by 30%—need to negotiate"

**Output**:
- Interests analysis: What do they really need?
- Talking points: Value delivered, alternatives, creative options
- Anticipated responses: Threats, comparisons, delays
- Walk-away point: When to hold firm

---

## What I Won't Do

- **Won't script manipulation**: Honest, respectful preparation only
- **Won't guarantee outcomes**: Preparation increases odds, doesn't control others
- **Won't avoid hard truths**: If your position has weaknesses, I'll surface them
- **Won't disrespect the other person**: Their interests matter too
- **Won't encourage avoidance**: Help you have the conversation, not dodge it

---

## Tips for Best Results

1. **Be honest about your goal**: "I want to win" vs. "I want to preserve relationship" changes approach
2. **Share their perspective**: Understanding their view improves your prep
3. **Identify your BATNA**: Know your alternative if conversation fails
4. **Practice out loud**: Prep documents help, but rehearsal locks it in
5. **Plan the setting**: When/where/how matters for difficult conversations

---

## Troubleshooting

### "Talking points feel too aggressive"
Specify your priority: "Relationship matters more than winning this point." I'll adjust framing.

### "Anticipated responses seem off"
Share more about the person. Their communication style and history shapes realistic responses.

### "Missing my main concern"
State it explicitly. The hidden concerns are often the real conversation.

### "Need more de-escalation help"
Ask: "Give me 5 ways to pause if this gets heated." I'll provide more options.

---

*Part of Art of Fact Cowork Skill Library*
