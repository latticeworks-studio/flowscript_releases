# Frame Walker Mode

Frame Walker mode is a specialised variant of FlowScript designed for building and planning mech configurations for the game **Frame Walker**. It uses the `.frame` file format and a dedicated set of component nodes.

---

## Opening a .frame File

Use **File → New .frame** to start a blank mech build, or **File → Open** and select an existing `.frame` file. You can also drag and drop a `.frame` file onto the app window.

When a `.frame` file is active:

- The **Frame Walker theme** is applied automatically
- The standard **+ Node** button is replaced by the **Frame Palette**
- The FlowBar is restricted to valid Frame Walker commands only
- The `.frame` badge appears in the title bar

---

## Frame Palette

The Frame Palette replaces the standard node toolbar. It lists all available Frame Walker components, grouped by category, with a search field at the top.

Click any component to add it to the canvas. Use the **toggle button** to collapse or expand category groups.

---

## Component Nodes

Frame Walker components are pre-configured nodes representing physical mech parts. Each has:

- **Fixed node type and name** — set by the component definition, not editable
- **Simulation properties** — efficiency, health, and active state
- **Output rate formula** — `base rate × efficiency × health × active × modifier`
- **Custom pin counts** — many components have specialised input/output configurations

### Categories include:

- Power generation and distribution
- Fuel and coolant systems
- Weapons and hardpoints
- Structural and chassis components
- Sensors and electronics

---

## Hardpoint Nodes

Hardpoint nodes represent weapon mounting points on the mech. They carry extra metadata:

- **Mech Part** — which part of the mech the hardpoint belongs to (torso, arm, leg, etc.)
- **Hardpoint ID** — the specific slot identifier
- **Side selector** — arm hardpoints (Hand, Shoulder, Forearm) show a **Left / Right Arm** selector

This metadata is written into the `.frame` file and read by the Frame Walker game for validation.

---

## Groups in .frame Mode

Group nodes work in `.frame` mode and can be renamed via the FlowBar:

```
renameNode(Group): Engine Bay
```

Double-click a group to enter it and build the sub-system inside.

---

## FlowBar in .frame Mode

The FlowBar is restricted in `.frame` mode. The following commands are **not available**:

- `addNode` — use the Frame Palette instead
- `addProperty` — properties are defined by the component specification
- `addShape` — not available in `.frame` mode
- `changeType` — component types are fixed

The following commands **do work**:

- `renameNode(name): newName` — rename a group node
- `zoom(all)` / `zoom(name)` — navigate the canvas
- `copyNode(name)` — duplicate a component
- `deleteNode(name)` — remove a component
- `showHelp` — open the help panel

---

## Saving .frame Files

Save as normal with **Ctrl+S** or **Ctrl+Shift+S**. The file is saved with the `.frame` extension. Frame Walker reads this file directly — keep the filename and path consistent with what the game expects.

---

## Switching Back to FlowScript

Open or create any `.flowscript` file. The theme and toolbar revert automatically. Your `.frame` file remains open in its own window if you used **File → New Window** to open it separately.
