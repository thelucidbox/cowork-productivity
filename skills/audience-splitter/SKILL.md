---
name: audience-splitter
description: --- Takes a single piece of information—project update, announcement, decision—and generates appropriately tailored versions for different audiences. Each version maintains...
---

# Audience Splitter

**Transform one update into versions tailored for different audiences—exec, team, client, and more.**

---

## What This Does

Takes a single piece of information—project update, announcement, decision—and generates appropriately tailored versions for different audiences. Each version maintains the core message while adjusting depth, tone, and focus for the specific audience.

| Output | What You Get |
|--------|--------------|
| exec-summary.md | Brief, outcome-focused leadership version |
| team-detail.md | Full context version for your team |
| client-update.md | Professional external version |
| slack-post.md | Casual quick-share format |
| email-draft.md | Formal email version |

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
> "Split this update for exec, team, and client: [your update]"

### Option 2: With Source File
> "Run audience splitter on the update in input/"

### Option 3: Selective
> "Create an exec summary and team update from this"

---

## What I Need From You

### Required
- **The core message**: What needs to be communicated
- **Target audiences**: Who needs versions (or use defaults)

### Optional (Enhances Output)
- **Audience context**: What each group already knows
- **Tone preferences**: Your communication style
- **Sensitive items**: What to include/exclude per audience
- **Previous communications**: For tone matching

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Email | Your writing style for tone matching | Use neutral professional |
| None required | Works standalone | Ask about preferences |

---

## Output Location

```
output/
└── versions/
    ├── exec-summary.md     # Leadership brief
    ├── team-detail.md      # Internal full version
    ├── client-update.md    # External professional
    ├── slack-post.md       # Quick internal share
    └── email-draft.md      # Formal email format
```

---

## Examples

### Example 1: Project Milestone
**Input**: "We completed the API integration ahead of schedule. Found and fixed 3 bugs during testing. Ready for client demo Thursday."

**Versions Generated**:
- **Exec**: "API integration complete, ahead of schedule. Client demo Thursday."
- **Team**: Full details including bug specifics, who fixed what, demo prep tasks
- **Client**: "Great news—integration is complete and we're ready to show you Thursday"
- **Slack**: "API integration done! Demo prep Thursday - check #project-x for details"

### Example 2: Challenge Communication
**Input**: "We're running 2 weeks behind on the mobile launch due to third-party API delays. Mitigation plan in place."

**Versions Generated**:
- **Exec**: Delay + impact + mitigation + new timeline (2 sentences)
- **Team**: Full context, what happened, who's doing what, support needed
- **Client**: Proactive communication with adjusted timeline and value statement
- **Stakeholders**: Impact on their workstreams, any action needed

### Example 3: Good News Announcement
**Input**: "Sarah got promoted to Senior Engineer"

**Versions Generated**:
- **All-hands**: Formal announcement with accomplishments
- **Team**: Celebratory, personal note about working with Sarah
- **Exec**: Brief FYI if relevant
- **LinkedIn**: Professional external announcement (if requested)

---

## What I Won't Do

- **Won't change facts**: Same truth, different packaging
- **Won't hide bad news**: Appropriate framing, not concealment
- **Won't send anything**: Draft only, you review and send
- **Won't guess at confidential boundaries**: Ask if unclear
- **Won't over-communicate**: Skip audiences that don't need the info

---

## Tips for Best Results

1. **Specify what's sensitive**: "Don't mention budget to client" shapes outputs
2. **Note what audiences know**: "Team knows context, exec doesn't"
3. **Share previous examples**: Past emails help match your voice
4. **Be explicit about purpose**: "Inform" vs "Get approval" changes approach
5. **Request specific channels**: "Need a Slack version" adds that output

---

## Troubleshooting

### "Versions are too similar"
The audiences may have similar information needs. Specify how they differ: "Exec cares about timeline, team cares about technical details."

### "Tone doesn't match my style"
Share a sample of your writing to each audience. I'll adjust to match.

### "Missing an audience"
Specify additional audiences: "Also need a version for the board" or "Add a customer support version."

### "Too formal / too casual"
State preference: "Team update should be very casual" or "Even exec version should be warm."

---

*Part of Art of Fact Cowork Skill Library*
