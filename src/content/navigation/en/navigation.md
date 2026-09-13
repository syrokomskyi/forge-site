---
kind: navigation
lang: en
targets:
  - id: home
    label: "Home"
    semanticTarget:
      kind: internal
      pageId: home
    group: navigation
  - id: github
    label: "GitHub"
    semanticTarget:
      kind: external
      href: "https://github.com/warpgogol/werkstatt"
    group: navigation
  - id: npm
    label: "NPM"
    semanticTarget:
      kind: external
      href: "https://www.npmjs.com/package/@warpgogol/forge"
    group: navigation
  - id: impressum
    label: "Impressum"
    semanticTarget:
      kind: internal
      pageId: impressum
    routeSlug: impressum
    group: legal
  - id: datenschutz
    label: "Datenschutz"
    semanticTarget:
      kind: internal
      pageId: datenschutz
    routeSlug: datenschutz
    group: legal
  - id: license
    label: "License (Apache 2.0)"
    semanticTarget:
      kind: external
      href: "https://github.com/syrokomskyi/forge/blob/main/LICENSE"
    group: legal
  - id: email
    label: "hi@warpgogol.com"
    semanticTarget:
      kind: external
      href: "mailto:hi@warpgogol.com"
    group: contact
---
