# Quality Checklist

Load this module when reviewing or finalizing a structural figure.

## Design Checks

- elements align to a visible or invisible grid
- spacing is deliberate rather than cramped
- no more colors are used than the figure needs
- font size remains readable in the compiled paper
- visual hierarchy is obvious
- arrow semantics are consistent
- background shading does not compete with foreground content

## Content Checks

- the figure has one clear message
- the figure is understandable without the main text
- the caption explains what matters
- symbols in the figure match the paper
- no title text appears inside the figure
- labels use paper terminology rather than internal project jargon

## Technical Checks

- editable SVG source is present
- structural figure is exported as vector output
- figure width fits the venue template
- the embedded PDF looks sharp after LaTeX compilation
- `\label` and `\ref` are used correctly
- the filename and placement are consistent with the paper layout

## Submission Gate

Before calling the figure done, verify:
- a reviewer can explain the point of the figure in one sentence
- the main contribution is visually more salient than the supporting machinery
- removing one element would not improve clarity
- the figure still works when printed or viewed at reduced size
