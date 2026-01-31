# Knowledge Capture — Rules & Guidelines

## Output Formatting Rules

### kb-article.md Format
```markdown
# [Problem Title]

**Category**: [Technical/Process/Tool/etc.]
**Last Updated**: [Date]
**Author**: [Name]
**Tags**: `tag1` `tag2` `tag3`

---

## Problem

[Clear description of what goes wrong / what's confusing]

### Symptoms
- [How you know this problem is occurring]
- [Error messages, behaviors, symptoms]

### When This Happens
- [Context: after upgrade, during peak load, etc.]

---

## Root Cause

[Why this happens—the underlying reason]

---

## Solution

### Quick Fix
[One-liner if possible]

### Step-by-Step

1. **[Step 1]**
   ```
   [code or command if applicable]
   ```
   [Explanation]

2. **[Step 2]**
   [Details]

3. **[Step 3]**
   [Details]

### Verification
[How to confirm the fix worked]

---

## What Didn't Work

[Document failed attempts to save others time]
- [Attempted solution 1]: [Why it failed]
- [Attempted solution 2]: [Why it failed]

---

## Gotchas

- [Edge case or warning 1]
- [Edge case or warning 2]

---

## Prevention

[How to avoid this problem in the future]

---

## Related Articles

- [[Related Topic 1]]
- [[Related Topic 2]]

---

## References

- [Link to documentation]
- [Link to external resource]
```

### quick-reference.md Format
```markdown
# Quick Reference: [Problem]

## TL;DR
[One sentence solution]

## Commands / Steps
```
[The fix in minimal form]
```

## When to Use This
[Brief context]

## Full Article
[[Link to full KB article]]
```

---

## Article Quality Standards

### Title
- Descriptive and searchable
- Include key terms people would search
- Good: "API Connection Timeout When Pool Exhausted"
- Bad: "Timeout Fix" / "That One Issue"

### Problem Section
- Clear enough that reader recognizes their situation
- Include actual error messages verbatim
- Specify version/context if relevant

### Solution Section
- Step-by-step, not prose
- Include actual commands/code
- Specify what to look for at each step
- End with verification step

### Gotchas Section
- Edge cases discovered
- Common mistakes
- "This works except when..."

---

## Tag Guidelines

### Standard Tags
- **Technical**: api, database, network, authentication
- **Tools**: npm, docker, aws, git
- **Process**: workflow, approval, onboarding
- **Type**: how-to, troubleshooting, explanation

### Tag Rules
- Lowercase
- Use existing tags when possible
- 3-6 tags per article
- Include tool/tech name
- Include problem type

---

## Content Rules

### Always Include
- Searchable problem description
- Actual error messages (verbatim)
- Step-by-step solution
- Verification step

### Include When Applicable
- Failed attempts
- Root cause explanation
- Prevention tips
- Related articles

### Never Include
- Credentials or secrets
- Personal blame
- Outdated information presented as current
- Untested solutions

---

## Quality Checklist

- [ ] Title is searchable
- [ ] Problem clearly described
- [ ] Error messages are verbatim
- [ ] Solution is step-by-step
- [ ] Verification step included
- [ ] Tags are appropriate
- [ ] Related articles linked
- [ ] Quick reference created

---

*Part of Art of Fact Cowork Skill Library*
