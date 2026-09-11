# Strava

| | |
|---|---|
| Abonnés | **8**, au 2026-09-10 |
| Abonnements | 12 |
| Profil | `https://www.strava.com/athletes/145437319` *(lien donné dans `journal/007-j-19-le-point-d-etape.md`)* |

## ⚠️ Huit abonnés : ce que le dossier pourra et ne pourra pas dire

Avec huit abonnés, **aucun chiffre issu de cette plateforme ne sera interprétable**. Un seul
lecteur y représente 12,5 % de l'audience : la variance d'une personne dépasse tout signal
possible. Le même constat a conduit à ne pas consigner le canal WhatsApp (7 contacts).

La différence, et la raison pour laquelle ce dossier existe : **Strava n'est pas une plateforme
de publication, c'est un journal d'entraînement.** Ce qu'il peut documenter n'est donc pas la
diffusion, mais l'**usage** :

- les descriptions d'activité ont-elles servi à renvoyer vers le blog, ou sont-elles restées
  purement sportives ?
- l'entraînement raconté correspond-il à celui décrit dans les articles — 70 à 80 km par semaine
  visés, 50 réellement atteints selon `journal/007-j-19-le-point-d-etape.md` ?
- la préparation « 100 % sable » identifiée comme manquante dans le bilan
  (`journal/014-bilan.md`) apparaît-elle dans les activités ?

Ces éléments valent pour eux-mêmes, indépendamment des kudos.

## Ce que Strava mesure, et ne mesure pas

| | |
|---|---|
| **Kudos** | l'équivalent des J'aime. À consigner dans `j7_likes` |
| **Commentaires** | `j7_commentaires` |
| Vues | **non fournies** — `j7_vues` restera vide, au sens « non exposé » |
| Partages | sans objet — `j7_partages` restera vide |

Strava rejoint donc le profil Facebook parmi les surfaces **sans dénominateur** : on saura
combien de gens ont réagi, jamais combien ont vu.

## Arborescence

```
Strava/
└── profil/     AAAA-MM-JJ-slug.md
```

Le champ `type` prend ici des valeurs propres à la plateforme : `activite` (une sortie
enregistrée), `publication` (un post Strava sans activité). Le champ `titre` reprend le titre
donné à l'activité, qui est le seul élément éditorial visible dans le fil des abonnés.

## Rappel

Les conventions de `posts-reseaux-sociaux/README.md` s'appliquent — en particulier
**vide ≠ zéro**, distinction ici plus importante qu'ailleurs puisque les vues ne sont
structurellement pas fournies.

---

# Synthèse du dossier

**Trois publications, toutes dans le club Marathon des Sables.** Aucune sur le profil personnel
(8 abonnés), qui n'a pas été consigné faute de données interprétables.

| Date | Post | Kudos | 💬 |
|---|---|---|---|
| 15 mars | Présentation de la Namibie | 34 | 1 *(le sien)* |
| 8 avril | Dernière sortie avant le départ | 31 | 0 |
| 15 juin | Namibie 2026, résumé de course | **89** | 2 |

**Total : 154 kudos, 3 commentaires.** Moyenne par post : 51 — la plus élevée de toutes les
surfaces de l'archive, profil Facebook (9,9), Instagram (9,5) et LinkedIn (11) compris.

## Ce que le dossier établit

**Le club vaut infiniment plus que le profil.** 8 abonnés contre 89 kudos sur une seule
publication. La distinction reproduit celle du dossier Facebook entre profil et groupes, avec
le même enseignement : **l'audience propre de Julien est négligeable partout ; ce qui porte ses
publications, ce sont les communautés auxquelles il accède.**

**Le post de présentation, mort deux fois sur Facebook, fonctionne ici.** Le même contenu a
produit 0 réaction dans deux groupes Facebook totalisant 88 500 membres, et 34 kudos dans ce
club. Ni la taille de l'audience ni le texte n'expliquent l'écart.

**Le récit d'après-course triple les posts de suivi** (89 contre 31 et 34) — même écart que sur
toutes les autres plateformes.

## ⚠️ Deux limites majeures

**Le nombre de membres du club n'a pas été relevé.** Sans lui, et sans le niveau d'engagement
habituel des autres publications, ces chiffres ne sont pas pleinement interprétables. Le
dossier Facebook a montré ce que coûte l'absence de cette référence : deux hypothèses fausses
sur le groupe *Course à pied*, réglées d'un coup d'œil au niveau de référence.

**Le kudos n'est pas la réaction Facebook.** Son coût social est plus faible, et sa réciprocité
entre membres d'un club plus forte. Les 89 kudos du 15 juin ne valent pas 89 lecteurs
attentifs, et ne se comparent pas terme à terme aux 81 réactions d'un groupe Facebook.

## ⛔ La limite structurelle : Strava n'autorise pas les liens

**Strava interdit la publication de liens.** Les adresses écrites `dans-le-desert[point]fr`
ne sont pas une maladresse : c'est un contournement de cette interdiction.

- 15 mars : `dans-le-desert[point]k-lif[point]com`, répété à l'identique en commentaire ;
- 8 avril : aucune mention du blog ;
- 15 juin : `dans-le-desert[point]fr`.

**Conséquence : aucune conversion n'est possible depuis cette plateforme, et aucune ne le
sera.** Ce n'est pas un réglage à corriger, c'est une propriété du canal.

La meilleure moyenne d'engagement du corpus (51 kudos par publication) est donc adossée à la
seule surface d'où personne ne peut arriver sur le blog — et rien ne peut changer cela.

**C'est la raison pour laquelle Strava est écarté de la stratégie à partir de septembre 2026**
(voir `strategie/segmentation.md`). L'arbitrage n'oppose pas l'engagement au trafic : il
constate qu'un canal sans lien ne peut servir aucun des trois objectifs retenus.
