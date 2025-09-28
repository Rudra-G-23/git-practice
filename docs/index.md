# Hello Data Points 👋

!!! quote "Desorption"
    __A small, fast CLI to display styled file/folder trees — perfect for documenting project structure, exporting to Markdown, or quickly inspecting repos.__

---

[![Show File Tree](https://img.shields.io/badge/show--file--tree-5317eb?logo=github&logoColor=black)](https://github.com/Rudra-G-23/show-file-tree) 
[![Downloads](https://img.shields.io/pypi/dm/show-file-tree.svg)](https://pypi.org/project/show-file-tree/)
[![PyPI](https://img.shields.io/pypi/v/show-file-tree.svg)](https://pypi.org/project/show-file-tree)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE.md)
[![Python versions](https://img.shields.io/pypi/pyversions/show-file-tree.svg)](https://pypi.org/project/show-file-tree/)
[![GitHub Issues](https://img.shields.io/github/issues/Rudra-G-23/show-file-tree)](https://github.com/Rudra-G-23/show-file-tree/issues)
[![GitHub pull requests](https://img.shields.io/github/issues-pr/Rudra-G-23/show-file-tree)](https://github.com/Rudra-G-23/show-file-tree/pulls)
[![Repo Size](https://img.shields.io/github/repo-size/Rudra-G-23/show-file-tree)](https://github.com/Rudra-G-23/show-file-tree)
[![Fast & Lightweight](https://img.shields.io/badge/fast%20%26%20lightweight-✅-brightgreen)](https://github.com/Rudra-G-23/show-file-tree)
[![Made with 💜 Python](https://img.shields.io/badge/Made%20with%20❤️-Python-brightgreen)](https://github.com/Rudra-G-23/show-file-tree)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-blue)](https://github.com/Rudra-G-23/show-file-tree/issues)

---

## Quick links
- **Getting started** — Installation & Quickstart.
- **CLI reference** — Complete flag list and examples.
- **Features** — What the tool can do.
- **Examples** — Real-world usage and exported Markdown.
- **Contributing** — How to contribute, tests, and release notes.
- **Changelog** — Release history.

---

### Install

=== "From PyPI"
    ```py linenums="1" hl_lines="2"
    # From PyPI
    pip install show-file-tree
    ```

=== "From UV"
    ```py linenums="1" hl_lines="2"
    # From UV
    uv pip install show-file-tree
    ```

=== "From Source"
    ```py linenums="1" title="From Source"
    # From source (dev)
    git clone https://github.com/Rudra-G-23/show-file-tree.git

    cd show-file-tree
    python -m venv .venv
    ```

=== "Windows PowerShell"
    ```ps1 linenums="1" title="Windows PowerShell"
    .venv\Scripts\Activate.ps1

    pip install -e ".[all]"
    ```

---
### Basic 


---

``` yaml
theme:
  features:
    - content.code.annotate # (1)
    - end  (2)
    - ldakfjfadfkj laksdfj   # (3)
    - kdlfjalkdf # (4)!
    - this is extra metric #(5)! 

```

1.  :man_raising_hand: I'm a code annotation! I can contain `code`, __formatted
    text__, images, ... basically anything that can be written in Markdown.
2.  check 2
3.  third is working
4.  may also work 
5.  no need of comment  i selcted this 5 options 



---

``` yaml
theme:
  features:
    - content.code.annotate # (1)
```

1.  :man_raising_hand: I'm a code annotation! I can contain `code`, __formatted
    text__, images, ... basically anything that can be written in Markdown.

---
```bash
show-file-tree [OPTIONS] (1) [ROOT_PATH] (2) COMMAND (3) [ARGS]...
```

1.  :man_raising_hand: I'm a code annotation! I can contain `code`, __formatted
    text__, images, ... basically anything that can be written in Markdown.
2.  this is 2nd
3.  dlaskjfdlf



```py linenums="1" title="Fundamental command"
# Print a tree of the current directory:
show-file-tree [OPTIONS] (1) [ROOT_PATH] (2) COMMAND (3) [ARGS]... (1) { .annotate }
```

1. :file: File 
2. Optional File Path
3. All the commands

---

```bash
show-file-tree [OPTIONS] (1) [ROOT_PATH] (2) COMMAND (3) [ARGS]... 
```

# (1) { .annotate: 'The options you want to use, like --size or --count.' }
# (2) { .annotate: 'The root directory to start the file tree from. Default is current directory (.)' }
# (3) { .annotate: 'The specific command or action to perform, e.g., --count or --size' }


--

# Usage — Annotated examples

This page demonstrates how to use **annotations** in Material for MkDocs to explain CLI syntax inline and in code blocks.

## Annotated inline text

Here is an example sentence with an inline marker (1) that opens an annotation.
Lorem ipsum dolor sit amet, (1) consectetur adipiscing elit.
{ .annotate }

1.  :information_source: This is an inline annotation. It can contain `code`, **bold**, lists, images, etc.

---

## Annotated code block (your CLI)

Use a fenced code block and put the annotate class on the outer block. Then list numbered annotations below the block — the numbers in the command become clickable markers.

```bash
show-file-tree [OPTIONS] (1) [ROOT_PATH] (2) COMMAND (3) [ARGS]...
# (1) { .annotate: 'The options you want to use, like --size or --count.' }
# (2) { .annotate: 'The root directory to start the file tree from. Default is current directory (.)' }
# (3) { .annotate: 'The specific command or action to perform, e.g., --count or --size' }

```

---

### Annotated Code Example in Markdown


```bash
show-file-tree [OPTIONS] (1) [ROOT_PATH] (2) COMMAND (3) [ARGS]...

{ .annotate }

1. **[OPTIONS]** → The options you want to use, like `--size` or `--count`.
2. **[ROOT_PATH]** → The root directory to start the file tree from.
   Defaults to current directory `(.)`.
3. **COMMAND** → The specific command or action to perform,
   e.g., `--count` or `--size`.

```



---


---

## File Path

!!! danger "File path miss Match"

    === "Incorrect File Path"
        ```bash
        show-file-tree [ROOT_PATH] COMMAND 
        ```
    === "Examples"
        !!! example "Incorrect File Path Examples"

        === "Example 1"
            ```bash
            show-file-tree . --size
            ```
        === "Example 2"
            ```bash
            show-file-tree "C:\Users\Rudra\Desktop\MLOPs" --count
            ```
        === "Example 3"
            ```bash
            show-file-tree "C:\Users\Rudra\Desktop\MLOPs"  --format md 
            ```

!!! success "File path  Match"

    === "Correct File Path"
        ```bash
         show-file-tree COMMAND [ROOT_PATH]
        ```
---

Markdown tree exported to: C:\Users\Rudra\Desktop\git-practice\git-practice-file-tree.md
---
Limit depth and show sizes & counts:

```
show-file-tree  -d 2 --size --count
```

Export the tree to Markdown (creates `<root>-file-tree.md`):

```
show-file-tree /path/to/project --format md --size
```

---

## Why use `show-file-tree`?

* **Fast, memory-safe traversal** — suitable for large directories.
* **Pretty terminal output** — icons, counts, human-readable sizes.
* **Powerful filtering** — globs, mtime/ctime windows.
* **Markdown export** — create readable project documentation automatically.
* **Themes & ASCII fallback** — works in CI or minimal terminals.

---

## Short CLI reference

```
# structure-related
--max-depth, -d       Maximum recursion depth
--gitignore / --no-gitignore  Respect .gitignore (default: on)
--hidden              Show hidden files
```

```
# sorting
--sort {name,size}
--order {asc,desc}
```

```
# output & display
--format {tree,md}
--size
--count
--no-icons
--theme {colorful,monokai,light,nocolor}
```

```
# filtering
--include, -i <PATTERN>
--exclude, -e <PATTERN>
--mtime-after <YYYY-MM-DD>
--mtime-before <YYYY-MM-DD>
--ctime-after <YYYY-MM-DD>
--ctime-before <YYYY-MM-DD>
```

```
# general
--version
--about
```

For the full reference, see the **CLI reference** page.

---

## Example: generate project documentation

```
# Create a Markdown file documenting your repo root
show-file-tree /home/user/my-project --format md --size --count
# -> my-project-file-tree.md
```

---

## Ready-made next steps

* 🔎 **Read the Getting Started** — installation + first run
* 📚 **Explore Examples** — real outputs and exported Markdown
* 🛠️ **Contribute** — tests, style, feature requests (see CONTRIBUTING.md)

---

## Footer / Contact

- Author: **Rudra Prasad Bhuyan** — [GitHub](https://github.com/Rudra-G-23) 
- License: MIT — see `LICENSE.md` 
- Changelog: `CHANGELOG.md`
