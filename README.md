# Launchpad guided reading

A simple, staged reading companion for Bryson et al., Science 344, 94–97 (2014), DOI: 10.1126/science.1248523.

## Publish with GitHub Pages

In Settings → Pages, select **Deploy from a branch**, **main**, and **/(root)**, then Save. The site files are already at the repository root and require no build step.

## Reader

Introduction → Results: Section 1 (Figure 1) → Results: Section 2 (Figure 2) → Results: Section 3 (Figure 3) → Conclusion and Discussion. Tap underlined terms and mapped figure labels for definitions. The desktop definition panel is on the right; on mobile it appears below the text. Each browser advances independently with the arrows; refreshing starts at the introduction. No accounts, analytics, database, or collected student answers.

## Edit

- `data.js`: canonical glossary definitions, aliases, reading sections, captions, and figure-label rectangles.
- `app.js`: staged reading and term interaction.
- `style.css`: responsive layout.
- `assets/figure-*.webp`: figure images.

Glossary entries have stable `id`, `term`, `definition`, `aliases`, and `source` fields. Add aliases to existing concepts before adding definitions. Figure hotspots reference those IDs; their `x`, `y`, `w`, and `h` are percentages of the figure image. Reading stages contain original article paragraphs, a companion discussion prompt, and an optional figure. Introduction discussion questions are displayed directly, with one question per line. The authors’ stated question and the abstract are omitted from the reader. Results: Section 1 asks only what the data were intended to show; Section 2 currently asks: “success? Guess we're done here.” State lives only in browser memory and is not synchronized or persisted.

## Sources and rights

Article: J. Barney Bryson and colleagues, *Optical Control of Muscle Function by Transplantation of Stem Cell-Derived Motor Neurons in Mice*, Science 344, 94–97 (2014). https://doi.org/10.1126/science.1248523

Article text and figure crops were prepared from the instructor-supplied PDF. Original text is reflowed with extraction artifacts repaired. Discussion prompts and the 77 glossary definitions are independently prepared teaching material. Publisher rights in the research article and figures remain with their owner; no license to that third-party content is granted here.

The glossary interaction was inspired by AAAS Science in the Classroom, annotated there by Polly Huang: https://www.scienceintheclassroom.org/research-papers/lights-motor-neurons-and-muscle-action

Genetic construct meanings were checked against the paper and supplementary methods: https://discovery.ucl.ac.uk/id/eprint/1426329/1/Bryson_et_al_2014_accepted_manuscript_for_Open_Access.pdf

## Classroom reveal codes

Each reading stage has a four-character `code` in `data.js`. Comparison is case-insensitive and accepts letters, numbers, and punctuation. The page is readable and glossary definitions work before unlocking. A correct code reveals that page's analysis highlights and its previous/next navigation. Incorrect codes do not advance the reader. Unlock state is a per-page Set held only in browser memory: previously unlocked pages stay open during the session, and refresh resets the session. This is a classroom pacing mechanism, not authentication or protected access; codes and content are inspectable static assets.

`analysis` contains the notes recovered from the original annotated PDF: `id`, `category`, `quote`, and `note`. Categories are FRAME, METHOD, EVIDENCE, INFERENCE, SCOPE, and LIMIT. The renderer matches normalized quotations to the current article and captions, preserving glossary buttons within highlights. Notes whose quoted passage was removed from the reader are not displayed. Tap a colored passage or focus it and press Enter to read its note; glossary terms continue to show their definitions in the same panel.
