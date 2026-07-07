---
name: rate-shopper-analysis
description: Analyze hotel competitor pricing, OTA displayed rates, parity, ranking, inclusions, restrictions, and demand dates from rate-shopper exports or OTA screenshots.
---

# Rate Shopper Analysis

Use this skill to turn competitor and OTA price observations into pricing recommendations.

## Inputs

Useful fields:

- Search date
- Stay date
- Hotel
- Competitor set
- Room type
- Rate
- Currency
- Tax inclusion
- Breakfast inclusion
- Cancellation policy
- Payment policy
- OTA channel
- Ranking position
- Review score
- Availability status
- Promotion or member rate

## Normalization

1. Compare only equivalent stay dates, occupancy, meal plan, cancellation policy, and room category when possible.
2. Separate tax-inclusive and tax-exclusive rates.
3. Mark non-equivalent comparisons clearly.

## Analysis Steps

1. Identify hotel price position versus competitor set: lowest, below median, at median, above median, or highest.
2. Calculate price gap against the lowest competitor, median competitor, and closest direct competitor.
3. Detect OTA parity issues and member-rate display risks.
4. Identify underpriced dates with high demand signals.
5. Identify overpriced dates without product, location, or review-score justification.
6. Recommend rate increases, holds, tactical discounts, restrictions, inclusion changes, or parity fixes.

## Pricing Rules

- Do not recommend matching the lowest price automatically.
- Consider review score, location, room quality, breakfast, cancellation policy, and brand strength before recommending a price cut.
- If the hotel is cheaper than weaker competitors on high-demand dates, recommend testing an increase.
- If competitor availability is limited, treat high competitor prices as demand signal rather than only a price gap.

## Output

Return Pricing Verdict, Competitor Position, Parity and Display Issues, Recommended Rate Moves, and Notes.
