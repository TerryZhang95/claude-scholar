# Architecture Figure

Load this module for model-structure diagrams, component interactions, and multi-branch systems.

## Purpose

This figure explains how the method is built:
- what the major components are
- how they connect
- where sharing, branching, fusion, or feedback occurs

It is stronger on structure than on chronological process.

## Best Fit

Use this module when the figure appears:
- in the model or method subsection
- for encoder-decoder, multi-branch, retrieval-augmented, or modular systems
- when the key question is "how are components organized?"

## Design Priorities

1. Make hierarchy visible.
2. Show which components are primary and which are support modules.
3. Make shared modules and repeated modules easy to recognize.
4. Avoid turning the figure into a literal software block diagram.

## Recommended Structure

Useful patterns:
- central shared encoder feeding multiple branches
- stacked hierarchy for upstream -> core -> downstream modules
- left-right input to output with vertical sub-branches
- grouped modules with enclosing panels for subsystems

## Representation Rules

- Use larger or filled boxes for primary modules.
- Use smaller or lighter boxes for auxiliary modules.
- Use repeated style for repeated structures.
- Mark shared components once instead of duplicating them unless duplication improves readability.

## What to Include

- named components the reader must remember
- fusion points, branch splits, and shared blocks
- key interfaces or artifacts between modules

## What to Exclude

- implementation-level operator chains
- every normalization, activation, or residual block unless central
- dense notation that belongs in equations

## Tool Guidance

- Default to **Python-generated editable SVG** for clean component diagrams.
- Export a PDF from the SVG for paper integration.

## Common Failure Modes

- all boxes have equal emphasis, so the novelty disappears
- repeated modules are redrawn manually and clutter the figure
- branch semantics are unclear
- a process figure and an architecture figure are merged into one overloaded layout

## Review Questions

- Is the novel module visually easier to identify than the standard backbone?
- Are repeated structures abstracted cleanly?
- Would splitting the figure into overview plus architecture improve comprehension?
