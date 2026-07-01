# ai-governance-policy-builder
> Stand up AI governance — classify your AI by risk, inventory it, draft the policy, and map it to the EU AI Act, NIST AI RMF, and ISO/IEC 42001. Guidance, not legal advice.

## Description
A governance-in-a-box advisor for teams putting AI oversight in place. From your AI-system inventory and context, it classifies each system by risk against the **EU AI Act** tiers (including Annex III high-risk and GPAI), builds a reusable **AI asset register**, drafts an **AI acceptable-use policy**, assembles a **governance framework** (roles, lifecycle gates, oversight) aligned to the **NIST AI RMF**, and produces a control crosswalk mapping obligation themes to **ISO/IEC 42001** and the evidence to keep. It's the structured advisory layer that generic policy templates don't give you — but it's **guidance, not legal advice**, and every regulatory specific is pointed to the official source for your qualified counsel or DPO to confirm.

## Compatibility
Advisory skill — no tooling or runtime required. Works from your AI-system inventory and context and drafts governance artifacts. **Guidance only, NOT legal advice — a qualified lawyer or DPO must review before adoption, and it does not certify compliance.** AI regulation is phased and moving (e.g. the EU AI Act timeline, subject to the Digital Omnibus) — verify current dates, penalties, and obligations against official sources.

## Keywords
AI governance, AI usage policy, EU AI Act, AI Act compliance, AI risk classification, high-risk AI, Annex III, AI asset register, AI inventory, NIST AI RMF, ISO 42001, AI management system, responsible AI, acceptable use policy, AI compliance framework, Chief AI Officer, AI governance framework

## Sample input
> "We're a mid-size company rolling out several AI tools — a CV-screening assistant, a customer chatbot, and an internal code assistant. Help us classify their risk, inventory them, draft an AI usage policy, and set up governance."

## Sample output
*(Illustrative shape — guidance, not legal advice; verify current rules officially.)*
- **Risk classification:** each system walked through the EU AI Act tiers — e.g. CV-screening → an Annex III (employment) *high-risk consideration* to confirm with counsel; chatbot → transparency-tier disclosure duties; code assistant → likely minimal — with a verify-current note on the moving timeline.
- **Asset register:** a reusable table (purpose, owner, risk tier, data + PII, model/provider, GPAI dependency, human-oversight, review date) plus a privacy-respecting way to surface shadow AI.
- **AI usage policy:** an AUP skeleton — approved tools, data-classification rules (what may/may not go into which AI), prohibited uses, human review, disclosure, incident reporting — flagged for legal/DPO/HR review.
- **Governance + control map:** roles (governance board, owners, DPO), model lifecycle gates, and a crosswalk of high-risk obligation themes ↔ NIST AI RMF (Govern/Map/Measure/Manage) ↔ ISO/IEC 42001, with the evidence to keep.

## Known limitations
- **Not legal advice** — it produces starting-point frameworks and drafts; it does not determine your legal obligations, tell you whether you're compliant, or certify compliance. A qualified lawyer / DPO / compliance professional must review before adoption.
- **Verify current rules** — the EU AI Act is phased and its timeline is moving (Digital Omnibus conditional delays). It never bakes a deadline or penalty figure; it points you to official EU sources (eur-lex.europa.eu, the EU AI Office, your national authority) to confirm dates and obligations for your category.
- **Describes, doesn't certify** — it helps you align to ISO/IEC 42001 and structure evidence; certification is a separate third-party audit.
- **Advisory only** — not AI security testing (see agentic-ai-security-advisor), not SOC 2 / ISO 27001 audit readiness (see grc-audit-readiness-advisor), and not a jurisdiction-by-jurisdiction legal database.
