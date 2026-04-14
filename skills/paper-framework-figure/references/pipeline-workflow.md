# Pipeline / Workflow Figure

Load this module for staged method flows, data-processing pipelines, or train-test workflows.

## Purpose

This figure explains ordered transformation:
- what enters the method
- what happens stage by stage
- what intermediate representations matter
- what comes out

It is stronger on sequence than on internal component detail.

## Best Fit

Use this module when the figure appears:
- at the beginning of Methods
- as a process overview
- for train/test pipelines
- for preprocessing -> model -> output style diagrams

## Design Priorities

1. Preserve reading order.
2. Make stage boundaries obvious.
3. Keep arrow semantics clean.
4. Show only the intermediate states that help understanding.

## Recommended Structure

Typical layouts:
- horizontal 3 to 5 stage pipeline
- top row for inference, bottom row for training signals
- grouped stages with background panels

Recommended stage naming:
- input / preprocessing
- feature extraction or encoding
- reasoning / matching / generation
- output / decision

## Arrow Policy

- solid arrows for main forward path
- dashed arrows for supervision or auxiliary loss
- dotted arrows for optional modules or retrieval paths

Avoid:
- bidirectional arrows unless the relation is genuinely symmetric
- crossing arrows that can be eliminated by layout changes

## Level of Detail

Include:
- major stages
- one or two important intermediate artifacts
- optional training branch if critical

Exclude:
- every low-level operator
- every tensor transform
- repeated identical substeps that can be collapsed into one labeled block

## Tool Guidance

- Default to **Python-generated editable SVG** for structured drafting.
- Export a PDF from the SVG for inclusion in the paper.

## Common Failure Modes

- pipeline becomes an architecture figure with too much internal detail
- stages are visually equal even though one stage is the method's contribution
- arrows encode too many different meanings without a legend or redundancy
- training and inference are mixed without clear separation

## Review Questions

- Can the reader follow the process without reading the section text?
- Is each stage named by function rather than by internal code name?
- Are intermediate labels necessary, or just clutter?
