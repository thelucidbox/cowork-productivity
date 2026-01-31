# Content Atomizer — Rules & Guidelines

## Output Formatting Rules

### twitter-thread.md Format
```markdown
# Twitter Thread: [Topic]

**Source**: [Original content title]
**Length**: [N] tweets
**Post**: [Suggested timing]

---

## The Thread

**1/** [Hook tweet—must grab attention]

**2/** [Expand on hook]

**3/** [Key point 1]

**4/** [Key point 2]

...

**[N]/** [Call to action]

---

## Thread Notes
- Hook optimization: [Notes on why this hook]
- Suggested timing: [Best posting time]
- Hashtags: [Relevant hashtags]
- Reply fodder: [What to expect/respond to]
```

### linkedin-post.md Format
```markdown
# LinkedIn Post: [Topic]

**Source**: [Original content]
**Length**: [X] characters
**Format**: [Story/List/Question/etc.]

---

## The Post

[Hook line—first 2 lines visible before "see more"]

[Body content—professional narrative]

[Call to action]

---

## Post Notes
- First 2 lines: [Why these hook]
- Best posting time: [Suggestion]
- Engagement strategy: [How to respond to comments]
```

### newsletter-section.md Format
```markdown
# Newsletter Section: [Topic]

**Source**: [Original content]
**Length**: [X] words
**Position**: [Feature/secondary/quick hit]

---

## The Section

### [Section Header]

[Opening hook]

[Key content—2-3 paragraphs]

[Transition to CTA]

**[Read the full post →](link)**

---

## Section Notes
- Link text: [Suggested CTA]
- Subject line option: [If this is the feature]
```

### quote-cards.md Format
```markdown
# Quote Cards: [Topic]

**Source**: [Original content]
**Cards**: [N] quotes extracted

---

## Quote 1
> "[Exact quote from source]"

**Visual notes**: [Background suggestion, emphasis]
**Best for**: [Instagram/Twitter image/etc.]

---

## Quote 2
> "[Quote]"

**Visual notes**: [Suggestions]
**Best for**: [Platform]

---

*Design specs: Use consistent brand colors, readable font, source attribution*
```

### video-clips.md Format
```markdown
# Video Clips: [Source Title]

**Source**: [Video file]
**Duration**: [Total length]
**Suggested clips**: [N]

---

## Clip 1: [Title]
**Timestamp**: [Start] - [End] ([Duration])
**Content**: [What happens in this clip]
**Best for**: [Platform/use case]
**ffmpeg command**:
```
ffmpeg -i input.mp4 -ss [start] -to [end] -c copy clip1.mp4
```

---

## Clip 2: [Title]
...
```

---

## Platform Guidelines

### Twitter/X
- Thread length: 5-15 tweets optimal
- Tweet length: Under 280 chars, ideally under 200
- Hook: Must work standalone
- End: Clear CTA (follow, retweet, reply)
- Format: No hashtags mid-thread, maybe 1-2 at end

### LinkedIn
- Length: 1200-1500 characters max
- First 2 lines: Must hook (before "see more")
- Format: Short paragraphs, use line breaks
- Tone: Professional but personal
- End: Question to drive comments

### Newsletter
- Length: 200-400 words for section
- Hook: Why reader should care
- Value: Standalone insight even without clicking
- CTA: Clear link to full content

### Quote Cards
- Length: Under 150 characters ideal
- Standalone: Must work without context
- Visual: Plan for text overlay on image
- Attribution: Include source/speaker

### Video Clips
- Length: 30-90 seconds for social
- Hook: First 3 seconds must grab
- Standalone: Should work without full context
- Platform: Square for feed, vertical for stories

---

## Atomization Principles

### Each Atom Must
- Stand alone (no "as I mentioned")
- Provide value independently
- Match platform conventions
- Reflect source accurately
- Have clear purpose

### Don't
- Create atoms from thin content
- Misrepresent source meaning
- Use same hook across platforms
- Force quantity over quality
- Include internal references

---

## Quality Checklist

Per Atom:
- [ ] Stands alone without source
- [ ] Platform-native format
- [ ] Accurate to source
- [ ] Clear value proposition
- [ ] Appropriate length
- [ ] Has CTA or purpose

Overall:
- [ ] Atoms cover source's key points
- [ ] Not repetitive across platforms
- [ ] Voice consistent with user's brand
- [ ] Each platform got unique angle

---

*Part of Art of Fact Cowork Skill Library*
