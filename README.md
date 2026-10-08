# AppADay 154: Service Hours Log

**Category:** S (Spirituality) | **Claude API:** No | **Shipped:** 2026-10-08

**Live:** https://augustineiacopelli.github.io/appaday-154-service-hours-log/
**Portfolio:** https://augustineiacopelli.github.io/appaday/

Service Hours Log keeps a running record of volunteer and ministry hours across every cause you serve, from church to Scouts to PTA. Log hours in seconds with quick chips, see totals per cause and per year, then print a signable report or export a CSV for your parish, troop, or school service summary.

## Features

The totals strip shows a large grand total for the selected year (or all time) with a tile for each cause carrying both its yearly and all time hours. The entry form defaults to today's local date and the last cause you used, accepts hours in quarter hour steps, and offers 0.5, 1, 2, and 4 hour chips. History lists entries newest first with cause and year filters, a running filtered total, inline editing, two tap delete, and Show more paging after 50 rows.

The report builder filters by cause and by this year, last year, a specific year, or a custom date range. It renders an on screen preview and a print layout with your volunteer name, organization line, a per cause breakdown when reporting on all causes, a totals row, and signature lines for the volunteer and a verifier (name, title, signature, date). The same report copies or downloads as a fully quoted CSV with a Total row.

Settings hold your volunteer name and organization line, plus cause management: add with a duplicate check, rename inline, reorder, archive, and delete only when a cause has no entries. Backup JSON downloads everything; Restore JSON validates the file before a two tap Replace overwrites local data.

## Data

All data stays in this browser under the localStorage key `appaday-154-service-hours` (version 1). The app starts with no causes, so every volunteer sets up their own. On first run the Log Hours card shows a starter panel with one tap suggestions (Church, Scouts, School, PTA, Food Bank, Hospital, Shelter, Youth Sports, Community) and a field for a custom name. Add as many as you like; each shows as added, and Done, start logging closes the panel once at least one exists. The panel also closes on its own after the first entry. The Manage link beside the Cause field jumps to Settings for later changes. Hours are summed in quarter hour units to avoid floating point drift. Back up periodically, since clearing site data erases the log.

## Stack

Single `index.html` with inline CSS and vanilla JavaScript. Google Fonts (Cormorant Garamond and Inter) is the only external dependency. Installs to the home screen as a full screen web app with its own icon.
