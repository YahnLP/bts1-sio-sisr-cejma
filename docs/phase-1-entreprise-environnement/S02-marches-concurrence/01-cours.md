# Cours – Marchés, concurrence et imperfections

*BTS SIO SISR 1re année – CEJM et CEJMA – S02 – à lire avant l'[étude de cas](02-etude-de-cas.md)*

> [!NOTE] Ce que tu dois savoir déjà
> - **Prérequis :** S01 (agents économiques, acteurs du numérique)

## À la fin de ce cours tu sauras

- [ ] Calculer un **prix d'équilibre** et interpréter un déplacement de la demande
- [ ] Distinguer les **formes de marché**
- [ ] Expliquer **barrières à l'entrée, asymétrie d'information, externalités**
- [ ] Calculer un **seuil de rentabilité** et un **coût moyen**
- [ ] Décrire le rôle des **banques et du marché financier**

## I. Qu'est-ce qu'un marché ?

Un **marché** est le lieu, réel ou virtuel, où se rencontrent des **offreurs** (qui vendent) et des **demandeurs** (qui achètent) pour échanger un bien ou un service à un **prix**.

- **Demande** : quantité que les acheteurs veulent acheter à un prix donné. Quand le prix **monte**, la demande **baisse**.
- **Offre** : quantité que les vendeurs veulent vendre à un prix donné. Quand le prix **monte**, l'offre **augmente**.
- **Prix d'équilibre** : prix pour lequel la quantité offerte égale la quantité demandée.

### Exemple chiffré

Sur le marché local des interventions de maintenance de postes, avec *p* le prix d'une intervention en euros :

- demande : **Qd = 1 000 − 2p** ;
- offre : **Qo = 200 + 2p**.

À l'équilibre, Qd = Qo : 1 000 − 2p = 200 + 2p, donc 4p = 800 et **p = 200 €**. La quantité échangée est **600** interventions (1 000 − 400 = 600 = 200 + 400).

| Prix | Demande | Offre | Situation |
|---|---|---|---|
| 150 € | 700 | 500 | **Pénurie** de 200 : la demande dépasse l'offre, le prix a tendance à monter |
| **200 €** | **600** | **600** | **Équilibre** |
| 250 € | 500 | 700 | **Surplus** de 200 : l'offre dépasse la demande, le prix a tendance à baisser |

**Quand la demande augmente** (par exemple une obligation réglementaire nouvelle), la courbe de demande se déplace : avec **Qd = 1 200 − 2p**, l'équilibre devient 1 200 − 2p = 200 + 2p, donc **p = 250 €** et **Q = 700**. Le prix et les quantités échangées augmentent.

## II. Les formes de marché

| Forme | Nombre d'offreurs | Pouvoir sur le prix | Exemple dans le numérique |
|---|---|---|---|
| **Concurrence pure et parfaite** | Très nombreux | Nul : le prix s'impose | Modèle théorique (jamais complètement réalisé) |
| **Concurrence monopolistique** | Nombreux, produits **différenciés** | Faible | Prestataires locaux de maintenance, applications mobiles |
| **Oligopole** | Quelques gros acteurs | Fort, mais **interdépendant** | Cloud public, systèmes d'exploitation, navigateurs |
| **Monopole** | Un seul | Très fort | Un fournisseur de logiciel de gestion sans équivalent |

La **concurrence pure et parfaite** suppose cinq conditions : **atomicité** (beaucoup d'acheteurs et de vendeurs, aucun ne pèse sur le prix), **homogénéité** du produit, **libre entrée et sortie** du marché, **transparence** de l'information et **mobilité** des facteurs de production. Elle sert de repère théorique.

## III. Concurrence et coopération

- **La concurrence** pousse à baisser les prix, à améliorer la qualité, à innover. Les entreprises se concurrencent par le **prix** ou par la **différenciation** (qualité, service, marque, expertise).
- **La coopération** : les entreprises s'allient quand c'est utile : **normes et standards** communs, **partenariats** commerciaux, projets **open source** où des concurrents mutualisent le développement.
- On parle de **coopétition** quand deux entreprises se font concurrence sur certains marchés et coopèrent sur d'autres.

## IV. Quand le marché fonctionne mal

| Imperfection | Définition | Exemple dans le numérique |
|---|---|---|
| **Barrière à l'entrée** | Obstacle qui empêche de nouveaux concurrents d'entrer | Coût de développement très élevé, brevets, effet de réseau, réglementation |
| **Asymétrie d'information** | Une partie en sait plus que l'autre | Le vendeur d'un ordinateur **reconditionné** connaît l'état de la batterie, pas l'acheteur |
| **Externalité** | Effet d'une activité sur des tiers, sans compensation par le prix | **Négative** : déchets électroniques, consommation d'énergie ; **positive** : standard ouvert profitant à tous |

### Les économies d'échelle : une barrière à l'entrée

Pour un éditeur, développer un logiciel coûte cher (**coûts fixes**), mais vendre une copie supplémentaire coûte presque rien (**coût marginal**).

Exemple fictif : coûts fixes de **600 000 €**, coût marginal de **2 €** par licence, prix de vente de **50 €**.

- **Seuil de rentabilité** : 600 000 ÷ (50 − 2) = **12 500 licences**.
- **Coût moyen** à 100 000 licences : 600 000 ÷ 100 000 + 2 = **8 €** ; à 12 500 licences : 600 000 ÷ 12 500 + 2 = **50 €**.

Un éditeur qui vend 100 000 licences produit à 8 € l'unité, alors qu'un **nouvel entrant** qui n'en vend que 12 500 revient à 50 €. L'acteur en place peut baisser son prix sans perdre d'argent : c'est une **barrière à l'entrée**.

### L'asymétrie d'information

L'économiste George Akerlof l'a illustrée en 1970 avec le marché des voitures d'occasion : si l'acheteur ne peut pas distinguer les bons véhicules des mauvais, il propose un **prix moyen**, ce qui fait **fuir** les bons vendeurs. Pour réduire ce problème, on utilise des **garanties**, des **labels**, des **contrôles indépendants**, des **avis vérifiés**.

## V. Les spécificités du numérique

- **Effets de réseau** : un service vaut davantage quand il a plus d'utilisateurs (messagerie, réseau professionnel). Ils favorisent un acteur dominant et rendent difficile l'arrivée d'un concurrent.
- **Coût marginal quasi nul** : une copie supplémentaire d'un logiciel ou d'un contenu coûte peu.
- **Plateformes** : elles mettent en relation deux côtés du marché (ex. développeurs et utilisateurs d'une boutique d'applications) et prennent une commission.
- **Normes et standards** : ils permettent de relier des systèmes entre eux, réduisent la dépendance à un fournisseur et favorisent la concurrence.

## VI. Le rôle des banques et du marché financier

| | Rôle | Exemple pour une ESN |
|---|---|---|
| **Banques** | Collectent l'épargne, accordent des **crédits**, gèrent les moyens de paiement | Prêt pour acheter un parc de serveurs de démonstration |
| **Marché financier** | Les entreprises lèvent des capitaux en émettant des **actions** (parts de propriété) ou des **obligations** (dettes) | Une ESN cotée qui augmente son capital pour racheter une concurrente |

La séance 10 revient en détail sur le **financement** d'une entreprise.

## Comprendre pas à pas

### Identifier une forme de marché en trois questions

1. **Combien de vendeurs ?** Un seul (monopole), quelques-uns (oligopole), beaucoup (concurrence).
2. **Combien d'acheteurs ?** Un seul acheteur (monopsone), quelques-uns, beaucoup.
3. **Peut-on entrer facilement ?** Les **barrières à l'entrée** (coûts fixes, réglementation, réseau d'utilisateurs) protègent ceux qui sont déjà là.

### Économies d'échelle : un exemple chiffré

Une société d'hébergement paie **100 000 €** de coûts fixes (salle, outils) et **5 € de coût variable** par client.

| Nombre de clients | Coût total | Coût moyen par client |
|---:|---:|---:|
| 10 000 | 100 000 + 5 × 10 000 = 150 000 € | **15 €** |
| 100 000 | 100 000 + 5 × 100 000 = 600 000 € | **6 €** |

Plus l'entreprise est **grande**, plus son coût par client **baisse** : un nouveau concurrent **petit** ne peut pas proposer les mêmes prix. C'est une **barrière à l'entrée**.

### Position dominante : ce qui est permis, ce qui ne l'est pas

| Situation | Légal ? |
|---|---|
| Être **leader** grâce à un meilleur produit | **Oui** |
| Utiliser sa position pour **fermer** l'accès aux concurrents (liaisons forcées, traitement préférentiel de ses propres services) | **Non** (abus de position dominante) |

> [!NOTE]
> La **taille** n'est pas une faute ; l'**abus** l'est.

Un cas réel est détaillé dans [Google et l'Autorité de la concurrence](04-cas-reels.md).

## À retenir

- Le **prix d'équilibre** égalise offre et demande ; si la demande augmente, le prix et les quantités augmentent.
- Formes de marché : **concurrence parfaite** (théorique), **concurrence monopolistique**, **oligopole**, **monopole**.
- Imperfections : **barrières à l'entrée**, **asymétrie d'information**, **externalités** (positives ou négatives).
- Le numérique : **effets de réseau**, **coût marginal faible**, **plateformes**, **normes**.
- Les entreprises **se concurrencent** et **coopèrent** (standards, partenariats, open source).
