---
kind: page
pageId: home
cosmicStar: Sirius
title: "Forge — AI can write the code. Forge keeps the project engineered"
description: "Forge is the engineering control layer for AI-assisted development. Contracts, decisions, workflows, and verification that stay with the project."
lang: en
dateModified: "2026-09-13"
datePublished: "2026-09-13"
blocks:
  - id: hero
    type: hero
    props:
      hideSectionNumber: true
      background:
        kind: "color"
      header:
        eyebrow: "Forge"
        heading: "AI can write the code. Forge keeps the project engineered."
        subheading: "Engineering rules stay with the project — regardless of which agent, model, or IDE you use."
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
      background:
        kind: solid
      density: normal
      header:
        eyebrow: "How Forge works"
        heading: "Five planes of engineering control"
        subheading: "Forge keeps engineering decisions in the project, not in the agent's memory."
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

        Every artifact lives in the repo. Every agent session starts from the same rules. No context is lost between sessions, models, or IDEs.
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
          left: "Forge IS"
          right: "Forge IS NOT"
        rows:
          - left: "Engineering control layer for AI-assisted development"
            right: "A code generator or AI coding assistant"
          - left: "Project contracts, decisions, and workflows that stay in the repo"
            right: "A replacement for your IDE or agent"
          - left: "Verification gates that enforce rules automatically"
            right: "A lock-in to a specific model or vendor"
          - left: "Framework-agnostic: works with any AI tool"
            right: "A runtime dependency in your production app"
  - id: quick-start
    type: markdown
    props:
      hideSectionNumber: true
      eyebrow: "Quick start"
      heading: "Start in one command"
      lead: "Scaffold a new Forge project with engineering rules built in."
      body: |
        ```bash
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
