---
name: quotes-and-estimates
description: Write estimates, proposals and contracts for a home-service job on General Dispatch from the trade's templates (good/better/best options, measured pricing, the notices the state requires), send the signing link, record estimates given another way, and follow up on the ones still open. Use when someone asks to quote a job, chase estimates, or see which estimates are still out.
---

# Quotes and estimates

- **Writing one:** read the MCP resource `skill://quotes` and follow it (`list_proposal_templates`, `create_quote`, then `send_quote` for the signing link; every price from the owner, the conversation or the price book). Never edit a sent version: `update_quote` makes a new one.
- **An estimate given another way** (on paper, in person): `mark_quote` on the job records it as sent, accepted or declined with the amount.
- **What's still out:** `list_jobs` — a job carries its estimate's state (`quote_status`); open ones went out and aren't decided.
- **Following up:** read `skill://estimate-followup`. Follow-up texts are proposals under the owner's rules; never promise a discount the owner didn't approve.

Sending a quote or invoice to a customer needs the business to be live; drafts are free.
