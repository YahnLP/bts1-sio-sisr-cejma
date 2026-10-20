# Étude de cas – Intrusion chez Optimum Compta

*BTS SIO SISR 1re année – CEJM et CEJMA – S07*

> [!NOTE]
> **Comment travailler.** Lis le dossier, puis réponds **par écrit** à chaque question, avec une réponse **construite et argumentée** : une idée, sa justification, l'exemple tiré du dossier. Ouvre ensuite « Voir la réponse attendue » pour te corriger. À l'épreuve E4, une réponse sans justification n'est pas complète.

## Dossier : une intrusion chez Optimum Compta

> [!NOTE]
> L'entreprise, les personnes et les chiffres sont **fictifs**.

### Document 1 – Les faits

**Optimum Compta** est un cabinet comptable de 30 salariés. **Samir**, administrateur système salarié, a reçu en janvier deux alertes de l'outil de supervision signalant que le **port d'administration à distance** (SSH) était **ouvert sur Internet** avec le compte **« admin »** et un mot de passe faible. Il a averti oralement son directeur, M. Roux, qui a répondu : « on verra après la période fiscale ». En avril, un attaquant se connecte avec ce compte, **chiffre les dossiers des clients** et demande une rançon. Le cabinet ne peut plus établir les déclarations fiscales de ses clients pendant trois semaines.

### Document 2 – Les conséquences

Un client, la société **Pavillon**, déclare un préjudice de **40 000 €** (pénalités fiscales et perte d'activité). Le contrat avec Pavillon prévoit une **responsabilité du cabinet plafonnée à douze mois d'honoraires**, soit des honoraires de **2 500 € par mois**. Il n'y a **pas de clause** excluant la faute lourde.

### Document 3 – Un second problème

En mars, par curiosité, Samir a **ouvert la messagerie personnelle** d'une salariée, Mme Dumas (dossier « Personnel »), pour y lire des échanges. Il n'avait aucune mission le justifiant. Mme Dumas l'a appris et a porté plainte.

### Questions

**1.** Qui est **l'auteur de l'infraction** d'intrusion ? Citez l'**article** et la **peine**. Quelle autre infraction commet-il en chiffrant les dossiers ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

L'**attaquant** commet l'**accès frauduleux** à un système de traitement automatisé de données (article **323-1** du Code pénal). Comme il a **modifié** les données (chiffrement), la peine monte à **5 ans d'emprisonnement et 150 000 €** d'amende. Il commet aussi une **entrave** au fonctionnement du système (article **323-2** : **5 ans** et **150 000 €**), puisque les dossiers sont inutilisables.
</details>

**2.** Pavillon peut-il **engager la responsabilité du cabinet** ? Vérifiez les **trois conditions**.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Responsabilité **contractuelle** (il y a un contrat). **Faute** : ne pas avoir corrigé une faille connue (accès ouvert et mot de passe faible) malgré deux alertes. **Dommage** : 40 000 € de préjudice. **Lien de causalité** : l'intrusion a rendu les dossiers inutilisables et empêché les déclarations. Les trois conditions sont réunies, si le prestataire n'a pas pris les mesures de sécurité attendues. Le cabinet pourra opposer la **force majeure** (cyberattaque), mais la faille était **connue**, ce qui l'affaiblit.
</details>

**3.** Calculez le **plafond de responsabilité** et ce que Pavillon peut obtenir. Cette clause est-elle opposable dans tous les cas ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Plafond : 12 × 2 500 = **30 000 €**. Pavillon pourrait obtenir 30 000 € sur 40 000 € de préjudice, soit 10 000 € laissés à sa charge. La clause **n'est pas opposable** si la **faute est lourde ou dolosive** ou si elle prive de sa substance l'obligation essentielle du cabinet (voir séance 4). Ignorer deux alertes sur une faille connue pendant plusieurs mois peut être discuté comme une **faute lourde** : Pavillon pourrait donc demander **plus de 30 000 €**.
</details>

**4.** **Samir** peut-il être poursuivi **civilement** par Pavillon ? Par son employeur ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Non en principe : il a agi **dans le cadre de sa mission** et l'**employeur répond** vis-à-vis des victimes de ses salariés (article 1242, alinéa 5). Samir n'a pas commis de faute **intentionnelle** (il a alerté). De plus, c'est le directeur qui a retardé la correction. L'employeur ne peut pas, en principe, lui demander de rembourser les dommages d'une erreur professionnelle.
</details>

**5.** Quelle est la **situation de Samir** au regard de l'ouverture de la messagerie de Mme Dumas ? Citez l'article et la peine encourue, puis la sanction **disciplinaire** possible.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Il a lu une **correspondance privée** sans mission : **atteinte au secret des correspondances** (article **226-15** du Code pénal), **1 an d'emprisonnement** et **45 000 €** d'amende. Être administrateur ne lui donne pas le droit de lire ce qui est privé. Sur le plan **disciplinaire**, c'est une faute qui peut être qualifiée de **grave** (voire lourde s'il y avait une intention de nuire) et justifier un **licenciement**. Mme Dumas peut aussi demander des **dommages-intérêts** (civil).
</details>

**6.** M. Roux, le directeur, peut-il voir sa **responsabilité** engagée ? À quel titre ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Oui. **Civil** : l'entreprise répond contractuellement envers Pavillon, et son dirigeant a pris la décision de ne pas corriger. **Pénal** : en tant que dirigeant, sur la **négligence** (article 121-3) si on démontre une **faute caractérisée** ; la **personne morale** peut aussi être poursuivie dans certains cas ; et le **manquement à la sécurité des données personnelles** (article 226-17) concerne tout traitement de données de clients et de salariés. L'appréciation dépend des faits et relève du juge.
</details>

**7.** Que **devait faire** Samir pour se protéger après la réponse « on verra après la période fiscale » ? Citez **trois** actions.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(1) **Confirmer par écrit** (courriel) l'alerte, le risque et la réponse reçue ; (2) **proposer une mesure** immédiate de faible coût (fermer le port, imposer une clé SSH, changer le mot de passe) ; (3) **escalader** vers une instance supérieure (direction générale, DPO, prestataire) si le risque est élevé ; conserver les **traces**. Il pouvait aussi **appliquer lui-même** la mesure d'urgence dans la limite de sa mission, avec information de la direction.
</details>

**8.** Rédigez **huit lignes maximum** à destination de M. Roux : les risques encourus par le cabinet et les mesures à prendre.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Réponse type : (1) **Risque civil** : indemnisation de Pavillon jusqu'à 30 000 € (davantage si la faute est jugée lourde) et d'autres clients ; (2) **risque pénal et administratif** : manquement à la sécurité des données ; (3) **image** et perte de clients ; (4) **mesures** : fermer l'accès, restaurer depuis des sauvegardes, notifier les clients et, si des données personnelles sont concernées, **notifier la CNIL** dans les délais (séance 15), (5) **traiter le cas de Samir** avec une procédure disciplinaire proportionnée, (6) **organiser la sécurité** : politique d'accès, procédure d'alerte écrite, formation. La note doit être **claire, hiérarchisée** et **chiffrée**.
</details>


## Je sais faire

Coche honnêtement ; ce que tu ne coches pas se reprend avant la séance suivante.

- [ ] Citer les trois conditions de la responsabilité civile
- [ ] Distinguer obligation de moyens et de résultat
- [ ] Citer 323-1, 323-2, 226-15 avec leurs peines
- [ ] Distinguer faute simple, grave et lourde
- [ ] Citer trois réflexes de protection d'un administrateur

**Ce que je dois reprendre :** ______________________

**Ma question à poser à l'enseignant :** ______________________
