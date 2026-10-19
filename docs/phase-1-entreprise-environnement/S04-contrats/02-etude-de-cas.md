# Étude de cas – Le contrat d'infogérance de la clinique Aubier

*BTS SIO SISR 1re année – CEJMA – S04*

> [!NOTE]
> **Comment travailler.** Lis le dossier, puis réponds **par écrit** à chaque question, avec une réponse **construite et argumentée** : une idée, sa justification, l'exemple tiré du dossier. Ouvre ensuite « Voir la réponse attendue » pour te corriger. À l'épreuve E4, une réponse sans justification n'est pas complète.

## Dossier : le contrat d'infogérance de la clinique Aubier

> [!NOTE]
> L'entreprise, le contrat et les chiffres sont **fictifs**. Les articles cités sont ceux du Code civil.

### Document 1 – Le contexte

La **clinique vétérinaire Aubier** (12 salariés) confie à l'ESN **Brise Informatique** l'exploitation de ses postes et de son serveur de dossiers cliniques. Le commercial de Brise a promis oralement : « **vous aurez 99,99 % de disponibilité** ». Le contrat signé, rédigé par Brise, n'a pas été négocié.

### Document 2 – Extrait du contrat

> **Art. 2 – Durée.** Le contrat est conclu pour **3 ans**, **reconduit tacitement** par périodes d'un an, sauf dénonciation **3 mois** avant l'échéance.
>
> **Art. 4 – Redevance.** **3 200 € HT par mois.**
>
> **Art. 5 – Niveau de service.** Brise s'engage à **rétablir** tout service critique dans un délai de **4 heures ouvrées**. Au-delà, une **pénalité de 2 % de la redevance mensuelle** est due **par tranche entière de 4 heures ouvrées de dépassement**, dans la limite de **20 % de la redevance mensuelle**.
>
> **Art. 8 – Responsabilité.** La responsabilité de Brise est **limitée à douze mois de redevances**, **quelle que soit la cause du dommage**.
>
> **Art. 9 – Réversibilité.** Aucune.

### Document 3 – L'incident

Le serveur de dossiers cliniques tombe en panne un lundi. Brise rétablit le service **14 heures ouvrées après la demande**. La clinique a dû reporter des opérations et estime son **préjudice à 90 000 €**.

### Questions

**1.** Qualifiez ce contrat : de gré à gré ou d'adhésion ? Quelle conséquence a cette qualification sur l'**article 8** ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Contrat d'**adhésion** : il a été rédigé par Brise et **non négocié**. Dans un contrat d'adhésion, une clause qui crée un **déséquilibre significatif** est **réputée non écrite** (article 1171). L'article 8 limite la responsabilité de Brise « quelle que soit la cause », ce qui peut être contesté comme déséquilibré. Il est aussi exposé à l'article 1170 si la clause vide de sa substance l'obligation essentielle de Brise (rétablir le service).
</details>

**2.** Calculez la **pénalité** due pour l'incident du document 3. Que se passerait-il pour un rétablissement après **64 heures** ouvrées ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

- Dépassement de l'incident : 14 − 4 = **10 heures**, soit **2 tranches entières** de 4 heures (8 heures) ; 2 × 2 % = **4 %** de 3 200 € = **128 €**.
- Pour 64 heures : dépassement de 60 heures, soit **15 tranches** ; 15 × 2 % = 30 %, supérieur au plafond de 20 % : la pénalité est **plafonnée** à 20 % de 3 200 € = **640 €**.
</details>

**3.** Quel **plafond de responsabilité** résulte de l'article 8 ? Que peut espérer la clinique pour un préjudice de 90 000 € ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Douze mois de redevances : 12 × 3 200 = **38 400 €**. Sauf si la clause est écartée (faute lourde, dol, article 1170 ou 1171), la clinique ne pourrait obtenir que **38 400 €** sur 90 000 € de préjudice, soit **51 600 €** de perte restant à sa charge.
</details>

**4.** La promesse orale de « 99,99 % de disponibilité » constitue-t-elle un **vice du consentement** ? Quelles informations manquent pour trancher ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Cela peut constituer un **dol** si Brise savait qu'elle ne pouvait pas tenir cet engagement et a **menti** (ou tu des informations déterminantes) pour obtenir la signature. Il faut savoir : si la promesse a été **déterminante** pour la clinique, si Brise **connaissait** ses limites techniques (le contrat ne garantit pas 99,99 %), et comment la clinique peut **prouver** une promesse **orale**. Cela relève aussi du **devoir d'information** (article 1112-1).
</details>

**5.** Quelle est la **sanction** possible pour Brise (articles 1217 et suivants) ? Quelle **démarche préalable** la clinique doit-elle accomplir ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

La clinique peut demander des **dommages-intérêts**, une **réduction du prix**, et dans les cas graves la **résolution** du contrat. Avant d'agir, elle envoie une **mise en demeure** écrite (demande de remédier au manquement dans un délai). Si l'inexécution est répétée, la résolution peut être demandée.
</details>

**6.** Quelles **clauses manquent** ou sont dangereuses pour la clinique ? Citez-en **trois** et proposez une rédaction courte pour l'une d'elles.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Clauses à revoir ou à ajouter : **réversibilité** (aucune : en fin de contrat, comment récupérer les dossiers cliniques ?), **plafond de responsabilité** (limité sans exception pour faute lourde), **données personnelles** (un contrat avec accès à des données exige une clause de sous-traitance : séance 13), **sauvegardes et reprise après sinistre** (rien n'est prévu), **tacite reconduction** (à surveiller, le préavis de 3 mois est une contrainte).

Exemple de rédaction : « À l'échéance ou à la résiliation du contrat, Brise restitue à la clinique, dans un délai de 30 jours et dans un format standard, l'ensemble des données et des configurations, et apporte son concours à la migration. »
</details>

**7.** Léa, salariée de Brise, est technicienne et **travaille 35 heures** par semaine. Quelle modalité de durée du travail Syntec lui est applicable ? À partir de quelle modalité parle-t-on de forfait annuel en jours ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

**Modalité 1** (horaire standard, 35 heures). Le **forfait annuel en jours** est la **modalité 3** : 218 jours par an, pour des **cadres autonomes**.
</details>

**8.** Comparez en cinq lignes le statut de **salarié d'ESN** et de **salarié porté** (qui trouve les clients, protection, risque).

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Le **salarié d'ESN** reçoit ses missions de son employeur, a un salaire régulier et une protection de salarié, mais moins de liberté. Le **salarié porté** trouve **lui-même** ses clients et négocie son prix, tout en étant **salarié** de la société de portage (protection sociale du salarié) ; son revenu dépend de son **activité commerciale** et il paie des frais de gestion à la société de portage. Le portage donne plus d'autonomie, au prix d'un risque d'inactivité plus élevé.
</details>


## Je sais faire

Coche honnêtement ; ce que tu ne coches pas se reprend avant la séance suivante.

- [ ] Citer les trois conditions de validité d'un contrat
- [ ] Distinguer erreur, dol et violence avec un exemple informatique
- [ ] Calculer une pénalité et un plafond de responsabilité à partir d'une clause
- [ ] Citer les sanctions de l'inexécution
- [ ] Citer les trois modalités de durée du travail Syntec

**Ce que je dois reprendre :** ______________________

**Ma question à poser à l'enseignant :** ______________________
