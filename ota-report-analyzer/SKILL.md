---
name: ota-report-analyzer
description: Analyze hotel OTA order exports, channel performance, commission, cancellations, refunds, net revenue, room-night contribution, and booking behavior.
---

# OTA Report Analyzer

Use this skill when the user provides Booking.com, Expedia, Trip.com, Ctrip, Meituan, Fliggy, Agoda, PMS, channel-manager, CSV, Excel, or pasted OTA order data.

## Inputs

Common fields:

- Order ID
- Channel or OTA
- Hotel name
- Room type
- Rate plan
- Check-in date
- Check-out date
- Booking date
- Cancellation date
- Order status
- Room nights
- Rooms
- Gross room revenue
- Promotion discount
- Platform subsidy
- Commission rate
- Commission amount
- Net revenue

## Analysis Steps

1. Normalize fields, dates, currencies, and order statuses.
2. Remove duplicate orders when an order ID exists.
3. Classify orders as stayed, future, cancelled, no-show, refunded, modified, or uncertain.
4. Calculate gross revenue, net revenue, commission, effective commission rate, room nights, ADR, cancellation rate, lead time, length of stay, revenue share, and room-night share.
5. Flag high cancellation channels, high commission leakage, unusual discounting, low net ADR, same-day booking spikes, missing room nights, and refunds without cancellation status.
6. Produce a management summary and recommended actions.

## OTA Rules

- Treat OTA-funded subsidy as platform funding unless the data says the hotel funded it.
- Prefer provided net revenue over estimated net revenue.
- Calculate ADR only on stayed or consumed room nights unless the user asks for on-books analysis.
- Separate cancelled bookings from stayed bookings.
- Do not judge channel value by order count alone.

## Output

Return these sections:

- Executive Summary
- KPI Table
- Channel Performance
- Findings
- Recommended Actions
- Data Quality Checks

Prioritize net revenue and room-night contribution over gross revenue and order count.
