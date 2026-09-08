# dans-le-desert — Archive de contenu

Archive de tous les articles du blog **[dans-le-desert.fr](https://dans-le-desert.fr)** — le carnet de route de Julien Leclerc, marcheur d'ultra : Marathon des Sables, trails, route, préparation, matériel et tout ce qui gravite autour.

Ce dépôt n'est **pas un projet de code**. Il n'y a rien à installer, rien à compiler, rien à lancer. C'est un espace de stockage, pensé pour trois usages :

1. **Conserver** tout le contenu publié, et celui à venir, en un seul endroit.
2. **Consulter et retrouver** un article rapidement, sans passer par le site.
3. **Servir de base de rédaction** : le corpus est la matière première et la référence de ton pour écrire les prochains articles.

---

## Contenu du dépôt

| Fichier / dossier | Rôle |
|---|---|
| `charte-editoriale.md` | La charte éditoriale : identité, voix, ton, rubriques, règles de transparence. **À lire avant toute rédaction.** |
| `journal/` | Tous les articles, un fichier Markdown par article. |
| `CLAUDE.md` | Contexte destiné à Claude Code (mêmes règles, formulées pour l'outil). |
| `.claude/agents/copywriter.md` | Agent Claude spécialisé copywriting et conversion, cadré par la charte. |

---

## Les articles

| # | Date | Titre | Rubrique | Série |
|---|---|---|---|---|
| 001 | 2026-02-05 | [Du Sahara à la Namibie : Pourquoi je remets le couvert (et cette fois, avec des guêtres !)](journal/001-du-sahara-a-la-namibie.md) | Récit | — |
| 002 | 2026-02-19 | [Jordanie : Là où tout a commencé (mes premiers 100 km)](journal/002-jordanie-la-ou-tout-a-commence.md) | Récit | — |
| 003 | 2026-03-05 | [Préparation Namibie : Le \"jour sans fin\" à Manille](journal/003-preparation-namibie-le-jour-sans-fin.md) | Préparation | — |
| 004 | 2026-03-11 | [J-45 : Le nez dans le guidon](journal/004-j-45-le-nez-dans-le-guidon.md) | Récit | — |
| 005 | 2026-03-19 | [MDS : 5 erreurs à faire pour vivre un enfer](journal/005-5-erreurs-a-faire-pour-vivre-un-enfer.md) | Récit | — |
| 006 | 2026-03-26 | [105 kg, un diabète et une idée saugrenue](journal/006-105-kg-un-diabete-et-une-idee-saugrenue.md) | Récit | — |
| 007 | 2026-04-06 | [J-19 : Le point d’étape](journal/007-j-19-le-point-d-etape.md) | Préparation | — |
| 008 | 2026-04-22 | [Optimiser son sac : la chasse aux grammes](journal/008-optimiser-son-sac.md) | Préparation | — |
| — | 2026-04-24 | [Manille - Windhoek : 20 heures de vol](journal/manille-windhoek-20-heures-de-vol.md) | Récit | mds-namibie-2026 |
| 009 | 2026-04-27 | [Étape 1 : Euphorie, citron et "cuisine aux chiottes"](journal/009-etape-1-euphorie-citron-et-cuisine-aux-chiottes.md) | Course | mds-namibie-2026 |
| 010 | 2026-04-28 | [Étape 2.1 : 37 km de sable et une nuit au sommet](journal/010-etape-2-37-km-de-sable-et-une-nuit-au-sommet.md) | Course | mds-namibie-2026 |
| 011 | 2026-04-29 | [Étape 2.2 : Montagnes russes](journal/011-etape-2-2-montagnes-russes.md) | Course | mds-namibie-2026 |
| 012 | 2026-04-30 | [Étape 3 : Le sprint final](journal/012-etape-3-le-sprint-final.md) | Course | mds-namibie-2026 |
| 014 | 2026-05-08 | [MDS Namibie : Le bilan](journal/014-bilan.md) | Réflexion | mds-namibie-2026 |
| 015 | 06/01/2026 | [ET MAINTENANT ?](journal/015-et-maintenant.md) | Réflexion | mds-namibie-2026 |

**15 articles · ~8 700 mots**

Les articles marqués `mds-namibie-2026` forment une série qui se lit à la suite.

---

## Comment un article est stocké

Chaque fichier est du Markdown précédé d'un bloc de métadonnées (*frontmatter*) délimité par `---`.

```markdown
---
title: "Étape 1 : Euphorie, citron et cuisine aux chiottes"
date: 2026-04-27
description: "Le résumé qui sert d'accroche et de description SEO."
category: 'Course'
series: mds-namibie-2026
---

Le corps de l'article, en Markdown.
```

### Champs obligatoires

| Champ | Valeurs |
|---|---|
| `title` | Le titre de l'article |
| `date` | Format ISO : `2026-04-27` |
| `description` | 2 à 4 phrases, dans la voix du blog (sert d'accroche et de description SEO) |
| `category` | `Préparation`, `Récit`, `Équipement`, `Nutrition`, `Interview`, `Course`, `Hors-série`, `Réflexion` |

### Champs optionnels

`image`, `series`, et pour les comptes rendus de course : `stageNumber`, `weather`, `temperature`, `firstFinisherTime`, `myFinishTime`, `myRanking`, ainsi que `audio`, `audioTitle` et `audioDescription` pour les enregistrements de terrain.

Un champ optionnel non utilisé peut être laissé vide (`""`) ou simplement omis.

### Nommage des fichiers

`NNN-titre-en-minuscules.md`, numéroté dans l'ordre de publication. Le `013` n'existe pas et `manille-windhoek-20-heures-de-vol.md` n'est pas numéroté : ces trous sont volontaires, on ne renumérote pas pour les combler. Un nouvel article prend le numéro libre suivant.

---

## Ajouter un article

1. Lire `charte-editoriale.md` — surtout la voix, la longueur cible (500 à 1 200 mots) et la rubrique visée.
2. Lire deux ou trois articles existants de la même rubrique pour retrouver le ton.
3. Créer `journal/NNN-slug.md` avec le frontmatter complet.
4. Vérifier que le frontmatter est complet et que le fichier apparaît dans l'index ci-dessus.

---

## Points de vigilance

- **Les images et les fichiers audio ne sont pas stockés ici.** Les chemins `../../assets/…` et les noms de fichiers `audio:` renvoient vers des médias hébergés ailleurs ; ils sont conservés pour la fidélité du contenu mais ne s'ouvriront pas depuis ce dépôt.
- **`stageNumber` est le numéro d'étape de la course, pas celui de l'article** : étape 2.1 → `2`, étape 2.2 → `3`, étape 3 → `4`.
- **La date de l'article 015 est ambiguë** : `06/01/2026` sera lu comme le 1ᵉʳ juin par un analyseur de dates, alors que le format laisse penser au 6 janvier. À normaliser en ISO. Tous les autres articles utilisent déjà `AAAA-MM-JJ`.

---

## Le blog publié

Les articles de cette archive sont publiés sur **<https://dans-le-desert.fr>**.

L'archive et le site en ligne peuvent diverger légèrement (une image, une correction de dernière minute) : ce dépôt garde le contenu, le site gère la publication.
