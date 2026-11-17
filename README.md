# Launchpad guided reading

A simple, staged reading companion for Bryson et al., Science 344, 94–97 (2014), DOI: 10.1126/science.1248523.

## Publish with GitHub Pages

In Settings → Pages, select **Deploy from a branch**, **main**, and **/(root)**, then Save. The site files are already at the repository root and require no build step.

## Reader

Introduction → cell preparation (Figure 1) → graft anatomy (Figure 2) → muscle function (Figure 3) → conclusions. Tap underlined terms and mapped figure labels for definitions. The desktop definition panel is on the right; on mobile it appears below the text. Each browser advances independently with the arrows; refreshing starts at the introduction. No accounts, analytics, database, or collected student answers.

## Edit

- `data.js`: canonical glossary definitions, aliases, reading sections, captions, and figure-label rectangles.
- `app.js`: staged reading and term interaction.
- `style.css`: responsive layout.
- `assets/figure-*.webp`: figure images.

Glossary entries have stable `id`, `term`, `definition`, `aliases`, and `source` fields. Add aliases to existing concepts before adding definitions. Figure hotspots reference those IDs; their `x`, `y`, `w`, and `h` are percentages of the figure image. Reading stages contain original article paragraphs, a companion discussion prompt, and an optional figure. The stated question and abstract are deferred disclosures. State lives only in browser memory and is not synchronized or persisted.

## Sources and rights

Article: J. Barney Bryson and colleagues, *Optical Control of Muscle Function by Transplantation of Stem Cell-Derived Motor Neurons in Mice*, Science 344, 94–97 (2014). https://doi.org/10.1126/science.1248523

Article text and figure crops were prepared from the instructor-supplied PDF. Original text is reflowed with extraction artifacts repaired. Discussion prompts and the 77 glossary definitions are independently prepared teaching material. Publisher rights in the research article and figures remain with their owner; no license to that third-party content is granted here.

The glossary interaction was inspired by AAAS Science in the Classroom, annotated there by Polly Huang: https://www.scienceintheclassroom.org/research-papers/lights-motor-neurons-and-muscle-action

Genetic construct meanings were checked against the paper and supplementary methods: https://discovery.ucl.ac.uk/id/eprint/1426329/1/Bryson_et_al_2014_accepted_manuscript_for_Open_Access.pdf
