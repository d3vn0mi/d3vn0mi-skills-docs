# grc-audit-readiness-advisor
> Get audit-ready for SOC 2, ISO 27001, and GDPR/DPIA — gap analysis, evidence, and a cross-framework crosswalk. Readiness prep, not the audit.

## Description
A GRC advisor that prepares your organization for a compliance assessment. From your current posture and target framework, it runs you through the readiness lifecycle — scope, control-gap analysis, remediation, evidence collection, and pre-audit review — with framework-specific depth for **SOC 2** (the 5 Trust Services Criteria, Type I vs Type II), **ISO/IEC 27001:2022** (the ISMS, Annex A, the Statement of Applicability, Stage 1/2), and **GDPR Article 35 DPIAs**. It builds an evidence playbook and a cross-framework crosswalk so one artifact can satisfy multiple frameworks. Crucially, it **prepares** you — it does not perform the audit, issue a SOC 2 report, grant ISO 27001 certification, or sign off a DPIA. Those are done by a licensed CPA firm, an accredited certification body, and your DPO.

## Compatibility
Advisory skill — no tooling or runtime required. Works from your current security/privacy posture and target framework, and produces a gap analysis, evidence playbook, and audit-readiness plan for SOC 2, ISO 27001, and GDPR/DPIA. **Readiness prep only — it does NOT perform the audit, issue a SOC 2 report, grant ISO 27001 certification, or sign off a DPIA (those require a licensed CPA firm / accredited body / your DPO), and it is not legal advice.** Framework criteria + templates evolve — verify against AICPA, ISO, and ICO/EDPB for your scope.

## Keywords
SOC 2, SOC 2 readiness, ISO 27001, ISO 27001:2022, GDPR, DPIA, data protection impact assessment, audit readiness, compliance gap analysis, Trust Services Criteria, Statement of Applicability, evidence collection, control mapping, GRC, security compliance, SOC 2 Type II, ISMS, pre-audit

## Sample input
> "We're a SaaS startup pursuing SOC 2 Type II and later ISO 27001, and we process EU customer data. Where are our gaps, what evidence do we need, and how do we avoid collecting the same thing three times?"

## Sample output
*(Illustrative shape — readiness prep, verify current criteria officially.)*
- **Readiness lifecycle:** scope → gap analysis → remediation → evidence collection → pre-audit review → **the external audit (where the licensed CPA firm / accredited body takes over)** → continuous monitoring, with SOC 2 Type II observation-window timing.
- **Gap register:** current control → required criterion → gap type (design / operating / evidence) → owner → remediation, prioritized risk × effort.
- **Evidence playbook:** the artifact that proves each control, how to name/date/index it, and the reminder that Type II evidence must span the whole observation period (no retro-collection).
- **Crosswalk:** an illustrative map where one artifact (e.g. an access review) covers SOC 2 CC6 + ISO 27001 Annex A access controls + a GDPR access-control obligation — so you gather evidence once.

## Known limitations
- **Readiness prep only** — it does NOT perform the audit, issue the SOC 2 report, grant ISO 27001 certification, or sign off a DPIA, and it will not claim you are "compliant" or "certified". A licensed CPA firm / accredited certification body / your DPO does the actual assessment.
- **Honest evidence only** — it will not help fabricate or backdate evidence or misrepresent posture; gaps are surfaced, not hidden.
- **Not legal advice** — GDPR/DPIA and contractual specifics go to your DPO and qualified counsel; it points to the official source (AICPA, ISO, ICO/EDPB) and never bakes a penalty figure.
- **Verify-current** — framework criteria, control counts, and templates evolve; validate against the official body for your scope.
- **Advisory only** — not the audit / not a GRC-automation platform; not AI governance (see ai-governance-policy-builder) or AI security testing (see agentic-ai-security-advisor).
