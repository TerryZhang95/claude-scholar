# Comparison / Motivation Figure

Load this module for figures that frame the problem, contrast prior work with the proposed idea, or visually motivate the method.

## Purpose

This figure should help the reader understand:
- what is wrong with prior approaches
- what gap or bottleneck motivates the paper
- how the proposed method changes the picture

It is argumentative. It should make the paper's necessity obvious.

## Best Fit

Use this module when the figure appears:
- in the Introduction
- before the method is fully introduced
- as "prior work vs ours"
- as a bottleneck / pain-point / intuition figure

## Design Priorities

1. Make the contrast immediate.
2. Reduce text and let layout carry the argument.
3. Highlight one decisive difference.
4. Keep the "ours" side visually stronger but not cartoonish.

## Recommended Layouts

- left: prior work, right: ours
- top: problem setting, bottom: proposed remedy
- three columns: challenge, limitation, proposed fix

## Visual Strategy

- use mirrored layout where possible
- keep comparable elements aligned across sides
- use one accent highlight only for the proposed idea or key bottleneck
- use callouts sparingly to label the actual point of difference

## What to Include

- the comparison baseline at the right abstraction level
- one or two failure points of the old approach
- one crisp depiction of the new mechanism or benefit

## What to Exclude

- a full method architecture
- too many baselines in one figure
- rhetorical claims that are not visually grounded

## Tool Guidance

- Default to **Python-generated SVG composition with imported assets**.
- Keep the editable SVG as the source artifact and export a PDF for the paper.

## Common Failure Modes

- prior work side is a straw man and loses credibility
- too much text makes the figure feel like a slide
- the comparison lacks a single explicit axis of difference
- the figure duplicates the abstract instead of clarifying the problem

## Review Questions

- Is the contrast understandable in under ten seconds?
- Does the figure motivate the paper without overselling?
- Would removing one panel make the comparison cleaner?
