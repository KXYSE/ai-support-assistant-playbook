# AI Support Assistant Playbook

A practical template for setting up an AI assistant that answers customer support questions for a B2B SaaS product, and for checking that it keeps doing a good job after launch.

I put this together from what I've learned designing and reviewing AI support assistants in a B2B SaaS company. Everything here is generic. The company in the examples, **Linewise**, is made up.

## Why this exists

Most AI support bots fail in the same three ways:

1. **They make things up.** They give an answer that sounds confident about pricing, refunds or features that don't exist.
2. **They don't know when to stop.** An angry customer or a billing dispute keeps getting bot replies when it should have gone to a person ten minutes ago.
3. **Nobody checks them after launch.** The prompt is written once and nobody reads the conversations again.

This playbook tackles all three: a prompt structure that limits what the assistant may say, clear escalation rules, and a simple review routine.

## What's inside

| File | What it's for |
| --- | --- |
| [`system-prompt-template.md`](system-prompt-template.md) | Fill-in-the-blanks system prompt: role, tone, what it may and may not say |
| [`escalation-rules.md`](escalation-rules.md) | When the assistant must hand over to a human, and how |
| [`guardrails.md`](guardrails.md) | Hard rules for sensitive topics (pricing, refunds, legal, data) |
| [`review-scorecard.md`](review-scorecard.md) | A scorecard for reviewing real conversations every week |
| [`examples/good-vs-bad-replies.md`](examples/good-vs-bad-replies.md) | Side-by-side replies with notes on what makes one better |

## How to use it

1. Copy `system-prompt-template.md` and fill in your product, tone and approved answers.
2. Agree the escalation rules with your support lead **before** launch.
3. Add your guardrails. Start strict and loosen them later.
4. After launch, sample conversations every week and score them with the scorecard.
5. Fix the prompt, not the symptoms. If the same mistake shows up twice, a rule is missing.

## What I've learned

- **Tone rules matter as much as facts.** Customers forgive "I'm not sure, let me get someone" far more than a wrong answer delivered confidently.
- **Every escalation should carry context.** The human who picks it up should never have to ask the customer to repeat themselves.
- **Pricing is the most dangerous topic.** During a price change, lock the assistant to approved wording only.
- **Review the conversations, not just the metrics.** Resolution rates can look healthy while customers are quietly annoyed.

---

Maintained by **Kingsley Iwunna**, customer experience and B2B account management, Lagos, Nigeria.
