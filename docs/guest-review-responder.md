# guest-review-responder
> Reply to guest reviews like a pro — de-escalate the bad ones, reinforce the good ones, stay truthful.

## Description
A reputation-management assistant for hospitality operators (hotels, short-term rentals, restaurants): it classifies each review, picks the right response framework, and drafts a truthful, on-brand, de-escalating reply — across Airbnb, Google, Booking.com, TripAdvisor, and Yelp. It also flags legal-sensitive complaints, shows you how to legitimately report policy-violating reviews, and turns recurring complaints into an operational fix list. Honest by design: it never writes fake reviews, never review-gates, and never admits liability on your behalf.

## Compatibility
Advisory skill — no tooling or runtime required. Works from the review text and context you provide. **Does not post, fabricate, or solicit reviews.** Platform rules and review laws change — verify current policies on the platform and at ftc.gov before acting.

## Keywords
guest review response, respond to reviews, Airbnb review reply, Google review response, hotel review management, negative review de-escalation, restaurant review reply, reputation management, review reply templates, Booking.com, TripAdvisor, Yelp, 1-star review, service recovery, hospitality, FTC review rule

## Sample input
> "Draft a reply to this Google review: '2 stars — room was clean but check-in took almost an hour and nobody apologised.' We're a mid-market boutique hotel; the front desk was short-staffed that night."

## Sample output
*(Illustrative shape — a truthful, de-escalating draft + an operator note.)*
- **Draft reply:** acknowledges the specific issue (the long check-in) → genuine empathy (not "sorry you feel that way") → honest ownership of the wait without over-promising → a concrete next step → a direct contact to take it offline → a brief, warm sign-off, matched to a mid-market register.
- **Operator note:** "This reads as an isolated staffing issue, not a legal-sensitive one — safe to post publicly. If check-in delays show up across several reviews, that's an operational signal (see the complaint-pattern workflow)."

## Known limitations
- **Advisory only** — it drafts; you post. It will not post, fabricate, or solicit reviews on your behalf.
- **Truthful responses only** — it refuses fake reviews, review-gating (soliciting only happy guests — an FTC/platform violation), impersonation, and bad-faith removal of honest negative reviews.
- **Legal-sensitive complaints** (injury, illness, discrimination, legal threats) → it drafts a brief empathetic public reply with **no admission of liability** and tells you to take it offline + escalate to management/legal. Not legal advice.
- **Platform rules + review laws change** — it frames specifics as "verify current" and points to the platform / ftc.gov rather than baking figures that go stale.
