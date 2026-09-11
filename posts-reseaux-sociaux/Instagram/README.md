# Instagram

Le compte Instagram a été **lancé le 11 mars 2026**, le même jour que l'ouverture publique du
blog — l'article `journal/004-j-45-le-nez-dans-le-guidon.md` l'annonce explicitement
(« Aujourd'hui, je lance officiellement mon blog et mon profil Instagram »).

## Le compte, au 2026-09-10

| | |
|---|---|
| Publications | **12** |
| Abonnés | **76** |
| Abonnements | 115 |

**Bio :**

> Père · Chef d'entreprise · Marcheur de déserts
> 🏜️ Jordanie · Sahara · Namibie

Deux liens en bio : le blog et UltraPack.

### Ce que ces chiffres impliquent pour la lecture du dossier

**76 abonnés.** C'est l'audience propre la plus petite de toute l'archive, de très loin — les
groupes Facebook consignés vont de 1 900 à 187 000 membres, et le profil Facebook de Julien
compte au minimum quelques centaines d'amis (7 posts y ont récolté jusqu'à 23 réactions).

Conséquence directe : **les chiffres bruts d'Instagram ne se comparent pas à ceux de Facebook.**
Un post à 20 réactions ici représenterait plus d'un quart de l'audience — proportion jamais
atteinte sur aucune surface Facebook. Toute lecture doit se faire **en proportion des 76
abonnés**, pas en valeur absolue.

**Plus d'abonnements (115) que d'abonnés (76).** Le compte suit plus qu'il n'est suivi : profil
de compte jeune, en phase de construction, et non de compte établi.

**Douze publications en six mois**, du 11 mars au 10 septembre 2026 — soit deux par mois. À
comparer aux 45 publications Facebook sur la même période. Instagram a reçu environ un quart
de l'effort de diffusion.

**Deux liens en bio (blog + UltraPack).** C'est le seul endroit de l'archive où un chemin de
conversion permanent existe : sur Facebook, chaque lien meurt avec son post. À garder en tête
si les vues Instagram s'avèrent significatives — un compte de 76 abonnés peut malgré tout
alimenter un lien pérenne.

## Arborescence

```
Instagram/
└── profil/     AAAA-MM-JJ-slug.md
```

Pas de sous-dossiers par surface, contrairement à Facebook : Instagram n'a pas de groupes. Le
format se note dans le champ `type` (`photo`, `carrousel`, `reel`, `story`).

## Ce qui change par rapport à Facebook

**Les vues existent ici.** Un profil Facebook personnel n'expose aucune portée — d'où un
`j7_vues` systématiquement vide sur les 45 posts du dossier Facebook. Instagram affiche des
vues (ou impressions, ou comptes atteints selon le type de contenu et le type de compte). Si
elles sont disponibles, **elles doivent être relevées** : ce sera la première fois de l'archive
qu'un dénominateur est mesurable, et donc la première fois qu'un taux d'engagement pourra être
calculé plutôt qu'un simple classement.

**Les abonnés sont connaissables.** Le champ `abonnes` était vide partout côté Facebook, faute
de connaître la taille de l'audience au moment de chaque post. Si le nombre d'abonnés à une
date donnée est retrouvable, il est à consigner — il permettra de distinguer une progression
d'une stagnation.

**Les partages ne sont pas la même chose.** Sur Instagram, le relais passe surtout par les
stories et les envois en message privé. À noter dans `j7_partages` si le chiffre est fourni,
en précisant en `Notes` de quelle métrique il s'agit.

## Republications vers Facebook

Au moins un post Instagram a été republié sur le profil Facebook :
`Facebook/profil/2026-05-09-4-jours-cest-fait.md`, marqué `crosspost: mds-namibie-cest-fait`.

Le champ `crosspost` doit être renseigné des deux côtés pour chaque contenu partagé entre
plateformes : c'est ce qui permettra de comparer Instagram et Facebook à contenu égal, comme
l'archive l'a fait entre le profil et les groupes Facebook.

## Champs supplémentaires, propres à Instagram

Instagram fournit des métriques que Facebook n'expose pas. Quatre champs s'ajoutent au
frontmatter standard pour ce dossier :

| Champ | Ce qu'on y met |
|---|---|
| `j7_enregistrements` | Enregistrements (saves) |
| `j7_visites_profil` | Visites du profil générées par le post |
| `j7_clics_lien` | **Appuis sur des liens externes** — la seule mesure de conversion vers le blog de toute l'archive |
| `j7_nouveaux_abonnes` | Abonnés gagnés grâce au post |

Le détail complet fourni par Instagram (répartition abonnés / non-abonnés, provenance des vues,
activité du profil) se consigne dans une section **Statistiques détaillées** du corps du
fichier, sans chercher à tout faire entrer dans le frontmatter.

⚠️ **Ces statistiques sont cumulées, pas à J+7.** Instagram affiche des totaux depuis la
publication. Pour des posts vieux de plusieurs mois, `j7_vues` et les autres compteurs sont donc
des cumuls sur toute la durée de vie du post — plus généreux qu'un vrai relevé à sept jours.
Le nom des champs est conservé pour l'homogénéité de l'archive, mais **ne pas comparer ces
valeurs à un relevé J+7 fait proprement par la suite**.

## Rappel de méthode

Les conventions de `posts-reseaux-sociaux/README.md` s'appliquent intégralement — en
particulier **vide ≠ zéro**, et les stats de l'import rétroactif relevées le 2026-09-10 sont
signalées dans les `Notes` de chaque fichier.

---

# Synthèse du dossier — périmètre MDS Namibie 2026

**Dix publications consignées**, du 11 mars au 12 mai 2026. Le compte en affiche douze au
total : deux manquent au dossier (voir « Lacunes » ci-dessous).

| Date | Post | Format | Vues | ❤️ | Taux | Clics | +Ab. |
|---|---|---|---|---|---|---|---|
| 11 mars | Jordanie · Sahara *(lancement)* | photos désert | 150 | 16 | **11,3 %** | **3** | **3** |
| 14 mars | Je marche, c'est un choix | carrousel texte | 114 | 3 | 2,6 % | 0 | 0 |
| 18 mars | Manille, 7h30 | photos ville | 132 | 6 | 5,3 % | 0 | 0 |
| 20 mars | 5 erreurs | carrousel texte | 109 | 5 | 7,3 % | **1** | 0 |
| 27 mars | Paysages du Sahara | photos désert | 117 | 11 | 10,3 % | 0 | 0 |
| 20 avril | Makati, run matinal | photos ville | 143 | 9 | 7,7 % | 0 | 0 |
| 24 avril | 3 escales, 3 continents | photo unique | 124 | 9 | 7,3 % | 0 | 0 |
| 26 avril | Swakopmund, J-1 | photos | **155** | 12 | 7,7 % | 0 | 0 |
| 11 mai | Récap MDS Namibie | photos désert | **158** | 13 | 8,2 % | **2** | **1** |
| 12 mai | Safari à Etosha | photos animaux | **101** | 11 | **10,9 %** | 0 | 0 |

**Totaux : 1 303 vues, 95 J'aime, 5 commentaires, 1 partage, 6 clics vers le blog,
4 abonnés gagnés.**

## Ce que ce dossier établit

**1. La portée est stable, l'engagement ne l'est pas.**
Les vues tiennent entre 101 et 158 (facteur 1,6) quel que soit le contenu ; le taux
d'engagement va de 2,6 % à 11,3 % (facteur 4,3). Sur un compte à audience propre, le contenu
ne décide pas de *combien de gens voient*, mais de *combien réagissent*.

C'est l'exact inverse du dossier Facebook, où un texte identique allait de 0 à 81 réactions
selon le groupe, sans qu'aucune variable relevée ne l'explique.

**2. Les hashtags n'apportent rien.**
Le seul post dont Instagram détaille la source (20 mars) montre **2 vues issues des hashtags
sur 109**, pour dix-neuf hashtags. Le post sans aucun hashtag (20 avril) réalise le troisième
meilleur score de vues du compte. Les listes de dix-neuf à vingt-et-un mots-clés recopiées
d'un post à l'autre sont sans effet mesurable.

**3. Un non-abonné ne réagit jamais.**
Depuis le 27 mars, **100 % des interactions viennent des abonnés** sur chaque post, sans
exception — alors que les non-abonnés représentent 13 à 36 % des vues. Ils regardent et
repartent.

**4. La conversion est marginale et concentrée.**
Six clics vers le blog en deux mois, dont trois sur le post de lancement. Six posts sur dix
comportaient un appel au blog ; ils totalisent ces six clics. Quatre abonnés gagnés, dont
trois au lancement.

**5. L'audience suit Julien, pas le sujet.**
Le post le plus engageant après le lancement est un carrousel d'animaux sans rapport avec la
course (10,9 %), devant le récap du MDS publié la veille (8,2 %). Avec 76 abonnés
majoritairement proches, ce compte n'est pas une audience de pratiquants.

## Ce que ce dossier ne permet pas d'établir

Aucune caractéristique de contenu ne prédit l'engagement de façon fiable. Trois lectures ont
été avancées puis fragilisées par la publication suivante :

- *les carrousels à texte incrusté font moins bien que les photos* — démenti par le post du
  20 mars (carrousel texte, 7,3 %) devant celui du 18 mars (photos, 5,3 %) ;
- *le sujet photographié trie les résultats, le désert engage plus que la ville* — démenti par
  le post du 20 avril (ville, 7,7 %) ;
- *la part de non-abonnés décroît continûment* — démenti par le post du 24 avril (remontée à
  36,3 %).

Dix publications ne suffisent pas. **Le seul énoncé robuste du dossier est négatif : les
hashtags ne servent à rien.**

## Comparaison Instagram / Facebook

Un seul couple à date identique et texte identique existe dans l'archive — le récap du 11 mai :

| | Instagram | Facebook *(profil)* |
|---|---|---|
| Vues | 158 | **inconnues** |
| J'aime | **13** | 6 |
| Clics vers le blog | **2** | **inconnus** |

Instagram fait deux fois les réactions du profil Facebook, et c'est la **seule plateforme de
l'archive où la conversion vers le blog soit mesurable**. Les 45 publications Facebook
n'offrent aucun moyen de savoir si quiconque a jamais cliqué.

## Lacunes du dossier

- **Post #9 non transmis** : situé entre le 26 avril et le 11 mai, donc pendant ou juste après
  la course.
- **Une douzième publication** figure au compteur du profil sans être consignée ici — hors
  périmètre MDS Namibie, vraisemblablement postérieure.
- **Deux dates approximatives** : 20 avril (Makati) et 12 mai (safari), déduites faute de
  repère dans le texte.
- **Le champ `abonnes` est vide partout** : le nombre d'abonnés à la date de chaque post n'est
  pas connu. Seul le total actuel l'est (76 au 2026-09-10).
