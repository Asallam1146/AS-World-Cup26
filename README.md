# AS Goal26

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
| Family (1/16) | AS Goal26 |
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

1. **Naming — renamed after rejection.** First submission as
   **AS World Cup26** (issue google/fonts#10780) was closed "not planned"
   by a GF reviewer: "World Cup 26" is a registered FIFA trademark for the
   2026 tournament, and GF can't publish a family whose name conflicts
   with it regardless of design origin. Renamed to **AS Goal26** — no
   tournament/organization reference, safe to resubmit.
2. **Source — resolved.** `sources/AS-WC26.glyphs` matches the shipped
   binary (single BOLD master, weightClass 900 in Glyphs).
3. **Commercial withdrawal — in progress.** You're pulling the MyFonts
   listing and Behance post. Confirm this is fully complete before
   re-checking the "no retail/pro version exists" box on the new issue.
4. **QA — not run.** Binaries should be run through
   [FontBakery](https://github.com/googlefonts/fontbakery)'s
   `googlefonts` profile before submission. Not run yet (native
   dependency `opentype-sanitizer` failed to build in this environment).
   You can run it locally: `pip install fontbakery[googlefonts]` then
   `fontbakery check-googlefonts fonts/ttf/*.ttf`.
5. **GitHub repo + CLA — done.** CLA signed. Repo needs the renamed
   binaries and updated docs pushed, then a new "Add Font" issue filed.

## How to actually submit (steps only you can do)

1. Push the renamed binaries (`ASGoal26-Regular.otf/.ttf`) and this
   updated README/DESCRIPTION to your existing repo, replacing the old
   `ASWorldCup26-Regular.*` files.
2. Verify "AS Goal26" is free of conflicts at namecheck.fontdata.com.
3. Go to https://github.com/google/fonts/issues → "Add Font" template →
   file a new issue with the same repo URL and the updated description,
   noting the old issue (#10780) and that this is a rename/resubmission.
4. Submit. Google's reviewers (via FontBakery CI checks + human review)
   will respond on the issue.

## What's in this folder

- `OFL.txt`, `AUTHORS.txt`, `CONTRIBUTORS.txt` — license and copyright,
  Ahmed Sallam.
- `sources/AS-WC26.glyphs` — original Glyphs source.
- `fonts/otf/ASGoal26-Regular.otf`, `fonts/ttf/ASGoal26-Regular.ttf`
  — corrected single-style binaries: family "AS Goal26", Regular/400
  labeling per GF single-weight convention, OFL license string + URL
  embedded, designer/manufacturer metadata added.
