# threat-intel
> Run the full cyber threat intelligence lifecycle — raw data to analyst-grade intelligence.

## Description
Enriches indicators (STIX/TAXII), profiles adversaries against MITRE ATT&CK, generates hunt hypotheses, prioritizes CVEs (CVSS + EPSS + KEV), and produces TLP-marked intelligence products — all governed by real analytic tradecraft (ACH, confidence language, source grading). Lawful and ethical by design: every assessment carries a confidence level and its sourcing.

## Compatibility
Advisory skill — no tooling or runtime required. Lawful OSINT methodology only; works on data you lawfully supply. Refuses collection via intrusion or stolen-data markets.

## Keywords
threat intelligence, CTI, IOC enrichment, STIX, TAXII, MITRE ATT&CK, adversary profiling, Diamond Model, threat hunting, hunt hypothesis, CVE prioritization, EPSS, CISA KEV, TLP, confidence assessment, analysis of competing hypotheses

## Sample input
> "We saw a suspicious IP and a file hash beaconing from an internal host. Enrich them, map the behavior to ATT&CK, and tell me what to hunt for — with confidence levels."

## Sample output
*(Illustrative shape.)*
- **Enriched indicators:** type, context, confidence band; expressed as STIX `indicator` objects for sharing.
- **ATT&CK + Diamond:** observed behavior mapped to techniques; activity placed on the four Diamond vertices.
- **Assessment:** likelihood and analytic confidence stated *separately* (ICD-203), with sourcing.
- **Hunt hypothesis:** "if actor uses T-XXXX, we'd see Y in Z telemetry" → where to look.
- **Product:** BLUF-structured, TLP-marked summary for the right audience.

## Known limitations
- **Does not collect intel by hacking** — lawful OSINT methodology only; refuses intrusion and stolen-data sources.
- **Attribution discipline:** it clusters and qualifies with confidence; it refuses unfounded "name the actor" requests.
- Enrichment/analysis quality depends on the data you provide; it is not a live feed and calls no external APIs for you.
- Hands finished detection-rule authoring to a detection/forensics workflow (it generates the hypothesis and the idea).
