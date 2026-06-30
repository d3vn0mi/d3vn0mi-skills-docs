# detection-engineering
> Author, test, and tune detection rules — Sigma + YARA — and map them to MITRE ATT&CK. Blue-team, defensive.

## Description
A detection engineer in a skill. It writes valid **Sigma** (SIEM/log) and **YARA** (file) detection rules, runs you through the detection-as-code lifecycle (hypothesis → develop → test → deploy → tune → maintain), reduces false positives the safe way, and maps every detection to **MITRE ATT&CK** so you can see coverage and gaps. Works from your logs/telemetry, a threat behavior, or a sample, and produces deployable rule text plus a tuning and coverage plan. Defensive by design — it builds detections for environments you own or are authorized to defend; it will not help evade detections or write malware.

## Compatibility
Defensive use only — for authorized environments you own or are contracted to defend. Advisory skill — no runtime required. Produces Sigma and YARA rules, false-positive tuning guidance, and ATT&CK coverage analysis; it does **not** help evade detections or write malware. Sigma schema, YARA syntax, and ATT&CK technique IDs evolve — validate against the current toolchain and ATT&CK release before deploying.

## Keywords
detection engineering, Sigma rules, YARA rules, detection as code, SIEM detection, threat detection, MITRE ATT&CK mapping, false positive tuning, blue team, SOC, alert tuning, detection rule, log analysis, threat hunting, security monitoring

## Sample input
> "We have Sysmon + a Splunk SIEM. We want to detect suspicious PowerShell and scheduled-task persistence, keep false positives down, and know our ATT&CK coverage."

## Sample output
*(Illustrative shape — benign detection signatures, defensive only.)*
- **Sigma rule:** a valid `process_creation` rule with named `selection` blocks, a `condition` (e.g. `selection and not filter`), a sensible `level`, and `attack.*` tags — ready to test in your SIEM.
- **YARA rule:** a valid `rule { meta / strings / condition }` where every defined string is referenced (no unused-string warnings), with the FP-vs-brittleness trade-offs explained.
- **Lifecycle + tuning:** test against true positives *and* benign data before deploy; precision-vs-recall guidance; safe, scoped, documented allowlisting (never a blanket rule-disable).
- **ATT&CK coverage:** each detection mapped to its real technique ID (e.g. T1059.001 PowerShell, T1053 Scheduled Task/Job), a coverage matrix with the gaps called out, framed verify-current.

## Known limitations
- **Defensive only** — it refuses evasion, detection-bypass, malware, or attacker tooling. It builds detections, not attacks.
- **You test + deploy** — rules are advisory; validate them in your own environment (true-positive *and* false-positive data) before production. A bad rule misses threats or floods analysts.
- **Verify-current** — Sigma schema, YARA versions, and MITRE ATT&CK technique IDs change; validate against the current toolchain and ATT&CK release.
- **No complete-coverage promise** — a detection is a hypothesis with gaps and false positives; the skill is honest about precision/recall trade-offs.
- Not a SIEM/EDR product or live deploy tool; not malware-analysis depth or a threat-intel feed (pair with the DFIR / threat-intel skills).
