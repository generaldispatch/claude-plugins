---
name: run-an-agency
description: Run many home-service businesses on General Dispatch as a marketing agency - create client businesses, assign your people, see every business's usage and status, white-label under your brand. Use when an agency wants to onboard clients, check on its businesses, or set things up across several of them.
---

# Run an agency

With the agency signed in (or an organization key), `whoami` lists every business you reach. `list_businesses` shows them with status; `create_business` starts a client's business (look it up first: `lookup_website` for a domain, `find_business` for a name and place); `assign_member` gives your people access; `get_agency_usage` is the meter. Business tools act in one business per call: pass `business: <slug>` when it isn't the one you stand in, and make one call per business for a change across several. Then set each one up with the `set-up-a-business` skill.
