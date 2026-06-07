# Getting Started with FlowScript

FlowScript is a visual programming tool built around a node canvas. You connect nodes to describe logic, data flow, or system structure — no typing required, unless you want to.

## Creating a File

Launch FlowScript. Use **File → New .flowscript** to start a fresh graph, or **File → Open** to load an existing one. You can also drag and drop a `.flowscript` file directly onto the app window.

Recent files are listed in the Open dialog for quick access.

## Your First Node

Three ways to create a node:

- Click **+ Node** in the top-left toolbar
- Type `addNode(my node name)` in the FlowBar and press Enter
- If the canvas is empty, click the animated bubble in the center

A new node appears on the canvas, selected and ready to move.

## Anatomy of a Node

Each node has:

| Part | Description |
|---|---|
| **Header** | Coloured bar showing the node name and type icon |
| **Input pins** | Square handles on the left — data or flow enters here |
| **Output pins** | Square handles on the right — data or flow leaves here |
| **Body** | Optional content: properties, nested graphs, or notes |
| **… menu** | Per-node options: Edit, Duplicate, Select connections, Delete |

## Connecting Nodes

Click and drag from any pin to another node's pin. The edge snaps when you get close. To drop a connection into empty space — release it there — FlowScript instantly creates a new action node and wires it up.

To delete an edge, select it and press **Del**.

## Navigating the Canvas

| Action | How |
|---|---|
| Pan | Click and drag on empty canvas |
| Zoom | Scroll wheel |
| Fit all nodes | Type `zoom(all)` in FlowBar |
| Jump to a node | Type `zoomNode(name)` in FlowBar |
| Search nodes | Type a partial name in the FlowBar — matching nodes highlight |

The **Minimap** in the bottom-right corner gives a live overview. Click or drag inside it to navigate. Scroll inside it to zoom.

## Saving

- **Ctrl+S** — save in place (prompts for a location the first time)
- **Ctrl+Shift+S** — Save As
- The title bar shows a `*` when there are unsaved changes

## Undo and Redo

- **Ctrl+Z** — undo
- **Ctrl+Y** — redo

Undo history is scoped to the current graph level. Entering a nested node starts a fresh history for that level.

## What's Next

- Learn all [FlowBar commands](flowbar-commands.md) to work faster without touching the mouse
- Explore [node types](node-types.md) to understand what each colour means
- Check [keyboard shortcuts](shortcuts.md) for a quick reference
