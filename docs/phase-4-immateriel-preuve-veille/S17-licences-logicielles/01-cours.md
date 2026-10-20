# Cours – Licences logicielles, logiciel libre et Creative Commons

*BTS SIO SISR 1re année – CEJM et CEJMA – S17 – à lire avant l'[étude de cas](02-etude-de-cas.md)*

> [!NOTE] Ce que tu dois savoir déjà
> - **Prérequis :** S16, S05

## À la fin de ce cours tu sauras

- [ ] Distinguer **propriétaire**, **libre**, **gratuit**
- [ ] Comparer **copyleft** et **permissif**
- [ ] Lire une licence **Creative Commons**
- [ ] Repérer un **écart** de licences
- [ ] Proposer un plan de **conformité**

## I. Une licence, qu'est-ce que c'est ?

Acheter un logiciel, c'est en réalité acquérir un **droit d'usage** défini par une **licence** : un contrat par lequel le titulaire des droits (séance 16) **autorise** certains usages et en **interdit** d'autres.

## II. Les grandes familles

| Famille | Principe | Exemples d'usage |
|---|---|---|
| **Propriétaire** | Droit d'**utiliser** selon des conditions strictes ; code source **fermé** ; copie, modification, redistribution **interdites** | Suites bureautiques commerciales |
| **Libre** | Quatre **libertés** : **utiliser**, **étudier**, **modifier**, **redistribuer** | Systèmes et outils libres |
| **Gratuiciel** (*freeware*) | Gratuit mais **propriétaire** | Utilitaires gratuits |
| **Partagiciel** (*shareware*) | Essai gratuit puis **paiement** | Logiciels d'essai |
| **Service en ligne (SaaS)** | Accès **par abonnement**, conditions d'utilisation | Messagerie et outils en ligne |

> [!NOTE]
> **Libre ne veut pas dire gratuit**, ni **sans règles** : une licence libre impose des **obligations** (conserver les mentions, redistribuer sous les mêmes conditions, etc.). Et **gratuit ne veut pas dire libre**.

## III. Les licences libres

| Licence | Famille | Obligations principales |
|---|---|---|
| **GPL** (GNU General Public License) | **Copyleft fort** | Une œuvre dérivée, redistribuée, doit l'être **sous la même licence** et avec ses sources |
| **LGPL** | Copyleft faible | Les bibliothèques peuvent être liées à du code propriétaire, sous conditions |
| **MIT**, **BSD** | **Permissives** | Conserver la mention de copyright et la licence ; pas d'obligation de partager les sources |
| **Apache 2.0** | Permissive | Idem, plus une **concession de brevets** et la mention des modifications |
| **AGPL** | Copyleft réseau | Même obligation si le logiciel est proposé **en service** à distance |

Le **copyleft** garantit que les libertés se **transmettent** ; une licence **permissive** laisse plus de latitude, y compris pour intégrer le code à un produit fermé.

### Compatibilité

Des licences ne se **combinent** pas toujours : un projet qui intègre un composant GPL doit respecter la GPL pour l'ensemble qu'il redistribue. **Avant** d'ajouter une dépendance, on vérifie sa licence.

## IV. Licences de contenus : Creative Commons

Pour les **œuvres** (textes, images, supports), les licences **Creative Commons** combinent quatre options :

| Option | Sens |
|---|---|
| **BY** | **Attribution** : citer l'auteur |
| **SA** | **Partage dans les mêmes conditions** |
| **NC** | **Pas d'utilisation commerciale** |
| **ND** | **Pas de modification** |

Exemple : **CC BY-SA** autorise l'usage, même commercial, avec citation de l'auteur et partage de l'œuvre dérivée sous les mêmes conditions ; **CC BY-NC-SA** interdit l'usage commercial.

## V. Gérer les licences en entreprise

| Pratique | Raison |
|---|---|
| **Inventaire** des logiciels et licences | Savoir ce qu'on a et ce qu'on a le droit de faire |
| **Suivi des quantités** (postes, utilisateurs, cœurs) | Éviter la **sous-licence** (utilisation sans droit) et le **gaspillage** |
| **Gestion des échéances** et renouvellements | Éviter ruptures et coûts imprévus |
| **Contrôle** des installations | Interdire les logiciels non autorisés (charte, séance 11) |
| **Audit** de l'éditeur | Un éditeur peut contrôler le respect de la licence : en cas d'écart, régularisation et **pénalités** |
| **Choix éclairé** | Comparer coût total (séance 5), dépendance, support, évolutivité |

> [!WARNING]
> Utiliser un logiciel **au-delà** de la licence (plus de postes, usage non permis) est une **contrefaçon** et peut mener à une demande de régularisation, voire des poursuites.

## Comprendre pas à pas

### Les trois idées reçues à corriger

| Idée reçue | Réalité |
|---|---|
| « Libre = gratuit. » | **Faux.** Un logiciel libre peut être vendu ; **gratuit ≠ libre** (voir la partie III). |
| « Libre = sans conditions. » | **Faux.** Toute licence libre a des conditions : la **MIT** demande de conserver la mention de licence ; la **GPL** impose de **fournir le code source** à qui reçoit le logiciel. |
| « Je ne distribue pas, donc la GPL ne me concerne jamais. » | **À nuancer.** Utiliser ou modifier un logiciel GPL **en interne** n'impose pas de publier le code ; les obligations naissent quand on **distribue** le logiciel (livraison à un client, mise en ligne). |

### Exemple guidé : quelle licence choisir pour mon développement ?

Une entreprise veut intégrer une bibliothèque dans un produit livré à ses clients.

1. **Quelle est la licence de la bibliothèque ?** (GPL, MIT, propriétaire…)
2. **Vais-je distribuer le produit ?** (oui, aux clients)
3. **Que m'impose la licence ?** MIT : garder la mention. GPL : le produit livré doit pouvoir être redistribué avec son code source sous GPL.
4. **Est-ce compatible avec mon modèle ?** Si l'entreprise veut garder son code fermé, **la GPL est incompatible** : il faut un autre composant ou une licence commerciale.

> [!TIP]
> Le réflexe à l'E4 : **nom de la licence → ce qu'elle autorise → ce qu'elle impose → conséquence pour l'entreprise**.

Pour une décision de justice, voir [Entr'ouvert contre Orange](04-cas-reels.md).

## À retenir

- Une licence = **droit d'usage** défini par contrat.
- **Libre** : utiliser, étudier, modifier, redistribuer ; **gratuit ≠ libre**.
- **Copyleft** (GPL) contre **permissif** (MIT, BSD, Apache).
- **Creative Commons** : BY, SA, NC, ND.
- En entreprise : **inventaire**, suivi des quantités, contrôle, préparation aux audits.
