# pen

A minimalist terminal text editor with live Python syntax highlighting, built
on the [`ascii_colors`](https://pypi.org/project/ascii_colors/) TUI framework.

## Install

```bash
pip install ascii-pen
```

Or, from a checkout of this directory:

```bash
pip install -e .
```

## Usage

```bash
pen                     # start with the welcome sample
pen path/to/file.py     # open an existing file, or create a new one
```

## Controls

| Key                               | Action                                    |
| --------------------------------- | ----------------------------------------- |
| Arrow keys, Home, End, PgUp, PgDn | Move the cursor                           |
| Enter, Backspace, Delete          | Edit                                      |
| Ctrl+S                            | Save (prompts for a path if untitled)     |
| Ctrl+O                            | Open another file                         |
| Ctrl+Q                            | Quit                                      |

## Features

- Live Python syntax highlighting (keywords, strings, numbers, comments,
  builtins).
- Line-number gutter with the current line highlighted.
- Vertical and horizontal scrolling driven by the cursor.
- Wide-character aware rendering.
- Modal file dialogs (Save As / Open) built on `App.push_modal`.

## License

MIT