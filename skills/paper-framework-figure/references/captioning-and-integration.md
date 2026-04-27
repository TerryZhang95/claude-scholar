# Captioning and Integration

Load this module when drafting the caption, checking notation consistency, exporting files, or integrating the figure into LaTeX.

## Caption Standard

Caption structure:

```text
Fig. N. [What the figure shows in one clause]. [What the main components, colors, arrows, or panels mean]. [What the reader should notice or take away].
```

Good caption properties:
- self-contained
- story first, inventory second
- names only the details the reader needs
- states the main takeaway explicitly

## Caption Anti-Patterns

- "Figure 1 shows our method."
- a mechanical color list with no story
- requiring the reader to decode the figure from the text first
- missing explanation for dashed or dotted arrows

## Example Pattern

```text
Fig. 1. Overview of the proposed framework. The input is encoded into a shared latent representation, which is processed by two task-specific branches for prediction and calibration. Solid arrows denote the main forward path, while dashed arrows denote auxiliary supervision. The key point is that both tasks are optimized through a shared representation rather than separate pipelines.
```

## Notation Consistency

- Every symbol in the figure must match the paper.
- In IEEE-style writing, symbols should also match the notation table.
- Do not invent a symbol only for the figure.

## Placement Rule

The figure should appear before or at its first substantial textual discussion.

Typical LaTeX reference form:

```latex
As illustrated in Fig.~\ref{fig:overview}, the method consists of three stages.
```

Keep `\label` inside the `figure` environment and after the `\caption`.

## File Management

Recommended workflow:
1. Create the source as an editable `.svg`, ideally from a Python generation step.
2. Export vector output as PDF.
3. Export PNG only for preview if needed.
4. Copy deliverables into `paper/figures/`.
5. Use bare filenames in `\includegraphics`.

Typical LaTeX usage:

```latex
\includegraphics[width=\columnwidth]{fig1_overview}
```

with:

```latex
\graphicspath{{figures/}}
```

## Final Checks

- caption is self-contained
- no title text is inside the figure
- width matches venue constraints
- font is readable in the compiled PDF
- vector output is used when possible
