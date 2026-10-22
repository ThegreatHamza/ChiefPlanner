# ChiefPlanner

ChiefPlanner is a browser-based construction scheduling prototype. It runs without a backend and stores projects in the current browser.

## Run locally
1. Download or clone this repository.
2. Open `index.html` in a modern browser. If your browser restricts local files, run a local static server (for example, `python -m http.server 8000`) and open `http://localhost:8000`.
3. Choose **Load sample** to explore the schedule, or add your own tasks.
4. Export JSON regularly to keep a portable backup.

## Features
- English and French interface
- Task register: add, edit, search, filter, and delete tasks
- Task types: tasks and milestones
- FS, SS, FF, and SF dependency relationships with working-day lag/lead
- CPM schedule calculations and critical-task indicators
- Gantt overview
- Browser-local persistence, undo/redo, JSON import/export
- Responsive layout and ChiefPlanner logo

## Deployment
This is a static website. On GitHub, open **Settings → Pages**, choose the `main` branch and `/(root)`, then save. The published site will be available at the URL GitHub Pages displays.

## Important limitations
- Data is stored per browser/device; it does not sync across devices.
- Exported JSON is the portable backup format.
- This is a planning aid, not a replacement for a reviewed contractual baseline. Validate dates, calendars, dependencies, and critical-path results before using a schedule for construction commitments.
- Test in a modern browser after changing scheduling logic. No live browser/CI execution is claimed by this README.
