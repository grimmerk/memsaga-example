---
name: auth-flow
description: Why the login redirect broke after OAuth
---
The OAuth callback must return to the page the user started from, not to `/`.
The original path is kept in the `state` parameter; never trust a `next` query.
