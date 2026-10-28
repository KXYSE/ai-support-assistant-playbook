# Escalation Rules

The assistant should hand over to a human **immediately** if any of these are true. It's better to escalate too often in the first month and relax the rules later than to leave an unhappy customer stuck with a bot.

## Always escalate

| Trigger | Example | Route to |
| --- | --- | --- |
| Customer asks for a person | "Can I talk to someone?" | Support queue |
| Strong frustration or anger | Caps, repeated complaints, "this is ridiculous" | Support lead |
| Billing dispute, refund or credit request | "I was charged twice" | Billing team |
| Cancellation or downgrade intent | "How do I cancel?" | Account manager |
| Legal, security or data request | Data deletion, contract terms, security questionnaire | Account manager + legal/security |
| Service outage affecting the customer's business | "None of our calls are going through" | Technical support (urgent) |
| The assistant has failed twice | Two answers that didn't solve it | Support queue |
| Anything outside the approved knowledge | New feature questions, custom setups | Support queue |

## Handover message to the customer

> "I want to make sure this is handled properly, so I'm passing you to [team/person]. They'll have everything we've discussed, so you won't need to repeat yourself. You can expect a reply within [time]."

## Internal summary (attached to every handover)

```
Customer: [name, company, plan/tier]
Issue: [one line]
Already tried: [steps the assistant took]
Customer mood: [calm / frustrated / angry]
Urgency: [low / medium / high, with reason]
```

## Review these rules monthly

Look at escalated conversations and ask:

- Were any escalated that the assistant could have handled? Add an approved answer.
- Were any **not** escalated that should have been? Add a trigger.
