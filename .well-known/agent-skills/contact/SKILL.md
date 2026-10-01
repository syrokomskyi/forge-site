---
name: contact
description: "Canonical contact-domain knowledge for forge-site - fetch the JSON endpoint for the current structured document."
metadata:
  schema: "gogol.agent.knowledge/contact@1"
  endpoint: "https://forge.warpgogol.com/api/agent/v1/contact.json"
---

# Contact knowledge

Canonical machine-readable knowledge for the `contact` domain of `forge-site`.

## Resource

- Endpoint: `https://forge.warpgogol.com/api/agent/v1/contact.json`
- Content type: `application/json`
- Schema: `gogol.agent.knowledge/contact@1`

## When to use this skill

Use this skill when an agent needs contact facts about forge-site - for example to answer questions that require canonical structured contact data - instead of scraping HTML pages.

## How to use

1. Fetch the endpoint with an HTTP GET; no authentication is required.
2. Parse the JSON document according to the schema identifier above.
3. Treat the returned document as the canonical source for this domain.
