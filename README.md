# FlightTracker Codex Setup

A small Codex plugin that packages a safe workflow for reviewing travel-related Gmail threads and preparing reply drafts.

The plugin does not contain Gmail credentials, messages, reservations, traveler information, or other private project data. Each user must install and authorize their own Gmail connector.

## Install

1. Add this repository as a Codex plugin marketplace:

   ```bash
   codex plugin marketplace add crorella/flighttracker-codex-setup
   ```

2. Restart the ChatGPT desktop app.
3. Open **Plugins**, select **FlightTracker Codex Setup**, and install **FlightTracker Workflows**.
4. Install and authorize the Gmail plugin for the account you want Codex to use.
5. Open a new task and try:

   ```text
   Use $manage-travel-email to find the current reservation thread and prepare a reply draft. Do not send it.
   ```

## What it does

- Finds and reads the live email thread before relying on itinerary details.
- Preserves the language of the conversation unless asked to change it.
- Updates an existing reply draft when possible.
- Creates drafts without sending them.
- Requires explicit authorization before sending, forwarding, canceling, booking, or changing a reservation.
- Avoids reusing unverified details from earlier trips.

## Repository layout

```text
.agents/plugins/marketplace.json
plugins/flighttracker-workflows/.codex-plugin/plugin.json
plugins/flighttracker-workflows/skills/manage-travel-email/SKILL.md
```

## Development checks

Run the skill and plugin validators before publishing changes:

```bash
python3 /path/to/skill-creator/scripts/quick_validate.py \
  plugins/flighttracker-workflows/skills/manage-travel-email

python3 /path/to/plugin-creator/scripts/validate_plugin.py \
  plugins/flighttracker-workflows
```

## Privacy

Do not add Gmail exports, browser recordings, screenshots, PDFs, itinerary reports, connector tokens, Codex session data, or personal memory files to this repository.

## License

MIT
