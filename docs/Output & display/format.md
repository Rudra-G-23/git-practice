# --format

The `--format` flag lets you **choose how the tree is displayed or exported**.

- `tree` (default) — Display the tree in the terminal with optional icons, counts, and sizes.
- `md` — Export the tree to a **Markdown file** for documentation purposes.

---

## Usage

### Terminal tree (default)
```
show-file-tree .
```

### Export to Markdown

```
show-file-tree --format md /path/to/project 
```

This creates a file named `<rootname>-file-tree.md` in your current directory.

---

## Example

### Terminal output (`--format tree`)

```
├── 📁 docs
│   └── readme.md
├── 📁 src
│   └── main.py
└── LICENSE
```

### Markdown export (`--format md`)

```
# Project Tree

- docs/
  - readme.md
- src/
  - main.py
- LICENSE
```

---

## Tip

Combine `--format md` with other flags like `--size` or `--count` to generate **rich, documented project trees**.
