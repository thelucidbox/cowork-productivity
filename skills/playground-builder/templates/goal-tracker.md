# Goal Tracker Playground Template

Use this template when building a playground for configuring goal/OKR tracking parameters.

## Layout

```
+------------------------+---------------------------+
|  Controls              |  Live Preview             |
|  ────────────────      |  (goal dashboard mockup)  |
|  Framework             |                           |
|  Review Cadence        |  ┌─────────────────────┐  |
|  Visualization Style   |  │ Q1 Objectives       │  |
|  Accountability        |  │ ═══════════════════ │  |
|                        |  │ O1: Launch v2 [75%] │  |
|  Presets               |  │ ▓▓▓▓▓▓▓▓░░ On Track │  |
+------------------------+  └─────────────────────┘  |
|  Prompt Output         |  [ Copy Prompt ]          |
+------------------------+---------------------------+
```

## Control specifications

| Control | Type | Options | Default |
|---------|------|---------|---------|
| Framework | Dropdown | OKRs, SMART Goals, North Star + Bets, Custom | OKRs |
| Review Cadence | Radio | Weekly, Biweekly, Monthly, Quarterly | Biweekly |
| Visualization | Dropdown | Progress Bars, Burndown, Traffic Light, Kanban | Progress Bars |
| Accountability | Multi-checkbox | Owner Assignment, Check-in Reminders, Blockers Log | All |
| Scoring Method | Radio | Binary, Percentage, Confidence Level | Percentage |
| Cascade View | Checkbox | on/off | off |

## Presets

| Preset | Description |
|--------|-------------|
| Startup OKRs | OKRs, weekly review, traffic light, all accountability |
| Enterprise Goals | SMART, monthly, progress bars, cascade view |
| Personal Growth | Custom framework, weekly, kanban, check-in reminders |
| Team Sprint | OKRs, biweekly, burndown, blockers log |

## Prompt output examples

**Standard OKRs:**
> Set up goal tracking using the OKR framework with biweekly reviews. Visualize progress with progress bars and percentage scoring. Enable owner assignment, check-in reminders, and blockers logging.

**Enterprise:**
> Configure enterprise goal tracking with SMART goals framework. Monthly review cadence with progress bar visualization and cascade view to show goal hierarchy. Include all accountability features.
