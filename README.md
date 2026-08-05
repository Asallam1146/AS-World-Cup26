# AS World Cup26

A single-weight display Arabic/Latin typeface designed by Ahmed Sallam
(Sallam Type).

## Family

One static style only — confirmed by you and by the source file (which
contains a single master/instance, named "BOLD" in Glyphs, weightClass
900 in the original design).

Per Google Fonts convention for single-static-weight families, the
shipped binary is labeled:

| nameID | Value |
|---|---|
| Family (1/16) | AS World Cup26 |
| Subfamily (2/17) | Regular |
| usWeightClass | 400 |

This is standard practice for GF: a family with only one file is always
named "Regular" / weight 400 regardless of how visually bold the design
is, so font pickers and CSS don't misbehave. The design itself stays
exactly as drawn — only the metadata labels changed.

Note: an earlier `AS-WorldCup26_V2-Regular.otf` was found in Downloads
alongside the Bold file, but its outlines are ~95% different from the
Bold design (confirmed by comparing CFF charstrings) and it has no
matching master in the Glyphs source. Per your confirmation that this
font is one weight only, that file was excluded from this package.

## Status

1. **Naming — decided.** Final family name: **AS World Cup26**. Note the
   trademark risk with "World Cup" (FIFA-associated term) still stands —
   Google Fonts reviewers may flag or reject it on that basis. Proceeding
   per your call; worst case is a rename request during review, not
   necessarily an outright rejection of the design.
2. **Source — resolved.** `sources/AS-WC26.glyphspackage` matches the
   shipped binary (single BOLD master, weightClass 900 in Glyphs).
3. **Commercial withdrawal — in progress.** You're pulling the MyFonts
   listing and Behance post. Do this before filing the GitHub issue —
   reviewers do check that no proprietary version exists elsewhere for
   the same family.
4. **QA — not run.** Binaries should be run through
   [FontBakery](https://github.com/googlefonts/fontbakery)'s
   `googlefonts` profile before submission. Not run yet (native
   dependency `opentype-sanitizer` failed to build in this environment).
   You can run it locally: `pip install fontbakery[googlefonts]` then
   `fontbakery check-googlefonts fonts/ttf/*.ttf`.
5. **GitHub repo + CLA — next action, yours to do.** See steps below.

## How to actually submit (steps only you can do)

1. Create a new **public** GitHub repository (e.g. `AS-World-Cup26`)
   under your own GitHub account.
2. Copy everything in this folder into that repo and push it.
3. Sign the Google CLA at https://cla.developers.google.com using the
   same GitHub account.
4. Go to https://github.com/google/fonts/issues, choose the
   "Submit an OFL Font" issue template, and fill it in — it will ask for
   the repo URL, your name, and a description (you can reuse
   `DESCRIPTION.en_us.html`).
5. Submit. Google's reviewers (via FontBakery CI checks + human review)
   will respond on the issue, usually flagging anything that needs
   fixing — naming, missing metadata, glyph coverage, etc.

## What's in this folder

- `OFL.txt`, `AUTHORS.txt`, `CONTRIBUTORS.txt` — license and copyright,
  Ahmed Sallam.
- `sources/AS-WC26.glyphspackage` — original Glyphs source.
- `fonts/otf/ASWorldCup26-Regular.otf`, `fonts/ttf/ASWorldCup26-Regular.ttf`
  — corrected single-style binaries: family "AS World Cup26", Regular/400
  labeling per GF single-weight convention, OFL license string + URL
  embedded, designer/manufacturer metadata added.
