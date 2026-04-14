# Foundations

Load this file for the shared logic that applies across figure types.

## Why This Figure Matters

Reviewer reading order is often:
- abstract
- introduction
- figures
- maybe the rest

That makes the framework or structural figure one of the first places where the paper either becomes clear or collapses into confusion. Treat it as a communication primitive, not decoration.

## Universal Design Rules

1. Caption must be self-contained.
2. Do not place a title inside the figure.
3. One figure should carry one main takeaway.
4. Use left-to-right or top-to-bottom flow unless the task is inherently geometric.
5. Keep structural figures in editable SVG and export companion PDF for the paper.
6. Never rely on color alone; use labels, shape, or line style as backup.
7. Keep figure text at or above readable print size; 8 pt is the lower bound.
8. Keep stroke weight and arrowhead style consistent.

## Layout Principles

- Align to an invisible grid.
- Preserve whitespace; cramped figures read as low quality.
- Use grouping panels or dashed enclosures for module membership.
- Show hierarchy through size, fill, line weight, and placement.
- Use one arrow style per semantic role.

Recommended arrow semantics:
- solid: main data or signal flow
- dashed: supervision, control, or auxiliary relation
- dotted: optional path or conditional branch

## Color Policy

### ML / AI Venues

Muted colors work better than saturated presentation-slide colors.

Recommended palette:
- fill: `#EBF3FB`, `#FEF3E2`, `#E8F8E8`
- border: `#2E86C1`, `#D68910`, `#1E8449`
- arrow: `#2C3E50` or `#555555`
- highlight: `#FDEDEC`
- text: `#1A1A1A`

### IEEE Venues

Prefer grayscale or two-tone styling with one restrained accent.

Recommended palette:
- primary fill: `#D6E4F0` or `#EAECEE`
- primary border: `#1A5276` or `#2C3E50`
- secondary fill: `#FDFEFE`
- accent: `#E74C3C` used sparingly for one highlighted element

### Colorblind Safety

Use Okabe-Ito colors when categorical distinctions matter:
- blue: `#0072B2`
- orange: `#E69F00`
- green: `#009E73`
- red: `#D55E00`
- purple: `#CC79A7`
- yellow: `#F0E442`

## Tool Selection

Choose tools by reproducibility and editable vector output.

Default priority:
1. **Python scripts** for layout, repeated geometry, and deterministic generation
2. **Editable SVG output** as the primary source artifact
3. **Reusable SVG assets** for icons and lightweight illustrations

Rule of thumb:
- If the figure can be described as boxes, arrows, labels, regions, and imported assets, stay in the Python-plus-SVG path.
- If the figure is geometric or notation-sensitive, still keep it in Python-plus-SVG unless there is a compelling reason not to.
- Do not introduce an external editor when Python and SVG can express the figure cleanly.

## Venue Constraints

### ML / AI Conferences

- Fig. 1 is often a teaser at the top of page 1.
- Landscape layout is usually preferred.
- Color can be richer than IEEE, but still disciplined.
- Caption should usually be 2 to 4 sentences.

### IEEE Journals

- System model figures often appear early and are notation-heavy.
- Grayscale or two-tone styling is safer.
- Symbols in the figure must match the paper notation exactly.
- Single-column width is typically about 3.5 in; double-column about 7.16 in.

### IEEE Conferences

- Space is tight; compactness matters more.
- If a framework figure is included, it should justify its page cost.

### Nature / Science / PNAS

- Journal production may re-render the figure.
- Submit high-quality source files.
- Sans-serif figure text is preferred.

## Decision Rule

When in doubt:
1. Identify the figure's primary rhetorical job.
2. Simplify to one message.
3. Choose the least complex Python-generated SVG layout that still communicates the story cleanly.
