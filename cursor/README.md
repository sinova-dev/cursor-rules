## Cursor: A New Hope – Star Wars Guide for New Developers 🌌

Welcome, young Padawan. This is your holocron 📜 for learning **Cursor**, an AI-powered code editor that helps you build software faster, with fewer bugs, and far less time spent fighting the dark side of boilerplate.

Think of Cursor as your **R2‑D2 co‑pilot** in the cockpit of your IDE: it reads the codebase, understands context, and helps you navigate, refactor, and generate code at hyperspeed.

Under the hood, Cursor is a **fork of VS Code**, so most of your muscle memory, keybindings, and extensions carry over. You gain an AI starfighter without having to relearn how to fly.

---

### The Main Purpose of Cursor (What the Jedi Council Intended)

- **Primary Mission**:  
  Cursor combines a modern editor (similar to VS Code) with deeply integrated AI so you can read and understand unfamiliar codebases faster, generate and refactor code safely, run multi-file edits while staying within your project’s rules, and chat with your codebase as if it were a knowledgeable master.

- **Key Capabilities (Your Jedi Powers)**:
  - **Chat with Your Codebase** – ask questions about files, flows, and architecture, and get answers in plain language.
  - **Generate & Rewrite Code** – create new functions, tests, or components and clean up existing code with targeted prompts.
  - **Smart Autocomplete** – let Cursor finish small blocks or whole functions based on what you’ve just written.
  - **Repo‑Aware Refactors** – make changes that respect existing patterns, project rules, and architecture across multiple files.
  - **Diff‑First Workflow** – review every AI suggestion as a diff before applying it, so you stay fully in control of the codebase.

---

### Advantages – The Light Side of Cursor ⭐

- **Speed of a Hyperspace Jump** – rapid prototyping, code generation, and refactoring with most boilerplate handled for you.
- **Deep Code Understanding** – ask natural-language questions about services, flows, and errors, and get quick summaries.
- **Consistency with the Jedi Code** – `.cursorrules` and project prompts help enforce your architecture and best practices.
- **Diff‑Driven Changes** – every AI suggestion appears as a diff so you can keep quality and style under control.
- **Great for Onboarding** – new devs can explore the codebase by asking questions instead of hunting through files.

---

### Cursor Modes – Your Lightsaber Forms

Cursor has several primary “forms” of interaction with AI. Choosing the right one is like choosing the right stance in a duel.

- **Ask Mode – The Jedi Archivist (Read‑Only Guidance)**

  - Open the AI sidebar with `Cmd+L` (macOS) or `Ctrl+L` (Windows/Linux).
  - Select **Ask** and treat it like a project‑aware Stack Overflow.
  - Great for:
    - Explaining what a file, function, or entire module does.
    - Proposing alternative implementations or architectures.
    - Spotting potential performance or security problems.
  - It **never changes code**—purely explanations, ideas, and planning.

- **Agent Mode – The Code Wizard (Project‑Wide Changes)**

  - This is Cursor’s “do it for me” mode. You describe the feature or refactor; it edits and creates files across the repo.
  - Examples:
    - “Build a login form with validation using our existing auth utilities.”
    - “Create a REST API for managing user profiles following our error‑handling conventions.”
    - “Refactor this component to TypeScript and fix type errors.”
  - Agent can even run terminal commands (installing packages, running tests, creating branches), which is why version control discipline is critical.

- **Edit Mode – The Precision Strike**

  - Select a piece of code in the editor and choose **Edit**.
  - Ask for targeted changes: “Optimize this loop,” “Rewrite to use early returns,” or “Fix this bug and explain what was wrong.”
  - Ideal for small refactors, focused bug fixes, or tightening up a single function/component.

- **Auto‑Run (Formerly YOLO) – The Dangerous Artifact**
  - Auto‑run lets Cursor execute certain terminal commands **without pausing for confirmation**.
  - This is powerful but risky—like giving an astromech droid full control of the hyperdrive.
  - Recommended usage:
    - Limit to safe commands such as running tests or linters.
    - Keep it **off** for anything that installs packages, modifies databases, or deploys code.

**Rule of Thumb:**

- “I want to understand something” → **Ask mode**
- “I want to build or change something substantial” → **Agent mode**
- “I want a tiny, precise edit” → **Edit mode** (or scoped Agent request)

[Cursor AI for Beginners: A Complete Guide](https://youtu.be/YG459bD8qmw?si=skjHezytt4crDIIH).
[Cursor AI tutorial for beginners](https://youtu.be/gqUQbjsYZLQ?si=Mm4ea1A9unvyOt2N).
[Cursor Agent: 10 Pro Tips!](https://youtu.be/WVeYLlKOWc0?si=rBHcJFpPDD3F2JgR).

---

### Essential Commands & Settings – Where the Controls Live

- **Open AI Chat / Ask Mode**

  - macOS: `Cmd + L`
  - Windows/Linux: `Ctrl + L`
  - This toggles the AI sidebar where you choose **Ask / Agent** and manage context.

- **Command Palette (All Cursor Commands)**

  - macOS: `Cmd + Shift + P`
  - Windows/Linux: `Ctrl + Shift + P`
  - Search for commands like “Cursor: Open Agent”, “Cursor: Toggle Auto‑Run”, or “Cursor: Open Settings” just like in VS Code.

- **Project Rules Settings**

  - Global/editor rules live in **Settings → Cursor → Rules** (wording may vary slightly by version).
  - For project‑specific rules, prefer `.cursorrules` or `.cursor/rules/` in your repo (see the “Cursor Rules – Your Jedi Code” section below).

- **MCP (Model Context Protocol) Settings**
  - Editor‑level MCP configuration is under **Settings → Cursor → MCP / Tools**.
  - Project MCP servers are defined in `.cursor/mcp.json` in your repo; Cursor picks these up automatically when the project is open.

Treat these menus like the control panels in your starfighter: once you know where they are, you can quickly tune rules, tools, and AI behavior for each mission.

[Cursor AI: Full Guide (rules, MCP)](https://youtu.be/eXp8TC0Sm6o?si=j5wj1YD6SqQ6TZuq).

---

### Getting Started – Your Padawan Training Path

Follow this path to become productive with Cursor quickly:

1. **Install Cursor**

   - Go to the official site:
     - [Cursor – AI Code Editor](https://www.cursor.com)

2. **Sign In & Connect Repositories**

   - Open Cursor, sign in, and clone or open your project repo.
   - Ensure your `.cursorrules` (and similar prompt files) are present so Cursor understands your project’s “Jedi Code.”

3. **Learn the Core UI (The Cockpit of Your X‑Wing)**

   - Explore:
     - The **editor** pane (code editing, inline prompts).
     - The **AI chat** panel (project-aware conversations).
     - The **diff / changes** view (review AI edits before applying).
     - The **terminal & tasks** integration (run tests, linters, and builds).

4. **Practice Everyday Workflows**

   - Ask Cursor to:
     - Explain a complex file or class.
     - Generate unit tests for a small, pure function.
     - Refactor a function for clarity and error handling.
     - Create a new feature skeleton following your established patterns.

5. **Adopt a “Trust, but Verify” Mindset**
   - Review diffs carefully.
   - Run tests and linters after AI-driven refactors.
   - Keep git commits small and meaningful, even when AI generated the code.

[I spent 400+ hours in Cursor, here’s what I learned](https://youtu.be/gYLNxUxVomY?si=EcQjRv__YCq_097o).
[Cursor AI Tutorial for Beginners (How I Code 159% Faster)](https://youtu.be/yk9lXobJ95E?si=Cn4YCUNlFJJD7KYX).

---

### Cursor Rules – Your Jedi Code for the AI 🧱

To keep your AI co‑pilot on the Light Side, you need a written **Jedi Code** for your project: this is what **Cursor Rules** are.

- **What Cursor Rules Are**  
  Cursor rules are markdown/ prompt files that describe your **coding standards, architecture decisions, and best practices**. Cursor reads them and uses them as guidance for every suggestion it makes, so AI output matches your team’s style instead of random examples from the galaxy.

- **Where to Put Them**
  - Simple setup: create a single `.cursorrules` file in your project root with your main guidelines.
  - Organized setup (recommended):

```plaintext
your-project/
├── .cursor/
│   └── rules/
│       ├── global.mdc      # Global development rules
│       ├── backend.mdc     # Backend-specific rules
│       ├── frontend.mdc    # Frontend-specific rules
│       └── ui.mdc          # UI/Styling rules
```

- **Reusing the Rules from This Repo**
  - You can import the shared rules from the `cursor-rules` repository directly into your project rules files, for example:

```markdown
@import https://raw.githubusercontent.com/sinova-dev/cursor-rules/master/.cursorrules
@import https://raw.githubusercontent.com/sinova-dev/cursor-rules/master/backend/nestjs-typescript-cursorrules-prompt-file/nestjs-conventions.mdc
@import https://raw.githubusercontent.com/sinova-dev/cursor-rules/master/frontend/nextjs-react-typescript-cursorrules-prompt-file/next-js-conventions.mdc
```

- This gives new projects a **complete set of enterprise-grade rules** on day one: core principles, backend conventions, frontend conventions, and UI guidelines, as described in the main repo `README.md`.

- **How to Use Them Day‑to‑Day**
  - Keep rules in sync with how your team actually writes and reviews code.
  - When you ask Cursor for help, assume it has read these rules—phrase prompts like _“follow our error‑handling rules”_ or _“respect our NestJS conventions”_.
  - Update rules when your architecture or standards evolve, so the AI keeps learning with your team.

For full details and copy‑pasteable imports, see the main guide in `README.md` of this repository.

[Cursor Just Got an Upgrade! Here’s What You Need to Know About Cursor Rules](https://youtu.be/1AxTVGxbkPs?si=sUBpMPTZX5cI9eNL).
[Cursor Rules guide for lazy devs. Setup rules in minutes with this quick tutorial!](https://youtu.be/FpJ48a5S5lU?si=oWQI92nv0OXNKoNL).

---

### Context, `.cursorignore`, and the Art of Focus

Cursor is only as strong as the **context** you give it. Think of context as the holocron shards you hand to the AI—too many random shards, and the vision becomes blurry.

- **Adding Context Explicitly**

  - In the chat sidebar, use:
    - **`@`** to add specific files, folders, or docs (for example `@package.json`, `@components/`, `@docs`).
    - **`#`** to focus on a particular file you’re discussing.
    - **`/` Add Open Files to Context** so the AI uses exactly what you are currently viewing.
  - Good context:
    - Relevant files, error logs, and specific functions you’re working on.
  - Bad context:
    - The entire repo for a tiny question, unrelated files, or long, messy past chats.

- **The `.cursorignore` Shield Generator**
  - Use a `.cursorignore` file in the project root to hide noisy paths (build artifacts, dependencies, logs) from the AI.
  - Example:

```plaintext
node_modules/
dist/
build/
.env
*.log
```

- This keeps the AI focused on your real code instead of getting lost in generated or third‑party files, as recommended in [Coding with Cursor: a Beginner’s Guide](https://www.siddharthbharath.com/coding-with-cursor-beginners-guide/).

- **Conversation Hygiene**
  - Start a **new chat** when switching to a new feature or bug.
  - Long, meandering threads cause the model to forget constraints and mix requirements—like trying to rewatch the whole saga at 10x speed.

---

### Tactical Tips – Fighting Bugs Like a Jedi

- **Ask for Rationale, Not Just Code**

  - Example: _“Refactor this function to follow early-return error handling and explain each change.”_

- **Constrain the Scope**

  - Specify files, modules, or functions to operate on.
  - Avoid “rewrite the whole repo” style prompts—this is how Death Stars are accidentally created.

- **Iterate in Small Steps**

  - Use short, focused prompts and apply changes incrementally.
  - Combine with your normal review process and CI pipeline.

- **Keep the Project Rules Up to Date**
  - Maintain `.cursorrules` and architecture docs so Cursor has accurate guidance.
  - Treat those prompts like canonical Jedi texts.

---

### MCP and Advanced Workflows – Calling the Droid Army

With **Model Context Protocol (MCP)**, Cursor can connect to external tools—documentation, browsers, design systems, and bug trackers—turning your AI into a full strike team, not just a lone Jedi.

- **Project‑Local MCP Setup**

  - Define project tools in `.cursor/mcp.json` so they only apply to that repo.
  - Global/editor‑wide tools can be managed from **Settings → Cursor → MCP / Tools**.

- **Useful MCP Servers from This Repo (Short List)**
  - **Context7** – fetch up‑to‑date docs and examples for libraries and frameworks without leaving Cursor.
    - More info: see `mcp/README.md` → **Context7**.
    - Video: [Context7 MCP quick intro](https://www.youtube.com/watch?v=qZfENAPMnyo).
  - **Sequential Thinking** – step‑by‑step reasoning for hard bugs, algorithms, and architecture decisions.
    - More info: `mcp/README.md` → **Sequential Thinking**.
    - Video: [Sequential Thinking MCP walkthrough](https://www.youtube.com/watch?v=RCFe1L9qm3E).
  - **Browser Tools** – drive a real browser for audits, screenshots, and end‑to‑end debugging.
    - More info & setup: `mcp/README.md` → **Browser Tools**.
    - Video: [Browser Tools MCP demo](https://www.loom.com/share/88f493eb9c114d3b901ea97e9251e5e6?sid=241311b6-b2a7-4b2d-9b6c-70c0f64f8062).
  - **Figma MCPs (Framelink & Dev Mode)** – pull real designs and tokens from Figma, then turn frames into code.
    - More info: `mcp/README.md` → **Framelink Figma MCP** and **Figma Dev Mode MCP**.
    - Videos: [Framelink / Figma MCP overview](https://www.youtube.com/watch?v=6G9yb-LrEqg), [Figma Dev Mode MCP guide](https://www.youtube.com/watch?v=yO3Wr7DEWF0).
  - **Jam MCP** – debug with user recordings, console logs, and network traces from Jam.
    - More info: `mcp/README.md` → **Jam MCP**.
    - Video: [Jam MCP debugging guide](https://jam.dev/docs/debug-a-jam/mcp).

For full setup instructions, environment variables, and more servers, open `mcp/README.md` in this repo and follow the Quick Start section.

[Cursor UPDATE: Code Editor just got EVEN BETTER! (MCP Servers, Codebase Understanding, Fusion Model)](https://youtu.be/2vJobjx1p6w?si=Ypw_7QULnnRvW3yz).
[Those MCP totally 10x my Cursor workflow…)](https://youtu.be/oAoigBWLZgE?si=hrgOersN9QTaYRni).

---

### A Simple Real‑World Flight Plan

Here’s a quick pattern you can use when building a feature with Cursor:

1. **Define the Mission (Ask Mode)**

   - Describe what you want (feature, bug fix, refactor) and ask Cursor to help you break it into tasks and outline the architecture.

2. **Lay the Foundations (Agent Mode)**

   - Have Agent scaffold the project structure, basic routes, and minimal UI or API endpoints.
   - Save design docs and decisions into a `docs/` folder for future AI context.

3. **Iterate Feature by Feature (Agent + Edit)**

   - For each small piece (a single endpoint or component), add only the relevant files to context and ask Agent to implement it.
   - Use Edit mode for surgical tweaks and bug fixes.

4. **Harden and Polish**

   - Ask Cursor to improve error handling, logging, and tests.
   - Use MCP (if configured) to run tests, inspect DBs, and check performance metrics.

5. **Review Like a Jedi Knight, Not a Droid**
   - Manually review diffs, run your full test suite, and do normal code review before merging.

---

### Recommended Resources & Videos Holo‑Records 📡

- **Official & General Resources**

  - **Official site**: [Cursor – AI Code Editor](https://www.cursor.com)
  - **Product overview / docs** (usually linked from the site’s navigation):
    - Official docs: [Cursor Documentation](https://docs.cursor.com)
    - Look for sections like _Docs_, _FAQ_, or _Changelog_ on `cursor.com` for the latest features and setup guides.
  - **Community learning hub**: [Cursor Directory – Learn](https://cursor.directory/learn) – curated videos and guides about Cursor, rules, MCP, and workflows.

- **Video Introductions & Deep Dives**

  - [Cursor AI for Beginners: A Complete Guide](https://youtu.be/YG459bD8qmw?si=skjHezytt4crDIIH)
  - [Cursor AI tutorial for beginners](https://youtu.be/gqUQbjsYZLQ?si=Mm4ea1A9unvyOt2N)
  - [Cursor Agent: 10 Pro Tips!](https://youtu.be/WVeYLlKOWc0?si=rBHcJFpPDD3F2JgR)
  - [I spent 400+ hours in Cursor, here’s what I learned](https://youtu.be/gYLNxUxVomY?si=EcQjRv__YCq_097o)
  - [Cursor AI Tutorial for Beginners (How I Code 159% Faster)](https://youtu.be/yk9lXobJ95E?si=Cn4YCUNlFJJD7KYX)
  - [Cursor Just Got an Upgrade! Here’s What You Need to Know About Cursor Rules](https://youtu.be/1AxTVGxbkPs?si=sUBpMPTZX5cI9eNL)
  - [Cursor Rules guide for lazy devs. Setup rules in minutes with this quick tutorial!](https://youtu.be/FpJ48a5S5lU?si=oWQI92nv0OXNKoNL)
  - [Cursor UPDATE: Code Editor just got EVEN BETTER! (MCP Servers, Codebase Understanding, Fusion Model)](https://youtu.be/2vJobjx1p6w?si=Ypw_7QULnnRvW3yz)
  - [Those MCP totally 10x my Cursor workflow…](https://youtu.be/oAoigBWLZgE?si=hrgOersN9QTaYRni)

---

### Final Words from the Council

Cursor is a powerful ally in your development journey, but remember that the **Force** is your engineering judgment, not the tool. Let Cursor amplify the Light Side practices you already follow—testing, clean architecture, thoughtful reviews—instead of tempting you to bypass them. When the path ahead is cloudy, pause like a Jedi Master: read the code, run the tests, talk with your squad, and then decide.

May your CI pipelines hum like well‑tuned hyperdrives, your logs be as clear as holocron records, and your refactors feel as precise as a lightsaber strike ⚔️ cutting through legacy code. May your builds be green, your lint clean, and your pull requests welcomed by the Council with unanimous approval.  
**May the Source be with you.** 💫
