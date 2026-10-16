# Worked Examples

All examples below are synthetic writing demonstrations. Their numbers and conditions are invented for illustration and are not research findings, recommended benchmarks, or text to insert into a real paper without evidence.

## Open with the research problem

**Before**

> With the rapid development of modern computing, efficient algorithms have become increasingly important. We propose a novel framework with several optimizations.

**After**

> Repeated scans dominate the analysis when each update changes a small part of the dataset. We maintain the affected regions during each update so that the next query visits the modified regions directly.

The revision identifies the object, obstacle, and idea. It replaces broad importance and novelty labels with a concrete relation. Use this direction only when the actual method has that behavior.

## Explain the unit of work

**Before**

> The method greatly improves efficiency through an effective grouping mechanism.

**After**

> The method replaces one destination lookup per item with one lookup per group and one contiguous transfer for the group.

The revision explains what work changes. The performance implication belongs with the matching evidence.

## Give the result its real scope

**Given synthetic evidence**: one phase takes 12 seconds in the baseline and 8 seconds in the new method. Complete execution takes 20 and 16 seconds, respectively.

**Incorrect**

> The method accelerates the application by 1.5×.

**Correct**

> The method accelerates the measured phase by 1.5× and reduces complete execution time by 20%.

The revision preserves both positive results and their actual boundaries. It does not turn the comparison into a caveat about limited application benefit.

## State a stable advantage directly

**Given synthetic evidence**: speedup remains between 1.6× and 2.0× over the defined test range.

**Self-weakening**

> Unfortunately, the speedup dips to only 1.6× in the sparse case.

**Launch-presentation style**

> The method maintains at least 1.6× speedup across the tested range and reaches 2.0× at the largest workload.

Follow with the supported explanation of how recurring work or fixed cost varies with workload. Do not add a generic weakness sentence.

## Explain a trade-off through the complete objective

**Given synthetic evidence**: variant A reduces a compute stage from 9 to 8 seconds but exposes 4 seconds of transfer. Variant B takes 9 seconds for the stage and exposes 1 second of transfer. Other costs are identical.

**Self-weakening**

> Variant B is still slower than A in computation.

**Launch-presentation style**

> Variant A shortens computation by moving transfer onto the foreground path. Variant B keeps most transfer off that path and completes the combined work in 10 seconds, compared with 12 seconds for A.

The revision explains the design objective and real trade-off. It retains the factual stage difference without making that difference the paper's contest.

## Replace a development diary with a design argument

**Before**

> We first tried regrouping every item, but it was too slow. We then tried incremental maintenance and found it worked better.

**After**

> Full regrouping revisits the entire dataset after each update. Incremental maintenance restricts this work to the affected regions, matching the small-update workload.

The revision presents alternatives by their work and suitability. Use a measured result separately if the argument depends on it.

## Define the scope once

**Before**

> The method improves performance, although the result applies only to the tested setting. The next experiment also shows improvement, but it cannot guarantee benefits elsewhere.

**After, in setup**

> The evaluation uses the specified dataset family with a fixed query budget.

**After, in results**

> The method reduces the median query time by 18%. The reduction increases with the fraction of unchanged records.

The conditions are explicit and the result is direct. These synthetic statements require matching data in a real manuscript.

## Keep the conclusion memorable

**Before**

> However, the method remains limited to the present representation, and further work is required.

**After**

> Maintaining the representation during updates removes repeated reconstruction from the query path. This principle provides a basis for extending the design to other update patterns.

The revision reinforces the mechanism and presents an extension direction. It does not claim that the extension has been implemented or evaluated.

## Keep unsupported details in working notes

If a draft claims a property that is not documented, do not supply a plausible detail. Record the exact item requiring verification, revise independent language issues, and leave the unresolved scientific choice to the author. The working note does not automatically become a defensive paragraph in the paper.
