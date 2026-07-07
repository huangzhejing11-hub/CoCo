---
name: hotel-revenue-dashboard
description: Build hotel revenue analysis from PMS, OTA, or channel-manager data. Calculates OCC, ADR, RevPAR, pickup, pace, lead time, length of stay, channel mix, cancellations, and demand signals.
---

# Hotel Revenue Dashboard

Use this skill to convert raw hotel booking, stay, PMS, OTA, or channel-manager data into revenue-management insight.

## Inputs

Useful fields:

- Stay date
- Booking date
- Check-in date
- Check-out date
- Room type
- Rate plan
- Channel
- Order status
- Room nights
- Available rooms
- Rooms sold
- Room revenue
- Net room revenue
- Cancellation date
- Market segment
- Promotion

## Core Metrics

- Occupancy: rooms sold divided by available rooms
- ADR: room revenue divided by rooms sold
- RevPAR: room revenue divided by available rooms
- Net ADR: net room revenue divided by rooms sold
- Net RevPAR: net room revenue divided by available rooms
- Cancellation rate: cancelled bookings divided by total bookings
- Lead time: check-in date minus booking date
- Length of stay: check-out date minus check-in date
- Pickup: change in on-books room nights or revenue over time
- Channel mix: share of revenue and room nights by channel

## Analysis Steps

1. Identify whether the data is stay-date based, booking-date based, or mixed.
2. Separate stayed, on-books future, cancelled, no-show, and tentative data.
3. Calculate KPIs by day, week, month, room type, rate plan, and channel.
4. Explain drivers such as volume effect, rate effect, channel mix, cancellation, room-type mix, events, and holidays.
5. Recommend pricing, restriction, inventory, and OTA exposure actions.

## Recommendation Rules

- If occupancy is high and pickup is strong, consider raising rates or closing low-margin promotions.
- If occupancy is low but lead time is short, use tactical OTA exposure instead of broad long-term discounting.
- If ADR is high but RevPAR is weak, diagnose unsold inventory before raising price.
- If OTA share is rising while net ADR is falling, check commission, promotion stacking, and direct-channel parity.
- If cancellations are concentrated in one channel, separate channel demand from reliable demand.

## Output

Return Revenue Snapshot, Demand Signals, Channel Mix, Date-Level Opportunities, Revenue Manager Notes, and Data Assumptions.
