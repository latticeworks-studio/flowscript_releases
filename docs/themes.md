# Themes

FlowScript ships with a set of built-in themes and lets you create your own. The active theme changes the colour of the canvas, nodes, edges, and UI chrome.

---

## Switching Themes

Open **Preferences** (top-right gear icon or **Edit → Preferences**). The **Theme** dropdown lists all built-in and user-created themes. Pick one — the canvas updates immediately.

---

## Creating a Theme

Type `newTheme(name)` in the FlowBar and press Enter. The **Theme Creator** modal opens.

In the Theme Creator you can set colours for:

- **Background** — canvas background
- **Node header** — the coloured bar at the top of each node
- **Node body** — the body area
- **Accent** — pins, edges, highlights
- **Text** — node labels and body text
- **Border** — node outlines

Click any colour swatch to open the **colour picker** — an HSV canvas with a hue bar. You can also paste a hex value directly into the hex field (`Ctrl+V`).

When you are done, type a name and click **Save**. The new theme is applied immediately and appears in the Preferences dropdown.

---

## Editing an Existing Theme

In **Preferences**, select the theme you want to change, then click the **✎** (edit) button next to the Delete button. The Theme Creator opens pre-filled with that theme's colours.

- **Save with the same name** — overwrites the existing theme
- **Change the name before saving** — creates a new theme, leaving the original untouched

---

## Deleting a Theme

In **Preferences**, select the theme and click **Delete**. Built-in themes cannot be deleted.

---

## Built-in Themes

| Theme | Description |
|---|---|
| **Default** | Dark teal and muted pink — the standard FlowScript look |
| **Shard** | Deep purple accent on dark slate |
| **Frame Walker** | Dark blue-grey, applied automatically when a `.frame` file is open |

> The Frame Walker theme is set automatically when you open a `.frame` file and restored when you return to a `.flowscript` file. You do not need to switch it manually.

---

## Tips

- Themes are saved in your local preferences file — they follow the app, not the `.flowscript` file.
- Sharing a theme is not yet supported, but the colours are stored as hex values in your config if you need to copy them manually.
