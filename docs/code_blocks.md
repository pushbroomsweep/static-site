---
title: Code Blocks
description: This is the YAML metadata header block
date: 2023-03-25
---

# Code Blocks

This page provides details about the different admonition blocks used in MkDocs material.

## Copy button in code blocks

A copy button can be added to all code blocks by including the following to `mkdocs.yml`.

```yaml title="mkdocs.yml"
theme:
  features:
    - content.code.copy
```

It can also be enabled for specific code blocks by using the syntax shown in the Raw Markdown tab. Note that the language identifier is also inside the brackets and preceded by a `.`.

=== "Raw Markdown"
    ````markdown
    ``` { .python .copy }
    # This is a code block with a copy button
    a = 5
    ```
    ````

=== "Output"
    ``` { .python .copy }
    # This is a code block with a copy button
    a = 5
    ```

It can also be disabled for specific code blocks by using the syntax shown in the Raw Markdown tab. Note again that the language identifier is also inside the brackets and preceded by a `.`.

=== "Raw Markdown"
    ````markdown
    ``` { .python .no-copy }
    # This is a code block without a copy button
    a = 5
    ```
    ````

=== "Output"
    ``` { .python .no-copy }
    # This is a code block without a copy button
    a = 5
    ```

## Code annotations

Code annotations can be added to comments in code blocks. The annotations follow straight after the code block.

=== "Raw Markdown"
    ````markdown
        ```python
        # comment (1)
        print("Hello")
        # (2)
        print("World")
        # (3)!
        ```

        1.  :man_raising_hand: I'm an annotation!
        2.  This is another annotation!
        3.  Adding a ! strips the comment in the line.
    ````

=== "Output"
    ```python
    # comment (1)
    print("Hello")
    # (2)
    print("World")
    # (3)!
    ```

    1.  :man_raising_hand: I'm an annotation!
    2.  This is another annotation!
    3.  Adding a ! strips the comment in the line.
    ```


Code annotations can also be placed inside admonition blocks. 

!!! note
    === "Raw Markdown"
        ````markdown
            ```python
            # comment (1)
            print("Hello")
            # (2)
            print("World")
            # (3)!
            ```

            1.  :man_raising_hand: I'm an annotation!
            2.  This is another annotation!
            3.  Adding a ! strips the comment in the line.
        ````

    === "Output"
        ```python
        # comment (1)
        print("Hello")
        # (2)
        print("World")
        # (3)!
        ```

        1.  :man_raising_hand: I'm an annotation!
        2.  This is another annotation!
        3.  Adding a ! strips the comment in the line.
        ```

## Code block title

A title can be added to code blocks by adding `title=<title>` after the language identifier.

=== "Raw Markdown"
    ````markdown
        ```python title="hello_world.py"
        print("Hello World")
        ```
    ````

=== "Output"
    ```python title="hello_world.py"
    print("Hello World")
    ```

## Line Numbers

Line numbers can be added to code blocks by adding `linenums="<start>"` after the language identifier.

=== "Raw Markdown"
    ````markdown
        ```python linenums="1"
        a = 1
        b = 2
        c = 3
        print(a+b+c)
        ```
    ````

=== "Output"
    ```python linenums="1"
    a = 1
    b = 2
    c = 3
    print(a+b+c)
    ```

Line numbers can also start from a number other than 1.

=== "Raw Markdown"
    ````markdown
        ```python linenums="6"
        a = 1
        b = 2
        c = 3
        print(a+b+c)
        ```
    ````

=== "Output"
    ```python linenums="6"
    a = 1
    b = 2
    c = 3
    print(a+b+c)
    ```


## Highlight specific lines
Line highlights can be added to code blocks by adding `hl_lines = "n1 n2 n3 ..."` after the language identifier. Line count starts at 1 regardless of the starting line number specified in `linenums`.

=== "Raw Markdown"
    ````markdown
    ```python hl_lines="1 2 4"
    a = 1
    b = 2
    c = 3
    print(a+b+c)
    ```
    ````

=== "Output"
    ```python hl_lines="1 2 4"
    a = 1
    b = 2
    c = 3
    print(a+b+c)
    ```


## Syntax highlighting inline code blocks

Inline codeblocks (with single backticks) can be syntax highlighted by prefixing them with a shebang `#!` directly followed by the corresponding language identifier.

=== "Raw Markdown"
    ````markdown
        Compare the difference between `#!py print("Hello World")` and `print("Hello World")`.
    ````

=== "Output"
    Compare the difference between `#!py print("Hello World")` and `print("Hello World")`.


## Tabbed code blocks

Tabbed code blocks are created by using `===` followed by the tab header followed by indented code blocks.

=== "Raw Markdown"
    ```markdown
    === "C"

        ```c
        #include <stdio.h>

        int main(void) {
          printf("Hello world!\n");
          return 0;
        }
        ```

    === "Python"

        ```python
        print("Hello world!")
        ```
    ```

=== "Output"
    === "C"

        ```c
        #include <stdio.h>

        int main(void) {
          printf("Hello world!\n");
          return 0;
        }
        ```

    === "Python"

        ```python
        print("Hello world!")
        ```

