# CLI Reference

```
 Usage: show-file-tree [OPTIONS] [ROOT_PATH] COMMAND [ARGS]...

 A small, fast CLI tool to display styled file/folder trees.


╭─ Arguments ──────────────────────────────────────────────────────────────────────────────────────────────────────────╮
│   root_path      [ROOT_PATH]  The root directory to start the tree from.                                             │
│                               [default: .]                                                                           │
╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
│ --help          Show this message and exit.                                                                          │
╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
╭─ Tree Structure ─────────────────────────────────────────────────────────────────────────────────────────────────────╮
│ --max-depth  -d                    INTEGER  Maximum recursion depth.                                                 │
│                                             [default: None]                                                          │
│ --gitignore      --no-gitignore             Respect .gitignore files.                                                │
│                                             [default: gitignore]                                                     │
│ --hidden                                    Show hidden files and directories.                                       │
╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
╭─ Sorting ────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
│ --sort         TEXT  Sort by 'name' or 'size'.                                                                       │
│                      [default: name]                                                                                 │
│ --order        TEXT  Sort order: 'asc' or 'desc'.                                                                    │
│                      [default: asc]                                                                                  │
╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
╭─ Output and Display ─────────────────────────────────────────────────────────────────────────────────────────────────╮
│ --format          TEXT  Output format: 'tree' or 'md'.                                                               │
│                         [default: tree]                                                                              │
│ --size                  Show file/directory sizes.                                                                   │
│ --count                 Show file/directory counts in folders.                                                       │
│ --no-icons              Disable icons in the output.                                                                 │
│ --theme           TEXT  Color theme: colorful, monokai, light, nocolor.                                              │
│                         [default: colorful]                                                                          │
╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
╭─ Filtering ──────────────────────────────────────────────────────────────────────────────────────────────────────────╮
│ --include       -i      TEXT  Include only paths matching this glob pattern.                                         │
│                               [default: None]                                                                        │
│ --exclude       -e      TEXT  Exclude paths matching this glob pattern.                                              │
│                               [default: None]                                                                        │
│ --mtime-after           TEXT  Filter by modification time after this date (YYYY-MM-DD).                              │
│                               [default: None]                                                                        │
│ --mtime-before          TEXT  Filter by modification time before this date (YYYY-MM-DD).                             │
│                               [default: None]                                                                        │
│ --ctime-after           TEXT  Filter by creation time after this date (YYYY-MM-DD).                                  │
│                               [default: None]                                                                        │
│ --ctime-before          TEXT  Filter by creation time before this date (YYYY-MM-DD).                                 │
│                               [default: None]                                                                        │
╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
╭─ General ────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
│ --version          Show version and exit.                                                                            │
│ --about            Show information about the package.                                                               │
╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────────────────────────╮
│ note   Manage notes for files and directories.                                                                       │
╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯

```