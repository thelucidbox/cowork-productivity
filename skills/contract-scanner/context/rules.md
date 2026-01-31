# Contract Scanner — Rules & Guidelines

## Output Formatting Rules

### contract-summary.md Format
```markdown
# Contract Summary

**Document**: [Contract name]
**Type**: [SaaS/Vendor/Employment/NDA/etc.]
**Parties**: [Party A] and [Party B]
**Your Role**: [Buyer/Seller/Customer/Provider]
**Date Reviewed**: [Date]

---

## DISCLAIMER

⚠️ This analysis is not legal advice. Always have contracts reviewed by a qualified attorney before signing.

---

## Key Terms

### Term & Renewal
- **Start Date**: [Date]
- **End Date**: [Date]
- **Term Length**: [Duration]
- **Renewal**: [Auto-renew/Manual/Terms]
- **Notice Period**: [Days required for termination/non-renewal]

### Financial Terms
- **Total Value**: [Amount]
- **Payment Terms**: [Schedule]
- **Price Changes**: [How/when prices can change]

### Key Obligations

**Your Obligations**:
- [Obligation 1]
- [Obligation 2]

**Their Obligations**:
- [Obligation 1]
- [Obligation 2]

### Termination
- **For Convenience**: [Terms]
- **For Cause**: [Conditions]
- **Effects**: [What happens on termination]

### Liability & Risk
- **Liability Cap**: [Amount/terms]
- **Indemnification**: [Who indemnifies whom, for what]
- **Insurance**: [Requirements]

### Intellectual Property
- **Ownership**: [Who owns what]
- **License Granted**: [What rights]
- **Work Product**: [Ownership of deliverables]

### Confidentiality
- **Definition**: [What's confidential]
- **Term**: [How long]
- **Exceptions**: [What's excluded]

### Data & Privacy
- **Data Ownership**: [Who owns data]
- **Data Use**: [How data can be used]
- **Data Return/Deletion**: [On termination]

---

## Important Dates

| Date | Event | Action Needed |
|------|-------|---------------|
| [Date] | Contract ends | Renewal decision |
| [Date] | Notice deadline | Notify if not renewing |
```

### red-flags.md Format
```markdown
# Potential Red Flags

**Document**: [Contract name]
**Reviewed**: [Date]

---

## DISCLAIMER

⚠️ These are potential concerns, not definitive legal problems. Discuss with your attorney.

---

## High Priority

### RF-001: [Issue Name]
- **Section**: [Section reference]
- **Language**: "[Quoted text]"
- **Concern**: [Why this might be problematic]
- **Common Alternative**: [What's more typical]
- **Question for Lawyer**: [What to ask]

---

## Medium Priority

### RF-002: [Issue Name]
...

---

## Low Priority / Notes

### RF-003: [Issue Name]
...

---

## Standard Terms (Not Flagged)

These are common terms that appear standard:
- [Term 1]
- [Term 2]
```

### questions-for-legal.md Format
```markdown
# Questions for Legal Review

**Document**: [Contract name]
**Prepared For**: [Lawyer name/firm]

---

## High Priority Questions

1. **Regarding [topic]**: [Question]
   - *Context*: [Why you're asking]

2. **Regarding [topic]**: [Question]
   - *Context*: [Why you're asking]

---

## Clarification Questions

3. **Section [X]**: [Question about interpretation]

---

## Negotiation Questions

4. **Is it typical to**: [Question about industry norms]

---

## Red Flags Discussion

5. **Re: [Red flag]**: [Question about significance]

---

## Areas for Negotiation

Based on analysis, these terms might be negotiable:
- [Term]: [Suggested change]
```

---

## Terms to Always Extract

### Core Terms
- Parties and roles
- Term and renewal
- Payment and pricing
- Termination rights
- Liability limits
- Indemnification
- Confidentiality
- IP ownership

### Contract-Type Specific

**SaaS/Software**:
- SLA and uptime
- Data ownership and portability
- Security requirements
- Breach notification

**Services**:
- Scope of work
- Acceptance criteria
- Change process
- Warranties

**Employment**:
- Non-compete/non-solicit
- IP assignment
- Benefits
- Termination conditions

---

## Red Flag Categories

### High Priority Red Flags
- Unlimited liability
- Broad indemnification (one-sided)
- Automatic renewal with short notice
- One-sided termination rights
- Perpetual license grants
- Unrestricted data use rights

### Medium Priority
- Long notice periods
- Limitation on remedies
- Broad confidentiality definitions
- Non-standard governing law
- Mandatory arbitration

### Low Priority (Note but don't alarm)
- Standard warranty disclaimers
- Typical limitation of liability
- Common integration clauses

---

## Quality Checklist

- [ ] All key terms extracted
- [ ] Important dates identified
- [ ] Red flags categorized by priority
- [ ] Questions prepared for lawyer
- [ ] Calendar entry created
- [ ] Disclaimer prominently displayed

---

*Part of Art of Fact Cowork Skill Library*
