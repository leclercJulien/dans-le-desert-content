# posts-reseaux-sociaux/

Le journal des publications réseaux sociaux. **Un fichier = un post.**

> **📊 Le bilan de ce dossier est dans `post-mortem-diffusion.html`** — 62 publications, cinq
> plateformes, ce qui est établi et les neuf explications abandonnées en route. Version en
> ligne : <https://claude.ai/code/artifact/be75c078-35a2-4816-ab3b-5c7b1ae87ef8>
>
> **La suite se joue dans `strategie/`**, qui remplace la méthode des six premiers mois.

Ce dossier n'est pas le blog : la charte éditoriale ne s'y applique pas, et ce n'est
jamais un échantillon de voix. Il sert de base de décision sur la diffusion — quel
format, quelle accroche, quel réseau, quel moment — pas de matière première pour écrire.

## Arborescence

La plateforme et la surface sont portées par le chemin, pas par le nom de fichier :

```
posts-reseaux-sociaux/
├── Facebook/
│   ├── profil/                     posts publiés sur le profil personnel
│   └── groupes/
│       └── <nom-du-groupe>/        un dossier par groupe
├── Instagram/
├── LinkedIn/
└── WhatsApp/
```

Nom de fichier : `AAAA-MM-JJ-slug.md` — par exemple
`Facebook/profil/2026-03-26-105-kg-diabete.md`.

Deux posts publiés le même jour sur la même surface se distinguent par leur slug ;
si vraiment nécessaire, suffixer `-2`.

## Les champs

| Champ | Ce qu'on y met |
|---|---|
| `titre` | Un intitulé court **pour s'y retrouver**, pas le texte du post |
| `plateforme` | `facebook`, `instagram`, `linkedin`, `whatsapp`, `strava`, `threads`, `x`, `youtube`, `tiktok` — redondant avec le chemin, gardé pour que le fichier se lise seul |
| `surface` | `profil`, `groupe`, `page` |
| `groupe` | Nom du groupe Facebook quand `surface: groupe`. Vide sinon |
| `type` | `texte`, `photo`, `carrousel`, `video`, `reel`, `story`, `lien` |
| `date` | Date de publication, **toujours en ISO** : `2026-03-26` |
| `url` | Lien vers le post. Vide s'il est supprimé ou introuvable |
| `audience` | Facebook : `public`, `amis`, `amis-sauf`, `personnalise`. Détermine si le post pouvait être partagé au-delà du cercle — un post en `amis` n'est pas comparable à un post `public` |
| `crosspost` | Slug partagé quand **le même contenu** part sur plusieurs surfaces (profil + 3 groupes, ou Facebook + LinkedIn). C'est ce qui permet de comparer à contenu égal. Vide sinon |
| `article` | L'article du journal que le post relaie : `journal/006-105-kg-un-diabete-et-une-idee-saugrenue.md`. Vide si le post ne renvoie nulle part |
| `campagne` | `k-lif`, `ultrapack`, `blog`, `perso`… ce que le post sert. Vide si rien |
| `abonnes` | Abonnés / membres du groupe **au moment du post**. Sert à relativiser les chiffres dans le temps. Vide si inconnu |

## Les stats

| Champ | Ce qu'on y met |
|---|---|
| `j7_vues` | Vues / impressions / portée, selon ce que donne la plateforme |
| `j7_likes` | Likes, réactions, kudos (Strava) |
| `j7_commentaires` | Commentaires |
| `j7_partages` | Partages, repartages |
| `j7_complet` | `true` si les 7 jours sont passés. `false` pour un post trop récent |

**Vide ≠ zéro.** Un champ laissé vide signifie « la plateforme ne donne pas cette
information ». `0` signifie « mesuré, et c'est zéro ». Ne jamais confondre les deux :
un profil personnel Facebook ne donne pas de vues, ce n'est pas pour autant que
personne n'a vu le post.

Un post de moins de 7 jours se consigne quand même : `j7_complet: false`, stats vides,
à compléter ensuite.

`j7_complet: false` sert aussi au cas inverse : un post ancien dont les compteurs n'ont
pas encore été relevés. La distinction se lit dans les `Notes`. Tant qu'il est à `false`,
le fichier ne compte pas dans une comparaison.

### Import rétroactif de septembre 2026

Les posts consignés lors du premier import portent des chiffres relevés **le
2026-09-10**, et non exactement à J+7 — les relevés d'époque n'existaient pas. Ils sont
traités comme des J+7 faute de mieux, et chaque fichier concerné le signale dans ses
`Notes`. Conséquence à ne pas oublier : ces chiffres sont **majorés** par rapport à un
vrai J+7, et d'autant plus que le post est ancien. Ils se comparent entre eux, pas avec
des relevés faits proprement à J+7 par la suite.

## Lire les chiffres d'un groupe

Deux références sont nécessaires avant d'interpréter le score d'une publication de groupe.
Sans elles, un chiffre ne veut rien dire — l'archive en porte deux démonstrations coûteuses.

- **Le niveau d'engagement habituel du groupe.** Le groupe *Course à pied* (17 300 membres)
  plafonne à 1 ou 2 réactions par post, tous auteurs confondus : les zéros de Julien y sont
  la norme, pas une sanction.
- **Le débit de publication.** Le groupe *Bref, je fais du trail...* reçoit une cinquantaine
  de posts par jour : ses 100 300 membres ne se convertissent jamais en attention, et une
  publication y disparaît en quelques heures.

Le membre utile n'est donc pas le nombre d'inscrits, mais le rapport entre l'audience et le
débit quotidien. Ces deux relevés se notent dans le `README.md` de chaque dossier de groupe.

### Ce que les quatre groupes donnent, une fois le débit connu

Relevés du 2026-09-10 :

| Groupe | Membres | Débit | Meilleur score de Julien |
|---|---|---|---|
| Running *(public)* | 71 200 | **aucun post le mois écoulé** | **725** ❤️ |
| Marathon des Sables *(privé)* | 12 100 | **~2 posts / mois** | 72 ❤️ |
| Bref, je fais du trail *(public)* | 100 300 | **~50 posts / jour** | 20 ❤️ |
| Course à pied *(privé)* | 17 300 | *non relevé*, groupe inerte | 0 ❤️ |

Le classement des résultats est **exactement l'inverse** du classement des débits. Les deux
groupes les plus calmes produisent les deux meilleurs scores ; le groupe le plus grand, noyé
sous cinquante publications par jour, arrive avant-dernier.

L'explication tient en une phrase : **dans un groupe calme, chaque publication est vue par
presque tout le monde.** Un groupe de 71 200 membres où personne ne publie est le meilleur
canal possible ; un groupe de 100 300 membres où tout le monde publie n'en est pas un.

⚠️ **Cette lecture a été testée, et réfutée.** Le groupe *Trail je suis addict* (97 900
membres, ~12,8 posts/jour) est le jumeau de *Bref, je fais du trail...* (100 300 membres,
~50 posts/jour) sur tout sauf le débit. À contenu identique et même jour, il devait produire
environ quatre fois plus. Il a produit **3 réactions contre 5**. Le débit n'explique pas les
écarts de l'archive ; il peut tout au plus plafonner la visibilité.

**Le relevé du débit reste utile** — il dit ce qu'un groupe peut offrir au mieux — mais il ne
sert pas à prédire un résultat.

## Ce qui n'a pas besoin d'être demandé

**Aucun post n'a jamais été boosté.** Toutes les portées de ce dossier sont organiques.

**Facebook / profil ne donne pas de vues.** `j7_vues` est vide sur toute cette surface,
définitivement — ce n'est pas une donnée manquante à aller chercher. Les posts de profil
se jugent donc à l'engagement brut (réactions, commentaires, partages), sans dénominateur :
on peut les classer entre eux, pas calculer un taux d'engagement.

## Le corps

Trois sections, seule la première est obligatoire :

- **Contenu** — le texte du post tel que publié, hashtags compris. C'est là qu'on lit
  ce qui accroche : première ligne, longueur, ton, présence d'une question.
- **Média** — ce qu'on voit sur la photo ou la vidéo, en une ligne.
- **Notes** — heure de publication, incident (post supprimé par l'algorithme, portée
  effondrée), ressenti.

Copier `_template.md` pour créer un fichier.
