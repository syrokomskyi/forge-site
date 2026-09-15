# auth.md

This site supports AI agent discovery via standard protocols.

## Discovery Endpoints

- **Agent Manifest**: `/.well-known/agent.json`
- **OpenAPI Spec**: `/.well-known/agent.openapi.json`
- **API Catalog**: `/.well-known/api-catalog` (RFC 9264 linkset+json)
- **MCP Server Card**: `/.well-known/mcp/server-card.json`
- **Agent Skills**: `/.well-known/agent-skills/index.json`
- **OAuth Protected Resource**: `/.well-known/oauth-protected-resource`
- **OAuth Authorization Server**: `/.well-known/oauth-authorization-server`
- **LLMs.txt**: `/llms.txt`

## Content Negotiation

This site supports `Accept: text/markdown` content negotiation (RFC-0785).
Send `Accept: text/markdown` to any HTML page to receive its markdown twin.

## Robots.txt

See `/robots.txt` for crawl directives and Content-Signal preferences.

## DNS-AID

DNS-AID SVCB record at `_index._agents.forge.warpgogol.com` points to this site's
agent.json manifest.

## Registration

This site supports anonymous agent access — no registration or credentials
are required to read public discovery endpoints.

- **Register URI**: `https://forge.warpgogol.com/auth`
- **Identity Type**: anonymous
- **Credential Type**: none
- **Claim URI**: `/.well-known/agent.json`

Agents can discover this site's capabilities by fetching the endpoints listed
above. For authenticated operations, use the OAuth 2.0 authorization code flow
with PKCE (S256) via the Authorization Server metadata at
`/.well-known/oauth-authorization-server`.

## Contact

For agent-related inquiries, refer to the contact information in the
Agent Manifest at `/.well-known/agent.json`.
