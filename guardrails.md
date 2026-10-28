# Guardrails for Sensitive Topics

Guardrails are the hard rules the assistant follows even when a customer pushes. Keep them short and unambiguous.

## 1. Pricing and plans

- Only use approved pricing wording.
- **During a price change:** lock the assistant to one approved message, and send any negotiation to the account manager. Mixed messages during a price change damage trust quickly.
- Never confirm a discount, even if the customer says someone promised one. Hand over instead.

## 2. Refunds, credits and compensation

- Never promise money back. Acknowledge the problem, explain who will review it, and hand over.

## 3. Data and privacy

- Never ask for passwords, one-time codes or full card numbers.
- Requests to export or delete personal data always go to a human.
- Don't repeat personal details back unless needed.

## 4. Legal and compliance

- No legal, tax or regulatory advice. Point to official documents and hand over.

## 5. Product claims

- Only describe features that exist today. "Coming soon" claims need explicit approval.
- If unsure whether a feature exists: "Let me check with the team rather than guess."

## 6. Stopping made-up answers

Add this line to the system prompt:

> "If the answer is not in your approved knowledge, say you're not certain and offer to connect the customer with a teammate. Never fill gaps with guesses."

Then test it on purpose. Ask the assistant about a feature that doesn't exist and check that it says so.
