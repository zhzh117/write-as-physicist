# Write As Physicist

An agent skill for drafting and revising physics papers, theses, abstracts, figure captions, and technical explanations in English or Chinese.

The skill helps make the physical question, evidence, and result easy to follow. It covers argument structure, precise claims, equation exposition, readable captions, and natural prose across theoretical, computational, and experimental physics.

## What it helps with

- **Build the argument.** Connect the question, observations or calculations, and supported conclusion; give each section and paragraph a clear purpose.
- **Match claims to evidence.** Preserve assumptions, uncertainty, numerical controls, measurement limits, and the distinction between results and interpretations.
- **Explain equations and figures.** Introduce physical meaning, define notation, and make panels, conditions, processing, and uncertainties readable.
- **Edit faithfully.** Preserve quantities, units, signs, citations, and the author's useful voice; identify missing facts separately from manuscript prose.
- **Remove empty prose.** Reduce inflated language, repetitive hedging, anticipatory disclaimers, and generic closing remarks while retaining qualifications that affect the science.

The complete guidance is in [SKILL.md](SKILL.md). [Nine worked examples](references/examples.md) cover condensed matter, statistical physics, and high-energy or gravitational physics, with theory, computation, and experiment represented in each group.

## Installation

Download or clone this repository, and keep its contents together in a folder named `write-as-physicist`. The folder must contain `SKILL.md` directly. Retain `references/`, `agents/`, and `assets/` alongside it.

### Codex CLI or IDE extension

Place the folder in one of these locations:

| Scope | Path to the installed main file |
| --- | --- |
| Personal | `~/.agents/skills/write-as-physicist/SKILL.md` |
| Current repository | `.agents/skills/write-as-physicist/SKILL.md` |

Select the skill through `/skills`, or mention `$write-as-physicist` in your prompt. These locations and invocation methods follow the [official Codex skill documentation](https://learn.chatgpt.com/docs/build-skills).

### Claude Code

Place the folder at `~/.claude/skills/write-as-physicist/` for personal use, or `.claude/skills/write-as-physicist/` within a project. Invoke it with `/write-as-physicist`. See the [official Claude Code skill documentation](https://code.claude.com/docs/en/skills).

### Other hosts

Use your host's installation process for an [Agent Skills](https://agentskills.io/specification) directory, preserving the relative paths. In ChatGPT environments where the skill has been installed, type `@` and select **Write As Physicist**. Host documentation determines the available installation and distribution options.

The skill contains Markdown guidance and an icon, with no executable scripts or package dependencies. File editing, browsing, and document export depend on the tools available in the host.

## Usage

Supply the passage, equations, or figure information, together with the intended audience, output language, and any length or journal requirements. Include the data and references needed to support scientific claims.

For example, in Codex:

```text
$write-as-physicist
Revise the introduction below for a condensed-matter theory paper.
Make the unresolved question and our contribution clear. Preserve the
model assumptions, citations, and strength of each claim. Keep it under
500 words.

[Draft and supporting context]
```

Other tasks can use the same skill:

- **Computational statistical physics:** revise a results paragraph to distinguish finite-size observations from an extrapolated limit, preserving the supplied convergence checks.
- **Experimental high-energy physics:** write a caption from panel descriptions, including event selection, plotted quantities, uncertainty definitions, and comparisons.
- **Gravitation:** explain a derivation, introducing the assumptions, notation, physical meaning, and relevant limits.
- **Any field:** review a conclusion for repeated caveats and state the supported result and its concrete implication.

The examples in `references/examples.md` distinguish reported physics from illustrative teaching inputs. Their numerical examples should be read in that context.

## Repository contents

| File | Purpose |
| --- | --- |
| [SKILL.md](SKILL.md) | Core instructions and skill metadata. |
| [references/examples.md](references/examples.md) | Nine worked writing examples. |
| [references/sources.md](references/sources.md) | Writing guides, physics sources, and editorial decisions. |
| [agents/openai.yaml](agents/openai.yaml) | OpenAI host display and invocation metadata. |
| [assets/icon.svg](assets/icon.svg) | Skill icon. |
| [CONTRIBUTING.md](CONTRIBUTING.md) | How to report problems and propose improvements. |
| [LICENSE](LICENSE) | MIT license text. |

## Sources and acknowledgments

The skill draws on scientific writing literature, physics exposition guides, and published research. The [source notes](references/sources.md) document these sources and the editorial choices made for this project.

Kiterlin’s [anti-defensive-writing](https://github.com/Kiterlin/anti-defensive-writing) informed the checks for redundant caveats, stacked hedges, anticipatory denials, and necessary scope. Siqi Chen’s humanizer](https://github.com/blader/humanizer) informed the checks for formulaic transitions, inflated language, repetitive structures, and chat-style filler. These editorial ideas were incorporated into separately written scientific-writing guidance. The physics examples and figure-caption instructions were developed for this project from the cited literature.

Both referenced projects are distributed under the MIT License.

## Contributing

Issues and pull requests are welcome. A short passage, the requested task, and the resulting output make a writing problem easier to assess. See [CONTRIBUTING.md](CONTRIBUTING.md) for the suggested format.

## License

This project uses the [MIT License](LICENSE). Referenced publications and external projects retain their own licenses.
