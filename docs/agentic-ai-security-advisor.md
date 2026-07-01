# agentic-ai-security-advisor
> Threat-model, test, and harden your agentic AI — the OWASP Top 10 for Agentic Applications, MITRE ATLAS, and NIST AI RMF, as a structured advisory workflow. Defensive.

## Description
A security engineer's advisor for agentic and LLM-powered systems. From your agent's architecture — tools, memory, autonomy level, data flows — it maps the attack surface and trust boundaries, walks the **OWASP Top 10 for Agentic Applications** against your design, builds a library of **defensive** adversarial test scenarios (mapped to the ASI categories and **MITRE ATLAS** techniques), recommends defense-in-depth controls aligned to the **NIST AI RMF**, and helps you assemble a pentest-brief-quality assessment with risk ratings and a residual-risk statement. It's the advisory reasoning layer that automated scanners don't give you. Authorized, defensive use only.

## Compatibility
Advisory skill — no tooling or runtime required. Works from your agentic-AI system description and produces a threat model, adversarial test scenarios, controls, and an assessment report. **Authorized defensive use only — for systems you own or are permitted to assess; it does not attack third-party systems or weaponize anything, and it does not certify a system "secure".** OWASP ASI Top 10, MITRE ATLAS, and NIST AI RMF evolve — validate framework names/IDs against the current primary source.

## Keywords
agentic AI security, LLM security, AI red teaming, OWASP Top 10 for Agentic Applications, ASI Top 10, prompt injection, tool misuse, MITRE ATLAS, AI threat modeling, NIST AI RMF, LLM guardrails, agent security assessment, AI pentest, secure AI deployment, multi-agent security

## Sample input
> "Threat-model our customer-support agent. It has three tools (send email, read the orders DB, issue refunds via an API), persistent per-user memory, and can act without human approval up to $100. What are our biggest risks and how do we test + harden it?"

## Sample output
*(Illustrative shape — defensive, sanitized. No runnable exploit strings.)*
- **Threat model:** trust boundaries (user input, tool outputs, retrieved memory, the refund API) and the agentic attack surface across planning, tool-use, memory, inter-agent, and human-interface planes; a data-flow map of where untrusted content enters reasoning.
- **ASI walk:** which of the ten OWASP Agentic categories apply — e.g. Agent Goal Hijack (ASI01), Tool Misuse (ASI02), Identity & Privilege Abuse (ASI03), Memory & Context Poisoning (ASI06) — with severity in *this* architecture.
- **Defensive test scenarios:** for each risk, *what to probe on your own system* and the control it validates (e.g. "confirm the agent refuses a refund instruction embedded in an inbound email") — mapped to ASI + a MITRE ATLAS technique. Not weaponized payloads.
- **Controls + assessment:** least-privilege tool scopes, a human-approval gate above a spend threshold, memory-write authorization, egress limits — mapped to NIST AI RMF (Govern/Map/Measure/Manage); plus an assessment skeleton with likelihood×impact ratings and a residual-risk statement (it reduces risk, it does not certify "secure").

## Known limitations
- **Authorized defensive use only** — it refuses helping attack, jailbreak, exfiltrate from, or weaponize against third-party systems, and refuses building attacker tooling/malware. It secures systems you own or are permitted to assess.
- **No certification / no guarantee** — an assessment reduces risk and surfaces gaps; it does not prove a system secure. It states residual risk explicitly.
- **Verify-current** — the OWASP ASI Top 10, MITRE ATLAS, and NIST AI RMF evolve; validate framework names/IDs against the current primary source before relying on them.
- **Advisory only** — it produces the threat model, scenarios, controls, and report method; you run the assessment in your environment. Not an automated scanner. Not AI *governance/regulatory* advice (see the governance skill) or legal advice.
- Pairs with the pentest-report skill (report assembly) and threat-intel / web-pentest for the broader program.
