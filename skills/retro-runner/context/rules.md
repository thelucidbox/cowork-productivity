# Retro Runner — Rules & Guidelines

## Output Formatting Rules

### retrospective.md Format
```markdown
# Retrospective: [Sprint/Project Name]

**Period**: [Date range]
**Team**: [Team name/members]
**Facilitator**: [Name]
**Date**: [Retro date]

---

## Summary

[2-3 sentence summary of the retro]

**Overall sentiment**: [Positive/Mixed/Challenging]

---

## What Went Well

### [Theme 1]
- [Specific observation]
- [Supporting detail]

### [Theme 2]
- [Specific observation]

---

## What Could Improve

### [Theme 1]
- **Observation**: [What happened]
- **Impact**: [Why it mattered]
- **System cause**: [Root cause—not individual blame]

### [Theme 2]
...

---

## Discussion Points

### [Topic raised]
- **Context**: [What prompted this]
- **Different perspectives**: [Views shared]
- **Conclusion**: [If any]

---

## Experiments for Next Sprint

| Experiment | Owner | Measure | Review Date |
|------------|-------|---------|-------------|
| [Specific change] | [Name] | [How to measure success] | [Date] |

---

## Action Items

- [ ] [Action]: @[Owner] by [Date]
- [ ] [Action]: @[Owner] by [Date]

---

## Previous Experiments Review

| Experiment | Result | Continue? |
|------------|--------|-----------|
| [From last retro] | [Success/Failed/Partial] | Yes/No |

---

## Kudos & Recognition

- [Name] for [specific contribution]
- [Team] for [achievement]
```

### experiments.md Format
```markdown
# Experiments: [Period]

## Experiment 1: [Name]

### Hypothesis
If we [change], then [expected outcome] because [reasoning].

### Specifics
- **What**: [Exact change to make]
- **Who**: [Owner]
- **Duration**: [How long to test]
- **Measure**: [How we'll know if it worked]

### Success Criteria
- [Quantitative metric]: [Target]
- [Qualitative observation]: [What to look for]

### Abort Criteria
Stop if: [Condition that means this isn't working]

---

## Experiment 2: [Name]
...
```

### patterns.md Format
```markdown
# Patterns Across Retros

## Recurring Issues

### [Issue Theme]
- Sprint 45: [Manifestation]
- Sprint 46: [Manifestation]
- Sprint 47: [Manifestation]
- **Root cause hypothesis**: [Why this keeps happening]
- **Suggested intervention**: [Systemic fix]

---

## Improving Areas

### [Area]
- Sprint 45: [State]
- Sprint 47: [Improved state]
- **What changed**: [Successful experiment/intervention]

---

## Stalled Experiments

| Experiment | Started | Status | Notes |
|------------|---------|--------|-------|
| [Name] | Sprint 45 | Not tried | No owner followed up |
```

---

## Facilitation Principles

### Focus on Systems
- Good: "Deployments were blocked by environment issues"
- Bad: "Bob didn't deploy on time"

### Specific Over Vague
- Good: "Standups averaged 25 minutes instead of 15"
- Bad: "Meetings are too long"

### Testable Experiments
- Good: "Try async standups via Slack for Sprint 48, measure thread engagement"
- Bad: "Have better standups"

---

## Content Rules

### Always Include
- Wins (celebrate success)
- Improvements (honest assessment)
- Experiments (specific, testable)
- Previous experiment review

### Avoid
- Individual blame
- Vague action items
- Repeating experiments that didn't work
- Ignoring chronic issues

---

## Quality Checklist

- [ ] Wins are specific and celebrated
- [ ] Improvements focus on systems
- [ ] Each experiment has owner, measure, duration
- [ ] Previous experiments reviewed
- [ ] No individual blame
- [ ] Action items have owners and dates

---

*Part of Art of Fact Cowork Skill Library*
