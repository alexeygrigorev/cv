# TAILORING — alexey-datadog

## Target

Datadog application, August 2026. Job posting:
`https://careers.datadoghq.com/detail/8112183/?gh_jid=8112183`
(note: the posting is gone — 404 as of Nov 2026 — so the exact role title
can't be re-verified; the CV angle below is preserved as-is).

Angle: senior production AI/ML systems + platform leadership + high-throughput
ML. Everything a monitoring/observability-adjacent hiring manager scans for —
reliability, scale numbers, ownership — is on page one.

## What changed vs the common source (`alexey/cv.yml`)

- **Dropped the Projects section.** The AI work (Slack Q&A, ops platform)
  already lives under Experience; duplicating it costs space
  (CV-PROCESS.md §5.4).
- **Dropped the education-programs bullet** under DataTalks.Club (kept the
  `Taught AI/ML to 100k+` line under Recognition instead).
- **Trimmed Recognition** to books + taught + Kaggle. Dropped `Top 100 GitHub`
  and `Author/speaker` for focus — they stay in the common source.
- **Kaggle line shortened** (no `Instagram Challenge`) to save a line.
- Everything else — headline, summary, skills, experience bullets,
  earlier-role details — is identical to the common source on purpose.

## Trace-back log (already applied to `alexey/cv.yml`)

General improvements discovered during this tailoring session that belong to
every future application, so they live in the common source:

- Headline → `AI Product Engineer — Production AI Systems`.
- Summary rewritten: 16 yrs SE / 14 yrs AI-ML, `identify user needs → ship
  working solutions`, `run a 100k+ community and develop tools`, `led the ML
  platform team at OLX`.
- Skills regrouped to Product Engineering / AI Engineering / Leadership /
  Production Systems (was Product & Delivery / Applied AI / Platform).
- OLX bullets reordered (platform → leadership → systems) and reworded:
  `platform for serving deep-learning models (~200 images/sec)`, not
  `production inference infrastructure`.
- DataTalks.Club bullets merged to two (end-to-end ownership incl. Slack Q&A;
  ops platform without the word `deterministic`).
- Earlier roles gained one-line `detail` each (AdTech/TB-scale; SEO/NLP;
  freelancing; Java SE) — rendered via the new optional `detail` field.
- Contact links gained `alexeygrigorev.com/cv`.
- Proposed-then-reverted (NOT in either file): Substack blog link.

## Reuse

Next position: `cp -r cv/alexey cv/alexey-<company>`, trim/add per the posting,
note the diff here. Never hand-edit generated `cv.html`/`cv.pdf`.
