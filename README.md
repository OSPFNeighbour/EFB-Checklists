# iPad Touch-Friendly Aircraft Checklist

This project provides a self-contained, offline-capable, touch-optimized checklist application for iPad or tablet use. It is designed to support structured aviation checklists, such as pre-flight and engine run-up procedures, with per-item persistence and section navigation.

Designed for and tested with OzRunway. When connected with Dropbox you can keep the lists folder in sync, no internet is required once the list is downloaded within OzRunway.

## Features

- ✅ Touch-friendly UI with large checklist items and tick indicators
- ✅ Grouped sections with subheadings
- ✅ Persistent checklist state saved in `localStorage` (per file)
- ✅ Reset button to clear progress and scroll to top
- ✅ "Contents" section at the top with links to each group
- ✅ Designed for full-screen use on iPad (Add to Home Screen)

## File Structure

Each checklist lives in a separate `.html` file (e.g. `preflight.html`, `runup.html`). Checklist data is embedded as a JavaScript array of groups and items.

## Customizing a Checklist

Edit the `checklistData` array in the script section:

```js
const checklistData = [
  {
    group: "Pre-Start",
    items: [
      { title: "Fuel Shut-off Valve", desc: "ON" },
      { title: "Mixture", desc: "FULL RICH" }
    ]
  },
  ...
];
