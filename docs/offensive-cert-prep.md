# offensive-cert-prep
> A hands-on tutor for offensive-security exams (OSCP & friends) — learn the methodology, practice in authorized labs.

## Description
Teaches the offensive curriculum the major hands-on pentest certs share — enumeration, web exploitation, Active Directory attacks, privilege escalation (Windows + Linux), pivoting, password attacks, buffer overflow, and the exam report — and walks you through *doing* it in authorized lab environments. Maps each cert (OSCP, PNPT, CPTS, eJPT, PenTest+, CEH, OSEP, CRTP, CRTO) to the topics, exam format, and study focus that matter. The deep companion to cert-suggester: that one tells you *which* cert; this one helps you *pass* it.

## Compatibility
For **authorized lab/exam practice only** — the cert's own lab, OffSec Proving Grounds, Hack The Box, or your own VMs. Assumes standard pentest tooling on your machine (Kali/Parrot Linux). Knowledge skill — no bundled runtime. Not for use against systems you don't own or aren't authorized to test.

## Keywords
OSCP prep, pass the OSCP, OSCP study guide, offensive security exam prep, pentest cert prep, Active Directory attacks, Kerberoasting, BloodHound, privilege escalation, pivoting, buffer overflow, OSCP exam report, PNPT, CPTS, eJPT, PenTest+, CEH, OSEP, CRTP, CRTO, HackTheBox prep, Proving Grounds, enumeration

## Sample input
> "I'm doing a Hack The Box machine in my own account and I've got a low-privilege shell on a domain-joined host. Walk me through the Active Directory attack path — and give me an OSCP study plan for the next 4 months."

## Sample output
*(Illustrative — the shape of the tutoring, not runnable commands.)*
- **AD attack path (methodology):** enumerate the domain with BloodHound → identify the shortest path to Domain Admin → check for Kerberoastable / AS-REP-roastable accounts → crack offline → move laterally with the recovered credential → abuse any ACL edges → work toward the DC. Each step explains *what to look for* and *which tool*, mapped to MITRE ATT&CK.
- **Study plan:** blueprint → gap self-assessment → week-by-week topic schedule → authorized-lab reps (Proving Grounds, TJ Null's OSCP-like list) → an AD-focused sprint → a full timed exam simulation → report practice. Exam logistics (cost/date/passing score) link to the official page.
- **Report:** the OSCP-style exam report skeleton — exec summary, methodology, per-host findings with reproducible steps + proof-flag evidence.

## Known limitations
- **Authorized lab/exam practice only.** It confirms an authorized context before giving hands-on steps and refuses unauthorized targets, exam braindumps/leaked solutions, and proctor evasion.
- **Teaches methodology — it does not run the tools or attack anything for you**, and it will not provide solutions to a cert's actual exam machines.
- **Exam details change** (format, cost, passing score, time limits) — the skill links the official exam page and tells you to verify; don't treat any specific as eternal.
- Techniques and tools are taught for the OSCP-tier curriculum; some niches (advanced AV/EDR evasion, exploit dev depth) point you onward (OSEP/OSED).
- No guarantee of passing — outcomes depend on your practice. It's a tutor, not a shortcut.
