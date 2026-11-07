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

## When Alexey asks to tailor a CV for a role

He typically pastes a posting, screenshots, or a recruiter message and asks
to adjust the CV, show it to him, and send it only after he confirms.
Do that work in this repo (`~/git/cv` on Hetzner).

1. Copy `cv/alexey` to `cv/alexey-<company>`, tailor `cv.yml`, and write
   `TAILORING.md` (target, requirement→evidence mapping, diff vs common,
   honest gaps, trace-back log). Keep every YAML line traceable to the
   truthfulness rule above.
2. Aim the tailored PDF at **one page** (`density: compact`). Show him the
   rendered PDF before sending anything.
3. Commit and push to main once he is happy with the file (or when he says
   to commit).
4. Send the outreach email only after he explicitly says to send it.

### Angle corrections (Nov 2026)

- The posting changes what to foreground, not the facts, and must not be
  mirrored into claims.
- For product / product-engineer roles, do not frame the CV as an
  AI-engineer résumé. Lead with product ownership.
  - DataTalks.Club: he develops and maintains all infrastructure and all
    products, internal and external, including AI Shipping Labs
    (in-session, 2026-11-07).
  - OLX: he owned the internal ML platform as a product for product groups
    across the company. Keep the title Senior → Lead → Principal Data
    Scientist; do not invent a Product Owner title.
- Put the blog in the header: [aishippingblog.com](https://aishippingblog.com)
  (also on the common source).
- When the CV will go out by email, omit the email address from the header.
  The recipient already has it.
- Never put a Calendly or booking link on the CV.

### Sending the CV by email

- Send from his personal Gmail (`alexey.s.grigoriev@gmail.com`), not work
  or Orin.
- Put the booking link in the email body, not the PDF:
  `https://calendly.com/dtc-alexey/30min`
- Keep the note short: greeting, that the CV is attached, the Calendly
  link, sign-off `Best,` / `Alexey`. Follow the email-rules skill (no
  dashes in the body).
- Attach the latest tailored PDF. Do not send until he says to send.
