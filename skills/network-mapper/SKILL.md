---
name: network-mapper
description: --- Analyzes your professional network from contacts, email, and calendar to assess relationship health. Identifies neglected connections, suggests reconnection outreach,...
---

# Network Mapper

**Analyze contacts for relationship health and generate reconnection suggestions.**

---

## What This Does

Analyzes your professional network from contacts, email, and calendar to assess relationship health. Identifies neglected connections, suggests reconnection outreach, and helps you maintain valuable relationships proactively.

| Output | What You Get |
|--------|--------------|
| network-health.md | Dashboard of relationship status |
| reconnection-drafts/ | Ready-to-send outreach |
| network-visualization.md | Your network structure |

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
> "Map my professional network health"

### Option 2: Focused Check
> "Who should I reconnect with this quarter?"

### Option 3: Specific Group
> "Check on my investor relationships"

---

## What I Need From You

### Required
- **Contacts access**: Address book integration or list

### Optional (Enhances Output)
- **Communication history**: Email/calendar for activity
- **Priority tags**: Who matters most
- **Relationship goals**: What you want from your network

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Contacts | Names, roles, organizations | Provide list |
| Email | Communication history | Estimate recency |
| Calendar | Meeting history | Skip meeting data |

---

## Output Location

```
output/
├── network-health.md          # Dashboard
├── reconnection-drafts/       # Outreach messages
└── network-visualization.md   # Structure map
```

---

## Examples

### Example 1: Full Network Audit
**Input**: Contacts + email + calendar access

**Output**:
- Active (30 days): 45 relationships
- Dormant (90+ days): 23 relationships
- At-risk (180+ days): 12 relationships
- Reconnection drafts for top 5 at-risk

### Example 2: Professional Segment
**Input**: "Check my mentor relationships"

**Output**:
- 4 mentors identified
- 2 overdue for check-in
- Personalized reconnection messages

### Example 3: Pre-Event Outreach
**Input**: "Conference next month—who should I reach out to?"

**Output**:
- Connections likely attending
- Dormant relationships to revive
- Intro request suggestions

---

## What I Won't Do

- **Won't contact anyone**: Drafts only
- **Won't share your network**: Private analysis
- **Won't spam suggestions**: Quality over quantity
- **Won't include personal contacts**: Unless specified
- **Won't pressure reconnection**: Suggestions, not obligations

---

## Tips for Best Results

1. **Tag VIP contacts**: Priority for monitoring
2. **Note context**: "Met at conference 2023" helps personalization
3. **Update regularly**: Quarterly network health checks
4. **Include why**: Why you want to stay connected
5. **Quality matters**: Don't reconnect for its own sake

---

## Troubleshooting

### "Too many reconnection suggestions"
Set priorities: "Only suggest top 10" or "Focus on investors."

### "Context is wrong"
Add notes to contacts. More context = better suggestions.

### "Missing important people"
Check if they're in your contacts. Add with relevant context.

### "Reconnection timing seems off"
Different relationships need different cadences. Specify: "Check investors monthly, colleagues quarterly."

---

*Part of Art of Fact Cowork Skill Library*
