# Debrief Engine — Rules & Guidelines

## Output Formatting Rules

### decisions.md Format
```markdown
# Decisions — [Meeting Name] — [Date]

## Decision 1: [Brief Title]
- **What**: [The decision in one sentence]
- **Context**: [Why this was discussed]
- **Rationale**: [Why this choice was made]
- **Dissent**: [Any disagreement noted, or "None recorded"]
- **Revisit**: [Date/trigger for revisiting, or "Final"]

## Decision 2: ...
```

### action-tracker.md Format
```markdown
# Action Tracker — [Meeting Name] — [Date]

| Owner | Action | Deadline | Status | Notes |
|-------|--------|----------|--------|-------|
| @name | Task description | YYYY-MM-DD | Pending | Context |

## Unassigned Actions
- [ ] [Action needing owner] — Flagged for assignment
```

### open-loops.md Format
```markdown
# Open Loops — [Meeting Name] — [Date]

## Needs Resolution
1. **[Question/Issue]**
   - Raised by: [Name]
   - Blocker for: [What this affects]
   - Suggested next step: [Recommendation]

## Parking Lot (Not Urgent)
- [Item] — Revisit in [timeframe]
```

### Follow-up Email Formats

**Team Update (Casual)**
- Subject line: "[Meeting] Recap + Action Items"
- Tone: Direct, friendly, bullet-focused
- Length: 150-300 words
- Structure: Quick summary → Decisions → Actions → Next steps

**Client Recap (Professional)**
- Subject line: "Following Up: [Meeting Topic] — [Date]"
- Tone: Professional, appreciative, clear
- Length: 200-400 words
- Structure: Thank you → Summary → Agreed items → Next steps → Sign-off

**Executive Summary (Brief)**
- Subject line: "[Topic]: Key Outcomes"
- Tone: Concise, factual, outcome-focused
- Length: 50-150 words
- Structure: Bottom line → Key decisions → Blockers if any

---

## Tone Guidelines

### Team Tone
- Use first names
- Contractions okay ("we'll" not "we will")
- Casual openers ("Hey team," "Quick recap:")
- Emoji sparingly if team culture supports it

### Client Tone
- Full names on first reference
- Formal but warm
- Professional openers ("Thank you for your time today")
- No emoji unless client uses them first

### Executive Tone
- Lead with outcome/decision
- No pleasantries—straight to point
- Bullet points preferred
- Flag blockers prominently

---

## Content Rules

### Always Include
- Every decision mentioned, even tentative ones
- All action items with best-effort owner assignment
- Questions that were raised but not answered
- Next meeting or follow-up timing if mentioned

### Always Exclude
- Side conversations marked as off-record
- Personal comments not relevant to outcomes
- Speculation about attendees' motivations
- Information marked as confidential for specific outputs

### Flag for Review
- Decisions without clear rationale
- Actions without owners
- Deadlines that seem unrealistic
- Potential conflicts between decisions

---

## Quality Checklist

Before finalizing outputs, verify:

- [ ] Every decision has context (not just "we decided X")
- [ ] Every action has an owner (or explicitly flagged as unassigned)
- [ ] Deadlines are specific dates, not "soon" or "later"
- [ ] Follow-up emails don't include internal-only information
- [ ] Open loops have suggested next steps
- [ ] Future brief captures relationship/preference insights
- [ ] No PII in outputs unless necessary
- [ ] Tone matches requested style

---

## Edge Case Handling

### Conflicting Information in Notes
- Note both versions
- Flag as "Needs clarification"
- Don't guess at resolution

### Missing Attendee Information
- Use names exactly as they appear in notes
- Mark email addresses as "[email TBD]"
- Suggest completing info before sending

### Vague Decisions
- Capture as written
- Add to open loops: "Decision X needs specificity"
- Don't invent details

### No Clear Decisions Made
- State "No formal decisions recorded"
- Focus action tracker on discussed next steps
- Note if meeting may have been exploratory

---

## Template References

Templates are stored in `context/templates/`:
- `team-followup.md` — Team email structure
- `client-followup.md` — Client email structure
- `exec-followup.md` — Executive email structure
- `future-brief.md` — Context file structure

---

*Part of Art of Fact Cowork Skill Library*
