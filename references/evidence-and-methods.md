# Evidence and Methods

Use this module to write accurate methods, setup, metrics, and result explanations. Apply the [launch-presentation principles](argument-and-narrative.md) to the manuscript narrative. Detailed operational evidence belongs in working records; it does not become a mandatory caveat after each result.

## Match evidence to the claim

| Claim | Useful supporting evidence | What does not establish it by itself |
|---|---|---|
| A design improves the overall objective | A comparison using the same overall measurement scope | A faster isolated component |
| A mechanism explains an improvement | Controlled variants, diagnostics, counts, distributions, or an applicable derivation | A change in total time alone |
| Two activities overlap | A valid execution timeline, dependency model, and overall elapsed time | Adding separately measured activity durations |
| A representation reduces work | Counts or analysis at the old and new units of work | Calling the representation efficient |
| A method fits a resource budget | Actual object sizes, live ranges, occupancy, and relevant overhead | Nominal capacity alone |
| Results agree with a reference | Matched inputs, defined diagnostics, normalization, and justified tolerance | Successful compilation or process exit |
| A method scales | A workload definition, reference scale, resource counts, and consistent efficiency metric | One larger run |
| A result transfers to another setting | The required properties and evidence in that setting | Similar names or nominal specifications |

Use the evidence already supplied. Identify an unsupported detail in the working notes rather than inventing it or launching new research.

## Record the comparison conditions

Describe the conditions that define the comparison. For computational work, these may include hardware, software versions, compiler settings, inputs, process and thread counts, placement, communication, precision, and timing boundaries. Keep full source, binary, input, and runner identities in the research records when available.

For other empirical work, use the analogous study conditions: population or material, selection criteria, collection setting, measurement procedure, analysis settings, and reference conditions. Select details relevant to interpreting the actual study rather than copying a checklist from another field.

A baseline name should identify a consistent version and configuration. If versions or settings differ, explain those differences at the point where they define the comparison. Do not silently equate different numerical precision, data selection, resource budgets, or procedures.

Distinguish a mechanism comparison within one setting from a comparison of complete systems in different settings. Both can be useful, but they answer different questions.

## Explain controlled variants

Adding components progressively and removing one component at a time answer different questions. Do not attribute an entire difference to one mechanism when other settings change as well.

Preserve common inputs and paths where possible. If a component depends on another component, explain the dependency or use a meaningful executable alternative. Do not describe an infeasible variant as a measured baseline.

In the manuscript, present variants as design-space choices and explain the selected design's purpose. Use each experiment to answer a named question, rather than recounting implementation trials.

## Define metrics before discussing results

Identify the numerator, denominator, scope, direction of improvement, and aggregation rule. A normalized quantity is not self-explanatory simply because it has no units.

For time-based comparisons:

- Speedup is baseline time divided by method time for the same measurement scope.
- Time reduction is `(baseline time - method time) / baseline time`.
- Throughput must pair a defined amount of completed work with the matching elapsed time.
- Component, phase, iteration, full step, and complete application times are distinct scopes.
- A maximum across workers and a sum across workers represent different quantities.
- Overlapping component durations need not sum to total elapsed time.

Do not multiply component speedups to claim an overall speedup. Preserve the measured overall result and use components to explain it.

Distinguish physical traffic from logical traffic, peak capability from measured utilization, model estimates from observations, and simulation results from physical-system measurements. Use the actual unit and definition consistently across prose, figures, captions, and tables.

## Account for preparation and recurring cost

Identify initialization, allocation, preprocessing, compilation, conversion, steady-state work, and finalization as applicable. State the measurement boundary once in the setup. Do not call a result end-to-end if essential costs are outside its boundary.

Separate a one-time cost from a recurring per-use cost. If a stable per-use saving is positive, a simplified break-even count is `ceil(preparation cost / per-use saving)`. Use that expression only when the workload and reuse assumptions apply; otherwise use actual cumulative cost or an appropriate model.

Explain costs through the design objective. A variant may shorten one stage while exposing work elsewhere. Show the resulting overall comparison rather than describing an isolated stage as a defeat.

## Preserve statistical meaning

Report the statistic actually used, such as mean, median, geometric mean, distribution, interval, or maximum. Use the real number of repetitions or observations. Do not invent error bars, uncertainty estimates, or significance from a single measurement.

Keep per-case summaries distinct from pooled summaries and ratios of aggregates. If values are normalized or averaged across cases, retain the rule and reference set. Do not replace a statistic with the most favorable observation during editing.

Use the study's own justified analysis and reporting conventions. A repetition count observed in another paper is a reference example, not a universal requirement.

## Preserve failure states in the records

Keep failed, unavailable, unsupported, and unmeasured states distinguishable. An out-of-memory event, timeout, crash, and run that never started are different states. None is a measured zero.

When an included figure contains such a case, label it correctly. This does not require adding every failed attempt to the manuscript. Select main-text material by its argumentative role and keep the complete operational record separately.

## Move from trend to mechanism

Begin with the comparison's main message, give the informative magnitude or trend, and connect it to the relevant work, data path, theoretical relation, or diagnostic. End with the capability the evidence establishes.

Avoid generic claims such as “the results demonstrate effectiveness.” Explain what changed: fewer decisions, less data movement, a changed sample distribution, a tighter bound, or another actual mechanism.

Conditions already defined in the setup do not need to be repeated in every sentence. Keep unresolved measurement questions in the working notes rather than attaching a defensive closing sentence to each paragraph.

Build success, execution success, numerical agreement, property verification, and reproducibility are separate claims. Describe each according to its actual evidence.
