# CV

Personal CV pipeline: one display-agnostic YAML source per variant → shared
renderer → Harvard-format HTML → PDF.

Based on the workshop
[`2026-07-08-ai-cv-pipeline`](https://github.com/AI-Shipping-Labs/workshops/tree/main/2026/2026-07-08-ai-cv-pipeline)
(playbook in `CV-PROCESS.md`, renderer in `cv/render.py` — both pulled verbatim
from upstream except one backward-compatible renderer extension: optional
`detail` on `experience_earlier` entries).

## Layout

| Path | Purpose |
|------|---------|
| `cv/alexey/cv.yml` | **Common source of truth. Edit this.** General improvements discovered while tailoring get traced back here. |
| `cv/alexey-datadog/cv.yml` | Datadog-tailored variant (Aug 2026) + `TAILORING.md` explaining the diff. |
| `cv/alexey-databricks/cv.yml` | Databricks Staff FDE variant + `TAILORING.md` (req 8653264002). |
| `cv/alexey-edtech/cv.yml` | EdTech variant (Berlin education companies) + `TAILORING.md`. |
| `cv/alexey-knowunity/cv.yml` | Knowunity-targeted variant + `TAILORING.md`. |
| `cv/render.py` | Shared renderer (`uv run render.py <person>` → `<person>/cv.html`). |
| `cv/*/cv.html`, `cv/*/cv.pdf` | Generated, git-ignored. Never edit by hand. |

## Workflow

```bash
cd cv
uv run render.py alexey           # common CV
uv run render.py alexey-datadog   # tailored variant

# PDF (Chrome → Print → Save as PDF, A4), or headless:
chromium --headless --no-pdf-header-footer \
  --print-to-pdf=alexey-datadog/cv.pdf file://$PWD/alexey-datadog/cv.html
```

New position: `cp -r cv/alexey cv/alexey-<company>`, tailor, add a
`TAILORING.md` noting the diff, and trace general improvements back to
`cv/alexey/cv.yml`.
