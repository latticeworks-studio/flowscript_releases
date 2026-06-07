# FlowBar Commands

The FlowBar is the command input at the bottom of the canvas. Press **Enter** to run a command, **Escape** to dismiss it. Use the **up arrow** to recall your last command.

Commands that take a node name support autocomplete — type the command and an opening `(` to see matching node names. Use **arrow keys** or **Tab** to pick a suggestion, **Enter** to confirm.

---

## Node Commands

### `addNode(name)`

Creates a new action node at the center of the canvas with the given name.

```
addNode(parse result)
```

---

### `renameNode(name): newName`

Renames an existing node. The colon separates the current name from the new one.

```
renameNode(old name): new name
```

> Autocomplete triggers after `(` and populates the current name. After selecting, type `: ` followed by the new name.

---

### `deleteNode(name)`

Deletes the named node and all its connected edges.

```
deleteNode(unused node)
```

---

### `copyNode(name)`

Duplicates the named node. The copy appears offset from the original and is automatically selected.

```
copyNode(my node)
```

---

### `babyNode(name)`

Creates a new node that starts tiny and grows to full size over 2 seconds. Same as `addNode` but with a spawn animation.

```
babyNode(sneaky node)
```

---

### `cookNode(name)`

Easter egg. "Cooks" the node by darkening its colours until it's almost black. Any interaction with the node restores it.

```
cookNode(that node)
```

---

## Pin Commands

### `addPins(name): count`

Adds input and output pins to a node. Pass the number of pin pairs to add.

```
addPins(my node): 2
```

---

### `changeType(name): type`

Changes the visual type of a node. Valid types: `action`, `condition`, `data`, `event`, `group`.

```
changeType(my node): condition
```

---

## Canvas Commands

### `zoom(all)` or `zoom(node name)`

Fits all nodes in view, or zooms to a specific named node.

```
zoom(all)
zoom(parse result)
```

---

### `addShape(box)` or `addShape(circle)`

Adds a resizable shape to the canvas at the center. Shapes are decorative — they have no pins. You can also right-click on empty canvas to add a shape at that position.

```
addShape(box)
addShape(circle)
```

---

## Node Properties

### `addProperty(name)`

Adds a property to the currently open nested node. Properties appear as interactive controls (checkbox, slider, dropdown) in the node body.

Only available when you are inside a node (nested view).

```
addProperty(speed)
```

---

## File & Template Commands

### `saveTemplate(node name)`

Saves the named node (and everything inside it) as a reusable template. Templates appear in a palette and can be placed on any canvas.

```
saveTemplate(my component)
```

---

## Theme Commands

### `newTheme(name)`

Opens the Theme Creator pre-filled with the given name. Design your colours, then save. If a theme with that name already exists you will be prompted to overwrite or rename.

```
newTheme(midnight)
```

---

## UI Commands

### `showHelp`

Opens the Commands & Shortcuts panel.

```
showHelp
```
