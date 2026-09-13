---
kind: navigation
lang: en
groups:
  - id: main
    label: "Main"
    items:
      - id: home
        label: "Home"
        semanticTarget:
          kind: page
          pageId: home
  - id: legal
    label: "Legal"
    items:
      - id: impressum
        label: "Impressum"
        semanticTarget:
          kind: internal
          pageId: impressum
        routeSlug: impressum
      - id: datenschutz
        label: "Datenschutz"
        semanticTarget:
          kind: internal
          pageId: datenschutz
        routeSlug: datenschutz
      - id: license
        label: "License (Apache 2.0)"
        semanticTarget:
          kind: external
          href: "https://github.com/syrokomskyi/forge/blob/main/LICENSE"
---
