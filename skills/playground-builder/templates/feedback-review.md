# Feedback Review Playground Template

Use this template when building a playground for configuring feedback synthesis settings.

## Layout

```
+------------------------+---------------------------+
|  Controls              |  Live Preview             |
|  ────────────────      |  (synthesized feedback)   |
|  Source Types          |                           |
|  Theme Sensitivity     |  ┌─────────────────────┐  |
|  Priority Weighting    |  │ Theme 1: UX Issues  │  |
|  Output Format         |  │ ████████░░ 8 mentions│  |
|                        |  │                     │  |
|  Presets               |  │ Theme 2: Performance│  |
+------------------------+  │ █████░░░░░ 5 mentions│  |
|  Prompt Output         |  └─────────────────────┘  |
+------------------------+---------------------------+
```

## Control specifications

| Control | Type | Options | Default |
|---------|------|---------|---------|
| Source Types | Multi-checkbox | Surveys, 1:1s, Reviews, Support, Social | Surveys, 1:1s |
| Theme Sensitivity | Slider | Broad → Granular | Medium |
| Priority Weighting | Radio | Equal, Frequency-based, Severity-based | Frequency |
| Output Format | Dropdown | Themes Only, With Quotes, Action Plan | With Quotes |
| Sentiment Analysis | Checkbox | on/off | on |
| Trend Comparison | Checkbox | on/off | off |

## Presets

| Preset | Description |
|--------|-------------|
| Quick Pulse | Surveys only, broad themes, equal weight |
| Deep Analysis | All sources, granular themes, severity-based, action plan |
| Executive Summary | Surveys + Reviews, broad themes, themes only |
| Support Triage | Support + Social, granular, severity-based |

## Prompt output examples

**Standard:**
> Synthesize feedback from surveys and 1:1s. Identify themes at medium granularity, weight by frequency, and include supporting quotes. Run sentiment analysis on each theme.

**Deep Analysis:**
> Perform comprehensive feedback synthesis across all sources (surveys, 1:1s, reviews, support tickets, social). Use granular theme detection with severity-based prioritization. Output as an action plan with supporting quotes and trend comparison to last period.
