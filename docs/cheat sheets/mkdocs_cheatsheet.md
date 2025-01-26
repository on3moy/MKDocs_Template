# Mkdocs Cheat Sheet

## Documentation
Mkdocs Documentation  
[mkdocs.org](https://www.mkdocs.org)

Material Documentation  
[mkdocs-materials](https://squidfunk.github.io/mkdocs-material/getting-started/)

Markdown Extensions  
[mkdocs-materials extensions](https://squidfunk.github.io/mkdocs-material/reference/)

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site folder with all other assets automatically.
* `mkdocs -h` - Print help message and exit.

## Project Folder Layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

## Code blocks

??? note Code Block Highlights
	Comes from markdown extentions


```py
import numpy as np
```

```py
import numpy as np
def foo():
    return 'hi'

foo()
```  
## Emojis
🦖🥚🦕

## Blocks with [admonition](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#supported-types)
Classes:
```['note', 'abstract', 'info', 'tip', 'success', 'question', 'warning', 'failure', 'danger', 'bug', 'example', 'quote']```

Expandable e.g.
```
??? danger "This is expandable"
	This is expandable, you can add note, example, and warning types
```

??? danger "This is expandable"
    This is expandable, you can add note, example, and warning types 

!!! note Your Title Here if you want
	 Hey! This is a note admonition type!

!!! abstract Your Title Here if you want
	 Hey! This is a abstract admonition type!

!!! info Your Title Here if you want
	 Hey! This is a info admonition type!

!!! tip Your Title Here if you want
	 Hey! This is a tip admonition type!

!!! success Your Title Here if you want
	 Hey! This is a success admonition type!

!!! question Your Title Here if you want
	 Hey! This is a question admonition type!

!!! warning Your Title Here if you want
	 Hey! This is a warning admonition type!

!!! failure Your Title Here if you want
	 Hey! This is a failure admonition type!

!!! danger Your Title Here if you want
	 Hey! This is a danger admonition type!

!!! bug Your Title Here if you want
	 Hey! This is a bug admonition type!

!!! example Your Title Here if you want
	 Hey! This is a example admonition type!

!!! quote Your Title Here if you want
	 Hey! This is a quote admonition type!

## Tasks  
A Nice Task List  
!!! note Note
	This nice task list is enabled by markdown extensions.  
	[lists](https://squidfunk.github.io/mkdocs-material/reference/lists/)

- [x] Complete  
- [ ] something  
- [ ] empty 