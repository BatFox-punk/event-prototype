# MMP Events prototype

Clickable prototype of an **Events** page for the Meetings Management Portal (MMP), covering the P3GP and ISET portals. It is a single static file with no build step and no dependencies: open `index.html` in a browser.

All data is sample data. Names, locations, dates, participant numbers, IT support contacts and survey links are invented for the demo (the survey links point to `example.org`). Exports, Key4Events and the other actions are simulated and only show a confirmation message.

## What it shows

- **Portal header** modelled on the current P3GP portal, with a new **Events** tab between Meetings and TDocs.
- **Events list**: title, dates, city and country (with flag), number of meetings, Registered and Attended participants (face to face and online, with icon tooltips), and status (Upcoming, Ongoing, Ended). Filter by period and search.
- **Event page**:
  - totals for meetings, Registered and Attended participants;
  - add a meeting (create, clone the first one, or link a standalone meeting) and detach a meeting;
  - one **Export** button (all participants per meeting);
  - **Event details**: body family, IT support, satisfaction survey URL, additional event information;
  - **Integration**: choose a provider (Key4Events by default), enter the API key, test and connect, sync, disconnect.
- **Events are locked only once they have ended.** Ongoing and upcoming events stay editable.
- **New**: choose between a standalone meeting, a meeting group and an event group, then fill in the level 1 details.
- **Meetings tab**: the existing meeting list in a more modern layout, with the same filters, expandable rows, row actions and a link to the event each meeting belongs to.
- **Two portals, one back end**: the dark bar at the top switches between the green P3GP front end and the ISET front end. The ISET front end is shown as under construction.

## Run it

Download `index.html` and double-click it. No server is needed.

## Publish it with GitHub Pages

1. Go to **Settings > Pages** in this repository.
2. Under **Build and deployment**, choose **Deploy from a branch**, then the `main` branch and the `/ (root)` folder.
3. Save, and wait a minute or two. The address appears at the top of the Pages settings.

Note: on a free GitHub account, Pages needs a public repository.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole prototype (HTML, CSS and JavaScript) |
| `README.md` | This file |
