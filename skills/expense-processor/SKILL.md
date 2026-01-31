---
name: expense-processor
description: --- Takes photos of receipts and transforms them into organized expense reports. Uses OCR to extract details, auto-categorizes expenses, flags...
---

# Expense Processor

**Transform receipt photos into categorized expense reports with anomaly detection.**

---

## What This Does

Takes photos of receipts and transforms them into organized expense reports. Uses OCR to extract details, auto-categorizes expenses, flags duplicates and anomalies, and generates reimbursement-ready documentation.

| Output | What You Get |
|--------|--------------|
| expense-report.xlsx | Categorized expense spreadsheet |
| anomalies.md | Duplicates, unusual amounts flagged |
| reimbursement-request.md | Ready-to-submit request |
| receipts-processed/ | Renamed, organized receipts |

---


---

## IMPORTANT: Always Ask First

When the user says "ready to work", "get to work", or loads this folder:

1. **Greet and explain** what this skill does
2. **Ask what they need**:
   > "I can help you with [skill purpose]. Would you like to:
   > 1. **Start fresh** - I'll guide you through what I need
   > 2. **Use files in input/** - I'll process what you've added
   > 3. **See an example** - I'll show you what this produces"

3. **Never auto-run** without confirming what the user wants

### Why This Matters
Users loading a skill folder expect guidance, not assumptions. Always confirm before processing.

## Quick Start

### Option 1: Natural Language
> "Process the receipts in my input folder"

### Option 2: Single Receipt
> "Add this receipt to my expenses"

### Option 3: Trip Summary
> "Process all receipts from my NYC trip"

---

## What I Need From You

### Required
- **Receipt images**: Photos of receipts (any format)

### Optional (Enhances Output)
- **Category hints**: What was this for? (meals, travel, supplies)
- **Project codes**: For allocation
- **Expense policy**: Your company's rules for flagging
- **Date range**: For filtering

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Local Files | Receipt images from input folder | Upload directly |
| OCR | Text extraction from images | Manual entry |

---

## Output Location

```
output/
├── expense-report.xlsx        # Main spreadsheet
├── anomalies.md               # Flagged items
├── reimbursement-request.md   # Submit-ready doc
└── receipts-processed/
    └── [renamed receipts]
```

---

## Examples

### Example 1: Monthly Processing
**Input**: 23 receipt photos from last month

**Output**:
- Spreadsheet: Date, vendor, amount, category for each
- Categories: Meals (12), Transport (6), Supplies (5)
- Anomalies: 2 duplicates detected, 1 unusual amount flagged
- Total: $847.23

### Example 2: Business Trip
**Input**: 15 receipts labeled "NYC trip"

**Output**:
- All receipts tagged to trip
- Per-day breakdown
- Category subtotals
- Reimbursement request ready for submission

### Example 3: Ongoing Tracking
**Input**: Weekly receipt dump

**Output**:
- Appended to running expense file
- Running monthly total
- Category trends over time

---

## What I Won't Do

- **Won't guess at unreadable**: Mark unclear items for review
- **Won't duplicate entries**: Detect and flag duplicates
- **Won't assume category**: Ask if uncertain
- **Won't delete originals**: Always preserve source images
- **Won't submit for you**: Generate docs, you submit

---

## Tips for Best Results

1. **Good photos help**: Flat, well-lit, readable
2. **Include context**: "Dinner with client" helps categorization
3. **Process regularly**: Weekly beats monthly for accuracy
4. **Keep originals**: Don't delete source photos
5. **Note project codes**: For proper allocation

---

## Troubleshooting

### "Receipt not readable"
Retake photo with better lighting. If original is faded, manually enter details.

### "Wrong category"
Provide category hints or adjust after generation.

### "Missing receipt"
Flag in anomalies for manual handling. Don't delete from report.

### "Duplicate detected but it's valid"
Override: "These are two separate purchases" and I'll un-flag.

---

*Part of Art of Fact Cowork Skill Library*
