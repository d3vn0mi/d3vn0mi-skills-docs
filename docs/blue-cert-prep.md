# blue-cert-prep
> A hands-on tutor for defensive-security exams (SOC analyst / blue team / DFIR) — learn the methodology, practice on authorized data.

## Description
Teaches the defensive curriculum the major blue-team certs share — log & SIEM analysis, network traffic analysis, endpoint triage & IR, detection engineering / threat hunting, and the incident-response lifecycle — and walks you through it on authorized data and free training labs. Maps each cert (GCIH, GCFA, GNFA, GCIA, GCED, GCDA, CompTIA CySA+, BTL1/BTL2) to the topics, exam format, and study focus that matter. Cross-references the dfir-forensics and threat-intel skills for deeper coverage.

## Compatibility
For **authorized monitoring / lab / exam practice only** — your own lab, authorized monitoring data, or free defensive ranges (CyberDefenders, LetsDefend, Blue Team Labs Online, Splunk BOTS). Assumes standard defensive tooling (Wireshark, Zeek, Splunk/ELK, Volatility). Knowledge skill — no bundled runtime. Not for use on data or systems you are not authorized to monitor or analyze.

## Keywords
blue team cert prep, SOC analyst certification, GCIH study, GCFA, GNFA, GCIA, CySA+ prep, BTL1, BTL2, log analysis, SIEM, Splunk, KQL, threat hunting, Sigma, detection engineering, incident response, NIST 800-61, network traffic analysis, pcap, endpoint triage, defensive security exam

## Sample input
> "I'm working an authorized SIEM case: a burst of failed logons then one success then a special-privileges event from a single source. Walk me through the triage — and give me a 4-month plan to pass BTL1."

## Sample output
*(Illustrative — the shape of the analysis tutoring, not raw findings.)*
- **Triage (methodology):** the failed-then-successful-logon-then-privilege pattern reads as a brute force that succeeded into a privileged session → scope by source and account → baseline whether that account/source is normal → pivot to process/network telemetry → classify. Maps to MITRE ATT&CK (Brute Force → Valid Accounts).
- **Query (shape):** filter the auth events by source + account, aggregate the failures, then correlate to the success — expressed as a representative SIEM query pattern (verify syntax for your platform).
- **Study plan:** blueprint → gap self-assessment → topic schedule → authorized-lab reps (CyberDefenders, LetsDefend, BTLO) → a detection/hunt sprint → a full practice scenario. Exam logistics link to the official page.

## Known limitations
- **Authorized use only.** It confirms an authorized data source before giving analysis steps and refuses unauthorized investigation, exam braindumps, and fabricating findings.
- **Teaches methodology — it does not run the tools or analyze data for you**, and it won't provide answers to a cert's actual exam.
- **Exam details change** (format, cost, passing score) — the skill links the official page and tells you to verify.
- **Deep forensics and CTI point onward** — disk/memory forensics defers to dfir-forensics; intelligence analysis to threat-intel. This skill is the SOC-analyst/exam-prep layer.
- No guarantee of passing — outcomes depend on your practice.
