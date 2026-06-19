# Essential Vim Commands

> *The most important commands for vim basics*

---

## Modes

-  `i` - enter insert mode from normal mode
-  `v` - enter visual mode
-  `esc` - enter normal mode from insert mode

## Working with files in buffers

In normal mode

- `:e <filename>` - open file in buffer
- `:w` - write (save) file)
- `:bp` - open previous buffer
- `:ls` - list files in current dir

## Copy, Cut & Paste

Using Visual Mode (Highlighting Text)

If you prefer selecting text visually before cutting or copying, use these steps:

1. Position your cursor where you want to start.
2. Press v (character selection), V (entire lines), or Ctrl + v (rectangualar block selection)
3. Move your cursor with the arrow keys or `h`, `j`, `k`, `l` to highlight the text
4. Press 
  - `d` to cut
  - `y` to copy. Move to your target location and press
  - `p` to paste

## Undo / Redo

How to `cmd + z` in vim

### Last Action

In Normal Mode

- `u` - undo
- `^r` - redo last undone action
- `U` - Undo all changes on current line

### Multi-Action Shortcuts

You can prepend a number to execute the command multiple times at once.

- `3u` : Undo the last 3 changes.
- `3 then Ctrl + r` : Redo the last 3 undone changes.

### Time-Travel Command

Vim can also jump back and forth to specific times in your editing history using Command-line mode:

- `:earlier 10m:` - Revert the file to its state from 10 minutes ago.
- `:later 5s:` - Move the file forward to its state from 5 seconds ago.

### Chronicling History (Undo Branches)

Unlike linear editors, Vim uses a branching undo tree so your changes are never truly lost. If you undo an edit, and then type something completely new, you can still access the old timeline:
        
- `g-` : Walk backward through the chronological states of the undo tree.
- `g+` : Walk forward through the chronological states of the undo tree.
— `:undolist` - list of all changes
---
