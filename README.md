# Moodi

A simple browser prototype based on the COMP4045 Moodi brainstorm presentation.

## Run

Download this repository using **Code → Download ZIP**, extract it, then serve the extracted folder with a local web server. For example, from this folder:

```sh
python3 -m http.server 4173
```

Then visit http://localhost:4173. No package installation or build is required.

## Included

- Daily mood and sleep check-ins with browser-local saving.
- Tasks, completion, deletion with undo, and workload hints.
- Calendar export as an .ics file (one-way export, no live sync).
- 25-minute focus and 5-minute break timers.
- One-minute breathing exercise and grounding prompt.
- Mochi companion, daily missions, XP, levels, coins and treats.
- Local Tree Hole journal with deletion and undo.
- Hong Kong support information, linked to Shall We Talk.
- Responsive layout, keyboard focus styles and reduced-motion support.

## Prototype boundaries

No account system, cloud database, shared feed, AI moderation, crisis detection, notifications or live calendar integration. Browser storage is not encrypted and should not be treated as a secure medical record. Check-ins and journal entries are not monitored. Clearing browser data removes saved information. Timer state resets when the page is reloaded; task, check-in, journal and reward state persists on the same browser origin. Sample tasks are clearly identified in the planner.

Support source: https://www.shallwetalk.hk/en/get-help/emergency-helplines/

## Files

`index.html`, `style.css`, `app.js`, `mascot.png`.

## Verification

JavaScript syntax check and HTTP serving passed. Browser checks confirmed check-in persistence and XP, task creation/completion, delete/undo, focus start/pause and guided breathing start. The read-only WebMCP study-plan tool returned expected data and rejected invalid input. Automated standalone browser testing was unavailable because its browser binary was not installed.

This repository contains the app source. GitHub repository storage does not by itself host the app. The localhost address works only while a local server is running on your computer.
