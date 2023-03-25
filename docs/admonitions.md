---
title: Admonitions
description: This is the YAML metadata header block
date: 2023-03-25
---

# Admonitions

This page provides details about the different admonition blocks used in Material for MkDocs.

##  Admonition block

Admonition blocks are created using `!!!` followed by the admonition name. Note (`note`) is the default block provided by Material for MkDocs.

=== "Raw Markdown"
    ````markdown
    !!! note
        This is a normal note.  
    ````

=== "Output"
    !!! note
        This is a normal note.  

Other admonition blocks available are `info`, `tip`, `abstract`, `success`, `failure`, `example`, `question`, `warning`,  `danger`, `bug` and `quote`.

## Admonition block with a title

A title can be added as a string after the admonition name.

=== "Raw Markdown"
    ````markdown
    !!! abstract "This is the abstract title"
        This is an abstract with a title.  
    ````

=== "Output"
    !!! abstract "This is the abstract title"
        This is an abstract with a title.  

## Admonition block without a title

An admonition block can be created without a title by adding an empty string after the admonition name.

=== "Raw Markdown"
    ````markdown
    !!! info ""
        This is an info without a title.  
    ````

=== "Output"
    !!! info ""
        This is an info without a title.  

## Collapsible blocks

Closed collapsible blocks are created using `???` instead of `!!!`.

=== "Raw Markdown"
    ````markdown
    ??? tip
        This is a tip as a closed collapsible block.  
        This requires `pymdownx.details` extension.
    ````

=== "Output"
    ??? tip
        This is a tip as a closed collapsible block.  
        This requires `pymdownx.details` extension.

Open collapsible blocks are created using `???+`.

=== "Raw Markdown"
    ````markdown
    ???+ success
        This is a success as an open collapsible block.  
        This requires `pymdownx.details` extension.
    ````

=== "Output"
    ???+ success
        This is a success as an open collapsible block.  
        This requires `pymdownx.details` extension.

## Inline blocks

Inline blocks share space with text. 

They can be aligned to the left by adding `inline` after the admonition name.

=== "Raw Markdown"
    ````markdown
    !!! question inline
        This is a question as a left inline block.  
    This is some content alongside the left inline block. It is written straight after the left inline block. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod nulla. 
    ````

=== "Output"
    !!! question inline
            This is a question as a left inline block.  
    This is some content alongside the left inline block. It is written straight after the left inline block. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod nulla. 

They can be aligned to the right by adding `inline end` after the admonition name.

=== "Raw Markdown"
    ````markdown
    !!! warning inline end
        This is a warning as a right inline block.  
    This is some content alongside the right inline block. It is written straight after the right inline block. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod nulla. 
    ````

=== "Output"
    !!! warning inline end
        This is a warning as a right inline block.  
    This is some content alongside the right inline block. It is written straight after the right inline block. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod nulla. 

## All admonition blocks

### Note

=== "Raw Markdown"
    ````markdown
    !!! note
        This is a note.  
    ````

=== "Output"
    !!! note
        This is a note.  

### Info

=== "Raw Markdown"
    ````markdown
    !!! info
        This is an info.  
    ````

=== "Output"
    !!! info
        This is an info.  

### Tip

=== "Raw Markdown"
    ````markdown
    !!! tip
        This is a tip.  
    ````

=== "Output"
    !!! tip
        This is a tip.  

### Example

=== "Raw Markdown"
    ````markdown
    !!! example
        This is an example.  
    ````

=== "Output"
    !!! example
        This is an example.  

### Question

=== "Raw Markdown"
    ````markdown
    !!! question
        This is a question.  
    ````

=== "Output"
    !!! question
        This is a question.

### Abstract

=== "Raw Markdown"
    ````markdown
    !!! abstract
        This is an abstract.  
    ````

=== "Output"
    !!! abstract
        This is an abstract.  

### Success

=== "Raw Markdown"
    ````markdown
    !!! success
        This is a success.  
    ````

=== "Output"
    !!! success
        This is a success. 

### Failure

=== "Raw Markdown"
    ````markdown
    !!! failure
        This is a failure.  
    ````

=== "Output"
    !!! failure
        This is a failure.

### Warning

=== "Raw Markdown"
    ````markdown
    !!! warning
        This is a warning.  
    ````

=== "Output"
    !!! warning
        This is a warning.

### Danger

=== "Raw Markdown"
    ````markdown
    !!! danger
        This is a danger.  
    ````

=== "Output"
    !!! danger
        This is a danger.

### Bug

=== "Raw Markdown"
    ````markdown
    !!! bug
        This is a bug.  
    ````

=== "Output"
    !!! bug
        This is a bug.

### Quote

=== "Raw Markdown"
    ````markdown
    !!! quote
        This is a quote.  
    ````

=== "Output"
    !!! quote
        This is a quote.

