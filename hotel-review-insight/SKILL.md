---
name: hotel-review-insight
description: Analyze hotel OTA guest reviews from Booking.com, Trip.com, Ctrip, Meituan, Agoda, Expedia, Google, or PMS surveys. Extract sentiment, themes, operational issues, and response priorities.
---

# Hotel Review Insight

Use this skill to turn hotel guest reviews into operational insight and OTA reputation actions.

## Inputs

Useful fields:

- Review ID
- OTA channel
- Review date
- Stay date
- Guest segment
- Rating
- Positive text
- Negative text
- Full review
- Room type
- Travel purpose
- Language
- Staff reply

## Analysis Steps

1. Normalize rating scales to 0-10 or 0-100.
2. Detect review language and translate only when needed.
3. Classify sentiment as positive, neutral, negative, or mixed.
4. Extract themes such as cleanliness, front desk, room condition, noise, breakfast, location, value, facilities, Wi-Fi, air conditioning, bathroom, check-in, parking, and OTA information accuracy.
5. Identify recurring operational issues and likely owner.
6. Compare themes by channel, room type, month, and rating band when data permits.
7. Draft short OTA replies for high-impact negative reviews if requested.

## Review Rules

- Do not overreact to one extreme review unless it describes safety, hygiene, or legal risk.
- Prioritize recurring, specific issues over vague complaints.
- Treat OTA information accuracy as a commercial issue, not only a service issue.
- Keep reply drafts concise, specific, polite, and avoid admitting legal liability.
- If ratings and text disagree, call out the mismatch.

## Output

Return Reputation Snapshot, Top Positive Drivers, Top Negative Drivers, OTA Content Fixes, Priority Actions, and Optional Reply Drafts.
