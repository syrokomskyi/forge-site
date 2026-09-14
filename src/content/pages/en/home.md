---
kind: page
pageId: home
cosmicStar: Sirius
title: "Forge — AI can write the code. Forge keeps the project engineered"
description: "Forge is the engineering control layer for AI-assisted development. Contracts, decisions, workflows, and verification that stay with the project."
lang: en
dateModified: "2026-09-14"
datePublished: "2026-09-13"
blocks:
  - id: hero
    type: hero
    props:
      hideSectionNumber: true
      header:
        eyebrow: "Forge"
        heading: "AI can write the code. Forge keeps the project engineered"
        subheading: "Engineering rules stay with the project — regardless of which agent, model, or IDE you use"
        level: 1
      ctaPrimaryLabel: "Get started"
      ctaPrimaryAriaLabel: "Get started with Forge"
      ctaPrimaryUrl: "#quick-start"
      ctaSecondaryLabel: "View on GitHub"
      ctaSecondaryAriaLabel: "View Forge on GitHub"
      ctaSecondaryUrl: "https://github.com/syrokomskyi/forge"
      tagline: "Open source · Apache-2.0"
  - id: how-forge-works
    type: entity-grid
    props:
      hideSectionNumber: true
      header:
        eyebrow: "How Forge works"
        heading: "Five planes of engineering control"
        subheading: "Forge keeps engineering decisions in the project, not in the agent's memory"
        level: 2
      body:
        kind: grid
        columns: 3
        items:
          - number: "01"
            title: "Contracts"
            description: "Project rules that agents must follow — naming, structure, boundaries, and conventions enforced at every session."
          - number: "02"
            title: "Decisions"
            description: "RFCs and ADRs that record why a choice was made, so the next agent understands the context without asking."
          - number: "03"
            title: "Workflows"
            description: "Skills that encode team process — from onboarding to deployment — as executable markdown agents can follow."
          - number: "04"
            title: "Verification"
            description: "Checks that enforce the rules automatically — typography, content, architecture, and DNA invariants validated on every commit."
          - number: "05"
            title: "Evolution"
            description: "DNA invariants that govern how the project itself changes — forward-only migrations, no silent breaking changes."
  - id: what-forge-does
    type: markdown
    props:
      hideSectionNumber: true
      heading: "What Forge does"
      body: |
        Forge gives your project a machine-readable engineering layer that every AI agent can understand:

        - **AGENTS.md** — instructions that tell agents how to work in this repo, which rules to follow, and which files to avoid.
        - **RFCs** — architecture proposals that agents can create, validate, and implement through a structured pipeline.
        - **ADRs** — lightweight decision records for local technical choices that don't need a full RFC.
        - **Skills** — reusable workflows encoded as markdown that agents execute step by step.
        - **Checks** — validators that run on every commit: typography, content discipline, architecture boundaries, DNA invariants.
        - **Missions** — scoped work units that track what changed, why, and how it was verified.

        Every artifact lives in the repo. Every agent session starts from the same rules. Zero context is lost between sessions, models, or IDEs.
  - id: plugins
    type: entity-grid
    props:
      hideSectionNumber: true
      header:
        eyebrow: "Plugins"
        heading: "Extend Forge with stack-specific rules and skills"
        subheading: "Plugins add validators, skills, and commands tailored to your stack — without modifying Forge itself"
        level: 2
      body:
        kind: grid
        columns: 3
        items:
          - number: "01"
            title: "Stack validators"
            description: "Plugins register check commands that enforce stack-specific invariants — tsconfig strictness, import boundaries, barrel exports, phantom dependencies — on every commit."
          - number: "02"
            title: "Skill packs"
            description: "Declare project-local skill packs with a custom prefix. Skills are markdown workflows that agents execute step by step — deploy, review, testing, onboarding."
          - number: "03"
            title: "Extension points"
            description: "Plugins can declare custom Compass contract blocks — source-file markers that compass.validate enforces, so your team's conventions become first-class checks."
  - id: available-plugins
    type: markdown
    props:
      hideSectionNumber: true
      heading: "Available plugins"
      body: |
        | Plugin | Stack | npm |
        | --- | --- | --- |
        | `@warpgogol/werkstatt-typescript` | TypeScript TurboRepo — tsconfig, import boundaries, barrel exports | [npm](https://www.npmjs.com/package/@warpgogol/werkstatt-typescript) |
        | `@warpgogol/werkstatt-phaser-game` | Phaser + Vite + Turborepo — browser games | [npm](https://www.npmjs.com/package/@warpgogol/werkstatt-phaser-game) |
        | `@warpgogol/werkstatt-godot-game` | Godot 4+ with C# — desktop and mobile games | [npm](https://www.npmjs.com/package/@warpgogol/werkstatt-godot-game) |
        | `@warpgogol/werkstatt-knowledge` | Evidence-backed knowledge bases | [npm](https://www.npmjs.com/package/@warpgogol/werkstatt-knowledge) |

        Each plugin registers stack-specific validators, skills, and commands. Install the one that matches your stack — or build your own by declaring a `forge.plugin.yaml` manifest in your package.
  - id: is-not
    type: comparison-cards
    props:
      hideSectionNumber: true
      header:
        eyebrow: "Forge IS / IS NOT"
        heading: "What Forge is — and what it isn't"
        level: 2
      body:
        kind: comparison
        labels:
          left: "Forge IS NOT"
          right: "Forge IS"
        rows:
          - left: "A code generator or AI coding assistant"
            right: "Engineering control layer for AI-assisted development"
          - left: "A replacement for your IDE or agent"
            right: "Project contracts, decisions, and workflows that stay in the repo"
          - left: "A lock-in to a specific model or vendor"
            right: "Verification gates that enforce rules automatically"
          - left: "A runtime dependency in your production app"
            right: "Framework-agnostic: works with any AI tool"
  - id: quick-start
    type: markdown
    props:
      hideSectionNumber: true
      eyebrow: "Quick start"
      heading: "Start in one command"
      lead: "Without a terminal — just tell your AI agent what to build"
      body: |
        Open a new folder in your AI IDE (Windsurf, Cursor, Claude Code, Codex CLI, or any IDE that supports AI agents) and paste this:

        ```
        Install https://npmjs.com/package/@warpgogol/forge in this folder and set up my project. I want to build: [describe your project]
        ```

        Replace `[describe your project]` with your idea — a game, a library, a knowledge base, anything. The agent installs Forge, scaffolds the project, and sets up a live preview. From there on, you just talk: describe what you want, and the agent builds it.

        **Prefer the terminal?**

        ```bash
        pnpm add -g @warpgogol/forge
        pnpm create @warpgogol/forge my-project
        cd my-project
        pnpm install
        pnpm exec forge doctor
        ```

        ✓ Project contracts validated  
        ✓ DNA invariants checked  
        ✓ Agent workflows ready  
        ✓ Verification gates configured  

        [npm package](https://www.npmjs.com/package/@warpgogol/forge) · [GitHub](https://github.com/syrokomskyi/forge)
  - id: faq
    type: markdown
    props:
      hideSectionNumber: true
      heading: "FAQ"
      body: |
        <details>
        <summary><strong>Does Forge depend on a specific AI model or IDE?</strong></summary>

        No. Forge is model-agnostic and IDE-agnostic. It works with Claude, GPT, Copilot, Cursor, Windsurf, or any agent that reads markdown files. The engineering rules live in the repo, not in a tool.

        </details>

        <details>
        <summary><strong>Is Forge a runtime dependency?</strong></summary>

        No. Forge is a development-time tool. It generates contracts, validators, and workflows that live in your repo. Your production app doesn't import or depend on Forge.

        </details>

        <details>
        <summary><strong>What does a new Forge project include?</strong></summary>

        A `forge.yaml` configuration, `AGENTS.md` instructions, `docs/` with RFC and ADR templates, `tools/kernel.config.ts` for command registration, CI workflows, and a `packages/` structure for shared libraries. Everything is scaffolded in one command.

        </details>

        <details>
        <summary><strong>Can I add Forge to an existing project?</strong></summary>

        Yes. Run `pnpm create @warpgogol/forge` in your existing repo and Forge will scaffold the engineering layer without touching your source code. Use `forge create --in-place` to configure an existing monorepo.

        </details>

        <details>
        <summary><strong>How are engineering rules enforced?</strong></summary>

        Forge registers validators that run as CI checks and local commands. Every commit triggers typography, content, architecture boundary, and DNA invariant checks. Rules are defined in the repo and can be extended per project.

        </details>
---
