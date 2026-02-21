# Antigravity PM Course — Project Context

## What This Repo Is

This is the **Antigravity for Product Managers** course — an interactive, AI-guided course that teaches Product Managers to use Antigravity (an AI coding/agent tool powered by Gemini 3.1 Pro) to do real PM work faster.

The course is structured as:
- **Course materials** (`course-materials/`) — the actual lesson content students interact with
- **Website** (`website/`) — Next.js site for the course landing page / delivery

---

## Project Structure

```
antigravity-pm-course/
├── course-materials/         # Student-facing course content
│   ├── .agent/
│   │   ├── rules/            # Persistent AI context rules (always loaded)
│   │   │   ├── course-instructor.md      # Teaching persona & style
│   │   │   ├── taskflow-context.md       # Fictional company context
│   │   │   ├── taskflow-terminology.md   # Consistent terminology guide
│   │   │   └── SCRIPT_INSTRUCTIONS.md   # How to follow teaching scripts
│   │   └── workflows/        # Slash commands (start-1-1.md etc.)
│   ├── company-context/      # TaskFlow company docs (COMPANY, PRODUCT, PERSONAS, COMPETITIVE)
│   └── lesson-modules/       # 9 lesson modules (1.1 through 2.3)
├── website/                  # Next.js course website
│   ├── pages/
│   ├── components/
│   └── styles/
├── IMPLEMENTATION_SPEC.md    # Spec for Cursor → Antigravity conversion
├── CLAUDE.md                 # This file
└── requirements.txt          # Python deps
```

---

## The Fictional Company: TaskFlow

All course exercises are set in **TaskFlow** — a fictional project management SaaS:
- Series B, $2.5M ARR, 10,000 users
- "Asana meets Linear" for remote-first teams
- Student is a Senior PM owning Activation & Onboarding
- Goal: raise activation rate 45% → 60%

---

## Key Conventions

### Course Materials
- Lesson scripts live in `lesson-modules/X.X-name/SCRIPT.md`
- Workflows are in `.agent/workflows/start-X-X.md` (slash commands)
- Rules in `.agent/rules/` are always-on context for the AI instructor
- All model references use **Gemini 3.1** (Flash / Pro / Pro High)
- File format is `.md` (not `.mdc`)

### Website
- Built with Next.js + Nextra
- Deployed on Vercel
- See `DEPLOY.md` for deployment steps

### Find/Replace Rules (Cursor → Antigravity)
| From | To |
|------|----|
| `.cursor/` | `.agent/` |
| `*.mdc` | `*.md` |
| `AI Pane` | `conversation view` |
| `Composer` | `Agent Manager` |
| `Gemini 3 Pro` | `Gemini 3.1 Pro` |
| `Gemini 3 Flash` | `Gemini 3.1 Flash` |

---

## Autonomy Levels (Antigravity-specific)

1. **Agent-driven** — full autopilot
2. **Agent-assisted** *(recommended)* — collaborative
3. **Review-driven** — analyze only, no generation

---

## Development Notes

- Always develop on the designated `claude/` branch
- No stray "Cursor" or `.cursor` references in course-materials
- Backup lives in `course-materials-backup-dec20/` — do not modify
