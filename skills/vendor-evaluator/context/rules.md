# Vendor Evaluator — Rules & Guidelines

## Output Formatting Rules

### vendor-comparison.md Format
```markdown
# Vendor Comparison: [Category]

**Evaluation Date**: [Date]
**Vendors Evaluated**: [List]
**Evaluated By**: [Name]

---

## Executive Summary

**Recommendation**: [Vendor] with [confidence level]
**Key Differentiator**: [Why this vendor]
**Main Trade-off**: [What you give up]

---

## Comparison Matrix

| Criterion (Weight) | Vendor A | Vendor B | Vendor C |
|--------------------|----------|----------|----------|
| [Must-Have 1] (5) | [Score] | [Score] | [Score] |
| [Must-Have 2] (5) | [Score] | [Score] | [Score] |
| [Nice-to-Have 1] (2) | [Score] | [Score] | [Score] |
| Pricing (3) | [Score] | [Score] | [Score] |
| **Weighted Total** | **[X]** | **[Y]** | **[Z]** |

Scoring: 1=Poor, 2=Below Average, 3=Meets, 4=Exceeds, 5=Excellent

---

## Score Justifications

### Vendor A

| Criterion | Score | Justification |
|-----------|-------|---------------|
| [Criterion 1] | [Score] | [Why this score] |
| [Criterion 2] | [Score] | [Why this score] |

### Vendor B
...

---

## Total Cost of Ownership (3-Year)

| Cost Component | Vendor A | Vendor B | Vendor C |
|----------------|----------|----------|----------|
| License/Subscription | $[X] | $[Y] | $[Z] |
| Implementation | $[X] | $[Y] | $[Z] |
| Training | $[X] | $[Y] | $[Z] |
| Integration | $[X] | $[Y] | $[Z] |
| Ongoing Support | $[X] | $[Y] | $[Z] |
| **3-Year Total** | **$[X]** | **$[Y]** | **$[Z]** |

---

## Deal-Breaker Analysis

| Deal-Breaker | Vendor A | Vendor B | Vendor C |
|--------------|----------|----------|----------|
| [DB 1] | ✓ Pass | ✓ Pass | ✗ Fail |
| [DB 2] | ✓ Pass | ✓ Pass | ✓ Pass |

---

## Risk Assessment

| Vendor | Key Risks | Mitigation |
|--------|-----------|------------|
| Vendor A | [Risk] | [Mitigation] |
| Vendor B | [Risk] | [Mitigation] |
```

### questions-for-vendors.md Format
```markdown
# Due Diligence Questions

## For All Vendors

### Pricing
1. What's included in the base price?
2. What triggers additional costs?
3. What are the contract terms and exit clauses?

### Security
1. What security certifications do you hold?
2. How is data encrypted at rest and in transit?
3. What's your incident response process?

### Support
1. What support levels are available?
2. What are your SLAs?
3. How do we escalate issues?

---

## Vendor-Specific Questions

### For [Vendor A]
1. [Question based on research gap]
2. [Question about unclear feature]
3. [Question about specific concern]

### For [Vendor B]
...

---

## Reference Check Questions

Ask existing customers:
1. How was implementation?
2. How responsive is support?
3. Any surprise costs?
4. Would you choose them again?
```

---

## Scoring Rules

### Score Definitions
- **5 (Excellent)**: Exceeds requirements, best-in-class
- **4 (Good)**: Fully meets requirements, strong offering
- **3 (Meets)**: Adequately meets requirements
- **2 (Below)**: Partially meets, has gaps
- **1 (Poor)**: Does not meet, significant gaps

### Justification Requirements
Every score must have:
- Specific evidence (feature, documentation, review)
- Comparison to requirement
- No generic justifications

---

## TCO Calculation

### Include
- License/subscription costs
- Implementation/migration
- Training
- Integration development
- Ongoing maintenance/support
- Hidden costs (storage, API calls, users)

### Time Horizon
- Default: 3 years
- Adjust based on contract lengths

---

## Quality Checklist

- [ ] All criteria scored
- [ ] Every score justified
- [ ] TCO calculated
- [ ] Deal-breakers evaluated
- [ ] Vendor-specific questions included
- [ ] Risks identified
- [ ] Recommendation has confidence level

---

*Part of Art of Fact Cowork Skill Library*
