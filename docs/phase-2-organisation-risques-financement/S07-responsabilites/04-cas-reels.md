# Cas réel – L'incendie d'OVH à Strasbourg : qui est responsable ?

*BTS SIO SISR 1re année – CEJM et CEJMA – S07*

> [!NOTE]
> **Comment travailler.** Lis le cas réel et ses sources, réponds par écrit aux questions, puis ouvre « Voir la réponse attendue ». Les faits viennent des sources citées en fin de page ; en cas de doute, **retourne à la source**. Ce cas complète l'étude de cas fictive de la séance.

## Le dossier

**Les faits.** Dans la nuit du **9 au 10 mars 2021**, un incendie détruit un datacenter d'**OVH** à **Strasbourg** (site SBG2). Un client, la société **France Bati Courtage**, avait loué un **serveur virtuel (VPS)** avec une **option de sauvegarde automatisée**. Les **sauvegardes** étaient stockées **dans le même bâtiment** que le serveur principal : elles ont été **détruites** avec lui. Le client a assigné OVH le **19 juillet 2021** et réclamait **plus de 6,5 M€**.

**La décision.** Le **26 janvier 2023**, le **tribunal de commerce de Lille Métropole** juge que :

- OVH a commis un **manquement contractuel** : le contrat décrivait un stockage **« physiquement isolé »** avec **trois réplications**, alors que les sauvegardes étaient au **même endroit** que le serveur principal ;
- la **faute lourde** d'OVH et de **graves manquements** aux règles de sécurité incendie ne sont **pas retenus** ;
- la présentation commerciale de l'option de sauvegarde ne correspondait pas à l'offre souscrite et avait été **créée ou modifiée après** l'incendie et la souscription.

**La condamnation.** Environ **101 100 €** :

| Poste | Montant |
|---|---:|
| Préjudice financier 2021 | 38 530 € |
| Perte d'un actif incorporel | 26 472 € |
| Atteinte à l'image | 20 000 € |
| Restitution de l'hébergement, des données et des sites | 9 100 € |
| Article 700 du Code de procédure civile (frais de procès) | 7 000 € |

Selon la source, une **action collective** de clients était toujours en cours. OVH pouvait faire appel.

## Pourquoi ce cas est utile

Il applique les trois conditions de la **responsabilité civile** (faute, dommage, lien de causalité) à un cas **contractuel** : la faute est un **manquement à une promesse** (stockage isolé) et non une simple malchance (l'incendie). Il montre aussi l'écart entre **ce que le client réclame** et **ce que le juge accorde**.

## Questions

**1.** Vérifie le total de la condamnation, puis compare-le à la demande initiale.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

38 530 + 26 472 + 20 000 + 9 100 + 7 000 = 101 102 €, soit environ **101 100 €**. Par rapport à plus de 6,5 M€ réclamés : 101 102 / 6 500 000 ≈ 1,6 % **au plus** (la demande était supérieure à 6,5 M€). Le juge **n'accorde pas** tout ce qui est réclamé : il faut **prouver** chaque préjudice.
</details>

**2.** Identifie la **faute**, le **dommage** et le **lien de causalité** dans ce cas.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

**Faute** : sauvegardes stockées au **même endroit** que le serveur, contrairement à ce que le contrat décrivait. **Dommage** : perte des données et préjudices financiers et d'image du client. **Lien de causalité** : si les sauvegardes avaient été **isolées**, elles auraient **survécu** à l'incendie.
</details>

**3.** Tu administres le serveur d'une PME. Cite **trois mesures** pour éviter que ce scénario ne se reproduise chez elle.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(1) **Au moins une copie hors site** (autre bâtiment ou prestataire) ; (2) **tester régulièrement la restauration** ; (3) **lire le contrat** du prestataire (ce qui est réellement promis pour la sauvegarde) et **conserver** ses documents commerciaux. Option : sauvegarde déconnectée (hors ligne).
</details>

## Sources

- [Le Monde Informatique – OVH condamné à verser plus de 100 000 euros](https://www.lemondeinformatique.fr/actualites/lire-incendie-sgb2-strasbourg-ovh-condamne-a-verser-plus-de-100-000-eteuro-89434.html) : faits, jugement du 26 janvier 2023, motifs, montants.
- Pour recouper : [Siècle Digital](https://siecledigital.fr/2023/02/06/ovhcloud-condamne-a-indemniser-un-de-ses-clients-apres-la-perte-de-ses-donnees/) et [Clubic](https://www.clubic.com/ovh/actualite-456327-pourquoi-ovh-est-condamne-a-verser-100-000-a-un-client-dont-le-serveur-a-brule-lors-de-l-incendie-de-strasbourg.html) (résultats de recherche, non lus en détail).

> [!NOTE]
> **À valider :** le jugement est de **première instance** ; l'article ne mentionne pas de clause limitative de responsabilité ni les suites d'un éventuel appel. Les faits sont issus de la presse ; le jugement fait foi.
