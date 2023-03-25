---
title: Content Tabs
description: This is the YAML metadata header block
date: 2023-03-25
---

# Content Tabs

## Tabbed blocks

Tabbed blocks are created by using `===` followed by the tab header followed by indented tab content.

=== "Raw Markdown"
    ````markdown 
    === "Unordered list"

        * Sed sagittis eleifend rutrum
        * Donec vitae suscipit est
        * Nulla tempor lobortis orci

    === "Ordered list"

        1. Sed sagittis eleifend rutrum
        2. Donec vitae suscipit est
        3. Nulla tempor lobortis orci
    ````

=== "Output"
    === "Unordered list"

        * Sed sagittis eleifend rutrum
        * Donec vitae suscipit est
        * Nulla tempor lobortis orci

    === "Ordered list"

        1. Sed sagittis eleifend rutrum
        2. Donec vitae suscipit est
        3. Nulla tempor lobortis orci

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
