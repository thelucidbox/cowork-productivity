---
name: content-atomizer
description: --- Takes your long-form content—blog post, video transcript, presentation—and atomizes it into platform-specific pieces. Each output is tailored to its...
---

# Content Atomizer

**Break long-form content into platform-specific pieces—each atom stands alone.**

---

## What This Does

Takes your long-form content—blog post, video transcript, presentation—and atomizes it into platform-specific pieces. Each output is tailored to its platform's format and audience expectations. Turn one piece of content into a week's worth of social media, newsletter segments, and quote cards.

| Output | What You Get |
|--------|--------------|
| twitter-thread.md | Numbered thread with hooks |
| linkedin-post.md | Professional narrative format |
| newsletter-section.md | Email-ready segment |
| quote-cards.md | Visual quote extractions |
| video-clips.md | Suggested clip timestamps |

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
> "Atomize my blog post into social content"

### Option 2: With File
> "Run content atomizer on article.md in input/"

### Option 3: Platform-Specific
> "Turn this into a Twitter thread and LinkedIn post"

---

## What I Need From You

### Required
- **Source content**: The long-form piece to atomize
- **Target platforms**: Where you want to publish (or use defaults)

### Optional (Enhances Output)
- **Key message**: What's the one thing you want people to remember?
- **Audience context**: Who follows you on each platform?
- **Voice notes**: Any platform-specific tone preferences
- **Hashtags**: Your standard hashtags per platform
- **CTA**: What action you want (follow, subscribe, read more)

---

## What I'll Pull Automatically

| Integration | What I Get | Fallback |
|-------------|-----------|----------|
| Local Files | Source content from input folder | Paste directly |
| Video (ffmpeg) | Suggested clip timestamps | Manual timestamp notes |

---

## Output Location

```
output/
└── atoms/
    ├── twitter-thread.md     # Thread with hooks
    ├── linkedin-post.md      # Professional format
    ├── newsletter-section.md # Email segment
    ├── quote-cards.md        # Visual quotes
    └── video-clips.md        # Clip suggestions
```

---

## Claude Artifacts (Interactive)

Ask Claude to create interactive artifacts you can use and return to:

| Artifact Type | What It Does | How to Request |
|---------------|--------------|----------------|
| **Content Atoms Grid** | See all atoms from one piece side by side | "Create a content atoms artifact" |
| **Quote Card Designer** | Preview and edit visual quote layouts | "Build a quote card artifact" |
| **Platform Preview** | See how content looks on each platform | "Make a platform preview artifact" |
| **Publishing Checklist** | Track which atoms have been published | "Create a publishing tracker artifact" |

### Example Artifact Requests

**Atoms Overview**
> "Create a React artifact showing all content atoms from this piece: Twitter thread, LinkedIn post, newsletter section, quote cards—in a grid view"

**Quote Card Previewer**
> "Build an artifact showing extracted quotes in card format with different background color options"

**Publishing Tracker**
> "Create a checklist artifact with each atom, platform, and published (yes/no) status"

### Tips
- Use the grid view to see your full content distribution at once
- The quote card previewer helps select the best visual quotes
- Track publishing to avoid posting duplicates

---

## Examples

### Example 1: Blog Post Atomization
**Input**: 2000-word blog post on productivity

**Output**:
- Twitter thread: 8 tweets, hook first, CTA last
- LinkedIn post: 1200 characters, professional angle
- Newsletter section: Key insights + link to full post
- Quote cards: 4 standalone quotes for Instagram/graphics
- Clip suggestions: If video exists, key moments

### Example 2: Podcast Episode
**Input**: 45-minute podcast transcript

**Output**:
- Twitter thread: Best insights as thread
- LinkedIn post: Key takeaway narrative
- Quote cards: Guest quotes highlighted
- Video clips: 5 suggested 30-60 second clips with timestamps

### Example 3: Presentation
**Input**: Conference talk slides and transcript

**Output**:
- Twitter thread: Main points as thread
- LinkedIn post: Professional recap
- Newsletter section: Summary for subscribers
- Quote cards: Key slide quotes
- Video clips: Strongest segments

---

## What I Won't Do

- **Won't post for you**: Creates ready-to-post content, you publish
- **Won't pad thin content**: If source is thin, atoms will be thin
- **Won't misrepresent**: Each atom reflects original accurately
- **Won't violate platform norms**: Follows each platform's conventions
- **Won't add fabricated quotes**: Only extracts what's actually in source

---

## Tips for Best Results

1. **Provide rich source**: More depth = more atoms possible
2. **Highlight key sections**: "The part about X is strongest" focuses extraction
3. **Share platform context**: "My LinkedIn is B2B, Twitter is casual"
4. **Include existing threads**: Show me your past posts for voice matching
5. **Specify call-to-action**: What do you want people to do?

---

## Troubleshooting

### "Atoms feel repetitive"
Source may have one main point. That's okay—fewer, stronger atoms beat forced variety.

### "Thread is too long/short"
Specify: "Max 5 tweets" or "Need at least 10 tweets for algorithm."

### "Tone doesn't match my brand"
Share examples of your existing content on each platform. I'll match your voice.

### "Missing platform I need"
Ask: "Also create a [platform] version" and I'll add it.

---

*Part of Art of Fact Cowork Skill Library*
