# Meeting Debrief Playground Template

Use this template when building a playground for configuring meeting debrief extraction settings.

## Layout

```
+------------------------+---------------------------+
|                        |                           |
|  Controls              |  Live Preview             |
|  ────────────────      |  (shows sample debrief    |
|  Extraction Depth      |   output updating in      |
|  [ ] Quick Sync        |   real-time as controls   |
|  [x] Standard          |   change)                 |
|  [ ] Comprehensive     |                           |
|                        |  ┌─────────────────────┐  |
|  Output Sections       |  │ ## Decisions        │  |
|  [x] Decisions         |  │ - Item 1            │  |
|  [x] Action Items      |  │                     │  |
|  [x] Open Questions    |  │ ## Action Items     │  |
|  [ ] Full Transcript   |  │ - @person: task     │  |
|                        |  └─────────────────────┘  |
|  Tone                  |                           |
|  ○ Casual              +---------------------------+
|  ● Professional        |  Prompt Output            |
|  ○ Executive           |                           |
|                        |  "Process my meeting      |
|  Action Item Format    |   notes using standard    |
|  [Dropdown ▼]          |   extraction..."          |
|                        |                           |
|  Presets: [Quick][Std] |  [ Copy Prompt ]          |
+------------------------+---------------------------+
```

## Control specifications

| Control | Type | Options | Default |
|---------|------|---------|---------|
| Extraction Depth | Radio | Quick Sync, Standard, Comprehensive | Standard |
| Decisions | Checkbox | on/off | on |
| Action Items | Checkbox | on/off | on |
| Open Questions | Checkbox | on/off | on |
| Follow-ups | Checkbox | on/off | off |
| Full Transcript | Checkbox | on/off | off |
| Tone | Radio | Casual, Professional, Executive | Professional |
| Action Format | Dropdown | Simple List, With Deadlines, Kanban-Ready | With Deadlines |

## Presets

| Preset | Settings |
|--------|----------|
| Quick Sync | Quick depth, Decisions + Actions only, Casual, Simple List |
| Standard | Standard depth, all except transcript, Professional, With Deadlines |
| Executive Brief | Quick depth, Decisions only, Executive, Simple List |
| Deep Dive | Comprehensive, all sections, Professional, Kanban-Ready |
| Team Handoff | Standard, Actions + Follow-ups, Professional, With Deadlines |

## Preview rendering

Show a mock debrief output that updates based on controls:

```javascript
function renderPreview() {
  const sections = [];

  if (state.showDecisions) {
    sections.push(renderDecisionsSection(state.depth));
  }
  if (state.showActions) {
    sections.push(renderActionsSection(state.actionFormat));
  }
  if (state.showQuestions) {
    sections.push(renderQuestionsSection());
  }
  // ...

  preview.innerHTML = sections.join('\n');
}
```

Use placeholder content that feels realistic:
- "Decided to proceed with Q2 launch date"
- "@Sarah: Finalize pricing model by Friday"
- "Open: Need clarification on compliance requirements"

## Prompt output examples

**Standard settings:**
> Process my meeting notes and extract decisions, action items, and open questions. Use a professional tone and format action items with assignees and deadlines.

**Quick Sync preset:**
> Process my meeting notes for a quick sync summary. Just capture key decisions and action items in a casual tone.

**Executive Brief preset:**
> Process my meeting notes into an executive brief. Focus only on decisions made, using executive-appropriate language. Keep it concise.

**Comprehensive:**
> Process my meeting notes comprehensively. Extract all decisions with context, action items in kanban-ready format with assignees and deadlines, open questions, and suggested follow-ups. Use a professional tone throughout.

## Sample HTML structure

```html
<div class="playground">
  <div class="controls">
    <section class="control-group">
      <h3>Extraction Depth</h3>
      <label><input type="radio" name="depth" value="quick"> Quick Sync</label>
      <label><input type="radio" name="depth" value="standard" checked> Standard</label>
      <label><input type="radio" name="depth" value="comprehensive"> Comprehensive</label>
    </section>

    <section class="control-group">
      <h3>Output Sections</h3>
      <label><input type="checkbox" id="decisions" checked> Decisions</label>
      <label><input type="checkbox" id="actions" checked> Action Items</label>
      <!-- ... -->
    </section>

    <section class="presets">
      <button onclick="applyPreset('quick')">Quick Sync</button>
      <button onclick="applyPreset('standard')">Standard</button>
      <button onclick="applyPreset('executive')">Executive</button>
    </section>
  </div>

  <div class="output-area">
    <div id="preview" class="preview"></div>
    <div class="prompt-output">
      <pre id="prompt"></pre>
      <button onclick="copyPrompt()">Copy Prompt</button>
    </div>
  </div>
</div>
```
