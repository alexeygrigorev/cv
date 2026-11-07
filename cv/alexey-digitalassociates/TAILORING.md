# TAILORING — alexey-digitalassociates

## Target

Digital Associates — Senior Product Engineer, 100% remote (EU).
Recruiter: Militza Kodzhabasheva
(`m.kodjabasheva@digitalassociates.de`), LinkedIn message, Nov 2026.

Project: next generation of an established manufacturing ERP (15 million
lines of code, 6,000–7,000 business processes). The work is to use AI to
see how the system is really used, lead discovery and requirements
engineering, evolve workflows while keeping the product upgradable, and
own agent-written implementation verified with independent tests.
Start immediately; 3 months, extension likely; full-time; English
required, German a plus.

Angle: product engineer who discovers real workflows, turns messy
operations into reviewable AI-assisted processes, and checks agent output
instead of trusting it. Not an ERP-domain specialist.

## Posting requirement → evidence mapping

- Capture and analyse business processes with AI → DataTalks "discover
  user problems, scope iterations"; DataOps turns messy operations
  (support, content, podcast, course ops) into reviewable workflows;
  Slack assistant reviewed from unanswered and corrected questions so it
  improves from real usage.
- Competitive analysis / benchmark workflows against the market → no
  evidenced formal competitive or market-benchmarking work. Not claimed.
- Revise existing workflows and design new ones → DataOps (SOPs,
  playbooks, recurring workflows, workflow state); Slack Q&A embedded in
  the community workflow.
- Plan product upgrades without breaking customer customisations → no
  ERP/customisation-upgrade evidence. Closest true fact is OLX platform
  work: standardizing how product groups build, deploy, and operate
  models. Not framed as upgrade-without-breaking-customisations.
- Own agent-based implementation and verify it with independent tests →
  "coding-agent-assisted workflows" for day-to-day operations; Slack
  assistant evaluations of retrieval and generation quality; DataOps
  "reviewable AI assistant jobs".
- Years of product development of business software (ERP, MES, planning,
  logistics) → no ERP, MES, planning, or logistics product work. Product
  engineering is for DataTalks.Club (education community) and OLX
  (marketplace ML platform). Not claimed.
- AI in requirements engineering, not just coding → evidenced as
  "problem discovery" and "discover user problems, scope iterations".
  The words "requirements engineering" are not used as a skill claim.
- Daily work with AI and coding agents, including verifying output →
  coding-agent-assisted operations; independent evaluation of the Slack
  assistant; reviewable assistant jobs on DataOps.
- At least one modernisation or replacement taken to go-live → shipped
  production systems (Slack assistant, DataOps, OLX duplicate-image
  detection and model-serving platform). These are new systems and
  platform standardization, not a replacement of a large ERP. Not
  described as an ERP go-live.
- Business-fluent English → books, conference speaking, English-language
  courses. German is listed as a plus on the posting; no language level
  is on the common CV, so none is added.

## What changed vs the common source (`alexey/cv.yml`)

- Headline → `Product Engineer — Ownership, Discovery, and Delivery`
  (no self-assigned "Senior"; dropped the AI-engineer framing).
- Summary opens as a product engineer, not a "product-minded AI
  engineer". Same year counts and credibility anchors. Emphasizes
  owning products end-to-end, reviewable workflows, and checking
  coding-agent work with evaluations. OLX is described as owning the
  ML platform as a product for internal product groups. Does not
  mention ERP, manufacturing, or market benchmarking.
- Skills: Product & Delivery first (same items as the common Product
  Engineering group). Agentic Engineering group from the common source
  (spec-driven development, software factories, loop engineering,
  context engineering, graph engineering — terms from his AI Shipping
  Blog). Production stack unchanged. No unverified skill names.
- One-page budget: `density: compact`; Projects dropped (Slack assistant
  and DataOps already evidenced under Experience); Recognition trimmed
  like the databricks variant (books + taught-100k + short Kaggle line).
- DataTalks DataOps and coding-agent bullets merged into one, to fit
  one page. The Zoomcamp/education-programs sentence is omitted here
  (the taught-100k recognition line stays).
- DataTalks first bullet leads with owning product work, not "AI product
  work" / LLM/RAG (the Slack Q&A assistant stays as the shipped example).
- OLX first bullet reframed toward product ownership of the internal ML
  platform for product groups (same leadership, team, and standardization
  facts; title stays Senior → Lead → Principal Data Scientist). The
  mentoring/architecture bullet is folded into that ownership bullet so
  the tailored PDF stays one page. The production-systems bullet now
  says "shipped" rather than "built".
- Header also includes his blog, https://aishippingblog.com (t695, 2026-11-07).
  Traced back to the common source.
- Email omitted from the header (t696, 2026-11-07); recruiter gets it from the message.
- Earlier roles and education unchanged.

## Honest gaps (do NOT paper over)

- No ERP, MES, planning, or logistics product experience.
- No formal competitive analysis or market benchmarking of workflows.
- No evidenced work on upgrading a large packaged product without
  breaking customer customisations.
- Delivery was to a community and internal product groups, not to an
  enterprise ERP customer.
- German proficiency is not stated on the common CV, so it is omitted.

## Trace-back log

- Agentic Engineering skill group added to `alexey/cv.yml` (terms from
  his blog: spec-driven development, software factories, loop
  engineering, context engineering, graph engineering).
- DataTalks infrastructure-and-products ownership (internal and
  external, including AI Shipping Labs) added from Alexey in-session
  (t687, 2026-11-07) and traced back to the common source summary and
  DataTalks experience bullet.
- OLX platform bullet reframed as owning the ML platform as a product
  for product groups (t688–t689, 2026-11-07) and applied to the common
  source as well. No title change. The tailored variant also shifts
  headline, summary, and DataTalks wording away from an AI-engineer
  frame toward product ownership.

## Reuse

Next position: `cp -r cv/alexey cv/alexey-<company>`, trim/add per the
posting, note the diff here. Never hand-edit generated `cv.html`/`cv.pdf`.
