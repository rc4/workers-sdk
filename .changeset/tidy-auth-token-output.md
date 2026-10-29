---
"wrangler": patch
---

Suppress decorative output from `wrangler auth token` in non-interactive contexts

When stdout is not attached to a TTY, Wrangler now suppresses its banner and post-command suggestions so command substitution such as `CLOUDFLARE_API_TOKEN=$(wrangler auth token)` captures only the token.
