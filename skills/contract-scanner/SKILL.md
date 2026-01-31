---
name: contract-scanner
description: --- Takes a contract document and extracts key terms, identifies potential red flags, and generates questions for legal review. Creates...
---

# Contract Scanner

**Extract key terms, red flags, and questions from contracts—NOT legal advice.**

---

## What This Does

Takes a contract document and extracts key terms, identifies potential red flags, and generates questions for legal review. Creates a summary for quick understanding and calendar reminders for critical dates. This is NOT legal advice—always have a lawyer review.

| Output | What You Get |
|--------|--------------|
| contract-summary.md | Key terms extracted |
| red-flags.md | Potential concerns flagged |
| questions-for-legal.md | Questions to ask your lawyer |
| calendar-entry.ics | Important dates |

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
> "Scan this vendor contract for key terms"

### Option 2: With File
> "Analyze the contract in input/"

### Option 3: Specific Focus
> "What are the termination clauses in this agreement?"

---

## What I Need From You

### Required
- **Contract document**: PDF, Word doc, or text

### Optional (Enhances Output)
- **Contract type**: SaaS, employment, NDA, vendor, etc.
- **Your role**: Are you the buyer or seller?
- **Concerns**: Specific areas to focus on
- **Comparison**: Other contracts to compare terms

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Local Files | Contract from input folder | Paste text |
| Calendar | Add important dates | Export .ics file |

---

## Output Location

```
output/
├── contract-summary.md      # Key terms
├── red-flags.md             # Potential concerns
├── questions-for-legal.md   # For your lawyer
└── calendar-entry.ics       # Important dates
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Contract Summary Card** | Key terms at a glance with status indicators | "Create a contract summary artifact" |
| **Red Flag Tracker** | List of concerns with severity and resolution status | "Build a red flag tracker artifact" |
| **Date Tracker** | Important contract dates with countdown | "Make a contract dates artifact" |
| **Comparison Matrix** | Compare terms across multiple contracts | "Create a contract comparison artifact" |

### Example Artifact Requests

**Contract Dashboard**
> "Create a React artifact showing: contract name, status, key terms (value, term, renewal), and days until action needed"

**Red Flag Review**
> "Build an interactive list of red flags with: severity (high/medium/low), clause reference, and checkbox for 'discussed with lawyer'"

**Contract Calendar**
> "Create a timeline artifact showing: start date, renewal notice deadline, and end date for all active contracts"

### Tips
- Use the date tracker to never miss a renewal deadline
- Update the red flag tracker after legal review
- The comparison matrix helps negotiate better terms

---

## Examples

### Example 1: SaaS Agreement
**Input**: Software subscription agreement PDF

**Output**:
- Summary: Term, pricing, data ownership, SLA
- Red flags: Auto-renewal (90 days notice), unlimited liability
- Questions: "What happens to data on termination?"
- Calendar: Contract end date, renewal notice deadline

### Example 2: Vendor Contract
**Input**: Professional services agreement

**Output**:
- Summary: Scope, fees, IP ownership, confidentiality
- Red flags: Broad indemnification clause
- Questions: "Should we cap indemnification?"
- Calendar: Payment milestones, deliverable dates

### Example 3: NDA Review
**Input**: Mutual NDA

**Output**:
- Summary: Parties, definition of confidential, term
- Red flags: Very broad definition, long term (5 years)
- Questions: "Is 5-year term standard for our industry?"

---

## What I Won't Do

- **Won't provide legal advice**: This is extraction, not counsel
- **Won't guarantee completeness**: May miss nuances
- **Won't replace lawyer review**: Always get professional advice
- **Won't sign for you**: Information only
- **Won't interpret complex terms**: Flag for expert review

---

## DISCLAIMER

**This skill provides document analysis, NOT legal advice.** Always have contracts reviewed by a qualified attorney before signing. Red flags identified are potential concerns, not definitive legal problems. Questions generated are starting points for discussion with your lawyer.

---

## Tips for Best Results

1. **Full document**: Partial contracts miss context
2. **Note your role**: Buyer vs. seller changes what matters
3. **Share concerns**: "I'm worried about liability" focuses analysis
4. **Include attachments**: Schedules and exhibits matter
5. **Ask your lawyer**: Use outputs to prepare for legal review

---

## Troubleshooting

### "Missing sections"
Some contracts reference external documents. Note what's missing.

### "Red flags seem minor"
May be standard terms. Discuss with lawyer to assess.

### "Need deeper analysis"
Ask for specific section review: "Analyze Section 7 in detail."

### "Different contract type"
Specify: "This is an employment contract, not vendor agreement."

---

*Part of Art of Fact Cowork Skill Library*
