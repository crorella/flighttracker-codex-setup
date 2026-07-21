---
name: find-cheapest-flights
description: Find the lowest-cost practical flight combinations by comparing cash and award sources, flexible dates, nearby airports, round trips, separate one-ways, mixed carriers, positioning flights, open jaws, and self-transfers. Use when the user asks for the cheapest flights, creative routings, fare comparisons, flexible-date searches, cash-versus-points analysis, or ways to reduce the total cost of an itinerary.
---

# Find Cheapest Flights

Search broadly, calculate the true trip cost, and distinguish protected itineraries from risky separate-ticket combinations. Dynamic airfare prevents proving a global minimum, so state the search coverage and any missing sources.

## Establish the search

1. Capture the origin and destination, travel dates or flexibility window, trip type, traveler count, cabin, checked-bag needs, acceptable stops, and nearby-airport tolerance.
2. Ask only for missing constraints that materially change the search. If the user says “cheapest possible,” default to economy, broad timing, nearby airports, and reasonable self-transfers, but label these assumptions.
3. Include points only when award tools are available or the user is open to points. Never treat points as free; include taxes, fees, and opportunity cost.

## Search independently and in parallel

Use every relevant source available rather than trusting a single aggregator:

- Search at least two independent cash sources, preferring live GDS or airline-direct pricing over cached or metasearch estimates.
- Check Google Flights or another broad metasearch source for schedule coverage.
- Check airline-direct sources for carriers omitted from GDS results, including Southwest when it serves the route.
- Check virtual-interlining or self-transfer sources for creative combinations.
- Check award availability across all programs before filtering by a presumed points balance.
- Search the departure-country and destination-country markets for international trips when supported; show currency and likely foreign-transaction costs.
- Report each source as successful, failed, unavailable, or skipped with a reason. Never hide missing coverage.

## Price all useful constructions

For round trips, always compare the published round-trip fare against independently searched outbound and return one-ways. Also test:

1. Mixed carriers in each direction.
2. Flexible dates, starting with the user's window and expanding only with permission.
3. Nearby origin and destination airports, including realistic ground-transfer costs.
4. Positioning flights to a cheaper gateway, with enough recovery time for separate tickets.
5. Open-jaw itineraries with a train, bus, ferry, or ground segment when appropriate.
6. Multi-city pricing versus separately priced segments.
7. Self-transfers and virtual interlining, including overnight accommodation when required.
8. Cash, award, and portal pricing when the user has access to those currencies or products.

Do not present hidden-city ticketing as a normal recommendation. Mention it only if the user explicitly requests it, and explain baggage, disruption, loyalty-account, and airline-contract risks.

## Compare true total cost

Calculate one all-in total for every finalist:

`fare + taxes + bags + seats + payment/FX fees + positioning + ground transfers + required hotel`

For awards, add cash surcharges and the opportunity cost of the points. For separate tickets, flag that a missed onward flight may require buying a replacement ticket. Price the full party together because low fare inventory may not cover every traveler.

## Verify finalists

1. Recheck the best candidates on a live bookable source immediately before recommending them.
2. Confirm airports, local dates, connection times, baggage rules, fare class, change rules, and whether connections are protected.
3. Treat cached award or metasearch results as leads until confirmed on the booking program or airline.
4. Never transfer points before live availability is confirmed; mention that transfers are usually irreversible.

## Present the result

Show a compact table sorted by all-in cost with:

- exact flights and local times;
- construction type;
- fare or points plus cash;
- all-in total for all travelers;
- baggage assumptions;
- protection status;
- booking source;
- material risks.

Then state:

1. Cheapest practical option.
2. Absolute cheapest option, if different, with its tradeoffs.
3. Best protected itinerary.
4. Round trip versus one-way-pair price delta.
5. Sources checked and coverage gaps.

Do not book, transfer points, purchase positioning travel, or make any other external commitment without explicit user authorization.
