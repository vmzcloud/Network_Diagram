# Network Diagram

Browser-based editor for drawing network topology diagrams. Single HTML file, no dependencies or build step.

## Features

- Device palette: Server, Cloud, PC, Router, Switch, Load Balancer, Textbox, Flame (zone)
- Place, select, move, and connect devices
- Multi-select with Shift / Cmd / Ctrl
- Flame zones that auto-fit around devices inside them
- Properties panel for labels and descriptions
- Save / load diagrams as JSON
- Export as PNG or PDF

## Quick start

Open `index.html` in a modern browser.

```bash
open index.html
```

Or serve it locally if your browser restricts file access:

```bash
python3 -m http.server 8080
# then visit http://localhost:8080
```

## Usage

1. Click a device in the left palette, then click the canvas to place it.
2. Use **Connect** and click two devices to link them.
3. Select a device to edit its label and description on the right.
4. **Save JSON** / **Load JSON** to persist diagrams.
5. **Export PNG** or **Export PDF** for sharing.

**Shortcuts:** Delete / Backspace removes the selection · Escape clears selection and returns to Select mode.

## Project structure

```
.
├── index.html   # Full app (UI + logic)
└── README.md
```
