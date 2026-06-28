# dfir-forensics
> Run a forensically-sound DFIR investigation end-to-end — Windows, Linux, Cloud, and memory.

## Description
A senior DFIR analyst in a skill: it guides the full incident-response lifecycle, interprets the artifacts you collect (event logs, registry, $MFT, auth logs, CloudTrail/Entra, memory dumps), reconstructs the timeline, maps findings to MITRE ATT&CK, and turns it into Sigma/YARA detections and a court-defensible report. Built for integrity — it preserves evidence, flags gaps, and never fabricates findings.

## Compatibility
Authorized, defensive DFIR work only. Knowledge skill (no bundled runtime) — assumes you run standard forensic tooling on your own machine (e.g. Volatility3, KAPE, Velociraptor, Autopsy, ELK). Works on artifact output you provide; no external service calls.

## Keywords
DFIR, incident response, digital forensics, breach investigation, compromise assessment, evtx, event log, Windows registry, $MFT, USN journal, memory forensics, Volatility, CloudTrail, Entra sign-in, MITRE ATT&CK, timeline, IOC, Sigma, YARA, chain of custody, malware analysis

## Sample input
> "Here are ~40 lines of Windows Security log: lots of 4625s for `svc_backup` from 10.0.0.5 over two minutes, then one 4624 Logon Type 3 for `svc_backup` from 10.0.0.5, then a 4672. What happened, and can you give me a detection?"

## Sample output
*(Illustrative — structure of what you receive, not raw evidence.)*

- **Interpretation:** high-volume failed logons against a single account followed by a success = **brute force that succeeded**, then a privileged network logon.
- **ATT&CK:** T1110 / T1110.001 (Brute Force) → T1021.002 + T1078 (Valid Accounts) → T1078 privileged session.
- **Timeline (UTC):** `<t0>` first 4625 … `<t0+2m>` 4624 Type 3 … `<t0+2m>` 4672 — single source `10.0.0.5`.
- **Detection (Sigma, shape):** `logsource: product=windows, service=security`; `detection:` threshold of 4625 by source+account then a 4624 success → `level: high`.
- **Report stub:** finding title, severity, affected asset, evidence reference + hash placeholder, remediation, chain-of-custody appendix.

## Known limitations
- **Guides and interprets — does not run the tools or perform acquisitions for you.** You collect/image evidence; the skill tells you what to look for and what it means.
- **Authorized, defensive use only.** Refuses anti-forensics (log wiping, timestomping), unauthorized investigation, and evidence fabrication.
- **No fabrication:** if data is missing it says so rather than guessing — so output quality depends on the artifacts you provide.
- Detection rules and ATT&CK mappings are starting points to validate in your environment, not drop-in production rules.
- Not legal advice; "court-defensible" means it *supports* admissibility (documented methodology, hashes, chain of custody), it does not guarantee a legal outcome.
