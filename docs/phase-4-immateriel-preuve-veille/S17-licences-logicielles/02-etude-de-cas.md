# Étude de cas – L'audit de licences de Studio Mosaïque

*BTS SIO SISR 1re année – CEJM et CEJMA – S17*

> [!NOTE]
> **Comment travailler.** Lis le dossier, puis réponds **par écrit** à chaque question, avec une réponse **construite et argumentée** : une idée, sa justification, l'exemple tiré du dossier. Ouvre ensuite « Voir la réponse attendue » pour te corriger. À l'épreuve E4, une réponse sans justification n'est pas complète.

## Dossier : l'audit de licences de Studio Mosaïque

> [!NOTE]
> L'entreprise et les personnes sont **fictives**.

### Document 1 – Le contexte

**Studio Mosaïque** est une agence web de 18 postes. Elle reçoit une lettre d'un éditeur de logiciels de retouche d'images demandant un **audit de conformité**.

### Document 2 – L'inventaire

| Logiciel | Licence achetée | Installations constatées |
|---|---|---|
| Retouche d'images (éditeur demandeur) | **12** licences | **18** postes |
| Suite bureautique | **18** licences | 18 postes |
| Outil de maquettage | Gratuit pour usage **non commercial** | Utilisé pour des **projets clients** |
| Éditeur de code | Licence libre **permissive** (MIT) | 18 postes |
| Bibliothèque JavaScript | Licence **GPL** | Intégrée dans le produit vendu à un client, **sans fournir les sources** |
| Image d'illustration | **CC BY-NC** | Utilisée sur le site **commercial** de l'agence |

Le prix catalogue d'une licence de retouche d'images est de **420 € par poste et par an**.

### Questions

**1.** Calculez l'**écart** de licences pour le logiciel de retouche et l'**ordre de grandeur** de la régularisation annuelle.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Écart : 18 − 12 = **6 postes** non licenciés. Régularisation annuelle de référence : 6 × 420 = **2 520 €** (hors pénalités, rétroactivité et frais éventuels que l'éditeur peut réclamer).
</details>

**2.** L'outil de maquettage gratuit « non commercial » peut-il être utilisé pour des projets clients ? Pourquoi ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Non : un usage pour des **projets clients rémunérés** est un usage **commercial**, exclu par la licence. Il faut une **licence commerciale** ou un outil alternatif.
</details>

**3.** La bibliothèque GPL intégrée au produit vendu : quelle est l'obligation ? Quelle solution ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

La GPL impose, en cas de **redistribution** d'une œuvre dérivée, de la placer sous **GPL** et de fournir les **sources**. Studio Mosaïque doit soit **fournir les sources** (licence du produit compatible), soit **remplacer** la bibliothèque par une alternative **permissive** ou négocier une **licence commerciale** si elle existe.
</details>

**4.** L'image CC BY-NC sur le site commercial est-elle utilisable ? Que faire ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Non : **NC** interdit l'usage **commercial**, et le site d'une agence est un usage commercial. Il faut **retirer** l'image, la **remplacer** par une image sous licence compatible (par exemple CC BY, avec mention de l'auteur) ou **obtenir l'autorisation**.
</details>

**5.** La licence MIT de l'éditeur de code impose-t-elle quelque chose au studio ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Très peu : **conserver la mention de copyright et la licence** si on redistribue le code. L'utilisation sur 18 postes est libre. Pas d'obligation de publier ses propres sources.
</details>

**6.** Quels sont les **risques** pour l'agence en cas d'audit ? Ordonnez-les.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(1) **Contrefaçon** et mise en demeure de **régularisation** (frais, rétroactivité) ; (2) risque **juridique** sur le produit vendu (GPL) pouvant entraîner l'obligation de publier les sources ou de retirer le produit ; (3) **image** et relation avec le client ; (4) coût de **remplacement** et de **migration**. Le plus lourd est souvent le produit livré au client avec une brique non conforme.
</details>

**7.** Proposez un **plan de mise en conformité** et une **procédure durable** (cinq actions).

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(1) **Répondre** à l'éditeur dans les délais, avec un inventaire exact ; (2) **acquérir** les 6 licences ou supprimer des installations ; (3) **corriger** les cas GPL, NC et outil gratuit ; (4) mettre en place un **inventaire permanent** et une **validation** avant toute nouvelle installation ou dépendance ; (5) **former** les équipes (licences, images, dépendances).
</details>


## Je sais faire

Coche honnêtement ; ce que tu ne coches pas se reprend avant la séance suivante.

- [ ] Distinguer libre et gratuit
- [ ] Comparer GPL et MIT
- [ ] Lire une licence Creative Commons
- [ ] Calculer un écart de licences
- [ ] Citer trois pratiques de gestion des licences

**Ce que je dois reprendre :** ______________________

**Ma question à poser à l'enseignant :** ______________________
