# Stratégie de diffusion — le système

Ce dossier n'est pas une analyse. C'est le mode d'emploi de la diffusion à partir de
septembre 2026. Il remplace la méthode des six premiers mois.

**Le bilan de cette première période** — 62 publications, cinq plateformes, ce qui est établi
et ce qui ne l'est pas — est dans `../posts-reseaux-sociaux/post-mortem-diffusion.html`
(également en ligne : <https://claude.ai/code/artifact/be75c078-35a2-4816-ab3b-5c7b1ae87ef8>).
Toutes les données chiffrées citées ici en viennent.

## Les quatre pièces

| Fichier | À quoi il sert |
|---|---|
| `README.md` *(ce fichier)* | les objectifs et les décisions de cadrage |
| **`segmentation.md`** | **les trois couches, les neuf groupes retenus, la doctrine de contenu de chacune** |
| `calendrier.md` | la montée en charge, le ratio 2:1, le recyclage, Instagram |
| `kpi.md` | ce qu'on mesure à 6 mois, 1 an et 3 ans — et le tableau de bord mensuel |
| **`baseline-blog.md`** | **l'audience réelle du blog, février-juin 2026 — le point de départ chiffré** |
| `convention-utm.md` | le balisage des liens — **le prérequis de tout le reste** |
| `protocole-publication.md` | les règles par plateforme, et les trois plateformes écartées |
| `pipeline-articles.md` | les briefs d'articles, tirés de demandes réelles de lecteurs |

## Le périmètre, arrêté en septembre 2026

**Deux plateformes : Facebook et Instagram.** Strava, LinkedIn et WhatsApp sont écartés — les
raisons sont dans `protocole-publication.md`.

**Neuf groupes Facebook sur seize**, répartis en trois couches concentriques
(`segmentation.md`). Les sept autres sont abandonnés : 73 500 membres cumulés, 13
publications, 44 réactions.

---

## 1. Ce qu'on cherche, et comment on le compte

Trois objectifs, retenus par Julien. **Aucun n'est un objectif de volume** — ce sont trois
objectifs de conversion. Le trafic n'est donc pas la cible, c'est le tuyau.

| # | Objectif | Compteur | Où il se lit |
|---|---|---|---|
| **A** | **Audience propre** | abonnés newsletter | outil d'analytics + back-office newsletter |
| **B** | **Contributions** | messages reçus via `publier-ici` ou `julien@dans-le-desert.fr` | boîte mail |
| **C** | **UltraPack** | inscriptions venues du blog | analytics, clics sortants vers `ultrapack.fr` |

Et **un seul indicateur intermédiaire** : les **sessions depuis les réseaux sociaux**. Il ne
sert pas de score, il sert de diagnostic — si les objectifs ne bougent pas, il dit si le
problème est en amont (personne n'arrive) ou en aval (les gens arrivent et repartent).

### Ce qu'on ne compte plus

- Les réactions et les J'aime. Six mois de données ont montré qu'ils ne prédisent rien et ne
  convertissent rien : 1 849 réactions ont produit 7 clics mesurés.
- Le nombre d'abonnés Instagram, LinkedIn, Strava. Cette audience appartient aux plateformes.
  Le canal WhatsApp l'a prouvé : 7 contacts après un appel lancé devant des milliers de
  personnes.

---

## 2. Le mois zéro : mesurer avant d'optimiser

**Septembre-octobre 2026 ne sert pas à performer, il sert à établir une base.**

Aucune cible chiffrée ne peut être fixée aujourd'hui : on ne connaît ni le trafic actuel du
blog, ni son taux de conversion vers la newsletter. Les fixer maintenant reviendrait à
inventer.

Trois choses à faire avant toute optimisation :

1. **Appliquer la convention UTM** (`convention-utm.md`) à tous les liens sortants, sans
   exception.
2. **Relever quatre chiffres**, une fois par mois : sessions depuis les réseaux, abonnés
   newsletter, messages de contributeurs, clics sortants vers UltraPack.
3. **Ne rien conclure pendant deux mois.**

### L'ordre de grandeur, désormais connu

L'analytics du blog donne la base réelle (`baseline-blog.md`) : **1 640 visiteurs sur cinq
mois**, dont **1 145 venus des réseaux, à 93 % de Facebook**. Environ 25 visiteurs par
publication Facebook.

Un blog convertit 1 à 3 % de ses visiteurs en abonnés. À rythme constant, le trafic actuel
donnerait **2 750 visiteurs par an**, soit **27 à 82 abonnés**. L'objectif de 100 est donc à
portée, mais seulement en améliorant le rendement — pas en publiant davantage.

**Et le levier est identifié, avec un facteur 10 à la clé** : voir le point 3.

---

## 3. Le levier principal : la promesse retenue

Le croisement des réactions et de l'analytics du blog donne le résultat le plus utile de
tout le dossier :

| Article | Réactions réseaux | Visiteurs blog | Rendement |
|---|---|---|---|
| **005 — 5 erreurs** | 239 | **626** | **2,6 visiteurs par réaction** |
| **006 — 105 kg** | **1 185** | 301 | 0,25 |

**Facteur 10 d'écart.** « 105 kg » raconte tout : le lecteur n'a aucune raison de cliquer.
« 5 erreurs » donne **deux erreurs sur cinq et garde les trois autres** — une promesse
nommée, dénombrée, et tenue seulement sur le blog.

**Un post à lien doit retenir quelque chose de nommé et de dénombrable.** Pas « la suite sur
le blog », mais « les trois autres sont sur le blog ».

À quoi s'ajoute la contrainte de portée : sur LinkedIn, un lien en clair **divisait la portée
par seize**. Les plateformes taxent le lien sortant. **On ne peut donc pas maximiser la portée
et le clic sur le même post** — d'où deux natures de publication.

| | **Post de présence** | **Post de conversion** |
|---|---|---|
| Proportion | ~3 sur 4 | ~1 sur 4 |
| Lien | **aucun** | un seul, balisé UTM |
| Contenu | le récit **en entier** — le lecteur n'a rien à faire | un extrait, avec une raison explicite d'aller lire la suite |
| Ce qu'on en attend | de la portée, des commentaires, de la reconnaissance dans la communauté | des sessions et des conversions |
| Ce qu'on mesure | portée, commentaires | **clics balisés, et rien d'autre** |

Le post de conversion ne fonctionne que porté par les posts de présence qui l'ont précédé.
Publier un lien dans une communauté où l'on n'est pas reconnu, c'est ce qui a produit les
six zéros de l'archive.

---

## 4. Le cycle mensuel

Quatre temps, dans cet ordre. Le premier est non négociable : c'est la seule donnée propre
que le dossier précédent n'a jamais eue.

### ① Relever — à J+7, sur chaque post


Chaque publication est consignée dans `posts-reseaux-sociaux/` **sept jours après sa
parution**, pas six mois plus tard. Le template et les conventions sont déjà en place.

Sur un nouveau groupe, relever **avant de publier** : le nombre de membres, le débit de
publication, et le niveau d'engagement habituel des autres membres. Sans cette référence,
un chiffre est illisible — le dossier `course-a-pied` a coûté deux hypothèses fausses faute
de ce relevé.

### ② Revoir — une fois par mois, 30 minutes

Quatre questions, dans cet ordre :

1. Lequel des trois objectifs a bougé ?
2. Quelle surface a produit des sessions balisées ? *(pas des réactions — des sessions)*
3. Quelle surface n'a rien produit deux mois de suite ? → on arrête d'y publier.
4. Qu'est-ce que les commentaires ont demandé ? → ça alimente le pipeline.

### ③ Briefer — l'objectif choisit l'article

C'est le renversement demandé. On n'écrit plus un article puis on cherche où le poster.

**L'objectif qui stagne désigne le type d'article à écrire :**

| Objectif en retard | Ce qu'il faut écrire |
|---|---|
| **A — audience propre** | un article utile qui appelle un retour régulier : suivi de préparation, série |
| **B — contributions** | une interview, ou un article qui montre qu'un autre que Julien peut écrire ici |
| **C — UltraPack** | un article de terrain sur le sac, la nutrition, l'arbitrage poids/calories |

Le sujet précis, lui, sort du pipeline (`pipeline-articles.md`), qui est alimenté par les
demandes réelles des lecteurs.

### ④ Publier — selon le protocole

`protocole-publication.md` : quoi faire, où, et surtout ce qu'on ne fait plus.

---

## 5. Les décisions déjà prises

Elles découlent des données, pas d'une hypothèse. Elles s'appliquent dès maintenant.

- **Tout lien sortant est balisé.** Sans exception. C'est la seule raison pour laquelle six
  mois de diffusion Facebook sont définitivement illisibles.
- **Les liens Strava redeviennent cliquables.** Meilleure moyenne d'engagement du corpus
  (51 kudos par post), zéro conversion possible parce que l'adresse est écrite
  `dans-le-desert[point]fr`.
- **On arrête les canaux morts** : groupe *Course à pied* (1-2 réactions par post tous auteurs
  confondus), *Trail et running en Bretagne*, *Trail à la Réunion*.
- **On arrête les posts qui résument le blog.** Sept publications de ce type, de 4 à 11
  réactions, sur des groupes dont la taille varie d'un facteur cent. C'est le seul format
  dont l'échec soit prévisible.
- **On garde le diabète comme porte d'entrée.** Cinq plateformes, le même constat : c'est la
  ligne du diagnostic qui fait écrire les gens, jamais les kilomètres.

---

## 6. Ce que ce système ne prétend pas faire

Il ne dit pas où publier pour réussir. Quatre prédictions ont été posées à l'aveugle dans le
dossier précédent, les quatre ont échoué, et neuf explications ont été abandonnées en route.
**Rien ne permet d'anticiper le rendement d'une communauté avant d'y avoir publié.**

Ce système sert à autre chose : **mesurer proprement pour arrêter vite.** Le gain n'est pas
de mieux choisir à l'avance, il est de ne plus dépenser neuf publications dans des canaux
qui ne rendent rien.
