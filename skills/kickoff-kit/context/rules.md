# Kickoff Kit — Rules & Guidelines

## Output Formatting Rules

### project-charter.md Format
```markdown
# Project Charter: [Project Name]

**Version**: 1.0
**Date**: [Date]
**Owner**: [Name]
**Sponsor**: [Name]

---

## Executive Summary

[2-3 sentence project overview]

---

## Goals & Objectives

### Primary Goal
[What this project will achieve]

### Success Metrics
| Metric | Target | Measurement |
|--------|--------|-------------|
| [Metric 1] | [Target] | [How measured] |
| [Metric 2] | [Target] | [How measured] |

---

## Scope

### In Scope
- [Deliverable 1]
- [Deliverable 2]
- [Deliverable 3]

### OUT OF SCOPE
⚠️ The following are explicitly NOT part of this project:
- [Not included 1]
- [Not included 2]
- [Not included 3]

### Assumptions
- [Assumption 1]
- [Assumption 2]

---

## Constraints

| Constraint | Details |
|------------|---------|
| Budget | [Amount or "TBD"] |
| Timeline | [End date or "TBD"] |
| Team | [Size/composition] |
| Technical | [Platform/tool constraints] |

---

## Milestones

| Milestone | Description | Target Date |
|-----------|-------------|-------------|
| M1: [Name] | [Description] | [Date] |
| M2: [Name] | [Description] | [Date] |
| M3: [Name] | [Description] | [Date] |
| Launch | [Description] | [Date] |

---

## Approval

| Role | Name | Date | Signature |
|------|------|------|-----------|
| Sponsor | | | |
| Owner | | | |
| Tech Lead | | | |
```

### stakeholder-map.md Format
```markdown
# Stakeholder Map: [Project Name]

## Stakeholder Overview

| Stakeholder | Role | Interest | Influence | Engagement |
|-------------|------|----------|-----------|------------|
| [Name] | [Role] | High/Med/Low | High/Med/Low | [Strategy] |

---

## Detailed Profiles

### [Stakeholder 1]
- **Role**: [Title/function]
- **Interest**: [What they care about]
- **Influence**: [Decision-making power]
- **Needs**: [What they need from project]
- **Concerns**: [Potential objections]
- **Engagement Strategy**: [How to keep them informed/involved]

### [Stakeholder 2]
...

---

## RACI Matrix

| Activity | [Person 1] | [Person 2] | [Person 3] |
|----------|------------|------------|------------|
| [Activity 1] | R | A | C |
| [Activity 2] | C | R | A |
| [Activity 3] | I | C | R |

Legend: R=Responsible, A=Accountable, C=Consulted, I=Informed

---

## Communication Plan

| Stakeholder | Channel | Frequency | Owner |
|-------------|---------|-----------|-------|
| [Name] | [Email/Meeting] | [Weekly] | [Who] |
```

### risk-register.md Format
```markdown
# Risk Register: [Project Name]

## Risk Summary

| Risk Level | Count |
|------------|-------|
| High | [N] |
| Medium | [N] |
| Low | [N] |

---

## Risks

### RISK-001: [Risk Name]
- **Category**: [Technical/Resource/External/Organizational]
- **Description**: [What could go wrong]
- **Probability**: High / Medium / Low
- **Impact**: High / Medium / Low
- **Risk Score**: [P x I]
- **Trigger**: [How we'll know it's happening]
- **Mitigation**: [How to prevent]
- **Contingency**: [What to do if it happens]
- **Owner**: [Who's watching]

### RISK-002: [Risk Name]
...

---

## Risk Matrix

|            | Low Impact | Med Impact | High Impact |
|------------|------------|------------|-------------|
| High Prob  | [IDs]      | [IDs]      | [IDs]       |
| Med Prob   | [IDs]      | [IDs]      | [IDs]       |
| Low Prob   | [IDs]      | [IDs]      | [IDs]       |
```

### milestone-1-breakdown.md Format
```markdown
# Milestone 1: [Name]

**Duration**: [X weeks]
**Goal**: [What this milestone achieves]
**Start**: [Date]
**End**: [Date]

---

## Deliverables

- [ ] [Deliverable 1]
- [ ] [Deliverable 2]
- [ ] [Deliverable 3]

---

## Task Breakdown

### Week 1

| Task | Owner | Estimate | Dependencies |
|------|-------|----------|--------------|
| [Task 1] | [Name] | [Hours/Days] | None |
| [Task 2] | [Name] | [Hours/Days] | Task 1 |

### Week 2
...

---

## Dependencies

- [Dependency 1]: [Status]
- [Dependency 2]: [Status]

---

## Definition of Done

This milestone is complete when:
- [ ] [Criterion 1]
- [ ] [Criterion 2]
- [ ] [Criterion 3]
```

---

## Content Rules

### Charter
- Always include OUT of scope (explicit)
- Goals must be measurable
- Constraints are realistic
- Milestones are <2 weeks each

### Stakeholders
- Include all affected parties
- Specify engagement level per stakeholder
- Note potential resistance

### Risks
- Minimum 5 risks identified
- Every risk has mitigation AND contingency
- Owner assigned to each risk

### Milestone Breakdown
- Tasks are 1-5 day chunks
- Dependencies explicit
- Clear definition of done

---

## Quality Checklist

- [ ] Charter has explicit OUT of scope
- [ ] Success metrics are measurable
- [ ] All constraints documented
- [ ] Stakeholders include decision-makers
- [ ] RACI is complete
- [ ] Minimum 5 risks identified
- [ ] Risks have mitigations
- [ ] Milestone tasks are <1 week
- [ ] Dependencies are mapped

---

*Part of Art of Fact Cowork Skill Library*
