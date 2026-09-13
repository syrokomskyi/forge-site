---
app: forge-site
version: 1.0.0
identity:
  systemStar: Sirius
  biome: handwerk-material-warm
  domain: forge.warpgogol.com
i18n:
  default: en
  supported:
    en:
      name: English
      hreflang: en-US
legalJurisdiction: DE
verification:
  google:
    method: meta-tag
    token: "pending-verification"
pages:
  - pageId: home
    semanticType: home
    output:
      sitemap:
        lastmod: "2026-09-13"
    routes:
      en: ""
    cosmicStar: Sirius
    planets:
      - cosmicPlanet: Europa
        pin: 1.5.0
      - cosmicPlanet: Ganymede
        pin: 1.5.0
      - cosmicPlanet: Janus
        pin: 1.2.0
      - cosmicPlanet: Dione
        pin: 1.5.0
      - cosmicPlanet: Hyperion
        pin: 1.5.0
  - pageId: impressum
    semanticType: legal
    output:
      sitemap:
        lastmod: "2026-09-13"
    routes:
      en: impressum
    locales:
      - en
    cosmicStar: Sirius
  - pageId: datenschutz
    semanticType: legal
    output:
      sitemap:
        lastmod: "2026-09-13"
    routes:
      en: datenschutz
    locales:
      - en
    cosmicStar: Sirius
---
