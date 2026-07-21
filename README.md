# FlightTracker Codex Setup

A Codex plugin for finding the cheapest practical combinations of flights across cash fares, awards, flexible dates, nearby airports, and creative ticket constructions.

The plugin contains no credentials, traveler information, booking records, or proprietary fare data. Search tools and paid data sources must be configured separately by each user.

## Install

1. Add this repository as a Codex plugin marketplace:

   ```bash
   codex plugin marketplace add crorella/flighttracker-codex-setup
   ```

2. Restart the ChatGPT desktop app.
3. Open **Plugins**, select **FlightTracker Codex Setup**, and install **FlightTracker Workflows**.
4. Open a new task and try:

   ```text
   Use $find-cheapest-flights to find the cheapest practical combinations from SFO to Madrid. Compare flexible dates and nearby airports.
   ```

## What it compares

- Published round trips versus two independently priced one-ways.
- Mixed carriers for outbound and return flights.
- Flexible travel dates and nearby airports.
- Positioning flights, open jaws, and multi-city pricing.
- Protected connections versus self-transfers and virtual interlining.
- Cash fares, award availability, and portal pricing when available.
- True all-in cost, including bags, seats, ground transfers, foreign-exchange fees, positioning, and required hotels.

The skill reports which sources succeeded or failed and rechecks finalists on a live booking source. It cannot guarantee a global minimum because fares and inventory change continuously.

## Repository layout

```text
.agents/plugins/marketplace.json
plugins/flighttracker-workflows/.codex-plugin/plugin.json
plugins/flighttracker-workflows/skills/find-cheapest-flights/SKILL.md
```

## Development checks

Run the skill and plugin validators before publishing changes:

```bash
python3 /path/to/skill-creator/scripts/quick_validate.py \
  plugins/flighttracker-workflows/skills/find-cheapest-flights

python3 /path/to/plugin-creator/scripts/validate_plugin.py \
  plugins/flighttracker-workflows
```

## Privacy

Do not add browser recordings, screenshots, PDFs, itinerary reports, account credentials, connector tokens, Codex session data, or personal memory files to this repository.

## License

MIT
