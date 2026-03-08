# PDayMinder

A QoL (Quality of Life) and medication tracker with a mobile-friendly dark UI.

## Features

- Track daily QoL across customizable time segments
- Log medications with dosage and timing
- Mini calendar view with color-coded day summaries
- CSV export/import of tracked data
- Data persists via Express.js backend (JSON file storage)

## Running Locally

```bash
npm install
npm start
# Open http://localhost:3000
```

The frontend is a single-page React app (via CDN, no build step). The Express server handles data persistence and serves the static frontend.

## API

- `GET /api/pdayminder/data` — retrieve all settings and day entries
- `POST /api/pdayminder/data` — upsert settings and/or day entries (merges with existing data)
