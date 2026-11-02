# General Dispatch for Claude Code

Run a home-service business (HVAC, plumbing, electrical, painting, roofing…) from Claude Code: customers and pipeline,
booking on real calendars, texting, follow-ups, quotes, the website and reviews, with Jack answering customers. Agencies
run every client business from one agent.

## Install

```
/plugin marketplace add ianscott313/general-dispatch-plugins
/plugin install general-dispatch@general-dispatch
```

The plugin adds two MCP servers:

- `general-dispatch` — `https://api.generaldispatch.ai/mcp`, signs you in once in the browser (OAuth).
- `general-dispatch-start` — `https://api.generaldispatch.ai/mcp/start`, no sign-in: `start_business` creates a free
  business and returns its key and a claim link for the owner.

And five skills: set up a business, build the website, quotes and estimates, review the business, run an agency. Each
points at the playbook the server itself serves (`skill://…`), so the instructions always match the tools.

Free to set up (up to 1,000 customers; nothing reaches a real customer until the business goes live).
Pricing: https://generaldispatch.ai/pricing · Docs: https://generaldispatch.ai/agents · Support: support@generaldispatch.ai
