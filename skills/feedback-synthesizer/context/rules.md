# Feedback Synthesizer — Rules & Guidelines

## Output Formatting Rules

### feedback-synthesis.md Format
```markdown
# Feedback Synthesis: [Topic/Source]
**Source**: [What was analyzed]
**Volume**: [N responses/comments/sources]
**Date Range**: [If applicable]

---

## Executive Summary

[3-5 sentence overview of key findings]

**Overall Sentiment**: [Positive/Mixed/Negative] ([X]% positive, [Y]% neutral, [Z]% negative)

---

## Key Themes

### Theme 1: [Name] (Mentioned [N] times)
**Sentiment**: [Positive/Negative/Mixed]
**Summary**: [What people are saying]
**Representative quotes**:
> "[Quote 1]" — [Source if attributed]
> "[Quote 2]"

### Theme 2: [Name]
...

---

## Pattern Analysis

### Consistent Feedback (Strong Signal)
- [Pattern]: [Evidence]

### Mixed Feedback (Needs Interpretation)
- [Pattern]: [Different perspectives]

### Outlier Feedback (Single Mentions)
- [Item]: [Context—don't overweight but don't ignore]

---

## Sentiment Breakdown

| Theme | Positive | Neutral | Negative |
|-------|----------|---------|----------|
| [Theme 1] | X% | Y% | Z% |
| [Theme 2] | ... | ... | ... |

---

## Priority Improvements

| Rank | Improvement | Impact | Effort | Source Frequency |
|------|-------------|--------|--------|------------------|
| 1 | [Item] | High | Medium | [N] mentions |
| 2 | [Item] | ... | ... | ... |

---

## Responses Needed

| Source | Issue | Urgency | Draft Available |
|--------|-------|---------|-----------------|
| [Name] | [Topic] | High/Med/Low | Yes |

---

## Raw Data Notes
- Total inputs processed: [N]
- Date range: [Range]
- Sources: [List]
```

### quotes-by-theme.md Format
```markdown
# Quotes by Theme

## [Theme 1]: [Name]

### Positive
> "[Quote]" — [Source]
> "[Quote]" — [Source]

### Negative
> "[Quote]" — [Source]

### Suggestions
> "[Quote]" — [Source]

---

## [Theme 2]: [Name]
...
```

### priority-improvements.md Format
```markdown
# Priority Improvements

## Must Address (High Impact, High Frequency)

### 1. [Improvement]
- **Source**: [N] mentions
- **Impact**: [Why this matters]
- **Suggested action**: [What to do]
- **Key quote**: "[Quote]"

### 2. [Improvement]
...

## Should Consider (Medium Priority)
...

## Monitor (Low Priority but Valid)
...
```

---

## Analysis Guidelines

### Theme Identification
- Group semantically similar feedback
- Minimum 2 mentions to constitute theme
- Single mentions go to "Outliers"
- Don't force-fit feedback into themes

### Sentiment Classification
- **Positive**: Praise, satisfaction, appreciation
- **Negative**: Complaints, frustration, requests for change
- **Neutral**: Factual observations, suggestions without valence

### Signal vs. Noise
Strong signal:
- Multiple independent sources
- Specific, detailed feedback
- Consistent across time

Potential noise:
- Single mention
- Vague complaints
- Outliers from typical respondent profile

### Frequency vs. Importance
- High frequency + high importance = Priority 1
- Low frequency + high importance = Don't ignore (strategic)
- High frequency + low importance = Consider if easy
- Low frequency + low importance = Acknowledge only

---

## Quote Selection Rules

### Good Representative Quotes
- Clearly articulate the theme
- Specific rather than vague
- Capture sentiment accurately
- Diverse sources when possible

### Quote Attribution
- If feedback is attributed: Include source
- If anonymous: Use "[Anonymous]" or omit
- Never reveal anonymous sources

### Quote Editing
- Fix obvious typos: Okay
- Truncate with [...]: Okay
- Change meaning: Never
- Correct grammar: Only if necessary for clarity

---

## Response Draft Guidelines

### When to Draft Response
- Negative feedback from important source
- Direct question requiring answer
- Complaint needing acknowledgment
- Request for follow-up

### Response Tone
- Acknowledge the feedback
- Don't be defensive
- Commit to what you'll do
- Thank them for sharing

### Response Template
```markdown
# Response to [Source]

**Regarding**: [Topic]
**Their feedback**: [Brief summary]

---

Hi [Name],

Thank you for [specific feedback]. [Acknowledgment of their point].

[Your response/commitment].

[Next steps if any].

[Sign-off]
```

---

## Quality Checklist

- [ ] All feedback sources processed
- [ ] Themes accurately represent content
- [ ] Sentiment analysis is defensible
- [ ] Quotes are representative
- [ ] Priorities based on clear criteria
- [ ] Responses drafted for required items
- [ ] Anonymous feedback stays anonymous
- [ ] Outliers noted, not dismissed

---

*Part of Art of Fact Cowork Skill Library*
