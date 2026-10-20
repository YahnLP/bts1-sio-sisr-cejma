# Cas réel – Dedalus Biologie : fuite de données médicales

*BTS SIO SISR 1re année – CEJM et CEJMA – S15*

> [!NOTE]
> **Comment travailler.** Lis le cas réel et ses sources, réponds par écrit aux questions, puis ouvre « Voir la réponse attendue ». Les faits viennent des sources citées en fin de page ; en cas de doute, **retourne à la source**. Ce cas complète l'étude de cas fictive de la séance.

## Le dossier

**Les faits.** **Dedalus Biologie** édite un **logiciel de gestion de laboratoires d'analyses**. Elle est **sous-traitant** des laboratoires, qui sont les **responsables de traitement**. Début **2021**, une **fuite de données** touche **plus de 500 000 personnes** : noms, numéros de sécurité sociale, médecins prescripteurs, dates d'examens et **informations médicales sensibles**. Les données ont été **publiées en ligne**.

**La décision.** En **avril 2022**, la CNIL sanctionne Dedalus Biologie d'une amende de **1,5 million d'euros**.

**Les manquements retenus.**

| Manquement | Article du RGPD | Constat |
|---|---|---|
| **Traitement au-delà des instructions** | 29 | Lors d'une **migration de logiciel** demandée par deux laboratoires, Dedalus a **extrait plus de données** que nécessaire |
| **Sécurité** | 32 | La fuite provient d'un **serveur** contenant des données d'anciens logiciels. Des **alertes** (d'un salarié et de l'**ANSSI**) sont restées **sans réponse** ; aucune procédure de **chiffrement** pour la migration |
| **Contrat de sous-traitance** | 28 | Le contrat de maintenance et les conditions de vente **ne comportaient pas** les clauses RGPD obligatoires |

Selon la source, c'est une **première** : la sanction d'un **sous-traitant** pour des insuffisances **contractuelles**. La CNIL a retenu une **négligence**, et la société n'a pas contesté le manquement.

## Pourquoi ce cas est utile

Il montre trois idées du cours : un **sous-traitant** a des **obligations directes** ; la **sécurité** (article 32) se joue aussi sur des gestes **banals** (serveur ancien, alerte ignorée) ; et le **contrat** (article 28) est une exigence **à part entière**.

## Questions

**1.** Le montant de **1,5 M€** est-il proche du plafond des amendes de niveau 1 (10 M€) ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Non : 1,5 / 10 = 0,15, soit **15 %** du plafond de 10 M€. Les manquements de sécurité et de contrat relèvent du **niveau 1** (10 M€ ou 2 % du chiffre d'affaires mondial, le plus élevé). La CNIL **proportionne** la sanction : gravité, nombre de personnes, nature des données, comportement.
</details>

**2.** Dedalus n'était **pas** responsable de traitement. Pourquoi a-t-elle pourtant été sanctionnée ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Parce que le RGPD impose des **obligations directes** au **sous-traitant** : traiter **seulement sur instruction** (article 29), assurer la **sécurité** (article 32), et encadrer sa relation par un **contrat** conforme (article 28). Être sous-traitant **ne protège pas** de la sanction.
</details>

**3.** Un technicien reçoit un **signalement de l'ANSSI** indiquant que des données de ton entreprise sont visibles en ligne. Décris **cinq actions**, dans l'ordre.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(1) **Prévenir** immédiatement le DPO, le RSSI ou la direction ; (2) **préserver les preuves** (journaux, copies), sans rien effacer ; (3) **contenir** la fuite (couper l'accès, fermer le serveur exposé) ; (4) **évaluer la gravité** et décider de la **notification à la CNIL** dans les **72 heures** après en avoir pris connaissance, si la violation présente un risque ; (5) **tracer** la décision dans le registre des violations. Ignorer l'alerte est précisément ce qui a été reproché à Dedalus.
</details>

## Sources

- [Solutions Numériques – Fuite de données de santé : la CNIL inflige 1,5 M€ d'amende au sous-traitant Dedalus](https://www.solutions-numeriques.com/decideur-entreprise/fuite-de-donnees-de-sante-la-cnil-inflige-15-me-damende-au-sous-traitant-dedalus/) : faits, montant, manquements.
- Pour recouper : [CNIL – lettre d'information d'avril 2022](https://www.cnil.fr/sites/default/files/atoms/files/lettre_information_cnil_avril_2022.html) et [Orrick – Fine for failing to enter into a data processing agreement](https://www.orrick.com/en/Insights/2022/04/French-Data-Protection-Authority-Fines-Processor-for-Failing-to-Enter-into-Data-Processing-Agreement) (résultats de recherche, non lus en détail).

> [!NOTE]
> **À valider :** faits issus d'un article de presse spécialisée ; la délibération de la CNIL fait foi. Le jour exact de la décision n'est pas précisé dans la source consultée.
