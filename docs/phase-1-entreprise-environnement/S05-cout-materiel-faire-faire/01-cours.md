# Cours – Coûts, chaîne de valeur, faire ou faire-faire, TCO et cadre juridique du matériel

*BTS SIO SISR 1re année – CEJMA – S05 – à lire avant l'[étude de cas](02-etude-de-cas.md)*

> [!NOTE] Ce que tu dois savoir déjà
> - **Prérequis :** S02 (coûts fixes et marginaux), S04 (contrats)

## À la fin de ce cours tu sauras

- [ ] Distinguer **coûts fixes, variables, complets** et calculer une **productivité**
- [ ] Situer des activités dans la **chaîne de valeur**
- [ ] Raisonner **faire ou faire-faire** avec des critères et un calcul
- [ ] Calculer un **TCO** et un **coût annuel**
- [ ] Citer les **garanties**, l'**obsolescence programmée**, la **réparabilité** et les **DEEE**

## I. Produire : facteurs de production et coûts

Pour produire, une entreprise combine des **facteurs de production** :

- le **travail** (les salariés) ;
- le **capital** (machines, matériel informatique, locaux, logiciels) ;
- les **consommations intermédiaires** (énergie, pièces, services achetés).

### Les coûts

| Type de coût | Définition | Exemple |
|---|---|---|
| **Coût fixe** | Ne dépend pas de la quantité produite | Loyer, licence annuelle de supervision |
| **Coût variable** | Augmente avec la quantité produite | Pièces remplacées, temps passé par intervention |
| **Coût complet** | Tous les coûts, y compris la part des **frais de structure** | Coût d'un technicien : salaire, charges, poste, formation, encadrement |
| **Coût moyen** | Coût total ÷ quantité | Coût d'une intervention |

Le **seuil de rentabilité** est la quantité à partir de laquelle les recettes couvrent tous les coûts : coûts fixes ÷ (prix − coût variable unitaire) (voir séance 2).

### La productivité

La **productivité** mesure ce qu'on produit **par unité de facteur utilisé**. Un **gain de productivité** permet de produire plus avec les mêmes moyens, ou autant avec moins.

Exemple : avant, réinstaller un poste prend **3 heures** (1/3 poste par heure). Avec un **déploiement automatisé**, 45 minutes soit **0,75 heure** (1,33 poste par heure). Le temps est divisé par 4 : la productivité est multipliée par 4, soit une **hausse de 300 %**.

## II. La chaîne de valeur

La **chaîne de valeur** (Michael Porter) décrit les activités qui **créent de la valeur** dans une entreprise, depuis les achats jusqu'au client.

| Activités principales | Activités de soutien |
|---|---|
| Logistique interne (réception, stockage), **production** du service, logistique externe (livraison, déploiement), **commercial** et marketing, **services** après-vente et support | **Infrastructure** de l'entreprise, **gestion des ressources humaines**, **technologie** (R&D, outils), **achats** |

La **marge** est la différence entre la valeur créée et le coût de toutes ces activités. Pour une ESN : la production correspond à l'intervention du technicien ; le support N1 est une activité de service ; la gestion des licences et du matériel relève des achats.

## III. Faire ou faire-faire

Pour chaque activité, l'entreprise choisit de la **faire elle-même** (internaliser) ou de la **confier** à un tiers (**externaliser**, ou **impartir**, on dit aussi **faire-faire** ou **sous-traiter**).

| Critère | Plutôt **faire** | Plutôt **faire-faire** |
|---|---|---|
| **Compétence** | Cœur de métier, savoir-faire stratégique | Activité éloignée du cœur de métier |
| **Coût** | Volume important et régulier | Besoin ponctuel ou faible |
| **Risque** | Données ou savoir-faire **sensibles** | Risque de dépendance à gérer par contrat |
| **Flexibilité** | Besoin stable | Besoin qui varie |
| **Qualité** | Contrôle direct | Contrôle par **contrat** (SLA) |

### Exemple chiffré : maintenance de 60 postes

| | **Interne** | **Externalisée** |
|---|---|---|
| Coût | 1 technicien : 46 000 € par an + 2 000 € d'outils = **48 000 €** | 60 postes × 45 € × 12 mois = **32 400 €**, plus 6 000 € de pilotage interne du contrat = **38 400 €** |
| Écart | | **−9 600 € par an**, soit **−20 %** |

L'externalisation est moins chère **à ce niveau de service**, mais il faut regarder aussi : le **délai d'intervention**, la **connaissance de l'entreprise**, la **dépendance** au prestataire, la **confidentialité**.

## IV. Le matériel : cycle de vie et coût total de possession

Le **cycle de vie** d'un équipement : **fabrication** → **achat** → **installation** → **usage et maintenance** → **fin de vie** (revente, réemploi, recyclage).

Le **TCO** (*Total Cost of Ownership*, coût total de possession) additionne **tous** les coûts d'un équipement sur sa durée d'usage :

> **TCO = achat + installation + (maintenance + énergie) × durée + remplacements − valeur de reprise**

Le **prix d'achat** n'est donc qu'une partie du coût. Le TCO se rapporte à la durée d'usage pour donner un **coût annuel**.

### Exemple : 20 portables, neuf ou reconditionné

| Par appareil | **Neuf** | **Reconditionné** |
|---|---|---|
| Achat | 900 € | 540 € |
| Installation | 40 € | 40 € |
| Maintenance par an | 25 € | 30 € |
| Énergie par an | 15 € | 22 € |
| Batterie à remplacer | 80 € (année 4) | 70 € (année 2) |
| Reprise en fin de vie | 60 € | 20 € |
| **Durée d'usage prévue** | **5 ans** | **4 ans** |
| **TCO** | 900 + 40 + 5 × (25 + 15) + 80 − 60 = **1 160 €** | 540 + 40 + 4 × (30 + 22) + 70 − 20 = **838 €** |
| **Coût annuel** | 1 160 ÷ 5 = **232 €** | 838 ÷ 4 = **209,50 €** |

Pour 20 appareils : **4 640 €** par an pour le neuf, **4 190 €** pour le reconditionné, soit **450 € d'écart par an** (environ **9,7 %**). Le reconditionné est moins cher **par an**, mais il faudra le **remplacer plus tôt**.

## V. Le cadre juridique de l'équipement

| Sujet | Règle |
|---|---|
| **Garantie légale de conformité** | Un consommateur est protégé pendant **2 ans** pour un bien neuf. Elle protège les **consommateurs** et non les professionnels |
| **Garantie des vices cachés** | Pour un **professionnel** aussi : un défaut caché **antérieur** à la vente, qui rend le bien impropre à l'usage (Code civil, articles 1641 et suivants). L'action doit être exercée dans les **2 ans** de la découverte du vice |
| **Garantie commerciale** | Garantie **contractuelle** supplémentaire offerte par le vendeur ou le fabricant |
| **Obsolescence programmée** | Techniques visant à **réduire délibérément la durée de vie** d'un produit pour augmenter son taux de remplacement : c'est un **délit** (Code de la consommation, article L441-2), puni de **deux ans d'emprisonnement** et de **300 000 € d'amende** |
| **Indice de réparabilité, puis de durabilité** | Note sur **10** affichée pour certains équipements (ordinateurs portables, téléviseurs, lave-linge…) ; l'**indice de durabilité** remplace progressivement l'indice de réparabilité à partir de 2025 |
| **DEEE** (déchets d'équipements électriques et électroniques) | Le **producteur** finance la collecte et le recyclage ; le **distributeur** reprend l'ancien appareil à l'achat d'un neuf (reprise « un pour un ») ; on ne jette pas un équipement électronique avec les ordures ménagères |

> [!NOTE]
> Un **ordinateur reconditionné** est un appareil d'occasion **testé, remis en état** et revendu avec une garantie. L'asymétrie d'information (séance 2) est réduite par la **garantie** et le **rapport de test**.

## À retenir

- Facteurs de production : **travail**, **capital**, **consommations intermédiaires** ; coûts **fixes**, **variables**, **complet**.
- **Productivité** : produire plus avec autant de moyens ; un gain de productivité peut s'exprimer en pourcentage.
- **Chaîne de valeur** : activités **principales** et de **soutien**.
- **Faire ou faire-faire** : compétence, coût, risque, flexibilité, qualité.
- **TCO** = achat + installation + (maintenance + énergie) × durée + remplacements − reprise ; on le rapporte à la **durée d'usage**.
- Cadre : garantie de **conformité** (consommateurs), **vices cachés** (professionnels), **obsolescence programmée** (délit), **réparabilité / durabilité**, **DEEE**.
