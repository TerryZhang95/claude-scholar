# System Model Figure

Load this module for IEEE-style topology, geometry, communication links, nodes, and coverage regions.

## Purpose

This figure explains the physical or logical setup of the studied system:
- entities and their roles
- geometry or topology
- communication or interaction links
- distances, radii, and regions

This is usually not a teaser figure. It is a notation-sensitive model figure.

## Best Fit

Use this module when the figure appears:
- in Section II System Model
- in IEEE journals or conferences
- for wireless, networking, edge, or multi-agent topologies

## Design Priorities

1. Keep notation exact.
2. Keep visual style conservative.
3. Show geometry cleanly.
4. Avoid decorative polish that weakens technical clarity.

## Preferred Style

- grayscale or two-tone
- sharp rectangles or circles over playful rounded UI shapes
- sparse accent color, if any
- explicit labels for nodes, regions, and distances

## Tool Guidance

Use **Python-generated editable SVG** even when:
- coordinates matter
- circles, angles, ranges, or distances must be precise
- the figure uses mathematical symbols heavily

The goal is still an editable SVG source plus a PDF export, not a separate LaTeX-native figure path.

## What to Include

- node types such as BS, AP, UAV, user, server
- links and their semantics
- radii, distances, coverage zones, interference zones
- region boundaries or cluster membership if analytically relevant

## What to Exclude

- marketing-style icons unless they genuinely clarify the entity type
- excessive color coding
- unexplained symbols
- topology detail not used anywhere in the model

## Notation Rule

Every symbol in the figure must either:
- match a symbol already used in the paper, or
- be defined in the caption or surrounding text immediately

Never introduce notation that exists only in the figure.

## Review Questions

- Do the labels in the figure exactly match the equations and notation table?
- Is the geometry precise enough to support the model assumptions?
- Does the Python layout logic make the geometry easy to revise after reviewer feedback?
