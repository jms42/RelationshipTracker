# RelationshipTracker

A single-file HTML app for mapping out relationships between people as a node-and-edge graph. No build step, no dependencies — just open [index.html](index.html) in a browser.

## Usage

1. Open `index.html` in your browser.
2. You start with one node ("You") in the middle of the canvas.
3. **Relationship Types** (sidebar): add a type with a name and color (e.g. "Friend" / blue). These colors are used for the connection lines. Click an existing type's color swatch to change it.
4. **Add Node** (sidebar): create a new person and connect them to one or more existing nodes, picking a relationship type for each connection.
5. Click any node to open the **Edit Node** panel, where you can:
   - Rename the node
   - Change the node's color
   - Add, change, or remove its connections
   - Delete the node (and all its connections)
6. Drag nodes around the canvas to rearrange the graph.
7. The **legend** (bottom-left of the canvas) shows each relationship type's color, and has a checkbox to show/hide the relationship-name text on the lines.
8. Use the `☰` button (top-left of the canvas) to hide/show the sidebar for a larger view of the graph.

## Saving your data

- **Save / Load** (sidebar): stores the graph in the browser's local storage. Persists across reloads in the same browser, but isn't a portable file.
- **Export File / Import File** (sidebar): downloads/uploads the graph as a `relationship-graph.json` file, saved to your browser's default Downloads folder. Use this to back up your graph or move it between browsers/machines.

The graph also auto-loads from local storage on page open, if a previous save exists.
