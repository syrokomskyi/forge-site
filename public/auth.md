# auth.md

This site supports AI agent discovery via standard protocols.

## Discovery Endpoints

- **Agent Manifest**: `/.well-known/agent.json`
- **OpenAPI Spec**: `/.well-known/agent.openapi.json`
- **API Catalog**: `/.well-known/api-catalog` (RFC 9264 linkset+json)
- **ARD Catalog**: `/.well-known/ard.json` (legacy alias `/.well-known/ai-catalog.json`)
- **Agent Skills**: `/.well-known/agent-skills/index.json` (+ per-domain `SKILL.md`)
- **LLMs.txt**: `/llms.txt`

## Content Negotiation

This site supports `Accept: text/markdown` content negotiation (RFC-0785).
Send `Accept: text/markdown` to any HTML page to receive its markdown twin.

## Robots.txt

See `/robots.txt` for crawl directives and Content-Signal preferences.

## DNS-AID

DNS-AID SVCB record at `_index._agents.forge.warpgogol.com` points to this site's
agent.json manifest.

## Agent Registration

This site supports anonymous agent access — no registration or credentials
are required to read public discovery endpoints or invoke published actions.
There is no registration endpoint by design: the agent surface is anonymous.

```json
{
  "agent_auth": {
    "skill": "https://forge.warpgogol.com/auth.md",
    "identity_types_supported": ["anonymous"],
    "anonymous": {
      "credential_types_supported": ["none"],
      "claim_uri": "https://forge.warpgogol.com/.well-known/agent.json"
    }
  }
}
```

- **Identity type**: `anonymous` — agents interact without user identity binding.
- **Credential use**: none are issued or required
  (`credential_types_supported: ["none"]`); every published endpoint is open.
- **Claim URI**: `/.well-known/agent.json` — the agent manifest is the only
  provisioning surface an agent needs to begin.

Agents can discover this site's capabilities by fetching the endpoints listed
above. All discovery endpoints are anonymous — no authentication flow exists.

## Contact

For agent-related inquiries, refer to the contact information in the
Agent Manifest at `/.well-known/agent.json`.
