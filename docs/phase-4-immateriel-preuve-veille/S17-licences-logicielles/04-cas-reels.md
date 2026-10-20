# Cas réel – Entr'ouvert contre Orange : une licence libre qu'on ne respecte pas

*BTS SIO SISR 1re année – CEJM et CEJMA – S17*

> [!NOTE]
> **Comment travailler.** Lis chaque cas réel et ses sources, réponds par écrit aux questions, puis ouvre « Voir la réponse attendue ». Les faits viennent des sources citées en fin de page ; en cas de doute, **retourne à la source**. Ces cas complètent l'étude de cas fictive de la séance.

## Le dossier

**Les faits.** **Entr'ouvert**, société coopérative, a créé **Lasso**, une bibliothèque libre de gestion d'identité diffusée sous licence **GNU GPL v2**. **Orange** a utilisé Lasso dans un logiciel livré dans le cadre d'un appel d'offres lancé en 2005 pour le portail « Mon service public ». Entr'ouvert reproche à Orange de ne pas avoir respecté les conditions de la GPL : **pas de code source fourni** et **pas de mention de l'auteur**.

**La procédure.**

| Date | Étape |
|---|---|
| 2011 | Entr'ouvert assigne Orange pour contrefaçon et parasitisme |
| 2019 | Orange gagne en première instance |
| 2021 | La cour d'appel de Paris confirme en partie et condamne Orange à 150 000 € pour concurrence parasitaire |
| 5 octobre 2022 | La Cour de cassation casse ces décisions et renvoie l'affaire |
| **14 février 2024** | La cour d'appel de Paris, sur renvoi, juge qu'Orange a **contrefait** Lasso |

**La condamnation (2024).** Orange et Orange Business Services sont condamnées ensemble à **860 000 €** :

| Poste | Montant |
|---|---:|
| Conséquences économiques négatives (manque à gagner) | 500 000 € |
| Préjudice moral | 150 000 € |
| Bénéfices réalisés | 150 000 € |
| Article 700 du Code de procédure civile (frais de procès) | 60 000 € |
| **Total** | **860 000 €** |

**Les motifs.** La cour retient notamment que Lasso est **incorporé** dans le logiciel d'Orange sans autorisation de l'auteur, que le logiciel a été **livré à l'État sans le code source de Lasso**, et que le **nom de l'auteur n'a pas été mentionné**. Elle juge aussi que la **violation d'une clause d'une licence de logiciel** peut être poursuivie comme **contrefaçon**, pas seulement comme manquement à un contrat.

## Pourquoi ce cas est utile

« Libre » ne veut pas dire « sans condition ». La GPL autorise l'usage et la modification, mais **impose des obligations** à qui **distribue** le logiciel (fournir le code source, conserver la licence et les mentions). Ne pas les respecter expose à une condamnation, même pour un très grand groupe.

## Questions

**1.** Vérifie le calcul de la condamnation : quel est le total des quatre postes ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

500 000 + 150 000 + 150 000 + 60 000 = 860 000 €. Attention : les **60 000 €** ne réparent pas le préjudice, ils couvrent les **frais de procès**.
</details>

**2.** Quelle obligation de la GPL Orange n'a-t-elle pas respectée, selon la cour ? Pourquoi la **distribution** a-t-elle de l'importance ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

L'obligation de **fournir le code source** (et de respecter les conditions de la licence) lors de la **distribution** du logiciel. Orange a **livré** le logiciel à l'État : il y a donc eu distribution. Sans distribution à un tiers, l'utilisation interne d'un logiciel sous GPL n'entraîne pas l'obligation de publier le code.
</details>

**3.** Ton entreprise intègre une bibliothèque sous GPL dans un logiciel livré à un client. Cite **trois actions** à mener avant la livraison.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(1) **Inventorier** les composants et leurs licences ; (2) **vérifier la compatibilité** de la licence avec le mode de distribution prévu ; (3) prévoir la **fourniture du code source** et conserver les **mentions de licence et d'auteur**. On peut aussi **remplacer** le composant ou demander une **licence commerciale** à son auteur.
</details>

## Sources

- [Décision de la cour d'appel de Paris du 14 février 2024 (RG 22/18071) – synthèse](https://interoperable-europe.ec.europa.eu/sites/default/files/news/2024-03/2024%20Entre-Ouvert%20vs%20ORANGE.pdf) : date, montants, motifs.
- [Next – Orange condamnée à 860 000 euros](https://next.ink/brief-article/orange-condamnee-a-860-000-euros-pour-contrefacon-et-violation-de-la-licence-libre-gnu-gpl/) : chronologie de la procédure.

> [!NOTE]
> **À valider :** faits et chiffres repris de la synthèse et de la presse ; le texte de l'arrêt (cour d'appel de Paris, 14 février 2024) fait foi.
