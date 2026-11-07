# Instructions for working on this repo (humans and agents)

## Truthfulness rule (strict — added Nov 2026 after a violation)

Every line of every `cv.yml` must trace to one of:

1. the full CV (`alexeygrigorev.github.io/_data/cv.yml` — career history, tech lists, numbers), or
2. facts Alexey shared in-session (session prompts, PDFs, links he provided).

Never do these:

- **Mirror posting language into claims.** Words like `embed`, `secure`,
  `customer-facing`, `timelines` must not appear unless his history evidences
  them. The posting may only influence the *angle* (what to foreground), never
  the *wording of facts*.
- **Promote vague skills.** A skill item needs an evidenced owner: e.g. `MVP scoping`
  (his DataTalks bullet), not `technical delivery`; `TB-scale data processing`
  (his Simplaex words), not `data pipelines`.
- **Guess contact details, metrics, dates, titles.** (Upstream §5.7 applies.)

Allowed:

- **Headline may name the target role** (e.g. `Forward Deployed Engineer — …`).
  Headlines are positioning, not employment claims (CV-PROCESS.md §4).
- **Reframing true work toward the posting** (e.g. internal platform leadership
  described as de-facto internal consulting — with his explicit confirmation
  and hedged wording).

## Workflow rules

- Edit `cv/alexey/cv.yml` (common source) for facts; variants are full copies
  with focused trims — never hand-edit generated `cv.html`/`cv.pdf`.
- Every variant keeps a `TAILORING.md`: target, requirement→evidence mapping,
  diff vs common, honest gaps, trace-back log.
- General improvements discovered while tailoring get traced back to
  `cv/alexey/cv.yml`; closed-application snapshots (e.g. datadog) are not
  backported — note that instead.
- When unsure whether something is backed: ask, don't invent.
- Verify with `uv run render.py <person>` + Chromium PDF + `pdfinfo` page count.
  Position-specific variants (`alexey-<company>`) target **1 page** via
  `density: compact` (drop Projects when those builds already appear under
  Experience). The common source (`alexey`) may be 2 pages.
