# Étude de cas – Habitat Valmont renouvelle son informatique

*BTS SIO SISR 1re année – CEJMA – S01*

> [!NOTE]
> **Comment travailler.** Lis le dossier, puis réponds **par écrit** à chaque question, avec une réponse **construite et argumentée** : une idée, sa justification, l'exemple tiré du dossier. Ouvre ensuite « Voir la réponse attendue » pour te corriger. À l'épreuve E4, une réponse sans justification n'est pas complète.

## Dossier : Habitat Valmont renouvelle son informatique

> [!NOTE]
> Les entreprises et les chiffres de ce dossier sont **fictifs**.

### Document 1 – Le contexte

**Habitat Valmont** est un bailleur social de 85 salariés. Sa **DSI** compte 2 personnes. Le parc comprend 85 postes de travail et un serveur de messagerie installé sur place, devenu trop ancien. La direction veut **migrer 85 boîtes de messagerie** et **réinstaller 60 postes** en 15 jours ouvrés. La DSI manque de temps : elle fait appel à une ESN, **Cobalt Services Numériques**, qui a déjà installé les imprimantes du site.

### Document 2 – La proposition de l'ESN (extrait)

| | **Option A – Régie** | **Option B – Forfait** |
|---|---|---|
| Moyens | 2 techniciens de Cobalt, **15 jours chacun** | Cobalt s'engage sur le **résultat** : 60 postes réinstallés et 85 boîtes migrées, recette signée |
| Prix | **460 € HT par jour et par technicien** | **15 900 € HT**, prix ferme |
| Direction du travail | La DSI de Valmont planifie les tâches | Cobalt planifie et fournit un compte rendu |

### Document 3 – Le choix de la messagerie (extrait du comparatif de la DSI)

| | **SaaS** (abonnement) | **Licence + serveur interne** |
|---|---|---|
| Prix | **5,40 € HT par utilisateur et par mois** | **130 € HT par utilisateur** à l'achat, puis maintenance de **20 %** du prix d'achat **par an** |
| Hébergement | Chez l'éditeur | Serveur de Valmont : **1 800 € HT par an** (matériel, énergie, administration) |
| Mises à jour et sécurité | Par l'éditeur | Par la DSI |

### Questions

**1.** Citez les **quatre acteurs** du dossier et précisez le **rôle** de chacun. Qui est le **client**, qui est le **prestataire** ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

- **Habitat Valmont** : organisation **cliente**, qui utilise l'informatique pour son métier (bailleur social).
- **Sa DSI** : gère le système d'information de Valmont ; elle pilote le projet.
- **Cobalt Services Numériques** : **ESN** prestataire, qui vend du temps ou un résultat à Valmont.
- **L'éditeur de la messagerie** : fournit le logiciel ou le service (SaaS).

Le **client** est Habitat Valmont ; le **prestataire** est Cobalt.
</details>

**2.** Calculez le prix de l'option A. Calculez ensuite le prix de l'option A si la charge de travail dépasse de **40 %** la prévision. Que vaut l'option B dans ce cas ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

- Option A prévue : 2 × 15 × 460 = **13 800 € HT**.
- Option A avec 40 % de dépassement : 13 800 × 1,4 = **19 320 € HT**.
- Option B : **15 900 € HT**, inchangé (prix ferme).

La régie est **moins chère** si tout se passe comme prévu (13 800 € contre 15 900 €), et **plus chère** si le travail dérape fortement (19 320 € contre 15 900 €).
</details>

**3.** À partir de quel dépassement de charge le forfait devient-il moins cher que la régie ? Arrondissez au dixième de pourcent.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Il faut que 13 800 × (1 + x) dépasse 15 900, soit 1 + x supérieur à 15 900 ÷ 13 800 ≈ 1,152. Le seuil est un dépassement d'environ **15,2 %** de la charge prévue (soit 2 100 € d'écart).
</details>

**4.** Qui porte le **risque de dérive** dans chaque option ? Reliez votre réponse à la notion d'obligation de **moyens** ou de **résultat**.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

- **Régie** : le risque est pour **Valmont** (il paie le temps passé) ; Cobalt a une obligation de **moyens** : fournir des techniciens compétents, pas garantir le résultat.
- **Forfait** : le risque est pour **Cobalt** (prix fixe) ; Cobalt a une obligation de **résultat** : 60 postes réinstallés et 85 boîtes migrées, recette signée.
</details>

**5.** Calculez le coût sur **5 ans** de chaque solution de messagerie. Quelle est la moins chère ? Citez **deux** limites de cette comparaison.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

- **SaaS** : 85 × 5,40 × 12 = 5 508 € par an, soit **27 540 €** sur 5 ans.
- **Licence** : achat 85 × 130 = 11 050 € ; maintenance 20 % = 2 210 € par an, soit 11 050 € sur 5 ans ; hébergement 1 800 € × 5 = 9 000 €. Total **31 100 €**.

Le **SaaS** est le moins cher (3 560 € d'écart) dans ce calcul. Limites possibles : le calcul **ignore le temps de la DSI** pour administrer le serveur (qui coûte aussi), la **dépendance** à l'éditeur (verrouillage, hausse des prix), le **coût de sortie** du SaaS, la question de la **localisation des données** (séance 13), l'évolution du nombre d'utilisateurs.
</details>

**6.** **Rédigez une recommandation** de dix lignes maximum à la direction de Valmont : quelle option de prestation, quelle solution de messagerie, et pourquoi ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Une réponse solide :

1. **Prestation** : le **forfait** est préférable : Valmont a une DSI de 2 personnes, donc peu de capacité à piloter une régie ; le **résultat** (recette signée) et le **prix ferme** sécurisent le budget, pour un surcoût de 2 100 € (15,2 %) par rapport à la prévision en régie.
2. **Précaution** : demander que le contrat décrive précisément le **périmètre** et les **critères de recette**, sinon le forfait donne lieu à des désaccords.
3. **Messagerie** : le **SaaS** est moins cher sur 5 ans (27 540 € contre 31 100 €) et allège la DSI (mises à jour et sécurité sont pris en charge).
4. **Vigilance** : vérifier la **réversibilité** (récupération des boîtes), la **localisation des données** et les conditions d'évolution des prix.

Un jury attend une **décision** claire, **justifiée** par des chiffres du dossier et **nuancée** par un risque.
</details>

**7.** Dans votre entreprise d'alternance : est-elle plutôt **cliente**, **prestataire**, ou les deux ? Qui sont ses **fournisseurs** informatiques ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Réponse personnelle. Elle doit : situer l'entreprise (ESN, DSI d'une organisation, éditeur…), nommer au moins **deux** partenaires (client, éditeur, hébergeur, distributeur) et préciser le **mode de facturation** s'il est connu.
</details>


## Je sais faire

Coche honnêtement ; ce que tu ne coches pas se reprend avant la séance suivante.

- [ ] Citer les cinq agents économiques et deux types d'échanges (B to B, B to C…)
- [ ] Distinguer une ESN, une DSI, un éditeur et un hébergeur
- [ ] Expliquer qui porte le risque en régie et en forfait
- [ ] Calculer le prix d'une prestation en régie et le seuil de rentabilité d'un forfait
- [ ] Comparer deux coûts sur plusieurs années

**Ce que je dois reprendre :** ______________________

**Ma question à poser à l'enseignant :** ______________________
