---
name: prep-kit-generator
description: --- Takes an upcoming meeting from your calendar and generates everything you need to walk in prepared. Researches attendees, surfaces...
---

# Prep Kit Generator

**Generate complete meeting preparation from a calendar event—attendee research, talking points, and agenda.**

---

## What This Does

Takes an upcoming meeting from your calendar and generates everything you need to walk in prepared. Researches attendees, surfaces prior conversation context, drafts an agenda, and creates a post-meeting template ready for notes.

| Output | What You Get |
|--------|--------------|
| attendee-profiles.md | Background on everyone in the meeting |
| talking-points.md | Suggested topics based on context |
| draft-agenda.md | Proposed meeting structure |
| post-meeting-template.md | Ready for your notes during/after |

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
> "Prep me for my 2pm meeting with Acme Corp"

### Option 2: With Calendar Link
> "Generate prep kit for [calendar event link]"

### Option 3: Manual Mode
> "Help me prepare for a meeting with [names] about [topic]"

---

## What I Need From You

### Required
- **Meeting identifier**: Calendar event, meeting title, or attendee names + topic

### Optional (Enhances Output)
- **Your goals**: What do you want to accomplish?
- **Concerns**: Anything you're worried about?
- **Prior context**: Previous meeting notes or email threads
- **Research depth**: Quick overview vs. deep dive

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Calendar | Event details, attendees, existing agenda | You provide meeting details |
| Web Search | LinkedIn profiles, company news, recent press | Note gaps in research |
| Email | Prior conversations with attendees | Process as first meeting |
| Contacts | Roles, relationship history, notes | Use available public info |

---

## Output Location

```
output/
├── attendee-profiles.md      # Who's in the meeting
├── talking-points.md         # What to discuss
├── draft-agenda.md           # Proposed structure
└── post-meeting-template.md  # Note-taking scaffold
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Attendee Cards** | Interactive profiles with key info at a glance | "Create attendee profile cards" |
| **Meeting Prep Checklist** | Track what you've prepared and what's left | "Build a meeting prep checklist artifact" |
| **Agenda Timer** | Interactive agenda with time allocation | "Make a timed agenda artifact" |
| **Notes Template** | Structured note-taking during the meeting | "Create an interactive notes template" |

### Example Artifact Requests

**Attendee Dashboard**
> "Create a React artifact showing attendee cards with: name, role, company, relationship status, and key notes"

**Meeting Prep Tracker**
> "Build a checklist artifact with: research done, agenda reviewed, goals set, materials ready—let me check them off"

**Live Agenda**
> "Create an interactive agenda where I can see time remaining per section and adjust on the fly"

### Tips
- Review attendee cards 10 minutes before the meeting for a quick refresh
- Use the prep checklist to ensure you don't miss anything
- The notes template keeps you structured during the actual meeting

---

## Examples

### Example 1: Client Sales Meeting
**Input**: "Prep me for tomorrow's call with Sarah Chen from TechStart"

**Output**:
- Attendee profile: Sarah's role (VP Product), company background, recent TechStart news
- Talking points: Based on prior emails, their stated needs, your solutions
- Agenda: Discovery questions, demo points, next steps discussion
- Post-meeting template: Sections for needs identified, objections, follow-ups

### Example 2: Internal Strategy Session
**Input**: Calendar event "Q2 Planning — Leadership Team"

**Output**:
- Attendee profiles: Each leader's domain and current priorities
- Talking points: Items from previous planning sessions, open decisions
- Agenda: Review structure, decision points, time allocation
- Post-meeting template: Decisions, owners, timeline sections

### Example 3: First Meeting with New Contact
**Input**: "Meeting with James Wilson, don't know much about him"

**Output**:
- Attendee profile: LinkedIn research, company info, mutual connections
- Talking points: Ice breakers, discovery questions, your value prop
- Agenda: Intro, learn about them, share about you, explore fit
- Post-meeting template: Contact info, interests, potential opportunities

---

## What I Won't Do

- **Won't access private information**: Only public/shared data
- **Won't fabricate background**: Unknown info marked as "Not found"
- **Won't schedule meetings**: Preparation only, you handle logistics
- **Won't contact attendees**: Research is passive/public
- **Won't assume relationship status**: I note what I find, you know the nuance

---

## Tips for Best Results

1. **Share your goals**: "I want to close this deal" vs. "Just an intro call" shapes the prep
2. **Flag sensitivities**: Let me know if there's history or tension
3. **Provide prior context**: Previous meeting notes dramatically improve talking points
4. **Request specific research**: "Focus on their recent product launch" targets output
5. **Run day-before**: Gives you time to review and customize

---

## Troubleshooting

### "Attendee profiles are thin"
Some people have limited public presence. Try:
- Providing their company for context
- Sharing any emails you've exchanged
- Noting their role if you know it

### "Calendar event not found"
- Verify event is on your connected calendar
- Try searching by meeting title instead
- Provide attendee names + topic manually

### "Talking points don't match my goals"
State your goals explicitly. "This is a negotiation about price" produces very different prep than "This is relationship building."

### "Need deeper research"
Specify "deep dive" mode or ask for specific research: "What has their CEO said about AI recently?"

---

*Part of Art of Fact Cowork Skill Library*
