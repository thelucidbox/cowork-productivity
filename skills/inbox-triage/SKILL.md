---
name: inbox-triage
description: --- Analyzes your email inbox, prioritizes messages based on sender importance and deadline mentions, categorizes by action type, and drafts...
---

# Inbox Triage

**Sort emails by priority with response drafts—clear your inbox intelligently.**

---

## What This Does

Analyzes your email inbox, prioritizes messages based on sender importance and deadline mentions, categorizes by action type, and drafts responses for important emails matching your tone.

| Output | What You Get |
|--------|--------------|
| inbox-triage.md | Prioritized email list |
| response-drafts/ | Draft replies for key emails |
| ignore-list.md | Safe-to-archive items |

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
> "Triage my inbox from the last week"

### Option 2: Specific Timeframe
> "Show me high-priority emails from today"

### Option 3: Focus Mode
> "What emails need response today?"

---

## What I Need From You

### Required
- **Email access**: Gmail or Apple Mail integration

### Optional (Enhances Output)
- **VIP list**: Who always gets priority
- **Filters**: Skip newsletters, focus on certain domains
- **Response style**: Examples of your email voice

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Gmail | Full inbox access | — |
| Apple Mail | Full inbox access | — |

---

## Output Location

```
output/
├── inbox-triage.md          # Prioritized list
├── response-drafts/
│   └── [email-subject].md   # Ready responses
└── ignore-list.md           # Safe to archive
```

---

## Examples

### Example 1: Morning Triage
**Input**: "Triage my inbox"

**Output**:
- Urgent (3): Client deadline, boss request, time-sensitive
- Today (5): Need response by EOD
- This week (8): Important but not urgent
- FYI (12): Read when able
- Archive (23): Newsletters, notifications
- Response drafts for urgent items

### Example 2: After Vacation
**Input**: "Triage 200 emails from last 2 weeks"

**Output**:
- Expired/no longer relevant: 45
- Need response: 23
- FYI only: 67
- Archive: 65
- Summary of what you missed

### Example 3: End of Day
**Input**: "What's urgent before I leave?"

**Output**:
- Must handle tonight: 2 emails
- Can wait until morning: 8 emails
- Response drafts for urgent items

---

## What I Won't Do

- **Won't send emails**: Draft only, you review and send
- **Won't delete**: Archive suggestions, not deletions
- **Won't expose contents**: Summarize without showing full text
- **Won't spam senders**: No auto-replies
- **Won't miss important**: When uncertain, err toward priority

---

## Tips for Best Results

1. **Define VIPs**: Boss, key clients, family members
2. **Share your filters**: "Skip anything from [domain]"
3. **Provide response examples**: Helps match your tone
4. **Review ignore-list**: Confirm before archiving
5. **Run regularly**: Daily triage beats weekly overwhelm

---

## Troubleshooting

### "Missing important emails"
Add sender to VIP list. Check spam/promotions folders.

### "Too many as urgent"
Refine criteria: "Only client emails and boss emails are urgent."

### "Response tone is wrong"
Share examples of emails you've sent. I'll match your style.

### "Can't access email"
Check integration settings. Re-authorize if needed.

---

*Part of Art of Fact Cowork Skill Library*
