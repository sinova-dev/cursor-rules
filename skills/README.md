# Agent Skills

This folder contains **Agent Skills** for Cursor—reusable instruction sets that teach the AI how to perform specific tasks, follow workflows, or apply domain knowledge when you ask for help.

## What Are Skills?

**Skills** are markdown-based instructions (each skill lives in a folder with a `SKILL.md` file) that extend the agent’s behavior for particular scenarios. Unlike **Cursor Rules** (which define coding standards and conventions), skills focus on *how to do a task*: step-by-step workflows, when to apply them, and what output or format to use.

| | **Cursor Rules** | **Agent Skills** |
|---|------------------|------------------|
| **Purpose** | Coding standards, conventions, style | Task-specific workflows and domain knowledge |
| **Location** | `.cursorrules` or `.cursor/rules/*.mdc` | `SKILL.md` inside a skill folder |
| **Use case** | “How we write code here” | “How to do X when the user asks” |

Examples of what skills can do:

- Review code using team standards  
- Generate commit messages in a preferred format  
- Apply framework-specific best practices (e.g. React, Next.js, NestJS)  
- Guide refactoring or performance optimization  

The agent uses each skill’s **name** and **description** to decide when to apply it, so descriptions should be clear and include trigger phrases.

## Skills in This Repository

These skills are available under `skills/`:

| Skill | Description |
|-------|-------------|
| **vercel-react-best-practices** | React and Next.js performance optimization (waterfalls, bundle size, server/client patterns, re-renders). Use when writing or refactoring React/Next.js code. |
| **nestjs-expert** | NestJS conventions and patterns. Use for backend or NestJS-related tasks. |
| **prisma-expert** | Prisma ORM usage and best practices. Use when working with databases or Prisma. |
| **tailwindcss-development** | Tailwind CSS usage and patterns. Use for styling and UI work. |
| **clean-code** | Clean code principles and refactoring. Use when improving code quality or structure. |

Each skill directory contains:

- `SKILL.md` – main instructions and metadata (required)
- Optional: `rules/`, `reference.md`, `examples.md`, or scripts

## How to Use These Skills in Your Project

### Option 1: Project skills (recommended for teams)

Make these skills available to Cursor for a specific project by copying or linking the skill folders into that project’s Cursor skills directory:

```text
your-project/
├── .cursor/
│   └── skills/           ← Cursor looks here for project skills
│       ├── vercel-react-best-practices/
│       │   └── SKILL.md
│       ├── nestjs-expert/
│       │   └── SKILL.md
│       └── ...
```

**Copy from this repo:**

```bash
# From your project root
mkdir -p .cursor/skills
cp -r /path/to/cursor-rules/skills/vercel-react-best-practices .cursor/skills/
cp -r /path/to/cursor-rules/skills/nestjs-expert .cursor/skills/
# ... add other skills you need
```

Then when you (or the agent) work in that project, Cursor can use these skills automatically when the task matches their descriptions.

### Option 2: Personal skills (all projects)

To use the same skills across all your projects, install them into your user-level Cursor skills directory:

- **Windows:** `%USERPROFILE%\.cursor\skills\`
- **macOS/Linux:** `~/.cursor/skills/`

Copy the skill folders from this repo’s `skills/` into that directory. Do **not** use `~/.cursor/skills-cursor/`—that is reserved for Cursor’s built-in skills.

### Option 3: Reference from this repo

If you keep this repository on disk, you can add skills to a project by symlinking (or copying) from `cursor-rules/skills/` into the project’s `.cursor/skills/` so you don’t duplicate files.

## When Skills Are Used

Cursor’s agent reads the **description** in each skill’s `SKILL.md` frontmatter. When your request matches that description (e.g. “optimize this Next.js page” or “review this React component”), the agent can load and follow that skill.

You can also explicitly ask for a skill by name or by task, e.g. “use the Vercel React best practices to refactor this component.”

## Adding or Creating a New Skill

1. **Add an existing skill from elsewhere**  
   Copy its folder (with `SKILL.md` and any supporting files) into `skills/<skill-name>/` in this repo, or into your project’s `.cursor/skills/`.

2. **Create a new skill**  
   - Add a new folder under `skills/<skill-name>/`.  
   - Create `SKILL.md` with YAML frontmatter (`name`, `description`) and the main instructions.  
   - Keep the body focused and under ~500 lines; put long reference material in separate files (e.g. `reference.md`, `examples.md`).  
   - Use the **create-skill** Agent Skill in Cursor for step-by-step guidance on structure, descriptions, and best practices.

Skill names should be lowercase, use hyphens, and be at most 64 characters (e.g. `vercel-react-best-practices`).

## Summary

- **Skills** = task- and workflow-focused instructions in `SKILL.md`; **Rules** = project coding standards in `.cursorrules` or `.cursor/rules/`.
- Skills in this repo live under `skills/`; use them by copying (or linking) into your project’s `.cursor/skills/` or your user `~/.cursor/skills/`.
- The agent picks skills by matching your request to each skill’s description; you can also refer to a skill by name or task when asking for help.
