# Verdict, for Gemini CLI

A [Gemini CLI](https://geminicli.com) extension that wires the hosted
**Verdict** MCP server into your terminal.

Verdict checks anything suspicious — a text, an email, a marketplace
listing, a job offer, an investment pitch, a link — and returns a plain
verdict: **REAL**, **SUSPICIOUS**, or **LIKELY SCAM**, with every check
shown in plain words and a clear "what to do next." Links are followed
safely server-side, look-alike domains are caught, domain age is read
from the registry, sender rules (SPF/DMARC) and known-bad lists are
checked, and every result carries a signed verdict certificate and a
shareable link that never contains the pasted content. Two tools:
`check_message`, `check_url`.

## Install

```bash
gemini extensions install https://github.com/nrupala/verdict-gemini-extension
```

No API key and no setup: the free tier is keyless (3 checks/day). Paid
plans — Pro $6/mo (unlimited, one person), Family $12/mo (5 people, one
family code, summary-only guard page) — live on the product site:
[verdict.aimlds.org](https://verdict.aimlds.org).

## What this repo is

This is a thin wrapper: it contains no server code. The extension
manifest (`gemini-extension.json`) points Gemini CLI at the hosted
Verdict MCP server (`https://verdict.aimlds.org/mcp`, Streamable HTTP,
stateless).

- Product: https://verdict.aimlds.org
- Privacy policy: https://verdict.aimlds.org/privacy
- Terms: https://verdict.aimlds.org/terms
- Support: info@aimlds.org

## License

Apache-2.0. See `LICENSE`.

---
Verdict is a product of 2351485 ALBERTA INC. · Built with Muse by Meta
