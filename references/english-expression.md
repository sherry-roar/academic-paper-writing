# Precise English Expression

Use this module for sentence-level editing after understanding the scientific meaning. The goal is accurate, readable prose, not conformity to a vocabulary blacklist or a detector score.

## Prefer an identifiable subject and action

Name the object that performs or undergoes the relevant action. “The estimator weights each observation by its uncertainty” explains more than “An effective weighting mechanism is leveraged.” Use authorial “we” for choices the authors make when appropriate to the field.

Prefer concrete verbs such as measures, partitions, estimates, samples, constrains, transfers, derives, or compares when they describe the actual operation. Words such as enables, improves, facilitates, and addresses can be accurate, but should not replace an explanation of what changes.

Passive voice is useful when the actor is unknown, irrelevant, or less important than the object. Do not rewrite every passive sentence mechanically.

## Make references and transitions explicit

“This” and “these” should refer to a nearby, identifiable idea. Add a noun when several antecedents are possible. Replace “the above results” with the result or comparison the argument actually uses.

Maintain topic continuity between sentences. When shifting from an observation to an explanation, name the relationship. Removing a connector does not repair a missing logical step; adding “moreover” does not establish one.

Use contrast to explain a genuine difference between existing approaches. For the paper's own less favorable comparisons, follow the launch-presentation principle and explain the supported objective or trade-off instead of introducing a self-weakening however sentence.

## Calibrate claims to evidence

| Wording | Appropriate use | Check before retaining it |
|---|---|---|
| shows, reports, measures | Directly observed or reported result | Is the observation actually available? |
| suggests, is consistent with | An interpretation compatible with evidence | Are plausible alternatives acknowledged where material? |
| causes, leads to | A causal claim | Does the design or derivation support causality? |
| proves, guarantees | A valid proof or explicit guarantee | Are assumptions, quantifiers, and argument complete? |
| significant | Statistical or clearly defined substantive meaning | Is the intended meaning and analysis supplied? |
| robust, scalable, efficient | A defined property supported by tests or analysis | Against which conditions, scale, cost, or disturbances? |
| first, novel, universal | A justified and necessary scope or priority claim | Has the relevant literature or domain been verified? |

Do not weaken an established theorem to “suggests” or upgrade an association to “proves.” Avoid repeated may, might, perhaps, and to some extent when the observation is definite. State the source of genuine uncertainty instead of adding vague hedges.

## Preserve technical language

Create a small term list when the manuscript is long or inconsistent. Keep technical names, symbols, stage boundaries, and dataset labels stable. Synonym variation can change meaning: accuracy, precision, correctness, validity, and reliability are not interchangeable.

Define abbreviations when first needed. Avoid acronyms that save little space or appear only once. Respect standard capitalization and the author's verified naming conventions.

Numbers, units, signs, inequalities, confidence intervals, normalization formulas, and significant digits are factual content. Do not round, convert, or “correct” them as a language edit. If a conversion is requested, record the formula and check every affected location.

## Check grammar in context

- Match subjects and verbs, including long noun phrases and intervening clauses.
- Check countable nouns, singular/plural agreement, articles, and determiners.
- Distinguish the first introduction of an object from later reference to a specific object.
- Keep lists parallel in grammatical form and logical level.
- Ensure modifiers attach to the intended noun and avoid dangling participial phrases.
- Compare time with time, methods with methods, and populations with comparable populations.
- Use respectively only when two lists have a clear, equal-length correspondence.
- Check whether a restrictive clause changes the population or condition being described.
- Preserve negation, modality, and quantifiers; changing some to all is a scientific change.

Do not change a grammatical convention merely because another field prefers a different one. Follow the target style when verified and keep usage consistent.

## Choose tense by function

Present tense often describes established knowledge, the paper's argument, formal definitions, and what a figure shows. Past tense often describes completed procedures and observations. Present perfect may describe a research stream continuing to the present.

Disciplinary conventions differ. Keep tense consistent with the function of the sentence and the author's appropriate convention; do not impose one tense on an entire section regardless of meaning.

## Remove empty evaluation

Replace unsupported adjectives with an operation, condition, comparison, or measurement. Delete words that add emphasis without information. Preserve an adjective when it has a defined technical meaning.

| Weak expression | Better direction |
|---|---|
| “The method achieves excellent performance.” | State the metric, comparator, and condition. |
| “This plays a crucial role.” | Explain what depends on the component and how. |
| “It is worth noting that the effect increases.” | State the increase directly and identify its relevance. |
| “The results validate effectiveness.” | State which claim the evidence supports. |
| “A comprehensive and groundbreaking framework” | Describe the framework's actual scope and contribution. |
| “The approach is simple and efficient.” | Describe the procedure and measured or derived cost. |

No word is reliable evidence of AI authorship. Do not promise that a revision will evade detection or make unsupported claims about how text was written.

## Use punctuation for readability

Split sentences when several independent claims or conditions obscure their relationship. Keep a longer sentence when it expresses a necessary relation clearly.

For newly written body prose and captions, this skill's house style avoids colons and normally replaces semicolons with sentence boundaries. Use at most one semicolon per paragraph when a closely connected parallel relation needs it. Titles, code, URLs, mathematical definitions, original reference titles, and author-approved existing sentences are necessary exceptions. This is a writing preference, not an official rule of any publisher; an explicit author choice takes precedence.

## Learn from reference papers responsibly

Extract rhetorical functions, information ordering, terminology conventions, and the level of detail. Do not copy distinctive wording or introduce a reference paper's results into the user's manuscript.

For each proposed sentence pattern, check the original claim and evidence first. A fluent replacement that changes the comparison baseline, certainty, population, or mechanism is an incorrect edit.

See [Worked examples](worked-examples.md) for synthetic before/after cases. Use them to understand decisions rather than as mandatory sentence templates.
