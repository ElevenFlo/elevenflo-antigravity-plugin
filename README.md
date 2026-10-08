# ElevenFlo plugin for Antigravity

Source-backed chapter 11 research inside Google Antigravity (IDE, Antigravity
2.0 desktop, and the `agy` CLI).

Search U.S. chapter 11 cases, dockets, and court filings. Read exact filing
text, review document summaries, trace related motions, objections, hearing
materials, and orders, follow docket updates, and query published
restructuring datasets. Responses link to the underlying court records for
verification.

## Install

```
agy plugin install https://github.com/ElevenFlo/elevenflo-antigravity-plugin
```

In the Antigravity IDE or desktop app, open **Customizations**, then the
**MCP** tab, and complete the sign-in prompt for the `elevenflo` server. The
browser opens an ElevenFlo consent screen; sign in or create an account.
Authentication is OAuth 2.1 authorization code with PKCE. The server supports
Client ID Metadata Documents and dynamic client registration, so there is no
API key or client secret to manage.

## What it adds

- One remote MCP server, `elevenflo` (`https://elevenflo.com/mcp`, Streamable
  HTTP), exposing read-only research tools. See the
  [tool catalog](https://elevenflo.com/docs/mcp/tool-catalog).
- One skill, `chapter-11-case-research`, telling the agent how to resolve a
  case, find the controlling filing, read and cite exact text, query typed
  datasets, and follow docket updates.

Start with `find_cases` to resolve a case, and call
`describe_structured_dataset` before querying a dataset.

## Account and limits

An ElevenFlo account is required. Free accounts get a monthly research credit
allowance; Pro and Team accounts get a substantially larger one. See
[elevenflo.com](https://elevenflo.com) for current plans.

## Links

- Docs: https://elevenflo.com/docs/mcp/overview
- Tool catalog: https://elevenflo.com/docs/mcp/tool-catalog
- Support: support@elevenflo.com or https://elevenflo.com/contact-us
- Privacy: https://elevenflo.com/privacy
- Terms: https://elevenflo.com/terms-of-use

## License

This plugin manifest, skill, and documentation are licensed under Apache-2.0
(see `LICENSE`). The ElevenFlo MCP service the plugin connects to is not
covered by that license; use of the service is governed by the ElevenFlo
[Terms of Use](https://elevenflo.com/terms-of-use) and
[Privacy Policy](https://elevenflo.com/privacy).

© ElevenFlo, Inc.
