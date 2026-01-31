# File Archaeologist — Rules & Guidelines

## Output Formatting Rules

### manifest.md Format
```markdown
# File Manifest

**Source Folder**: [Path]
**Analyzed**: [Date]
**Total Files**: [N]
**Total Size**: [Size]

---

## Summary

| Category | Count | Size |
|----------|-------|------|
| Documents | [N] | [Size] |
| Images | [N] | [Size] |
| Installers | [N] | [Size] |
| Other | [N] | [Size] |

---

## File Inventory

### Documents

| New Location | Original Name | Original Location | Action |
|--------------|---------------|-------------------|--------|
| [new path] | [old name] | [old path] | Renamed/Moved |

### Images
...

---

## Undo Information

To restore original structure:
1. Reference this manifest
2. Move files back to original locations
3. Rename to original names
```

### delete-candidates.md Format
```markdown
# Delete Candidates

**Source Folder**: [Path]
**Total Candidates**: [N]
**Potential Space Saved**: [Size]

---

## IMPORTANT

⚠️ Review each item before deleting. These are suggestions only.

---

## Confident Deletions

These are almost certainly safe to delete:

| File | Location | Size | Reason |
|------|----------|------|--------|
| .DS_Store | [path] | 4KB | System file |
| *.tmp | [path] | 2MB | Temp file |

---

## Duplicates

| Keep | Delete | Size |
|------|--------|------|
| [file1] | [file2] (duplicate) | [size] |

---

## Large Files to Review

| File | Size | Last Modified | Keep? |
|------|------|---------------|-------|
| [file] | 500MB | 2 years ago | ? |

---

## Old Installers

| Installer | Version | Size | Current Available |
|-----------|---------|------|-------------------|
| [file] | 2.1 | 150MB | 3.0 available |
```

### rediscovered-items.md Format
```markdown
# Rediscovered Items

Files that might be worth revisiting:

---

## Potentially Valuable

### [File Name]
- **Location**: [Path]
- **Created**: [Date]
- **Last Modified**: [Date]
- **Why Flagged**: [Never opened / Draft / Interesting content]

---

## Unfinished Work

| File | Type | Last Modified | Preview |
|------|------|---------------|---------|
| [draft] | Document | [Date] | [First line...] |

---

## Forgotten Projects

| Folder | Files | Last Activity |
|--------|-------|---------------|
| [project] | [N] | [Date] |
```

---

## Analysis Rules

### File Classification
- **Documents**: .pdf, .doc, .docx, .txt, .md, .xls, .xlsx
- **Images**: .jpg, .png, .gif, .heic, .svg
- **Installers**: .dmg, .pkg, .app, .exe, .msi
- **Archives**: .zip, .tar, .gz, .rar
- **Code**: .py, .js, .html, .css, etc.
- **Media**: .mp3, .mp4, .mov, .wav

### Rename Logic
1. Extract date from metadata or content
2. Identify descriptive content
3. Apply naming convention
4. Preserve extension

### Duplicate Detection
- Compare file hashes
- Compare size + date
- Note which is "original" (older)

---

## Safety Rules

### Never Delete
- Files modified in last 7 days
- Files with "keep" or "important" in name
- Files in protected locations
- When in doubt

### Ask Before
- Deleting duplicates
- Removing old files
- Changing file structure

---

## Quality Checklist

- [ ] All files cataloged
- [ ] Manifest is complete
- [ ] No files lost
- [ ] Renames are descriptive
- [ ] Delete candidates are justified
- [ ] Original locations preserved

---

*Part of Art of Fact Cowork Skill Library*
