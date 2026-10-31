# loopdesk-demo-tickets

Ticket destination for the [LoopDesk](https://github.com/VenusTokyo/loopdesk) demo.

Issues here are opened by the LoopDesk widget when its agent cannot find a
known fix for a user's problem. Each one carries the agent's diagnosis, the
user's own words, a metadata table, console errors, failed network requests
and a link to the screenshot.

When an issue here is **closed**, a webhook fires back into LoopDesk, the
agent drafts a user-facing solution, a human approves it, and the solution is
published to the knowledge base and committed to the main repository.

## Labels

| Label | Meaning |
|---|---|
| `sub:billing` / `sub:projects` / `sub:analytics` | which sub-product the report came from |
| `from:loopdesk` | opened by the widget, not by hand |
| `needs-triage` | not yet looked at |

Routing is configured in `owners.yml` in the main repository.

> This repository exists to hold demo tickets. The product code lives in
> [VenusTokyo/loopdesk](https://github.com/VenusTokyo/loopdesk).