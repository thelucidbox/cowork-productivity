---
name: playground-builder
description: Creates interactive HTML playgrounds for productivity workflows. Configure meeting debriefs, project kickoffs, feedback synthesis, and goal tracking visually, then copy the generated prompt.
---

# Productivity Playground Builder

Creates self-contained HTML playgrounds that let users visually configure productivity workflows, see a live preview, and copy out a ready-to-use prompt.

## When to use this skill

When the user wants to:
- Configure a meeting debrief extraction (what to capture, tone, format)
- Plan a project kickoff (scope, stakeholders, milestones)
- Set up feedback synthesis rules (sources, themes, priorities)
- Define goal tracking parameters (OKRs, metrics, review cadence)

## How to use this skill

1. **Identify the playground type** from the user's request
2. **Load the matching template** from `templates/`:
   - `templates/meeting-debrief.md` — Configure debrief extraction settings
   - `templates/project-kickoff.md` — Plan project scope and timeline
   - `templates/feedback-review.md` — Set up feedback synthesis rules
   - `templates/goal-tracker.md` — Define goal/OKR tracking parameters
3. **Follow the template** to build the playground
4. **Open in browser** with `open <filename>.html`

## Core requirements (every playground)

- **Single HTML file.** Inline all CSS and JS. No external dependencies.
- **Live preview.** Updates instantly on every control change.
- **Prompt output.** Natural language instruction, not a value dump. Only mentions non-default choices.
- **Copy button.** Clipboard copy with "Copied!" feedback.
- **Sensible defaults + presets.** Include 3-5 named presets (e.g., "Quick Sync", "Executive Briefing", "Deep Dive").
- **Dark theme.** System font for UI, monospace for code/values.

## State management pattern

```javascript
const state = { /* all configurable values */ };
const DEFAULTS = { /* initial values */ };

function updateAll() {
  renderPreview();
  updatePrompt();
}
```

## Prompt output pattern

```javascript
function updatePrompt() {
  const parts = [];

  // Only mention non-default values
  if (state.tone !== DEFAULTS.tone) {
    parts.push(`using a ${state.tone} tone`);
  }

  // Use qualitative language
  if (state.detailLevel === 'comprehensive') {
    parts.push('with comprehensive detail');
  }

  prompt.textContent = `Process my meeting notes ${parts.join(', ')}.`;
}
```

## Available templates

### Meeting Debrief (`meeting-debrief.md`)
Configure how meeting notes are processed:
- Extraction depth (quick/standard/comprehensive)
- Output sections (decisions, actions, questions, follow-ups)
- Tone (casual/professional/executive)
- Action item format (simple list, assigned with deadlines, kanban-ready)

### Project Kickoff (`project-kickoff.md`)
Plan project initialization:
- Scope definition (narrow/standard/comprehensive)
- Stakeholder mapping depth
- Risk assessment level
- Timeline granularity (milestones only, weekly, daily)

### Feedback Review (`feedback-review.md`)
Set up feedback synthesis:
- Source types (surveys, 1:1s, reviews, support tickets)
- Theme detection sensitivity
- Priority weighting
- Output format (themes, recommendations, action plan)

### Goal Tracker (`goal-tracker.md`)
Define goal tracking parameters:
- Framework (OKRs, SMART, custom)
- Review cadence (weekly, biweekly, monthly)
- Progress visualization style
- Accountability features
