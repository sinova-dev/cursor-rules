# Code review skills pack

Dedicated folder for agent code-review workflows (general + Nest + Next + React/TS).

| Skill | Focus | Source |
|-------|--------|--------|
| `code-reviewer` | General PR/diff review (correctness, security, reliability, tests) | [d0ublecl1ck/code-reviewer](https://github.com/d0ublecl1ck/code-reviewer) |
| `code-review-excellence` | Review process, severity labels, TS/JS patterns | [wshobson/agents](https://github.com/wshobson/agents) |
| `nextjs-code-review` | Next App Router: RSC boundaries, Server Actions, caching, middleware | [giuseppe-trisciuoglio/developer-kit](https://github.com/giuseppe-trisciuoglio/developer-kit) |
| `nestjs-code-review` | Nest controllers, DI, DTOs, guards, severity findings | same |
| `nestjs-code-audit` | Full Nest repo audit (read-only) | [amirtaherkhani/nestjs-agent-skills](https://github.com/amirtaherkhani/nestjs-agent-skills) |
| `nestjs-architecture-principles` | Nest architecture (audit dependency) | same |
| `nestjs-oop-design-patterns` | OOP / SOLID (audit dependency) | same |
| `nestjs-features-performance` | Features / perf / security (audit dependency) | same |
| `react-code-review` | React/TS review (React 19, hooks, a11y) | developer-kit |

**Note:** `typescript-react-reviewer` is listed on skills.sh under bastani-inc/atomic but was **not present** in that GitHub repo at sync time. `react-code-review` is included instead as the React/TS reviewer.

To use in a project, copy/symlink each skill into `.cursor/skills/<name>/`.
