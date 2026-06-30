# cloud-cert-prep
> A hands-on tutor for cloud-security exams (AWS / Azure / GCP) — learn the methodology, practice in your own account.

## Description
Teaches the cloud-security curriculum the major cloud certs share — the shared-responsibility model & cloud IAM, the per-provider security services (AWS, Azure, GCP), and cloud detection/logging/incident response — and walks you through configuring and checking it in your own authorized account. Maps each cert (AWS Security – Specialty, Azure AZ-500 / SC-200 / SC-100, Google Professional Cloud Security Engineer, ISC2 CCSP) to the topics, exam format, and study focus that matter. Cross-references the threat-intel and dfir-forensics skills for deeper coverage.

## Compatibility
For **authorized practice in your own cloud accounts / free tier / labs only** — never test or reconfigure tenants you don't own. Cloud lab resources **incur real charges** — use the free tier and tear down after every session. Knowledge skill — no bundled runtime.

## Keywords
cloud security cert prep, AWS Security Specialty study, SCS-C03, AZ-500 prep, SC-200, SC-100, Microsoft security, Azure security engineer, Google Professional Cloud Security Engineer, CCSP, cloud IAM, shared responsibility model, CloudTrail, GuardDuty, Defender for Cloud, Microsoft Sentinel, Security Command Center, cloud detection, VPC Service Controls

## Sample input
> "I'm studying for the AWS Security Specialty in my own free-tier account. Explain the shared-responsibility split, walk me through setting up threat detection, and give me a study plan."

## Sample output
*(Illustrative — the shape of the tutoring, not a full runbook.)*
- **Shared responsibility:** the provider secures the cloud (hardware, hypervisor, managed-service internals); you secure what's *in* the cloud (your data, identities/access, configuration) — and the line shifts by service model (IaaS → you own more; SaaS → you own data + access).
- **Threat detection (methodology):** turn on the API audit log → enable the managed threat-detection service that reads it → aggregate findings into the posture hub → route to your SIEM. Each step names the service and what "secure" looks like; cost-aware (free tier, tear down).
- **Study plan:** blueprint → gap self-assessment → topic schedule → hands-on labs (provider free tier, official skill platforms) → a detection/IAM sprint → a scenario run. Exam logistics link to the official page.

## Known limitations
- **Authorized own-account use only.** It refuses helping against tenants you don't own and refuses exam braindumps; it reminds you cloud labs cost money — tear down.
- **Teaches methodology — it does not run or change anything in your account for you.**
- **Exam details + cloud services change** (codes, retirements like AZ-500, console steps) — the skill links the official page and tells you to verify; e.g. it carries a soft retirement warning, not a baked date.
- **Deep cloud forensics + CTI point onward** — to dfir-forensics and threat-intel.
- No guarantee of passing — outcomes depend on your practice.
