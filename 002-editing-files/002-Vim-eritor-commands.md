
# 🖥️ Command Line Essentials (Vim/Nano)

This cheat sheet includes essential commands for cursor movement, editing, searching, and working with text in **Vim** or **Nano**.

---

## 📍 Essentials

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `h`            | Move the cursor left (normal mode).                                          |
| `j`            | Move the cursor down (normal mode).                                          |
| `k`            | Move the cursor up (normal mode).                                            |
| `l`            | Move the cursor right (normal mode).                                         |
| `w`            | Move the cursor to the start of the next word.                              |
| `b`            | Move the cursor to the start of the previous word.                          |
| `e`            | Move the cursor to the end of the current word.                             |
| `0`            | Move the cursor to the beginning of the line.                               |
| `$`            | Move the cursor to the end of the line.                                     |
| `^`            | Move the cursor to the first non-blank character of the line.               |

---

## ✂️ Editing Text

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `i`            | Start insert mode at the cursor position.                                   |
| `a`            | Start insert mode after the cursor.                                         |
| `o`            | Insert a new line below the current line and start insert mode.             |
| `Esc` or `Ctrl+[ `| Exit insert mode.                                                       |
| `d`            | Delete the character under the cursor.                                      |
| `dd`           | Delete the current line.                                                    |
| `c`            | Delete the character under the cursor and start insert mode.                |
| `cc`           | Delete the current line and start insert mode.                              |

---

## 🎯 Operators

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `d`            | Deletes from the cursor to the movement location.                           |
| `c`            | Deletes from the cursor to the movement location and starts insert mode.    |
| `y`            | Copies from the cursor to the movement location.                            |
| `>`            | Indents one level.                                                          |
| `<`            | Unindents one level.                                                        |

---

## 📋 Marking Text (Visual Mode)

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `v`            | Start visual mode (select text character by character).                     |
| `V`            | Start linewise visual mode (select full lines).                             |
| `Ctrl+v`       | Start visual block mode (select text block).                                |
| `Esc` or `Ctrl+[ `| Exit visual mode.                                                     |

---

## 📋 Clipboard

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `yy`           | Yank (copy) a line.                                                         |
| `p`            | Paste after the cursor.                                                     |
| `P`            | Paste before the cursor.                                                    |
| `dd`           | Delete (cut) a line.                                                        |
| `x`            | Delete (cut) the current character.                                          |
| `X`            | Delete (cut) the previous character.                                         |

---

## 💾 Exiting

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `:w`           | Write (save) the file, but don’t quit.                                       |
| `:wq`          | Write (save) and quit.                                                      |
| `:q`           | Quit (fails if anything has changed).                                        |
| `:q!`          | Quit and throw away changes.                                                |

---

## 🔍 Search/Replace

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `/pattern`     | Search for the pattern forward.                                              |
| `?pattern`     | Search for the pattern backward.                                             |
| `n`            | Repeat search in the same direction.                                         |
| `N`            | Repeat search in the opposite direction.                                     |
| `:%s/old/new/g`| Replace all occurrences of `old` with `new` throughout the file.             |
| `:%s/old/new/gc`| Replace all occurrences of `old` with `new` with confirmation.             |

---

## ⏪ General

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `u`            | Undo the last action.                                                        |
| `Ctrl+r`       | Redo the last undone action.                                                 |

---

## 🚀 Advanced

### Cursor Movement

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `Ctrl+d`       | Move down half a page.                                                      |
| `Ctrl+u`       | Move up half a page.                                                        |
| `}`            | Go forward by paragraph (next blank line).                                  |
| `{`            | Go backward by paragraph (next blank line).                                 |
| `gg`           | Go to the top of the page.                                                  |
| `G`            | Go to the bottom of the page.                                               |
| `: [num] [enter]`| Go to that line number.                                                     |

---

### Character Search

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `f [char]`     | Move forward to the given character.                                        |
| `F [char]`     | Move backward to the given character.                                       |
| `t [char]`     | Move forward to before the given character.                                 |
| `T [char]`     | Move backward to before the given character.                                |
| `;`            | Repeat the search forward.                                                  |
| `,`            | Repeat the search backward.                                                 |

---

## 🖊️ Editing Text

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `J`            | Join the line below to the current one.                                      |
| `r [char]`     | Replace the character under the cursor with the specified character.         |

---

## 📐 Visual Mode

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `O`            | Move to the other corner of the block.                                      |
| `o`            | Move to the other end of the marked area.                                   |

---

## 📂 File Tabs

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `:e filename`  | Edit a file.                                                                |
| `:tabe`        | Make a new tab.                                                             |
| `gt`           | Go to the next tab.                                                         |
| `gT`           | Go to the previous tab.                                                     |
| `:vsp`         | Vertically split windows.                                                   |

---

## 🔖 Marks

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `m{a-z}`       | Set mark {a-z} at the cursor position.                                      |
| `'{a-z}`       | Move the cursor to the start of the line where the mark was set.            |
| `''`           | Go back to the previous jump location.                                       |

---

## 🏷️ Text Objects

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `di(`          | Delete everything inside the parentheses.                                   |

---

## 🔄 General

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `.`            | Repeat the last command.                                                     |
| `Ctrl+r + 0`   | In insert mode, inserts the last yanked text.                               |
| `gv`           | Reselect the last selected block of text (from visual mode).                |
| `%`            | Jumps between matching parentheses or brackets.                             |

