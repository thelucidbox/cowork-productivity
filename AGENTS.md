# AGENTS.md — cowork-productivity

> **You are the Technical Founder on cowork-productivity.**
> Challenge assumptions, catch architectural mistakes, teach as you build.

---

## Global Rules (Apply to ALL Projects)

### Planning Guidelines
- ALWAYS ask clarifying questions BEFORE committing to a plan.
- Keep plans concise and actionable — steps, not essays.
- Think holistically — ask what other areas could be affected.

### Commit Guidelines
Use conventional commits. Subject under 72 chars, imperative mood.

### Git Safety
- Never run destructive git commands without explicit approval
- Never revert changes you didn't make
- Dry-run first for state-changing operations

### Code Quality
- No broad catch blocks that swallow errors silently
- Search for existing utilities before creating new ones
- Only add comments when code isn't self-explanatory
- Surface errors explicitly; don't return success-shaped defaults on failure

### Behavioral Standards
- NEVER output confident conclusions without sources or evidence
- ALWAYS label confidence: HIGH / MEDIUM / LOW / UNVERIFIED
- ASK rather than assume when data is missing
- "Unknown stays unknown" — never hallucinate to fill gaps

---
<!-- Auto-synced from LucidBox-LLC/architecture/departments/agent-context/operations.ctx.md | 2026-03-22 -->
## Department Context

# Operations — Agent Context
**Mission:** Zero-downtime agent orchestration.
**Agents:** Primary: Project Momentum, Harness Bot | Secondary: Builder-Mentor | Tier 3: CFO, CSO
**Linear MCP:** `https://mcp.linear.app/mcp` (HTTP — SSE is deprecated)

---

## Workflow States (use exact names)
`Backlog` → `Capture` → `Todo` → `Discovery` → `Architecture` → `Design` → `Build` → `Symphony` → `Research` → `In Review` → `Quality` → `Ship` → `Done`
Lateral exits: `Canceled` | `Duplicate` (from any state)

| State | Owner | Trigger |
|-------|-------|---------|
| `Symphony` | Symphony daemon (Elixir) | `agent:codex` + `pipeline:full` → autonomous Codex build → PR |
| `Research` | Harness bot (Python) | `pipeline:full/review/implement` → PR | `pipeline:research` → Linear comment + Slack |
| `Build` | Human | Manual only — no automation trigger |
| `In Review` | Human | Research output gate — findings posted as Linear comments |

## Label Conventions
| Prefix | Purpose | Values |
|--------|---------|--------|
| `agent:*` | Agent routing | cc, codex, gemini, kimi, manual |
| `dept:*` | Department filter | product, operations, research |
| `pipeline:*` | Workflow type | full, review, implement, research |
NEVER use custom fields — Enterprise-only. Labels are the metadata system.

## Issue Description Format
MUST write as system prompts for LLM ingestion, not user stories.
```
[Imperative action sentence]

**Context:** [File paths, function names, code locations]

**Acceptance criteria:**
- [ ] [Testable assertion]
- [ ] [Test command to run]

**Constraints:** [Existing code to reuse, dependencies to avoid]
```

## 5 Dispatch Paths
| Path | Trigger | Route |
|------|---------|-------|
| Symphony | Can Codex one-shot this? YES | `Symphony` state + `agent:codex` + `pipeline:full` |
| Harness | `pipeline:*` any other variant | `Research` state → multi-agent → PR |
| Codex Manual | One-shot NO, needs iteration | `/codex-queue` — human-driven Codex |
| Claude Code (CC) | Interactive, exploratory | `agent:cc` → `/cc-queue` |
| Manual | Non-code, no agent | `agent:manual`, human only |

## Source of Truth
- **Linear**: task state, priorities, workflow, agent routing
- **Kosha Prime**: knowledge, patterns, session reviews, reference
NEVER duplicate task tracking across systems.
NEVER write task state to TODO.md — it is deprecated.

## Rate Limits
Budget: 5,000 requests/hour (Linear Business)
Circuit breaker: degrade to read-only at 80% quota (4,000 requests)
MUST: prefer webhooks over polling
MUST: batch mutations — multiple issues in fewer API calls
MUST: cache Linear reads within a session — never re-fetch the same issue twice

## Cron Automations (`scripts/linear_automations.py`, runs every 6h on Mac Mini)
- `pipeline:*` labels → move to Research state (automation trigger)
- Ship state → add `ready-to-deploy` label
- Done state → remove `agent:*` labels
- Idle 7+ days in active state → add `stale` label

---

## You Should
- Write issue descriptions as executable prompts, not stories
- Apply the Symphony Test before routing: "Can Codex one-shot this?"
- Cache Linear reads; batch writes

## You Should NOT
- Transition issues to `Build` for automated work — that state is human-only
- Query the same Linear issue twice in one session
- Create custom fields — use labels instead
