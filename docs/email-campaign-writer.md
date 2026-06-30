# email-campaign-writer
> Write email campaigns that convert — and that are permission-based and compliant by construction.

## Description
An email-marketing copywriter and compliance guardrail in one skill. It writes subject lines + preview text, body + a single clear CTA, and full multi-email sequences (welcome, nurture, re-engagement, post-purchase), plus a deliverability checklist — all behind a hard permission gate. It will not help you spam: it asks how your list was built and refuses purchased, scraped, or non-consented lists. Every campaign is structured to meet CAN-SPAM / GDPR / CASL basics (honest subject + sender, a working unsubscribe, a physical postal address, lawful consent). Compliance content is practical guidance, **not legal advice** — verify with the regulator or counsel for your jurisdiction.

## Compatibility
Advisory skill — no tooling or runtime required. Works from your offer, audience, and list-consent details. **Permission-based only — it will not help send to purchased lists or write non-compliant email, and it does not send mail.** Email law (CAN-SPAM/GDPR/CASL) varies by jurisdiction and changes — this is guidance, not legal advice; verify with the official regulator or counsel.

## Keywords
email marketing, email campaign, subject lines, email copywriting, drip campaign, email sequence, newsletter, welcome series, CAN-SPAM, GDPR email, CASL, email deliverability, SPF DKIM DMARC, unsubscribe, open rate, click rate, CTA, ESP

## Sample input
> "We sell a project-management SaaS to freelancers. People opt in on our site. Write us a welcome sequence and tell me how to stay deliverable and compliant."

## Sample output
*(Illustrative shape — permission-based, honest, not legal advice.)*
- **Welcome email:** an honest subject that matches the body, a value-first opening, **one** primary CTA, and a footer with a working unsubscribe + physical postal address.
- **Subject-line set:** several options driven by clarity/relevance/curiosity-with-substance — no clickbait, no fake "Re:".
- **4-email sequence:** goals, cadence, and exit criteria per email, plus a preference center so people can opt *down* (fewer emails) not just out.
- **Deliverability + compliance:** SPF / DKIM / DMARC explained correctly (sender authentication, not content filters), list-hygiene and reputation tips, and a CAN-SPAM / GDPR / CASL checklist — framed *not legal advice, verify for your jurisdiction*.

## Known limitations
- **Permission-based only** — it refuses purchased / rented / scraped / harvested lists and cold spam; it asks how your list was built.
- **Not legal advice** — CAN-SPAM / GDPR / CASL are summarized for guidance; requirements vary by jurisdiction and change. Verify with the official regulator (FTC / ICO / CRTC) or counsel. No penalty figures are baked in.
- **Advisory only** — it writes copy and plans; it does not send mail, manage your list, or configure your domain. Deliverability also depends on your ESP and DNS setup.
- Not your brand voice itself (pair with brand-voice-framework), not an ESP/CRM integration.
