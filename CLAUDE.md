# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Purpose

This is **not a code project**. It is the archive of the blog *dans-le-desert* (<https://dans-le-desert.fr>) — Julien Leclerc's French-language carnet de route as an ultra-endurance walker-runner: desert races, trails, road, preparation, gear, and everything around them.

Every article published on the blog, and every article to come, is stored here as Markdown. The archive exists so the corpus is quick to consult, quote and search — and so it can serve as the raw material and reference voice when drafting the next article.

The first fifteen articles cover the Marathon des Sables Namibie 2026, which is now over. The blog has since broadened: the desert stays the fil rouge and the name, but any race of the same family belongs here. Do not treat Namibia as the subject.

Two things live here:

- `charte-editoriale.md` — the editorial charter. **Read it in full before writing or reworking any article.** It is the spec for tone, length, structure, and what the blog refuses to be.
- `journal/*.md` — the articles, oldest first.

There is nothing to build, lint, run or test. Do not add tooling, `package.json`, scripts or CI unless explicitly asked.

## Using the archive to write

The existing articles are the voice sample. Before drafting, read a few whose `category` matches what you're writing (`Course` for a stage report, `Préparation` for gear and training, `Récit` for a backstory) — the charter describes the register, the corpus demonstrates it.

Recurring material worth knowing, all of it already narrated somewhere in `journal/`: the gaiters fiasco in Morocco, the 12.5 kg "sac de la kiffance" trimmed to 6.5 kg, training in Manila's humidity, managing **type 2 diabetes** on the course, the road from 105 kg, the walker-who-also-runs stance, and the running mate met in Jordan. Reuse the facts; don't retell an anecdote a previous article already owns.

Julien is an expat in Manila, an entrepreneur, and diabetic (type 2 — the articles never state the type, so do not write "type 1").

## Writing rules that come from the charte

The constraints most easily violated:

- **French only.** Spoken register, written the way one talks.
- **500–1 200 words.** Existing articles run 500–970.
- **Three voices in priority order**: the anti-hero (self-deprecating, funny) first, the reflective voice second, the explorer (Namibian landscape) third.
- **Structure**: a strong opening scene, image or question → the story → a *chute* (a reflection or a joke that lands). H2 subheads are used, but sparingly, and as hooks rather than descriptive labels.
- **Never** performance logs (splits, rankings as bragging, VO2max), or complaint diaries.
- Practical guides (gear, packing, mistakes, nutrition) are welcome, but written **from lived experience, never from authority**: « voilà ce que j'ai raté » rather than « voilà ce qu'il faut faire ». The charter has a table of the exact phrasings to use and avoid.
- Sponsors (k-lif.com), UltraPack and affiliate links are allowed and must be **explicitly flagged** — never slipped into a race report. Only gear actually used on the ground gets mentioned, and criticism of a partner's product stays permitted.
- Emojis are allowed as punctuation, rarely.

## File naming

`NNN-slug-in-kebab-case.md`, numbered in publication order. Gaps are intentional (`013` does not exist) and `manille-windhoek-20-heures-de-vol.md` is unnumbered — do not renumber to close either. A new article takes the next free number.

## Frontmatter

Articles are stored with a consistent frontmatter block. Nothing here validates it, so match the existing articles exactly rather than inventing fields.

Always present: `title`, `date`, `description` (the SEO/teaser blurb, in the blog's voice, 2–4 sentences), and `category`, one of `Préparation`, `Récit`, `Équipement`, `Nutrition`, `Interview`, `Course`, `Hors-série`, `Réflexion`.

There is **no `status` field** — it was removed from every article. Publication state is not tracked in this archive. Do not reintroduce it when creating an article.

Optional, and safe to leave as `""`: `image`, `stageNumber`, `weather`, `temperature`, `firstFinisherTime`, `myFinishTime`, `myRanking`, `audio`, `audioTitle`, `audioDescription`, `series`.

Race reports (`category: 'Course'`) carry the full race block: `stageNumber`, `weather`, `temperature`, `firstFinisherTime`, `myFinishTime` (formatted `"4h11 (+1h31)"`, gap to the winner in parentheses), `myRanking`, `series: mds-namibie-2026`.

Two quirks in the existing data, worth not copying:

- `stageNumber` is the **race** stage index, not the article number: étape 2.1 → 2, étape 2.2 → 3, étape 3 → 4.
- `015` dates itself `06/01/2026`, which any `Date` parser reads as 1 June, not 6 January. Use ISO (`2026-04-27`) everywhere.

Image paths (`../../assets/…`) and `audio` filenames point at media hosted elsewhere, not stored here — they are recorded for fidelity and will not resolve locally.
