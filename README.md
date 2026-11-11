# Visual Grounding in VLA Driving — OMEGA Lab project page

Project page for **Does Visual Information Play a Decisive Role in Vision-Language-Action Model
Driving Behavior?**, in the OMEGA Lab style.

- Paper: <https://arxiv.org/abs/2605.31041>
- Page: <https://omega-hkustgz.github.io/projects/vla-driving-visual-grounding/> (live once the lab site lists it)

## Working on the page

The page is `index.html` plus `assets/`; there is no build step. Rules for agents are in
[`AGENTS.md`](AGENTS.md).

```sh
node tools/check.mjs     # what CI runs
node tools/serve.mjs     # look at it locally
```

Every pull request gets a preview link, posted on the pull request. A push to `main` asks the
lab site to republish.

## Sources

Everything on the page comes from public material. Keep this list current.

| On the page | Source |
| --- | --- |
| Title, authors, affiliation, text | arXiv 2605.31041v1 (29 May 2026). The text paraphrases the abstract and Sections I, III, IV and V; it adds no claims. "ITSC 2026" in the eyebrow and the BibTeX note follow the paper's own first-page footnote (accepted by ITSC 2026). The page title is the lab site's short name for the project; the paper title is the subtitle. |
| `framework.webp`, `case-study.webp` | Figs. 1 and 2 of the paper, from the PNG files in the arXiv source, resized to 2400 px wide (`magick`, then `cwebp -q 90`). `social.jpg` is Fig. 1 on a 1200 × 630 canvas for link previews. |
| Results table, headline numbers, numbers in the text | Tables I–III of the paper, copied from the LaTeX source and combined into one table: the three tables share their columns and their no-perturbation row. Bracketed changes are the paper's own. Row names spell out the paper's abbreviations (GR, Random, FastV, Block-4/8). The paper's per-table bold marks are not carried over, because they are relative to each separate table. |
| Evidence label | Fig. 2 is a closed-loop run in the NeuroNCAP simulation environment (Section IV-E): Simulation. |

Not on the page because no public material exists: a code repository (so there is no Code
button), demo video, and the perturbation implementations or evaluation logs. The paper has no
separate ablation tables; Algorithm 1 is summarised in the Method text.
