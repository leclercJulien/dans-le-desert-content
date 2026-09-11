# Convention UTM — balisage des liens sortants

**Règle unique : aucun lien vers le blog n'est publié sans balisage.** C'est ce qui manquait
aux 62 publications de `posts-reseaux-sociaux/`, et c'est la seule raison pour laquelle
45 publications Facebook sont définitivement non mesurables.

## Le format

```
https://dans-le-desert.fr/journal/<article>/?utm_source=<plateforme>&utm_medium=<surface>&utm_campaign=<article>&utm_content=<lieu-precis>
```

| Paramètre | Ce qu'on y met | Valeurs |
|---|---|---|
| `utm_source` | la plateforme | `facebook` · `instagram` · `linkedin` · `strava` |
| `utm_medium` | le type de surface | `groupe` · `club` · `profil` · `bio` · `commentaire` |
| `utm_campaign` | l'article visé, en kebab-case | `optimiser-son-sac`, `105-kg-diabete` |
| `utm_content` | **le lieu précis** | slug du groupe : `du-trail-et-puis-cest-tout` |

`utm_content` est le paramètre décisif. C'est lui qui dira **quel groupe amène des lecteurs**
— information qu'aucune donnée de réaction ne fournit, et qu'aucun des six derniers mois ne
permet de reconstituer.

## Exemples

```
# Post dans un groupe Facebook
https://dans-le-desert.fr/journal/008-optimiser-son-sac/?utm_source=facebook&utm_medium=groupe&utm_campaign=optimiser-son-sac&utm_content=marathon-des-sables

# Lien en commentaire sur LinkedIn
https://dans-le-desert.fr/journal/006-105-kg.../?utm_source=linkedin&utm_medium=commentaire&utm_campaign=105-kg-diabete&utm_content=profil

# Lien en bio Instagram, changé à chaque nouvel article
https://dans-le-desert.fr/journal/008-optimiser-son-sac/?utm_source=instagram&utm_medium=bio&utm_campaign=optimiser-son-sac&utm_content=profil

# Publication dans le club Strava — le lien doit être cliquable
https://dans-le-desert.fr/journal/009-etape-1.../?utm_source=strava&utm_medium=club&utm_campaign=recit-namibie&utm_content=marathon-des-sables
```

## Cohérence avec l'existant

Le blog utilise déjà des UTM dans l'autre sens — vers k-lif et UltraPack :

```
https://ultrapack.fr/?utm_source=dansledesert&utm_medium=blog&utm_campaign=softlaunch_sept26&utm_content=article_cappadoce_perou_islande
```

Même logique, sens inverse. `utm_source` désigne toujours **d'où vient le lecteur**.

## Les liens sortants du blog aussi

Pour mesurer l'objectif **C** (inscriptions UltraPack), les liens du blog vers `ultrapack.fr`
doivent porter l'article d'origine dans `utm_content` — pratique déjà en place, à
systématiser sur les encarts à venir :

```
https://ultrapack.fr/?utm_source=dansledesert&utm_medium=blog&utm_campaign=encart&utm_content=article-008-optimiser-son-sac
```

C'est ce qui dira **quel article vend UltraPack**, et donc lesquels méritent un encart.

## Trois pièges à éviter

**Le raccourcissement n'est pas nécessaire — et un raccourcisseur public est déconseillé.**

Contrairement à une idée reçue, **les UTM survivent à un raccourcisseur** : bit.ly redirige
vers l'URL complète, paramètres compris, et l'analytics les lit normalement. Ce qui se perd,
c'est le *referrer* — que les UTM remplacent précisément.

Mais sur les deux plateformes retenues, **le problème de longueur ne se pose pas** :

- **Facebook** remplace l'URL par une carte d'aperçu. L'URL peut même être **supprimée du
  texte une fois la carte chargée** : le post reste propre, la carte reste cliquable et
  pointe vers l'adresse balisée.
- **Instagram** met le lien en bio, dans un champ dont la longueur est invisible.

Si un lien court est malgré tout souhaité, **le faire sur son propre domaine** :
`dans-le-desert.fr/go/optimiser-sac` en redirection vers l'URL balisée. Astro gère les
redirections nativement. Trois avantages : le domaine reste visible (confiance), aucune
dépendance à un tiers, et les clics deviennent comptables indépendamment de l'analytics.

**À éviter dans tous les cas : un raccourcisseur public à domaine générique.** Pas pour
l'attribution, qui fonctionne — mais parce qu'un lien opaque publié dans un groupe Facebook
modéré, où Julien est un invité sous condition, est exactement le type de signal qui attire
la modération.

**Ne pas mettre d'UTM sur les liens internes au blog.** Un lien d'un article vers un autre
article balisé écrase la source d'origine dans la session : le lecteur venu de Facebook
devient un lecteur venu du blog.

**Un lien par post.** Deux liens balisés différemment dans la même publication rendent
l'attribution ambiguë, et les données de l'archive ont montré qu'un post à deux appels ne
convertit pas mieux.

## Où le noter

Le champ `url` du frontmatter de chaque fichier de `posts-reseaux-sociaux/` reçoit **le lien
balisé tel que publié**. C'est ce qui permettra, au relevé mensuel, de rapprocher les
sessions de l'analytics des publications qui les ont produites.
