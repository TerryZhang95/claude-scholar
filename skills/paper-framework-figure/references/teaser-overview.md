# Teaser / Overview Figure

Load this module for paper-level overview figures, especially Fig. 1 in the Introduction.

## Purpose

This figure should sell the paper quickly. It gives the reviewer a mental model of:
- the problem
- the method structure
- the core novelty
- the expected outcome

It is not a full methods diagram. It is a compressed visual argument.

## Best Fit

Use this module when the figure appears:
- at the top of page 1
- in the Introduction
- as a high-level overview before technical details

## Design Priorities

1. Show the whole story in one glance.
2. Make the novelty visually explicit.
3. Reduce internal implementation detail.
4. Favor visual hierarchy over exhaustive completeness.

## Recommended Structure

Common layouts:
- problem -> method -> outcome
- input world -> core mechanism -> benefit
- prior limitation vs proposed idea
- three-stage summary with one highlighted central contribution

Typical ingredients:
- one or two input-side elements
- one central method block or conceptual mechanism
- one output or benefit region
- one highlighted novelty callout

## What to Include

- high-level modules only
- icons or illustrations where they improve recognition
- short labels, not paragraph text
- one explicit visual emphasis on the main contribution

## What to Exclude

- tensor dimensions
- minor submodules
- training losses unless central to the claim
- too many arrows crossing the page
- implementation details that belong in the architecture figure

## Tool Guidance

- Default to **Python-generated SVG composition with imported SVG assets**.
- Keep the editable SVG as the source of record and export a PDF for the paper.

## Section Relationship

This module aligns most strongly with:
- Introduction
- abstract-adjacent explanation
- contribution summary

If the figure is really a comparison-driven opening figure, also load `comparison-motivation.md`.

## Review Questions

- Can a reviewer explain the paper after seeing only this figure and caption?
- Is the core novelty visually more salient than the baseline pipeline?
- Would removing one block improve clarity?
- Does the figure still work in grayscale or low-saturation print?
