# Cas réel – 37signals quitte le cloud : coût total et faire-faire

*BTS SIO SISR 1re année – CEJMA – S05*

> [!NOTE]
> **Comment travailler.** Lis le cas réel et ses sources, réponds par écrit aux questions, puis ouvre « Voir la réponse attendue ». Les faits viennent des sources citées en fin de page ; en cas de doute, **retourne à la source**. Ce cas complète l'étude de cas fictive de la séance.

## Le dossier

**Les faits.** **37signals**, éditeur des logiciels **Basecamp** et **HEY**, louait ses infrastructures chez **AWS** : sa facture cloud était d'environ **3,2 millions de dollars par an**. L'entreprise a décidé de **racheter ses propres serveurs**. Elle a acheté environ **700 000 dollars** de matériel **Dell**, **amorti dès 2023** selon ses propres chiffres. Sept applications, dont HEY, ont été **migrées** hors d'AWS, travail terminé à l'**été 2023**.

**Les économies annoncées.** En 2024, la facture cloud est tombée à environ **1,3 million de dollars par an**, entièrement pour le **stockage** (AWS S3). L'entreprise annonce **près de 2 millions de dollars d'économies par an**, et, au total, **plus de 10 millions** sur cinq ans (contre 7 millions prévus initialement), en incluant le **déplacement du stockage** (environ **10 pétaoctets**) vers des équipements en propre, qui devrait économiser environ **4 millions** sur cinq ans.

> [!WARNING]
> Ces chiffres sont **publiés par l'entreprise elle-même** (billet de son cofondateur). Ils décrivent **sa situation** : une équipe d'**administrateurs expérimentés**, une charge **stable** et **prévisible**. Ce n'est pas une règle générale.

## Pourquoi ce cas est utile

Il applique « **faire ou faire-faire** » et le **coût total de possession** à l'hébergement : **louer** (coût variable, souplesse) ou **posséder** (investissement, mais coût **plus bas** si la charge est stable et les compétences présentes).

## Questions

**1.** Vérifie l'ordre de grandeur des économies annuelles à partir des deux factures.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

3,2 - 1,3 = 1,9 million de dollars par an, soit **près de 2 millions**, conforme à l'annonce. L'économie réelle dépend aussi des **coûts propres** (hébergement des serveurs, électricité, personnel) que ce calcul **ne compte pas**.
</details>

**2.** Le matériel coûte 700 000 $ ; il est « amorti » en 2023 selon l'entreprise. Calcule en mois le **délai de retour** en supposant 1,9 M$ d'économie annuelle, puis explique pourquoi ce calcul est **trop optimiste**.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

700 000 / 1 900 000 ≈ 0,37 an, soit environ **4,4 mois**. C'est **optimiste** car il **ignore** l'hébergement physique, l'électricité, la maintenance, le **temps** des équipes et le **renouvellement** du matériel : le **coût total de possession** doit tout intégrer.
</details>

**3.** Une PME de 30 postes, avec un seul technicien, envisage de **quitter** son prestataire cloud pour installer ses serveurs. Cite **trois critères** de décision.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(1) **Compétences** disponibles (administration, sécurité, supervision) ; (2) **stabilité** de la charge (un besoin qui varie beaucoup favorise le cloud) ; (3) **coût total** sur plusieurs années, **tous coûts compris** ; (4) **continuité** (sauvegarde, astreinte, reprise d'activité) ; (5) **risques** (panne, sinistre : voir le cas d'OVH en séance 7).
</details>

## Sources

- [DHH – Our cloud exit savings will now top $10 million over five years](https://world.hey.com/dhh/our-cloud-exit-savings-will-now-top-10-million-over-five-years-c7d9b5bd) : facture cloud, matériel, économies, stockage (source de l'entreprise).
- Pour recouper : [DCD – 37signals claims it saved almost $2m last year](https://www.datacenterdynamics.com/en/news/37signals-claims-it-saved-almost-2m-last-year-from-cloud-repatriation) et [The Register – 37signals is completing its on-prem move](https://www.theregister.com/2025/05/09/37signals_cloud_repatriation_storage_savings) (résultats de recherche, non lus en détail).

> [!NOTE]
> **À valider :** chiffres **non audités**, issus de l'entreprise ; la date du billet est d'octobre 2024 (d'après le texte consulté) et la suite du projet de stockage n'est pas vérifiée.
