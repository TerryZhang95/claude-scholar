# Multi-Panel Layout

Load this module when the structural figure is split into panels such as `(a)`, `(b)`, `(c)`.

## Purpose

Use multiple panels when one message needs staged exposition, not when several unrelated stories are competing for space.

Good reasons to use panels:
- overview plus zoom-in
- problem vs method
- training vs inference
- architecture plus deployment scenario

Bad reason:
- trying to save page space by cramming two unrelated figures together

## Panel Design Rules

1. Panels should still support one overall message.
2. Each panel should have a distinct role.
3. Reading order should be obvious.
4. Panel labels should be consistent in placement and style.

## Common Patterns

- `(a)` system setup, `(b)` method overview
- `(a)` prior work, `(b)` proposed method
- `(a)` training pipeline, `(b)` inference pipeline
- `(a)` global overview, `(b)` architecture detail

## Composition Guidance

- Keep panel widths and spacing regular.
- Use shared styling across panels.
- Avoid repeating legends or labels when a shared legend can do the job.
- If one panel is dominant, let size reflect that hierarchy.

## Venue Notes

- Nature-style layouts often use bold panel labels in the lower-left or upper-left depending on house style.
- IEEE papers usually benefit from simpler panel composition with restrained annotation.
- ML conferences tolerate more explanatory callouts if the figure remains clean.

## Review Questions

- Are the panels one argument or two different figures forced together?
- Does each panel justify its space?
- Could one panel be moved into the appendix or converted into a separate figure?
