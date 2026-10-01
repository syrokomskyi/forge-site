---
name: legal
description: "Canonical legal-domain knowledge for forge-site — fetch the JSON endpoint for the current structured document."
metadata:
  schema: "gogol.agent.knowledge/legal@1"
  endpoint: "https://forge.warpgogol.com/api/agent/v1/legal.json"
---

# Legal knowledge

Canonical machine-readable knowledge for the `legal` domain of `forge-site`.

## Resource

- Endpoint: `https://forge.warpgogol.com/api/agent/v1/legal.json`
- Content type: `application/json`
- Schema: `gogol.agent.knowledge/legal@1`

## When to use this skill

Use this skill when an agent needs legal facts about forge-site — for example to answer questions that require canonical structured legal data — instead of scraping HTML pages.

## How to use

1. Fetch the endpoint with an HTTP GET; no authentication is required.
2. Parse the JSON document according to the schema identifier above.
3. Treat the returned document as the canonical source for this domain.
