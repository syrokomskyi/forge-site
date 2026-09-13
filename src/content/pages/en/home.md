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
      ctaSecondaryUrl: "https://github.com/warpgogol/werkstatt"
      tagline: "Open source · Apache-2.0"
  - id: what-controls
    type: impact
    props:
      hideSectionNumber: true
      header:
        eyebrow: "What Forge controls"
        heading: "Five planes of engineering control"
        subheading: "Forge keeps engineering decisions in the project, not in the agent's memory"
        level: 2
      body:
        kind: stats
        stats:
          - value: "Contracts"
            label: "Project rules that agents must follow"
          - value: "Decisions"
            label: "RFCs and ADRs that record why"
          - value: "Workflows"
            label: "Skills that encode team process"
          - value: "Verification"
            label: "Checks that enforce the rules"
          - value: "Evolution"
            label: "DNA invariants that govern change"
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
    type: final-cta
    props:
      hideSectionNumber: true
      header:
        eyebrow: "Quick start"
        heading: "Start in one command"
        subheading: "Scaffold a new Forge project with engineering rules built in"
        level: 2
      ctaGroup:
        items:
          - label: "pnpm create @warpgogol/forge"
            ariaLabel: "Copy the Forge start command"
            variant: primary
            target:
              kind: anchor
              anchor: "copy-command"
          - label: "npm package"
            ariaLabel: "View Forge on npm"
            variant: secondary
            target:
              kind: external
              href: "https://www.npmjs.com/package/@warpgogol/forge"
          - label: "GitHub"
            ariaLabel: "View Forge on GitHub"
            variant: secondary
            target:
              kind: external
              href: "https://github.com/warpgogol/werkstatt"
  - id: architecture
    type: markdown
    props:
      hideSectionNumber: true
      heading: "Architecture"
      body: |
        ![Forge architecture diagram](/assets/forge/diagrams/forge-architecture-1440w.webp)

        Forge sits between your AI tools and your codebase. It ensures that every agent session follows the same engineering rules — contracts, decisions, workflows, and verification gates.
  - id: cli-demo
    type: markdown
    props:
      hideSectionNumber: true
      heading: "See it in action"
      body: |
        ```bash
        $ pnpm create @warpgogol/forge my-project
        $ cd my-project
        $ pnpm install
        $ pnpm exec forge doctor
        ✓ Project contracts validated
        ✓ DNA invariants checked
        ✓ Agent workflows ready
        ✓ Verification gates configured
        ```
  - id: footer
    type: markdown
    props:
      hideSectionNumber: true
      heading: ""
      body: |
        **Forge** · Apache-2.0 · [GitHub](https://github.com/warpgogol/werkstatt) · [npm](https://www.npmjs.com/package/@warpgogol/forge) · Made by [Warpgogol](https://warpgogol.com)
---
