---
name: ota-rules-auditor
description: Audit hotel OTA rate plans, promotions, cancellation policies, inventory controls, price parity, package rules, member discounts, and commission risk.
---

# OTA Rules Auditor

Use this skill when the user wants to check whether OTA settings are logical, risky, conflicting, or financially harmful.

## Inputs

Accept OTA rule text, screenshots converted to text, channel-manager settings, rate plan tables, promotion setup, cancellation policy text, contract terms, or spreadsheet exports.

Useful fields:

- OTA channel
- Room type
- Rate plan
- Meal plan
- Cancellation policy
- Prepayment policy
- Promotion name
- Discount rate
- Member discount
- Coupon funding
- Commission rate
- Min stay
- Max stay
- Advance booking window
- Blackout dates
- Stop sell dates
- Close to arrival
- Close to departure
- Inventory allocation

## Audit Areas

1. Rate and parity: check whether the same room and same conditions have inconsistent rates across channels.
2. Cancellation and payment: check whether flexible, semi-flexible, and non-refundable policies are priced logically.
3. Promotion stack: calculate combined discounts from base reduction, member discount, mobile discount, coupons, early-bird, and long-stay offers.
4. Inventory restrictions: find stop-sell, min-stay, close-to-arrival, and close-to-departure rules that block valuable demand.
5. Policy clarity: flag unclear breakfast, child fee, extra bed, deposit, invoice, refund, and check-in rules.

## Severity

- High: likely revenue loss, guest dispute, parity issue, overbooking, or unenforceable policy.
- Medium: may reduce conversion, margin, or operational clarity.
- Low: wording or setup issue with limited immediate impact.

## Output

Return these sections:

- Audit Verdict
- Top Risks
- Rule Conflicts
- Net Rate Check
- Recommended OTA Settings
- Questions To Confirm

Always calculate the combined effect of stacked discounts when data permits. Do not assume OTA-funded coupons reduce hotel revenue unless the source says the hotel funds them.
