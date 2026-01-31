# Project Kickoff Playground Template

Use this template when building a playground for configuring project initialization parameters.

## Layout

```
+------------------------+---------------------------+
|  Controls              |  Live Preview             |
|  ────────────────      |  (project charter preview)|
|  Project Type          |                           |
|  Scope Definition      |  ┌─────────────────────┐  |
|  Stakeholder Depth     |  │ Project: [Name]     │  |
|  Risk Assessment       |  │ Scope: Medium       │  |
|  Timeline Granularity  |  │ Timeline: 8 weeks   │  |
|                        |  │ Stakeholders: 5     │  |
|  Presets               |  └─────────────────────┘  |
+------------------------+---------------------------+
|  Prompt Output         |  [ Copy Prompt ]          |
+------------------------+---------------------------+
```

## Control specifications

| Control | Type | Options | Default |
|---------|------|---------|---------|
| Project Type | Dropdown | Feature, Initiative, Program | Feature |
| Scope Definition | Slider | Narrow → Comprehensive | Medium |
| Stakeholder Mapping | Radio | Key Only, Extended, Full Org | Extended |
| Risk Assessment | Radio | Light, Standard, Thorough | Standard |
| Timeline | Dropdown | Milestones Only, Weekly, Daily | Weekly |
| Include RACI | Checkbox | on/off | on |
| Include Success Metrics | Checkbox | on/off | on |

## Presets

| Preset | Description |
|--------|-------------|
| Quick Feature | Narrow scope, key stakeholders, milestones only |
| Standard Initiative | Medium scope, extended stakeholders, weekly timeline |
| Enterprise Program | Comprehensive scope, full org, daily timeline, thorough risk |
| MVP Sprint | Narrow scope, no RACI, milestones only |

## Prompt output examples

**Standard:**
> Create a project kickoff package for a new feature. Include medium-scope definition, stakeholder mapping for the extended team, standard risk assessment, and weekly timeline breakdown. Generate RACI matrix and success metrics.

**Quick Feature:**
> Create a quick project kickoff for a new feature. Focus on narrow scope with key stakeholders only. Just milestones, no detailed timeline needed.
