# TaskFlow Terminology Guide

**Purpose:** Ensure consistent language when teaching the Antigravity for Product Managers course. Always use these terms exactly as written.

---

## Product Terms (Use These)

| Use This | Not This |
|----------|----------|
| **Workspace** | Project (at top level) |
| **Project** | Board, List, Container |
| **Task** | Ticket, Item, Card |
| **Epic** | Theme, Initiative |
| **Cycle** | Sprint, Iteration, Period |
| **Assignee** | Owner, Responsible |
| **Due date** | Deadline, Target date |

---

## Antigravity Terms (Use These)

| Use This | Not This |
|----------|----------|
| **Agent Manager** | Composer, AI Pane |
| **Conversation view** | Chat, Thread |
| **Editor view** | Code view, IDE mode |
| **Workflow** | Command, Prompt template |
| **Rules** | Instructions, System prompt |
| **Autonomy level** | Mode |
| **Agent-driven** | Autopilot, Full auto |
| **Agent-assisted** | Collaborative, Co-pilot |
| **Review-driven** | Ask mode, Read-only |
| **Planning Mode** | Plan mode |
| **Fast Mode** | Quick mode |
| **@ mention** | Reference, Tag |

---

## Autonomy Levels (Explain These Precisely)

### Agent-driven
- Full autopilot — the agent plans, writes, tests, and iterates independently
- Use when: You have a clear goal and want hands-off execution
- PM use case: "Build me a complete PRD for the mobile onboarding feature"

### Agent-assisted *(recommended default)*
- Collaborative — agent suggests, human reviews and controls
- Use when: You want to stay involved but move faster
- PM use case: "Help me draft the success metrics section of this PRD"

### Review-driven
- Agent analyzes and reviews only — does not generate or change anything
- Use when: You want a second opinion, not new output
- PM use case: "Review my PRD and flag any gaps — don't rewrite it"

---

## Planning Mode vs Fast Mode

### Planning Mode
- Agent thinks deeply before acting
- Creates artifacts: `task.md`, `implementation_plan.md`, `walkthrough.md`
- Best for: Complex multi-step PM work (PRDs, strategy docs, research synthesis)
- Requires: Gemini 3.1 Pro (High) for best results

### Fast Mode
- Agent responds directly and quickly
- No planning artifacts created
- Best for: Quick questions, simple edits, learning exercises
- Works great with: Gemini 3.1 Flash or Gemini 3.1 Pro

---

## Artifacts (Planning Mode Output)

| Artifact | Purpose |
|----------|---------|
| `task.md` | Living checklist — tracks what the agent is doing |
| `implementation_plan.md` | Technical blueprint — the full plan before execution |
| `walkthrough.md` | Proof of work — screenshots, summaries, decisions made |

---

## Company Context Terms

Always refer to the fictional company and its context correctly:

- **Company name:** TaskFlow
- **Product:** Project management SaaS ("Asana meets Linear for remote teams")
- **Stage:** Series B, $2.5M ARR, 10,000 users
- **Student role:** Senior PM owning Activation & Onboarding
- **Goal:** Increase activation rate from 45% → 60%
- **Manager:** Sarah Chen (Head of Product)

---

**Use this terminology consistently across all modules. When students use wrong terms, gently correct them with the right word in context.**
