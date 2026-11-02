---
name: set-up-a-business
description: Set up a home-service business (HVAC, plumbing, electrical, painting, roofing…) on General Dispatch from its name or website - profile, hours, services and prices, the owner's rules, customers imported, calendar connected, Jack ready to answer. Use when someone wants to get their business (or a client's) running on General Dispatch, or asks for a CRM, booking or an AI receptionist for a trade business.
---

# Set up a business on General Dispatch

1. **Connect.** If the `general-dispatch` server asks you to sign in, the owner signs in once in the browser. With no sign-in available (a script, a headless run), use the `general-dispatch-start` server: `start_business` with the business's name and timezone (and its website, which fills in the phone, address, hours, logo and colors) returns an API key for the main server and a **claim link**. Give the owner the claim link; they open it to see the business and go live.
2. **Read the playbook.** Read the MCP resource `skill://onboarding` and follow it: it walks the profile, people, policy, price book, brand, imports and calendar, writing only what the owner confirms.
3. **Check progress** with `get_setup_progress` after each step; it says what is left.
4. **Show it working.** `text_as_customer` sends a test customer's text; watch Jack answer and book it on the calendar. That is the moment to suggest going live (`go_live` returns the price and the link). The free plan holds up to 1,000 contacts; nothing reaches a real customer until the business is live.

Rules the tools enforce, so you don't have to: consent on every number, quiet hours, the owner's ask-first rules, and sends are proposals (`send_message` returns queued, needs_approval or denied, never sent).
