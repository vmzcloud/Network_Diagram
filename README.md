# Network Diagram

Browser-based editor for drawing network topology diagrams. Single HTML file, no dependencies or build step.

## Features

- Device palette: Server, Cloud, PC, Router, Switch, Load Balancer, Firewall, Textbox, Table, Frame
- Drag-and-drop from the palette onto the canvas, or click-to-place
- Connect devices; style links as solid/dotted with optional arrows
- Colored Frame zones that auto-fit around devices inside them
- Table object with flexible rows and columns
- Pan and zoom the canvas (wheel, middle-drag, Space+drag, header controls)
- Multi-select with Shift / Cmd / Ctrl
- Properties panel for labels, descriptions, frame color, table cells, link style
- Save / load diagrams as JSON
- Export as PNG or PDF

## Quick start

Open `Network_Diagram.html` in a modern browser.

```bash
# Windows
start Network_Diagram.html

# macOS
open Network_Diagram.html
```

Or serve it locally if your browser restricts file access:

```bash
python3 -m http.server 8080
# then visit http://localhost:8080/Network_Diagram.html
```

## Usage

1. Drag a device from the left palette onto the canvas, or click a palette item then click the canvas.
2. **Table**: when placing, enter size as `rows x cols` (e.g. `3x4`). Edit cells in the properties panel (semicolon-separated, e.g. `A1;B1`).
3. Use **Connect** and click two devices to link them. Select a link to set solid/dotted style and arrows.
4. Place a **Frame** to group devices; pick a color in the properties panel.
5. **Pan**: middle-mouse drag, Space+drag, or drag empty canvas. **Zoom**: mouse wheel or header +/−.
6. **Save JSON** / **Load JSON** to persist diagrams (includes view and styles).
7. **Export PNG** or **Export PDF** for sharing.

**Shortcuts:** Delete / Backspace removes the selection · Escape clears selection · Ctrl/Cmd + / − / 0 zoom

## Project structure

```
.
├── Network_Diagram.html   # Full app (UI + logic)
└── README.md
```
