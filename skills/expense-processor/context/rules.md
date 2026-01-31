# Expense Processor — Rules & Guidelines

## Output Formatting Rules

### expense-report.xlsx Format
| Column | Description |
|--------|-------------|
| Date | Transaction date |
| Vendor | Business name |
| Description | What was purchased |
| Category | Expense category |
| Amount | Total with tax |
| Currency | USD, EUR, etc. |
| Project | Project code |
| Receipt | Filename reference |
| Status | Processed/Review/Flagged |
| Notes | Additional context |

### anomalies.md Format
```markdown
# Anomalies Report

## Duplicates Detected

| Receipt 1 | Receipt 2 | Confidence |
|-----------|-----------|------------|
| [file1] | [file2] | [%] |

Action: Review and remove duplicate.

---

## Unusual Amounts

| Receipt | Amount | Reason |
|---------|--------|--------|
| [file] | $X | Above typical for category |

Action: Confirm legitimate.

---

## Unreadable Receipts

| Receipt | Issue | Extracted |
|---------|-------|-----------|
| [file] | [problem] | [partial info] |

Action: Manual entry needed.

---

## Policy Violations

| Receipt | Violation | Policy |
|---------|-----------|--------|
| [file] | [issue] | [rule] |

Action: Verify compliance or justify.
```

### reimbursement-request.md Format
```markdown
# Expense Reimbursement Request

**Employee**: [Name]
**Period**: [Date range]
**Submitted**: [Date]

---

## Summary

| Category | Count | Amount |
|----------|-------|--------|
| Meals | [N] | $[X] |
| Travel | [N] | $[X] |
| Supplies | [N] | $[X] |
| **Total** | **[N]** | **$[X]** |

---

## Expense Details

[Table of all expenses]

---

## Attachments

All receipts attached in receipts-processed/ folder.

---

## Certification

I certify these expenses were incurred for legitimate business purposes.

Signature: _____________
Date: _____________
```

---

## OCR Processing Rules

### Extract
- Date
- Vendor name
- Total amount (with tax)
- Individual items if readable
- Payment method

### Handle Uncertainty
- Mark confidence level
- Flag for review if <70% confidence
- Show extracted text for verification

---

## Categorization Rules

### Default Categories
- **Meals**: Restaurants, coffee, food delivery
- **Travel**: Flights, hotels, rideshare, trains
- **Transport**: Uber, Lyft, taxi, parking
- **Supplies**: Office supplies, equipment
- **Software**: Subscriptions, licenses
- **Professional**: Training, conferences
- **Other**: Uncategorized

### Auto-Categorization
Based on vendor name matching.

---

## Duplicate Detection

### Check For
- Same vendor + same date + same amount
- Same amount within 24 hours
- Identical receipt images

### Handling
- Flag as potential duplicate
- Don't auto-delete
- Require human confirmation

---

## Quality Checklist

- [ ] All receipts processed
- [ ] Amounts match receipt totals
- [ ] Categories assigned
- [ ] Duplicates flagged
- [ ] Anomalies documented
- [ ] Originals preserved
- [ ] Totals calculated correctly

---

*Part of Art of Fact Cowork Skill Library*
