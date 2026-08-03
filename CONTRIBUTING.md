# Contributing to Awesome EU AI Act

Thank you for helping keep this list accurate and useful.

These rules were rewritten in August 2026 after auditing the list against its own previous
criteria. Several existing entries failed them, and several rules were unenforceable as
written. Rather than apply rules selectively, they now describe what this list actually
does. Where a judgement call remains, it says so.

## How to Add an Entry

1. Fork this repository
2. Edit `README.md` — add your entry to the section it belongs in. **There is no required
   order within a section**; append to the end and it will be placed during review.
3. Format: `**[Name](URL)** — One-sentence description. Key differentiator.`
4. Open a Pull Request titled `Add [Tool Name] to [Section Name]`
5. **If you are involved with the project, say so in the PR.** One line is enough.

## Criteria for Inclusion

- **Directly relevant** — EU AI Act compliance, AI governance, or closely related standards
  (ISO 42001, NIST AI RMF). A general-purpose ML tool with a compliance page does not qualify;
  the EU AI Act relevance has to be in the product, not in the marketing.
- **Actively maintained** — updated within the last 12 months.
- **Old enough to judge** — roughly 3 months of history, or demonstrable use: releases, a
  published package, actual users. A repository created days before the PR cannot be assessed,
  and this list is not a launch channel. This is not a verdict on quality — come back later.
- **Open-source** — public repository with an OSI-approved licence, and the `LICENSE` file
  actually present. If the PR states a licence, it has to match the repository.
- **Commercial** — a free tier, a self-serve trial, or complete public product documentation.
  "Book a demo" is not an evaluation path. Neither is a lead-capture quiz.

## Enterprise entries marked (demo-only)

Some platforms define this market but cannot be evaluated without talking to sales. Excluding
them would make the list less useful; listing them silently next to tools you can actually try
would be misleading. So they are listed and marked **(demo-only)**.

This is a narrow exception, not a way around the criteria above. It applies to established
platforms with a substantial public footprint — analyst coverage, named EU AI Act functionality,
a real customer base. It does not apply to a product whose deliverable is invisible until you
pay for it.

If you think an entry is wrongly marked, or wrongly unmarked, open an issue. That is a fair
argument to have in the open.

## Disclosure, self-promotion, and the maintainer's own tool

**Submitting your own project is welcome.** Most good entries arrive that way. Disclose it and
it is judged on the same criteria as anything else.

What is not welcome is **list-seeding**: the same entry filed to many lists within days, from a
repository with no history, often generated rather than written. That gets closed, with a reason.

The line is disclosure plus substance — not who is submitting. So, to be explicit about the
obvious conflict of interest: **the maintainer's own tool, the Venturalitica SDK, is listed in
Developer Tools & SDKs.** It is held to the criteria above and can be challenged in an issue like
any other entry. A list whose maintainer hides their own interest is worth less than one that
states it plainly.

## Criteria for Removal

- No activity for more than 12 months
- Project deprecated or abandoned
- No longer relevant to the EU AI Act
- The entry's claims stopped being true — a dead link, a changed licence, a lapsed certification,
  a number that moved

Removals are neither personal nor permanent. Fix the cause and open a PR to restore it.

## Style Guide

- One sentence, sentence case, plus a differentiator
- **No pricing.** It changes.
- **No funding figures** unless they carry information a reader needs. "$504M raised" does not
  explain what a tool does; a major certification or EU AI Pact signatory status might.
- **Claim the article, not the paragraph.** Say "Art. 12", not "Art. 12(3)", unless the finer
  mapping is publicly documented. Paragraph-level mappings to draft harmonised standards usually
  live in an Annex ZA that is not public.
- **Link to the thing that earns the listing** — the repository or the documentation, not a
  landing page selling an audit.

## What NOT to Include

- Paid-only tools with no public evaluation path (see the marked exception above)
- Generic ML tools with no AI governance relevance
- Tools not relevant to the EU market or the EU AI Act specifically
- List-seeding and undisclosed self-promotion

## Questions?

Open an issue or join the discussion in [GitHub Discussions](../../discussions).
