---
title: Formatting
description: This is the YAML metadata header block
date: 2023-03-25
---

# Formatting

## Highlighting changes

=== "Raw Markdown"
    ````markdown 
    Text can be {--deleted--} and replacement text {++added++}. This can also be
    combined into {~~one~>a single~~} operation. {==Highlighting==} is also
    possible {>>and comments can be added inline<<}.

    {==

    Formatting can also be applied to blocks by putting the opening and closing
    tags on separate lines and adding new lines between the tags and the content.

    ==}
    ````

=== "Output"
    Text can be {--deleted--} and replacement text {++added++}. This can also be
    combined into {~~one~>a single~~} operation. {==Highlighting==} is also
    possible {>>and comments can be added inline<<}.

    {==

    Formatting can also be applied to blocks by putting the opening and closing
    tags on separate lines and adding new lines between the tags and the content.

    ==}

## Highlighting text

=== "Raw Markdown"
    ````markdown
    - ==This was highlighted==
    - ^^This was inserted^^
    - ~~This was deleted~~
    ````

=== "Output"
    - ==This was highlighted==
    - ^^This was inserted^^
    - ~~This was deleted~~

## Subscripts and superscripts

Subscripts can be created using tilde (`~`) and superscripts can be created using caret (`^`).

=== "Raw Markdown"
    ````markdown
    - H~2~O
    - A^T^A
    ````

=== "Output"
    - H~2~O
    - A^T^A

## Displaying keyboard keys

Keyboard keys can be displayed between two `++`s. See <https://facelessuser.github.io/pymdown-extensions/extensions/keys/> for more about keys.

=== "Raw Markdown"
    ````markdown
    - ++ctrl+alt+del++
    - ++ctrl+shift+p++
    ````

=== "Output"
    - ++ctrl+alt+del++
    - ++ctrl+shift+p++

## Emojis

=== "Raw Markdown"
    ````markdown
    :smile:
    ````

=== "Output"
    😄

## Images

### Center alignment 

Images can be center aligned with HTML using the `figure` and `figcaption` tags.

=== "Raw Markdown"
    ````markdown
    <figure markdown>
        ![Image title](https://dummyimage.com/600x400/){ width="300" }
        <figcaption>Image caption</figcaption>
    </figure>
    ````

=== "Output"
    <figure markdown>
        ![Image title](https://dummyimage.com/600x400/){ width="300" }
        <figcaption>Image caption</figcaption>
    </figure>

### Light and Dark mode toggles

Light and dark mode images can be toggled by appending a `#only-light` or `#only-dark` hash fragment to the image URL

=== "Raw Markdown"
    ````markdown
    <figure markdown>
        ![Image title](https://dummyimage.com/600x400/f5f5f5/aaaaaa#only-light)
        ![Image title](https://dummyimage.com/600x400/21222c/d5d7e2#only-dark)
        <figcaption>Light and Dark mode toggle</figcaption>
    </figure>
    ````

=== "Output"
    <figure markdown>
        ![Image title](https://dummyimage.com/600x400/f5f5f5/aaaaaa#only-light)
        ![Image title](https://dummyimage.com/600x400/21222c/d5d7e2#only-dark)
        <figcaption>Light and Dark mode toggle</figcaption>
    </figure>

## Lists

### Definition lists

Definition lists (or description lists) can be created as follows:

=== "Raw Markdown"
    ````markdown
    `Item 1`
    :   Description of Item 1

    `Item 2`
    :   Description of Item 2
    ````

=== "Output"
    `Item 1`
    :   Description of Item 1

    `Item 2`
    :   Description of Item 2

### Task lists

Unordered list items can be prefixed with [ ] to render an unchecked checkbox or [x] to render a checked checkbox.

=== "Raw Markdown"
    ````markdown
    - [x] Lorem ipsum dolor sit amet, consectetur adipiscing elit
    - [ ] Vestibulum convallis sit amet nisi a tincidunt
        * [x] In hac habitasse platea dictumst
        * [x] In scelerisque nibh non dolor mollis congue sed et metus
        * [ ] Praesent sed risus massa
    - [ ] Aenean pretium efficitur erat, donec pharetra, ligula non scelerisque
    ````

=== "Output"
    - [x] Lorem ipsum dolor sit amet, consectetur adipiscing elit
    - [ ] Vestibulum convallis sit amet nisi a tincidunt
        * [x] In hac habitasse platea dictumst
        * [x] In scelerisque nibh non dolor mollis congue sed et metus
        * [ ] Praesent sed risus massa
    - [ ] Aenean pretium efficitur erat, donec pharetra, ligula non scelerisque

## Equations

### Inline equations

Inline equation blocks are created between `$` (same as latex)

=== "Raw Markdown"
    ````markdown
    $x^2 + y^2 = z^2$
    ````

=== "Output"
    $x^2 + y^2 = z^2$

### Equation blocks

Standalone equation blocks are created between `$$` (same as latex).

=== "Raw Markdown"
    ````markdown
    $$\frac{a}{b} = \frac{c}{d}$$
    ````

=== "Output"
    $$\frac{a}{b} = \frac{c}{d}$$

## Abbreviations

Abbreviations can be created with `*` immediately followed by the term or acronym to be associated in square brackets.

=== "Raw Markdown"
    ````markdown
    The HTML specification is maintained by the W3C.

    *[HTML]: Hyper Text Markup Language
    *[W3C]: World Wide Web Consortium
    ````

=== "Output"
    The HTML specification is maintained by the W3C.

    *[HTML]: Hyper Text Markup Language
    *[W3C]: World Wide Web Consortium


