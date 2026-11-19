---
name: transhumanist-race-diagram
description: "Visualize AI capability and human enhancement trends with explicit concepts, stable entity colors and honest evidence provenance."
---

# Transhumanist race diagram

Needs: Diagram or chart tools and sources for factual claims.

## Set the concept and comparison

The same phrase can mean quite different diagrams. Never skip settling these because the request looks obvious: a request that names only the topic gets all four questions. Ask only about what the request leaves open; if it already specifies an item, do not ask about it. The four things to settle:

1. **Core concept**: capability curves, parallel research tracks, competing approaches, or a milestone timeline.
2. **Visual style**: line chart, lanes, convergence view, or branching tree.
3. **Number of versions**: default to about three so there is real choice without overload.
4. **Content basis**: grounded in researched facts, purely conceptual, or a mix.

People often answer tersely (for example "concepts A and C, each"). Read that literally as a full concept-by-version matrix, and say up front roughly how many diagrams are coming. The person usually wants options to compare, not one finished diagram.

- Valid: provide the requested concept-by-variant matrix.
- Invalid: replace several requested concepts with one diagram.
- Invalid: ask about concept, style, count or basis when the request already gave them.

## Chart code and rendering path

Read any available data-visualization guidance (palette, mark specs, color follows the entity) before writing chart code, every time, so a set of versions looks like one system.

Pick the path by content. Trends, multiple series and magnitude comparisons suit a charting library with hardcoded hex colors when the library draws to canvas, since canvas cannot resolve style variables. Discrete milestones and structural diagrams suit raw SVG with a fixed viewBox.

## Define entities and preserve colors

Keep one color per entity across every variant. Define longevity, cognitive enhancement, physical pain reduction, AI as an accelerant and adjacent developments where used. Adjacent developments are a catch-all, not the other tracks combined.

A new entity takes the next unused palette slot, and the mapping gets recorded for later sets. Never reassign an existing entity's color to make room.

Each track row should carry a short one-line definition of the track label itself (what "pain reduction" or "adjacent developments" refers to), not an explanation of what the rank numbers mean.

- Valid: use the same longevity color in the line chart and evidence cards.
- Invalid: recolor entities by rank or label adjacent developments as convergence.

## Represent evidence honestly

Cite factual trials, dates and results; label abstract shapes and subjective ranks. For grounded versions, use facts already researched in the conversation; with none on hand, do a quick round of research first. Never invent trial names, dates or numbers to look grounded.

For relative scores, rank entities against each other first, then spread the ranks across the full scale (for five tracks, evenly spaced ranks from top to bottom of the scale). Scoring each track alone on the evidence found makes every score cluster high and the chart says nothing. Disclose the scoring method; do not pass stretched ranks off as measured quantities.

Describe curated-source selection bias. State where the material came from in one plain sentence after a one-sentence description of what the diagram is, naming the source (for example a search tool or a document set).

Write that provenance sentence in first person, as what the author did ("I gathered these from ..."), not as something the reader did. Name the kind of source or the platform, never a bare internal channel or folder name an outside reader cannot place. Keep it plain: no label, no italics, no extra justification, and no asides pointing at other charts.

Under the chart, use either simple rows (tag, colored dot, name, definition) or detailed evidence cards (a card per track in that track's color, with dated findings). Choose cards when the person asks for the fuller version; if you restore earlier content, reconcile it against later corrections first, then say plainly what you brought back and why.

Preserve the title, the subtitle and each track row's definition in the deliverable through every edit round, and recheck them after each pass.

After showing the versions, ask which land or whether a different mix is wanted. Let the picture carry its own summary rather than restating it in prose.

- Valid: label a radar as a qualitative relative ranking with dated evidence.
- Invalid: display subjective momentum as objective measured progress.
