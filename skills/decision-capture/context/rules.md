# Decision Capture — Rules & Guidelines

## Output Formatting Rules

### decision-framework.md Format
```markdown
# Decision Framework: [Brief Title]
**Date**: [Date]
**Decision Owner**: [Name]
**Status**: In Analysis / Ready for Decision / Decided

---

## Situation

### Context
[2-3 paragraphs describing the decision context]

### Why Now
[What triggered this decision point]

### Stakeholders
| Stakeholder | Interest | Influence |
|-------------|----------|-----------|
| [Name/Role] | [What they care about] | High/Med/Low |

### Constraints
- **Budget**: [Amount or "Flexible"]
- **Timeline**: [Deadline or "No hard deadline"]
- **Technical**: [Limitations]
- **Political**: [Organizational factors]

---

## Decision Criteria

| Criterion | Weight | Definition |
|-----------|--------|------------|
| [Criterion 1] | [1-5] | [What this means] |
| [Criterion 2] | [1-5] | [What this means] |
| ... | ... | ... |

### Weighting Rationale
[Why these weights]

---

## Options Analysis

### Option A: [Name]
**Summary**: [One sentence]

| Criterion | Score (1-5) | Notes |
|-----------|-------------|-------|
| [Criterion] | [Score] | [Why] |
| ... | ... | ... |

**Weighted Score**: [Total]

**Pros**:
- [Pro 1]
- [Pro 2]

**Cons**:
- [Con 1]
- [Con 2]

**Reversibility**: High / Medium / Low
[Explanation]

### Option B: [Name]
...

---

## Comparison Matrix

| Criterion (Weight) | Option A | Option B | Option C |
|--------------------|----------|----------|----------|
| [Criterion] (W) | Score | Score | Score |
| **Weighted Total** | **X** | **Y** | **Z** |

---

## Assumptions

### Stated Assumptions
- [Assumption 1]: [Source/validation]
- [Assumption 2]: [Source/validation]

### Surfaced Assumptions
- [Hidden assumption discovered]: [Implication]

### Assumption Risks
- If [assumption] is wrong: [Impact]

---

## Recommendation

### Primary Recommendation
**[Option Name]** with [confidence level: High/Medium/Low]

### Rationale
[2-3 paragraphs explaining why]

### Key Trade-offs Accepted
- [Trade-off 1]
- [Trade-off 2]

### Dissenting Considerations
[Why someone might choose differently]

---

## Decision Review

### Review Trigger
Revisit this decision if:
- [Condition 1]
- [Condition 2]

### Success Criteria
We'll know this was the right decision if:
- [Measurable outcome 1]
- [Measurable outcome 2]

---

## Next Steps (If Approved)
1. [Immediate action]
2. [Follow-up action]
3. [Communication/announcement]
```

### options-matrix.md Format
```markdown
# Options Comparison: [Decision Title]

| Factor | Option A | Option B | Option C | Notes |
|--------|----------|----------|----------|-------|
| **Cost** | [Value] | [Value] | [Value] | [Context] |
| **Time** | [Value] | [Value] | [Value] | [Context] |
| **Quality** | [Rating] | [Rating] | [Rating] | [Context] |
| **Risk** | Low/Med/High | ... | ... | [Context] |
| **Reversibility** | Easy/Hard | ... | ... | [Context] |

## Quick Summary
- **Best for cost**: [Option]
- **Best for speed**: [Option]
- **Best for quality**: [Option]
- **Most reversible**: [Option]
```

---

## Analysis Guidelines

### Criteria Selection
Include at minimum:
- Cost / Resource impact
- Time / Speed to outcome
- Quality / Effectiveness
- Risk / Uncertainty
- Reversibility / Flexibility

Add context-specific:
- Stakeholder alignment
- Strategic fit
- Team capability
- Scalability
- Maintenance burden

### Scoring Rules
- 1: Poor / Does not meet
- 2: Below average / Partially meets
- 3: Average / Adequately meets
- 4: Above average / Exceeds
- 5: Excellent / Far exceeds

### Weight Guidelines
- 5: Must-have, deal-breaker importance
- 4: Very important, significant factor
- 3: Important, meaningful consideration
- 2: Nice-to-have, secondary factor
- 1: Minor, tie-breaker only

---

## Assumption Surfacing

### Questions to Uncover Assumptions
- "What would need to be true for Option X to work?"
- "What are we taking for granted?"
- "What if [stakeholder] has different priorities than stated?"
- "What external factors could change?"

### Common Hidden Assumptions
- Market conditions will stay stable
- Team has necessary skills
- Timeline is realistic
- Budget won't change
- Stakeholder support will continue
- Technology will perform as expected

---

## Recommendation Rules

### Confidence Levels
- **High**: Clear winner, robust across assumptions
- **Medium**: Best option but sensitive to assumptions
- **Low**: Close call, recommend pilot/test

### When NOT to Recommend
- Options are genuinely equivalent
- Critical information is missing
- Decision owner needs to apply values not captured

### Dissent Requirement
Always include "why someone might choose differently" — validates that trade-offs are acknowledged.

---

## Quality Checklist

- [ ] Situation fully captures context
- [ ] Criteria reflect stated priorities
- [ ] All viable options included
- [ ] Scores are justified, not arbitrary
- [ ] Assumptions explicitly stated
- [ ] Hidden assumptions surfaced
- [ ] Recommendation aligns with weighted analysis
- [ ] Trade-offs clearly acknowledged
- [ ] Review triggers defined
- [ ] Next steps actionable

---

*Part of Art of Fact Cowork Skill Library*
