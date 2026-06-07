# Node Types

Every node in FlowScript has a **type** that controls its colour and the icon shown in the header. Types are visual only — they do not affect how data flows between nodes. Use them to communicate intent at a glance.

---

## Action

The default type. Represents an operation, step, or process.

- **Colour:** teal / muted pink header
- **Icon:** cube outline
- **Use for:** function calls, steps in a sequence, transformations

---

## Condition

Represents a decision or branch point.

- **Colour:** muted green header
- **Icon:** diamond
- **Use for:** if/else logic, gates, filters, validation checks

---

## Data

Represents a value, record, or data structure.

- **Colour:** muted blue header
- **Icon:** layers
- **Use for:** variables, constants, data stores, models

---

## Event

Represents a trigger or signal.

- **Colour:** muted amber/brown header
- **Icon:** bolt
- **Use for:** user input, timers, webhooks, state changes

---

## Group

A container node. Double-click to enter it and build a sub-graph inside. Group nodes expose their inner graph's input and output pins on the outside.

- **Colour:** muted slate header
- **Icon:** grid
- **Use for:** encapsulating a sub-system, reusable logic blocks, organising large graphs

> Groups can be saved as **templates** and reused across files.

---

## Changing a Node's Type

Three ways:

1. Open the **… menu** → **Edit** → change the Type dropdown
2. FlowBar: `changeType(node name): type`
3. The type icon in the node header is shown in the Edit modal

---

## Notes

Notes are a special node type that exist outside the action/condition/data/event system. They have no pins and display free text directly on their body. Use them to annotate your graph.

Add a note with the **+ Note** button in the toolbar.

---

## Shapes

Shapes (box and circle) are decorative canvas elements — they have no type, no pins, and no body. Use them to draw boundaries, group areas visually, or add structure to a large canvas.

Add via right-click on empty canvas, or `addShape(box)` / `addShape(circle)` in FlowBar.
