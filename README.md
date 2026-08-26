# Multichannel sequence — a Claude skill

Writes a cold outreach sequence for **one hypothesis** — ICP × signal × offer —
across email and LinkedIn, for a B2B service company: custom development,
outstaffing, dedicated teams, engineering outsourcing.

It is the procedure behind the guide *«Як написати мультиканальний сіквенс»
(v3, August 2026)* by [Victor Shulga](https://victorshulga.com), Fractional CRO.
The guide is the reasoning; this skill runs it.

## Install

```bash
npx skills add victor-shulga/multichannel-sequence
```

User-level (available in every project):

```bash
npx skills add -g victor-shulga/multichannel-sequence
```

Then ask your agent for a sequence:

> Write a cold sequence for CTOs at US Series A fintechs that opened 5+ backend
> roles this quarter. We sell dedicated mobile teams. 3 mailboxes, list of 1,800.

## What it does differently

- **Picks the anchor before it writes a word.** Signal (an event with a date),
  data-point (a measurable state with a comparison), or a segment insight. Under
  10% of the list carrying an anchor → it tells you to rebuild the list instead
  of writing copy.
- **Refuses the call.** No meeting request, no calendar link, anywhere in a cold
  sequence. The soft CTA is split into three blocks with different costs.
- **Sizes the campaign against real capacity** — `mailboxes × 25 × 20` — not
  against the size of the market.
- **Four emails plus a close**, not the 8–12 touches of the 2024 playbook.
- **Writes the LinkedIn invite note** and stops optimising accept rate: the note
  costs 0–4 points of accept and returns 1.5–1.9× more replies.
- **Ships a measurement plan with an honest denominator** and a benchmark that
  depends on the anchor type. 1.5% replies is normal with no anchor; a signal
  campaign returning 1.5% is not a signal campaign.

## What is in it

| File | Content |
|---|---|
| `SKILL.md` | The procedure: gate → anchor → sizing → email → LinkedIn → self-check → measurement |
| `references/sequence-types.md` | The three anchors, expiry windows, the comparison formula, worked examples |
| `references/email.md` | Infrastructure, capacity math, letter anatomy, subject lines, P.S., cadence, reply handling |
| `references/linkedin.md` | Invite note, first message, three touches, limits, worked examples, what stopped working |
| `references/multichannel.md` | Both channels on one person, the N table, LinkedIn-first, what the 2024 playbook got wrong |
| `references/benchmarks.md` | Denominators, benchmarks per anchor type, test math, stop rules |
| `references/checklist.md` | The pre-send checklist |

## Not for

A single reply or objection · batch analysis of replies already received · warm
or inbound follow-up · writing the ICP itself.

## Sources

Benchmarks carry their sample size in the text. Where a number comes from a
vendor report with no disclosed sample, it is either excluded or marked as an
estimate. Belkins (7.5M emails, 15.1M LinkedIn touches, 2025), Expandi (13.2M
invites), SmartReach, Woodpecker, Gong.

MIT licensed. Built by [Victor Shulga](https://victorshulga.com) — Fractional CRO
for B2B service companies.
