---
name: file-archaeologist
description: --- Takes a messy folder and transforms it into organized structure. Uses content analysis to rename files descriptively, groups related...
---

# File Archaeologist

**Analyze messy folders, rename intelligently, and surface forgotten treasures.**

---

## What This Does

Takes a messy folder and transforms it into organized structure. Uses content analysis to rename files descriptively, groups related items, identifies duplicates, and surfaces forgotten files that might still be valuable.

| Output | What You Get |
|--------|--------------|
| organized-folder/ | Intelligently reorganized files |
| manifest.md | What's in the folder and where |
| delete-candidates.md | Suggested safe deletions |
| rediscovered-items.md | Forgotten files worth revisiting |

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
> "Organize my Downloads folder"

### Option 2: Specific Folder
> "Analyze and organize ~/Documents/Projects-Old/"

### Option 3: Discovery Mode
> "What's worth keeping in my Desktop clutter?"

---

## What I Need From You

### Required
- **Folder path**: Which folder to analyze

### Optional (Enhances Output)
- **Naming convention**: How you like files named
- **Categories**: How you organize (by project, date, type)
- **Keep patterns**: What you definitely want to keep

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Local Files | Full folder access | — |
| File metadata | Dates, sizes, types | — |

---

## Output Location

```
output/
├── organized-folder/        # Reorganized structure
├── manifest.md              # Index of everything
├── delete-candidates.md     # Safe to delete
└── rediscovered-items.md    # Worth revisiting
```

---

## Examples

### Example 1: Downloads Cleanup
**Input**: Downloads folder with 500 files

**Output**:
- Organized by type: Documents, Images, Installers, Archives
- Renamed: IMG_4521.jpg → "2024-01-15-tax-receipt.jpg"
- Delete candidates: 45 installers, 23 duplicates
- Rediscovered: Contract draft never signed

### Example 2: Project Archive
**Input**: Old projects folder

**Output**:
- Organized by project name
- Duplicates identified
- Delete candidates: Temp files, build artifacts
- Rediscovered: Unfinished project with good ideas

### Example 3: Desktop Rescue
**Input**: Cluttered desktop

**Output**:
- Sorted into meaningful folders
- Screenshots grouped
- Temp files flagged
- Active work surfaced

---

## What I Won't Do

- **Won't delete without permission**: Suggest, never delete
- **Won't lose anything**: Original locations preserved in manifest
- **Won't rename without reason**: Descriptive names only
- **Won't ignore your patterns**: Follow your organization style
- **Won't touch system files**: Skip critical system folders

---

## Tips for Best Results

1. **Start with safe folder**: Test on backup first
2. **Share naming preferences**: "I like YYYY-MM-DD prefixes"
3. **Define categories**: "Organize by project name"
4. **Review before moving**: Check manifest before committing
5. **Keep originals**: Don't delete source until satisfied

---

## Troubleshooting

### "Renamed files incorrectly"
Provide naming preferences. Original names preserved in manifest.

### "Missed important files"
Check manifest for original locations. Undo by moving back.

### "Too aggressive on deletions"
Delete list is suggestions only. Review each before removing.

### "Didn't process subfolders"
Specify: "Recursively organize including subfolders"

---

*Part of Art of Fact Cowork Skill Library*
