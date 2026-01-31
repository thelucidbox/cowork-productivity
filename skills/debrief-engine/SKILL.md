---
name: debrief-engine
description: Takes your raw meeting notes—bullet points, voice transcriptions, scribbles—and transforms them into a structured debrief package. You get clear decisions...
---

 # Debrief Engine

**Transform messy meeting notes into actionable decisions, tracked items, and polished follow-ups.**

---

## What This Does

Takes your raw meeting notes—bullet points, voice transcriptions, scribbles—and transforms them into a structured debrief package. You get clear decisions documented, action items assigned, open questions captured, and professional follow-up emails drafted in your choice of tone.

| Output | What You Get |
|--------|--------------|
| decisions.md | Every decision made, with context and rationale |
| action-tracker.md | Who's doing what, by when |
| open-loops.md | Questions raised but not resolved |
| follow-ups/ | Draft emails ready to send (team/client/executive versions) |
| future-brief.md | Context file for your next meeting with these people |

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
> "Debrief my product sync from this morning—here are my notes"

### Option 2: With Files
> "Run debrief engine on the meeting notes in input/"

### Option 3: Manual Mode
> "Help me process these meeting notes into a structured debrief"

---

## What I Need From You

### Required
- **Meeting notes**: Raw notes from the meeting (any format: bullet points, transcription, voice memo transcript)
- **Meeting context**: What was this meeting about? (can be inferred from notes)

### Optional (Enhances Output)
- **Attendee list**: Who was there (for assigning actions)
- **Prior context**: Link to previous meeting notes or email threads
- **Tone preference**: Team (casual), Client (professional), Executive (brief)
- **Calendar event**: I'll pull attendees and agenda automatically

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Calendar | Attendees, meeting title, agenda | You tell me who was there |
| Email | Prior thread context, relationship history | Process notes as standalone |
| Contacts | Full names, roles, email addresses | Use names from your notes |

---

## Output Location

```
output/
├── decisions.md          # Decisions with context
├── action-tracker.md     # Assigned tasks with deadlines
├── open-loops.md         # Unresolved questions
├── follow-ups/
│   ├── team-update.md    # Casual internal version
│   ├── client-recap.md   # Professional external version
│   └── exec-summary.md   # Brief leadership version
└── future-brief.md       # Context for next meeting
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Action Tracker Board** | Kanban of action items with owners and due dates | "Create an action tracker artifact" |
| **Decision Log** | Running log of decisions with context and rationale | "Build a decision log artifact" |
| **Open Loops Dashboard** | Track unresolved questions and their status | "Make an open loops tracker" |
| **Meeting Summary Card** | One-glance summary of the meeting outcomes | "Create a meeting summary artifact" |

### Example Artifact Requests

**Action Tracker Kanban**
> "Create a React artifact with columns: To Do, In Progress, Done—showing each action item with owner and due date"

**Decision Log**
> "Build an interactive log where I can record decisions with: date, decision, rationale, and stakeholders informed"

**Meeting Dashboard**
> "Create a dashboard showing: decisions made (count), actions assigned (by owner), and open loops remaining"

### Tips
- Use the action tracker during the meeting to assign items in real-time
- The decision log becomes valuable documentation over time
- Update open loops as questions get resolved between meetings

---

## Examples

### Example 1: Product Team Sync
**Input**: "product sync notes - discussed Q2 roadmap, Sarah wants to push mobile launch to March, we agreed to cut feature X, need budget approval from finance, john will handle API docs by friday"

**Output**:
- Decision captured: Mobile launch moved to March, Feature X cut from scope
- Actions: John → API docs by Friday, [Unassigned] → Get budget approval from finance
- Open loop: Budget approval pending
- Follow-up drafted for team

### Example 2: Client Discovery Call
**Input**: Voice memo transcript from client call + calendar event

**Output**:
- Decisions: Proceeding with Phase 1, weekly check-ins confirmed
- Actions assigned based on attendee roles
- Client follow-up email drafted (professional tone)
- Future brief includes client preferences and communication style

### Example 3: Executive Briefing
**Input**: "exec briefing - CEO approved headcount, concerns about timeline, wants weekly updates, legal reviewing contract"

**Output**:
- Exec summary: One paragraph with key outcomes
- Action tracker: Weekly updates scheduled, legal follow-up flagged
- Future brief: Note CEO's timeline concerns for next meeting

---

## What I Won't Do

- **Won't fabricate decisions**: If your notes are ambiguous, I'll flag it as an open question
- **Won't assign actions without names**: Unassigned items go to "TBD" with a flag
- **Won't send emails**: I draft them, you review and send
- **Won't access meetings I'm not given**: Only processes notes you provide
- **Won't guess at confidential information**: I work with what you share

---

## Tips for Best Results

1. **Include names when possible**: "Sarah suggested..." helps me assign actions correctly
2. **Note disagreements**: I'll capture both sides and flag as needing resolution
3. **Mention deadlines**: Even rough ones ("by end of week") help prioritize
4. **Flag confidential items**: Tell me what shouldn't appear in client-facing outputs
5. **Provide calendar event**: Automatic attendee lookup saves time and improves accuracy

---

## Troubleshooting

### "Actions aren't assigned to the right people"
Provide the attendee list or link to the calendar event. Without knowing who was in the meeting, I make best guesses based on names mentioned.

### "Missing context from previous meetings"
Drop previous meeting notes in the input folder or reference prior debriefs. Each future-brief.md I create is designed to feed into the next debrief.

### "Tone doesn't match my style"
Specify your preferred tone explicitly, or provide an example email you've sent before. I'll match your voice.

### "Too much/too little detail"
Tell me your preference: "Keep it brief" or "Include full context." I'll adjust output length accordingly.

---

*Part of Art of Fact Cowork Skill Library*
