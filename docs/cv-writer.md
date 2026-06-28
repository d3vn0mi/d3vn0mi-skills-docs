# cv-writer
> Turn raw experience + a job posting into an ATS-safe resume and matching cover letter.

## Description
Rewrites your background into an ATS-parseable resume and a tailored cover letter, mirroring the exact keywords the posting screens for and quantifying impact — without inventing experience or numbers you didn't earn. Knows what applicant tracking systems choke on (tables, columns, header-only contact info) and writes around it.

## Compatibility
Advisory skill — no tooling or runtime required. Works from text you provide (your experience + the job description).

## Keywords
resume, CV, cover letter, ATS, applicant tracking system, keyword optimization, resume tailoring, career change, job application, quantified achievements, resume writing

## Sample input
> "Here's my experience (5 years backend dev, led a payments migration) and this job posting for a Senior Platform Engineer. Tailor my resume and write a cover letter."

## Sample output
*(Illustrative shape.)*
- **Resume:** single-column, standard headings; bullets rewritten as `action → what → quantified result`, e.g. "Led payments migration cutting checkout latency ~30% (real figure requested if not provided)."
- **Keyword alignment:** posting terms mirrored where you genuinely match (e.g. "platform reliability", "IaC").
- **Cover letter:** 3 short paragraphs — hook, evidence mapped to the posting's top 2 requirements, close.
- **ATS self-check:** flags anything that would break a parser.

## Known limitations
- **Never fabricates.** If you don't supply a metric it asks for the real number rather than inventing one — output is only as strong as what you provide.
- Optimizes formatting/keywords; it can't guarantee an interview or that a specific ATS will parse perfectly.
- Built for job-application resumes/cover letters, not academic CVs with publication lists (it will say so and offer a basic version).
