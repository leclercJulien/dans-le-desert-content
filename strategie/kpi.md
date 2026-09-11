# KPI — ce qu'on mesure, et à quel horizon

Trois horizons, trois jeux d'indicateurs. **Chaque KPI répond à une seule question**, et
aucun ne se lit isolément de son horizon : un bon chiffre à six mois peut parfaitement
accompagner un échec à trois ans.

Tous les relevés se font **à J+7** pour les publications, **mensuellement** pour le blog.

---

## Horizon 6 mois — interaction et trafic

> *« Générer de l'interaction (like, commentaire) et augmenter l'audience vers le blog. »*

| # | KPI | Comment on le lit | Base de départ |
|---|---|---|---|
| **1** | **Réactions moyennes par publication, par couche** | mesure la justesse du contenu pour la couche — jamais comparer une couche à une autre | C1 : 34 · C2 : 15-46 · C3 : 47-363 |
| **2** | **Commentaires par publication, par couche** | **l'indicateur de qualité**, plus fiable que les réactions : commenter coûte plus que cliquer | C1 : 7,2 · C2 : 5,0 · C3 : 8,6 |
| **3** | **Sessions blog issues des réseaux** *(balisées UTM)* | le seul chiffre qui compte pour l'objectif « audience vers le blog » | **~1 145 visiteurs sur 5 mois**, dont 93 % Facebook |
| **4** | **Visiteurs par publication Facebook** | l'efficacité réelle d'un post | **~25** |
| **4bis** | **Visiteurs par réaction** | ⭐ le rendement de conversion — voir `baseline-blog.md` | **005 : 2,6 · 006 : 0,25** |
| **5** | **Groupes actifs** | discipline d'arrêt : un groupe sous le seuil deux mois de suite sort de la rotation | 9 (+1 en sursis) |

**Ce que le KPI 3 apporte n'est pas le volume, c'est l'attribution.** Le volume était déjà
connu de l'analytics du blog — 1 145 visiteurs venus des réseaux sur cinq mois. Ce qu'aucune
donnée existante ne dit, c'est **quel groupe** les a envoyés. C'est la seule raison d'être du
dispositif UTM, et elle suffit à le justifier.

**Le KPI 4bis est le plus important des cinq.** L'archive montre un rapport de 1 à 10 entre
deux articles : « 5 erreurs » rapporte 2,6 visiteurs par réaction, « 105 kg » 0,25. Classer
les publications sur les réactions conduit donc à préférer exactement le mauvais contenu
quand l'objectif est le trafic.

### Seuil d'arrêt d'un groupe

Un groupe sort de la rotation s'il fait, **deux publications consécutives**, moins de la
moitié de la moyenne de sa couche. Le seuil se recalcule chaque trimestre.

---

## Horizon 1 an — communauté et conversion

> *« Une communauté solide et engagée, des inscrits newsletter qui grossissent, un taux de
> clic fort. »*

| # | KPI | Comment on le lit |
|---|---|---|
| **6** | **Abonnés newsletter, net mensuel** | l'audience qui appartient au blog, et pas aux plateformes |
| **7** | **⭐ Taux d'abonnement newsletter, PAR COUCHE** | **le KPI décisif de la segmentation** — voir ci-dessous |
| **7bis** | Taux de conversion session → abonné, global | 1 à 3 % est la norme d'un blog. En dessous de 1 %, le problème est sur le blog, pas sur les réseaux |
| **8** | **Commentateurs récurrents** | **le vrai indicateur de communauté** — nombre de personnes ayant commenté au moins 3 fois sur 12 mois |
| **9** | **Contributions reçues** | messages via `publier-ici` ou `julien@dans-le-desert.fr` |
| **10** | **Inscriptions UltraPack venues du blog** | clics sortants balisés vers `ultrapack.fr` |

### Sur le KPI 8 — il existe déjà, et il est mesurable

L'archive identifie quatre lecteurs récurrents sur six mois : **Cindy Martin** (deux groupes,
deux fois « je suis à un cheveu de m'inscrire »), **Pascal Dv** (qui poursuit la même
plaisanterie d'un groupe à l'autre), **Mickaël Martinez**, **Marie-Ange Urban**.

Quatre personnes. C'est la taille réelle de la communauté aujourd'hui, et c'est ce chiffre
qu'il faut faire monter — pas les 1 849 réactions.

### Sur le KPI 7 — celui qui valide ou invalide la segmentation

Les trois couches ne sont **pas** un entonnoir : on n'attend de personne qu'il migre d'une
couche à l'autre. Chaque couche est servie pour elle-même.

Le modèle repose donc sur une autre hypothèse, et c'est elle qu'il faut tester :
**chaque couche doit convertir pour son propre compte.**

| Couche | Ce qu'elle doit produire | Comment on le lit |
|---|---|---|
| **haute** *(novices)* | des **abonnés**, pas seulement des réactions | abonnés attribués à `utm_content` des groupes de la couche |
| **intermédiaire** *(trail)* | des **lecteurs réguliers** | sessions récurrentes, pages par session |
| **basse** *(pairs MDS)* | des **commentaires et des contributions** | commentateurs récurrents, messages `publier-ici` |

**Le cas à surveiller de près : la couche haute amène beaucoup de trafic et n'abonne
personne.** Elle produirait alors du bruit — et il faudrait la réduire, ou changer ce qu'on y
publie, pas la laisser tourner parce que les chiffres bruts sont flatteurs.

L'archive ne permet pas de trancher : les 725 réactions du groupe *Running* n'ont laissé
aucune trace côté blog, mais **aucun lien n'était balisé**, donc on ne sait pas si des gens
sont venus lire. Il faut environ **un trimestre** pour que ce KPI devienne lisible.

Un lecteur de la couche haute qui s'abonne sans jamais courir plus de 10 km est un **succès
complet**. Le blog peut avoir des lecteurs qui ne pratiqueront jamais — c'est le cas de tout
récit d'aventure.

### Sur le KPI 7bis — le calcul, désormais chiffré

Un blog convertit 1 à 3 % de ses visiteurs en abonnés. **100 abonnés sur un an supposent donc
3 000 à 10 000 visiteurs venus des réseaux.**

La base réelle est connue : **1 145 visiteurs sur cinq mois**, soit environ **2 750 sur un
an** à rythme constant. L'objectif de 100 abonnés est donc atteignable **si et seulement si**
le taux de conversion tient le haut de la fourchette — ou si le trafic augmente.

Deux leviers, dans cet ordre de rendement :

1. **Le format du post à lien.** L'écart entre « 5 erreurs » (2,6 visiteurs par réaction) et
   « 105 kg » (0,25) est d'un facteur 10. Bien construire la promesse vaut plus que publier
   davantage.
2. **La clôture des articles.** Le formulaire fonctionne — testé dans le navigateur Facebook
   le 2026-09-11 — mais **les quatre articles les plus lus n'invitent à rien**. 1 173
   visiteurs, 71 % du trafic, repartent sans avoir été sollicités. Le taux de conversion
   n'est pas faible : il est structurellement nul. Voir `baseline-blog.md`.

---

## Horizon 3 ans — positionnement

> *« Positionner dans-le-desert comme un blog de référence de l'ultra à étapes en autonomie —
> désert, jungle, steppes, Antarctique, Patagonie. »*

| # | KPI | Pourquoi c'est celui-là |
|---|---|---|
| **11** | **Part du trafic direct + recherche organique** | **le KPI de référence.** Un blog de référence est *trouvé*, pas *poussé*. **Base de départ : 1,2 %** (20 visiteurs Google sur 1 640) |
| **12** | **Articles d'invités publiés** | une référence attire des contributeurs. Zéro à ce jour, alors que le format est annoncé depuis l'article 015 |
| **13** | **Mentions et sollicitations externes** | invitations, citations, demandes d'interview, partenariats non sollicités |
| **14** | **Couverture hors désert** | nombre de terrains traités au-delà du sable — jungle, steppe, glace. Le positionnement annoncé l'exige, le corpus n'en contient aucun |

### KPI 11 — pourquoi c'est celui du positionnement

Un blog qu'on pousse n'est pas une référence ; un blog qu'on cherche l'est. Aujourd'hui,
**98,8 % du trafic est poussé** — 20 visiteurs sur 1 640 sont venus par Google. La base n'est
pas nulle, elle est très basse, et c'est la courbe qui comptera.

Le jour où une part significative du trafic arrive en direct ou par recherche, le
positionnement est acquis, quels que soient les chiffres de réactions. C'est lent, ça ne
bougera pas avant longtemps, et **il faut le relever dès le premier mois** pour avoir la
courbe.

À surveiller aussi : les requêtes de marque (« dans le désert blog », « Julien Leclerc MDS »)
si l'outil d'analytics les expose.

### KPI 14 est un angle mort du corpus

Seize articles, tous sur le sable. Le positionnement à trois ans porte sur l'ultra à étapes
en autonomie **tous terrains**. Aucun contenu n'existe sur la jungle, la Mongolie,
l'Antarctique ou la Patagonie — alors que l'article 016 les évoque déjà comme destinations
envisagées.

---

## Le tableau de bord mensuel

Six chiffres, trente minutes, le premier lundi du mois :

1. Sessions blog depuis les réseaux, **par groupe** *(via `utm_content`)*
2. Abonnés newsletter — net du mois
3. Messages de contributeurs reçus
4. Clics sortants vers UltraPack
5. Réactions et commentaires moyens du mois, **par couche**
6. Part de trafic direct + organique

**Ce qu'on ne met pas dans le tableau de bord :** le nombre total de réactions, les abonnés
Instagram, la taille des groupes. Ce sont des chiffres qui montent sans rien signifier.
