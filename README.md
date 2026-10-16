# Academic Paper Writing

A self-contained agent skill for drafting and revising English academic papers for journals and conferences. It connects the research question, argument, evidence, section structure, and sentence-level expression in one workflow.

The guidance is independent of a particular venue, publisher, institution, research project, or scientific platform. It supports empirical, computational, theoretical, qualitative, and mixed-methods work by selecting the guidance relevant to the study. It does not impose one manuscript structure on every discipline.

## What the skill covers

- Develop a coherent research argument and align contributions with evidence.
- Draft titles, abstracts, introductions, related work, methods, results, discussions, and conclusions.
- Present the strongest supported contribution with concrete mechanisms and purposeful comparisons.
- Preserve numbers, equations, terminology, comparison conditions, and author intent during editing.
- Keep facts and comparison conditions accurate while avoiding a defensive, technical-report tone.
- Write informative captions and produce readable, traceable figures and tables.
- Revise in direct, collaborative, or batch mode, including optional bilingual explanations.
- Check the current requirements of the actual target journal or conference.
- Prepare evidence-based responses to reviewers when explicitly requested.

## Install

The repository root is the skill folder. Keep its name as `academic-paper-writing` and retain `SKILL.md`, `references/`, and `agents/` together.

For Codex, clone the repository into your configured skills directory, normally `$CODEX_HOME/skills/academic-paper-writing` or `~/.codex/skills/academic-paper-writing` when `CODEX_HOME` is unset. Replace `<repository-url>` with the repository's clone URL; access to a private repository is required.

```sh
git clone <repository-url> ~/.codex/skills/academic-paper-writing
```

Alternatively, download and extract the packaged archive, then copy its `academic-paper-writing` folder into your skills directory. Load the skill in a new session if your host discovers skills at session start.

For other agents that support `SKILL.md`, use the host's skill-installation mechanism. Otherwise, open `SKILL.md` as the entrypoint and read the linked reference modules as needed. The core guidance is plain Markdown and has no executable hooks, required MCP servers, model-specific dependencies, or external service requirements.

## Use

Invoke `$academic-paper-writing` and provide the relevant text or files. Include the task, allowed edit scope, target audience or venue if known, and any verified results or reference papers needed to support the claims.

```text
Use $academic-paper-writing to polish this abstract. Preserve every number,
technical term, and conclusion. Return the revised text and a short change summary.
```

```text
Use $academic-paper-writing to revise my introduction and contribution list.
First check whether the research gap, method, and evaluation answer the same
question. Make the authorized edits directly and flag unsupported claims.
```

```text
Use $academic-paper-writing to help draft the results section from the attached
tables and study protocol. Lead with the strongest supported result, explain
the mechanism and trade-offs, and keep missing-evidence notes separate from prose.
```

```text
Use $academic-paper-writing to review this paper for the specified conference.
Check the current official author instructions, including format, anonymity,
supplementary material, and required disclosures. Report what remains unverified.
```

Use direct mode for ready-to-apply edits, collaborative mode for requested checkpoints, and batch mode for consistent edits across several sections. A venue is optional for ordinary writing work. If none is specified, the skill uses general academic style and leaves venue compliance unverified.

## Contents

| File | Purpose |
|---|---|
| [SKILL.md](SKILL.md) | Entry point, scope, workflow, and reference routing |
| [Argument and narrative](references/argument-and-narrative.md) | The launch-presentation principle, contribution framing, and paragraph logic |
| [Section guidance](references/section-guidance.md) | Section-specific reasoning and drafting practices |
| [English expression](references/english-expression.md) | Precision, grammar, cohesion, claim strength, and editing examples |
| [Evidence and methods](references/evidence-and-methods.md) | Study reporting, comparisons, uncertainty, and scientific boundaries |
| [Figures and tables](references/figures-and-tables.md) | Visual argument, captions, accessibility, and production checks |
| [Revision workflow](references/revision-workflow.md) | Editing modes, reference-driven style, translation, and reviewer responses |
| [Venue and integrity](references/venue-and-integrity.md) | Official requirements, citation verification, ethics, and submission checks |
| [Working templates](references/working-templates.md) | Adaptable argument maps, evidence ledgers, and revision records |
| [Worked examples](references/worked-examples.md) | Synthetic examples of structural and sentence-level decisions |
| [Final checks](references/final-checks.md) | Focused checks before delivering edits or preparing submission files |

All references are bundled and use relative links. Read only the modules needed for the task.

## Evidence and privacy

The skill never supplies missing research results, references, author details, or submission status. Illustrative examples are explicitly synthetic. Placeholders belong in working drafts and must be resolved before submission.

No source manuscripts, research datasets, reviewer reports, credentials, local paths, infrastructure settings, or project-specific results are included. Using the skill does not authorize uploading a manuscript, contacting anyone, running experiments, changing research code, or submitting a paper.

## License and attribution

See [LICENSE](LICENSE) for the package license and [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) for retained attribution. Local release evidence and generated archives are excluded from Git history.
