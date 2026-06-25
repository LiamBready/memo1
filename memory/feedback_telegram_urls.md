---
name: feedback-telegram-urls
description: Telegram eats underscores in URLs — always wrap URLs in backticks
metadata: 
  node_type: memory
  type: feedback
  originSessionId: ba91100d-7445-4516-b3ef-cead0c7e70c3
---

Telegram's markdown parser strips underscores from URLs (interprets `_` as italic). Always wrap URLs containing underscores in backticks so they render correctly.

**Why:** Ondrej noticed the underscore in `user_ondrej.md` was being dropped in rendered links.

**How to apply:** Any time I share a URL with an underscore in a Telegram channel, use backtick formatting: `` `https://...` ``
