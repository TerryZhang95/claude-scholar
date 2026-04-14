# Python and SVG Workflow

Load this module by default. It defines the standard workflow for structural figures.

## Default Position

Assume a **Python-first workflow** for all figure types in this skill.

The standard output pair is:
- an **editable SVG** as the source artifact
- a **PDF** exported from that SVG for paper integration

## Why This Is the Default

- low token overhead compared with GUI workflows
- reproducible and version-control friendly
- easy for an agent to generate and revise
- suitable for structured diagrams, topology, and asset composition
- keeps the editable source in a portable vector format

## Core Stack

Use the simplest stack that satisfies the figure:

1. **Python script**
   Defines positions, repeated structures, labels, connectors, and layout rules.

2. **Editable SVG**
   Stores the figure in a tool-agnostic vector format.

3. **PDF export**
   Provides the paper-ready artifact for LaTeX inclusion.

4. **External SVG assets**
   Optional, only when icons or silhouettes improve recognition.

## Operating Principle

Separate the figure into layers:
- **structure**: boxes, arrows, panels, regions, labels
- **assets**: imported SVG icons or silhouettes
- **export**: SVG for editing, PDF for inclusion

Build structure first. Add assets second. Finalize caption and export last.

## Suggested Workflow

1. Write a compact figure specification.
2. Decide the layout logic in Python.
3. Generate or assemble the editable SVG.
4. Add only the assets that materially improve recognition.
5. Export PDF from the SVG.
6. Draft the caption after the figure structure stabilizes.

## Output Standard

Every finalized figure should have:
- one editable SVG source
- one exported PDF

Optional:
- PNG preview for quick inspection

## Review Questions

- Is the SVG still clean and editable after generation?
- Does the Python script capture the layout logic rather than hard-coding every minor tweak?
- Can the same script be revised quickly after paper feedback?
