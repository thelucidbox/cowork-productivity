# Scope Creep Detector — Rules & Guidelines

## Output Formatting Rules

### scope-analysis.md Format
```markdown
# Scope Analysis: [Project Name]

**Original Date**: [Date of original spec]
**Analysis Date**: [Today]
**Comparison Period**: [Duration]

---

## Executive Summary

**Scope Change**: [X]% [increase/decrease] from original
**Classification**: Significant creep / Moderate creep / Minor drift / On track

[2-3 sentence summary]

---

## Original Scope

### Stated Goals
- [Goal 1]
- [Goal 2]

### Deliverables
- [Deliverable 1]
- [Deliverable 2]

### Explicitly Out of Scope
- [Item 1]
- [Item 2]

---

## Current State

### Current Expectations
- [Expectation 1]
- [Expectation 2]

### Added Since Original
- [Addition 1]
- [Addition 2]

### Removed Since Original
- [Removal 1]

---

## Comparison Summary

| Category | Original | Current | Change |
|----------|----------|---------|--------|
| Features/Deliverables | [N] | [N] | +[N] |
| Estimated Effort | [X] | [Y] | +[Z]% |
| Timeline | [X weeks] | [Y weeks] | +[Z] |

---

## Drift Classification

| Item | Type | Impact | Source |
|------|------|--------|--------|
| [Item] | New Scope / Clarification | High/Med/Low | [Who requested] |
```

### drift-items.md Format
```markdown
# Drift Items: [Project Name]

## New Scope (Not Originally Agreed)

### DRIFT-001: [Item Name]
- **Description**: [What was added]
- **When Added**: [Date/phase]
- **Requested By**: [Who]
- **Rationale Given**: [Why it was added]
- **Impact Estimate**: [Hours/cost]
- **Classification**: Scope Creep

### DRIFT-002: [Item Name]
...

---

## Clarifications (Within Original Intent)

### CLAR-001: [Item Name]
- **Description**: [What was clarified]
- **Original Statement**: [Vague original]
- **Clarified To**: [Specific interpretation]
- **Impact**: [Minimal/expected]
- **Classification**: Legitimate Clarification

---

## Removed Items

### REM-001: [Item Name]
- **Description**: [What was removed]
- **Impact**: [Reduced scope by X]
```

### renegotiation-points.md Format
```markdown
# Renegotiation Points: [Project Name]

## Current Situation
[Brief summary of where things stand]

## Options to Present

### Option 1: Extend Timeline
- **Change**: Add [X] weeks to schedule
- **Benefit**: Deliver full current scope
- **Trade-off**: Later delivery
- **Talking point**: "To deliver everything now expected, we need [X] more weeks"

### Option 2: Add Resources
- **Change**: Add [X] team members
- **Benefit**: Maintain timeline with current scope
- **Trade-off**: Increased cost of $[X]
- **Talking point**: "We can hit the original date with additional resources"

### Option 3: Reduce Scope
- **Change**: Remove/defer [specific items]
- **Benefit**: Hit original timeline and budget
- **Trade-off**: Features deferred
- **Talking point**: "To hit our original date, we recommend deferring [X, Y, Z]"
- **Recommended cuts**: [Prioritized list]

### Option 4: Accept Current State
- **Change**: Acknowledge expanded scope
- **Benefit**: All stakeholders aligned
- **Trade-off**: [Whatever applies]
- **Talking point**: "Let's formally acknowledge the expanded scope"

---

## Conversation Script

**Opening**: "I wanted to align on where we are versus our original agreement..."

**Present Facts**: "Our original scope included [X]. We're now at [Y]. That's [Z]% more."

**Options**: "I see three paths forward: [brief options]"

**Ask**: "Which direction makes sense for the business?"

---

## Do NOT Say
- "You added scope" (sounds accusatory)
- "This isn't what we agreed" (creates defensiveness)

## DO Say
- "The project has evolved" (neutral)
- "Let's align on current expectations" (collaborative)
- "Here are our options" (solution-oriented)
```

---

## Classification Rules

### Scope Creep (New Scope)
- Not mentioned in original spec
- Not a reasonable interpretation of original
- Represents new functionality/work
- Requires additional effort

### Clarification (Within Original)
- Vague original statement made specific
- Reasonable interpretation of intent
- Normal discovery during development
- No significant effort beyond expected

### Gold Plating (Self-Inflicted)
- Added by team without request
- "Nice to have" treated as requirement
- Should be flagged separately

---

## Quality Checklist

- [ ] Original spec accurately represented
- [ ] Current state objectively captured
- [ ] Each drift item classified fairly
- [ ] Impact estimates are reasonable
- [ ] Options are viable (not strawmen)
- [ ] Talking points are professional
- [ ] No blame language

---

*Part of Art of Fact Cowork Skill Library*
