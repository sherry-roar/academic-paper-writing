# Figures, Tables, and Captions

Read this module when designing a figure, editing its caption, or checking visual evidence. The methods here are writing and design guidance, not publisher-specific specifications.

## Give each visual a role

Choose the question the visual answers before selecting its form. Connect it to the paper's central contribution. In the surrounding prose, state the strongest message explicitly rather than making readers search through every mark.

| Purpose | Useful form | Key check |
|---|---|---|
| Compare a small number of methods or conditions | Grouped bars, dots, or a compact table | Same baseline, metric, and order |
| Show a trend over an ordered variable | Lines with distinguishable markers | Meaningful numerical axis and consistent conditions |
| Show variation or distribution | Box, violin, scatter, interval, or distribution plot | Real observations and an explained summary |
| Explain resource or time components | Decomposition with absolute totals | Components and overlap are defined correctly |
| Explain dependencies or execution | Pipeline diagram or timeline | Actual order, dependencies, startup, and completion |
| Explain method structure | Overview diagram | Objects, transformations, and interfaces are identifiable |
| Present exact values or configurations | Table | Units, denominators, and labels are explicit |

Do not force every experiment into the same chart type. A figure should make the important relationship easier to inspect than a prose list would.

## Keep visual identity consistent

Assign method identities consistently across related figures. Assign stage identities consistently within decompositions. Do not let one color simultaneously mean a method and a stage in the same visual.

Use panels, patterns, line styles, markers, or direct labels when the figure has another categorical dimension. Preserve method order between panels. A candidate palette is a local design choice, not an official academic rule.

Use redundant encodings so readers can distinguish cases in grayscale and with common color-vision differences. Give pale fills enough contrast through borders, patterns, or suitable text. Prefer a clean background and restrained grid over gradients, decorative shadows, or three-dimensional bars.

## Make axes and statistics interpretable

- Show units for dimensional metrics.
- Identify the baseline for speedup and the denominator for normalized values.
- Define the population or total behind percentages.
- Mark logarithmic scales explicitly.
- Start bar charts at zero unless a clearly disclosed alternative serves a legitimate purpose.
- Use reference lines for meaningful quantities such as a baseline ratio or capacity threshold.
- Explain error bars, intervals, sample counts, and aggregation using the actual data.
- Keep absent or failed measurements distinct from zero.

Avoid a dual axis unless the relationship needs it and each scale is clear. Do not use matching colors or proximity to imply equivalence between different quantities.

Do not merge a peak result, an arithmetic average, and a geometric mean into one unlabeled notion of performance. If cases are sorted, state the sorting rule and preserve the defined case set.

## Structure diagrams and timelines

A method overview should show the central representation or reasoning before minor implementation detail. Use consistent shapes and arrows for the same semantics. Distinguish data flow, control, and dependencies when they differ.

Timelines should represent real dependencies and include relevant startup, waiting, and completion. Do not draw an indefinitely perfect steady state to imply overlap that has not been established. Labels should identify the task or iteration associated with each operation.

Diagram clarity cannot justify changing the algorithm or implying an execution path absent from the implementation.

## Captions

Give the experiment or object, necessary conditions, panel meanings, and unusual encodings. Define information unique to the figure; avoid repeating the complete legend or explaining familiar chart grammar.

Place detailed causal analysis in the body text. Keep common setup details in the setup section and refer to them consistently. Apply the skill's prose house style to newly written captions: avoid colons, use sentence boundaries instead of repeated semicolons, and avoid parentheses that carry essential qualifications.

If a caption uses a takeaway, ensure it matches the plotted evidence. Do not repeat the same conclusion in the title, caption, legend, and every panel.

## Tables

Use clear row and column headings with units and defined references. Align comparable values and apply consistent precision. Use emphasis sparingly to guide the principal comparison, with a stated rule if highlighting best values.

Explain abbreviations and exceptional cells through concise notes. Use a clear symbol or label for unmeasured cases. Keep captions and notes readable instead of shrinking a dense table until its contents no longer work at publication size.

## Inspect the actual publication size

Check the figure within the real one-column or two-column layout. Inspect labels, ticks, legends, panels, line widths, captions, and grayscale legibility at that size. A figure that looks clear when enlarged may fail after insertion.

For line plots and diagrams, retain editable sources and prefer vector output when the production requirements allow it. For raster material, check resolution at its actual physical dimensions. Use the current venue instructions for required formats, fonts, and resolution rather than assuming fixed universal values.

If a figure is crowded, reduce competing information, reorganize panels, or choose a better form. Do not solve the problem only by reducing font size.

## Keep the visual traceable

Retain the data selection, transformation or normalization formula, plotting source, and export identity. A screenshot is not an adequate replacement for the underlying editable figure and evidence.

Borrow organizational ideas from reference figures rather than copying their art, data, claims, or presumed exact colors. Read the actual figure before describing its visual method.

Check scientific semantics first, then the reader's main comparison, then publication-size visual quality.
