# Étude de cas – Le service desk de Maréchal Logistique

*BTS SIO SISR 1re année – CEJMA – S08*

> [!NOTE]
> **Comment travailler.** Lis le dossier, puis réponds **par écrit** à chaque question, avec une réponse **construite et argumentée** : une idée, sa justification, l'exemple tiré du dossier. Ouvre ensuite « Voir la réponse attendue » pour te corriger. À l'épreuve E4, une réponse sans justification n'est pas complète.

## Dossier : le service desk de Maréchal Logistique

> [!NOTE]
> L'entreprise, les personnes et les chiffres sont **fictifs**.

### Document 1 – L'entreprise

**Maréchal Logistique** emploie **320 salariés** répartis sur 4 entrepôts. La DSI compte 7 personnes : une **responsable**, **Hélène** ; trois techniciens N1 ; deux techniciens N2 ; un expert N3. Un seul numéro de téléphone et un portail permettent de déclarer un problème. Beaucoup de salariés appellent directement « le technicien qu'ils connaissent », ce qui empêche de suivre les demandes. Les techniciens se **coordonnent surtout oralement**, sans procédure écrite.

### Document 2 – Les chiffres d'un mois

**1 200 tickets** ; résolus en N1 : **70 %** ; en N2 : **22 %** ; en N3 : **8 %**. Coût moyen par ticket : **12 €** (N1), **45 €** (N2), **130 €** (N3). Hélène propose de créer une **base de connaissances** et des **procédures** pour le N1, avec un objectif de **80 %**, **16 %** et **4 %**.

### Document 3 – Les ressources

Serveurs et postes (matériel), un **outil de gestion des tickets** (logiciel), la **connaissance** accumulée par les deux N2 les plus anciens (jamais écrite), un budget annuel, une **certification ITIL** passée par Hélène.

### Document 4 – Deux situations de management

**Situation A** : un entrepôt est paralysé par une panne réseau. Hélène dit à l'équipe : « Karim, tu coupes le switch 2. Léa, tu passes sur le câble principal. Pas de discussion. »

**Situation B** : Hélène réunit les techniciens pour choisir l'outil de gestion des tickets : elle présente trois options, écoute les avis, puis la décision est prise **en commun**.

### Questions

**1.** Classez les ressources du document 3 en **tangibles**, **intangibles**, **humaines** et **financières**. Quelle ressource est la plus **fragile** ? Pourquoi ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

- **Tangibles** : serveurs et postes.
- **Intangibles** : outil de gestion des tickets (logiciel), connaissance accumulée par les deux N2.
- **Humaines** : les compétences des techniciens, la certification d'Hélène.
- **Financières** : le budget annuel.

La plus fragile : la **connaissance non écrite** des deux N2 : si l'un d'eux part, elle disparaît. Il faut la **formaliser** (base de connaissances).
</details>

**2.** Quel **mécanisme de coordination** domine aujourd'hui ? Lequel proposez-vous de renforcer ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Aujourd'hui l'**ajustement mutuel** (échanges oraux) domine. On propose de renforcer la **standardisation des procédés** (procédures écrites, escalade) et la **standardisation des résultats** (objectifs de résolution par niveau).
</details>

**3.** Quel **style de management** illustrent les situations A et B ? Justifiez et dites si les choix sont adaptés.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

- **A : autoritaire**, Hélène décide seule et donne des ordres, sans discussion : style **adapté** à l'urgence (panne qui paralyse un entrepôt).
- **B : participatif**, elle consulte et décide en commun : style **adapté** à un choix d'outil qui touche le quotidien de tous et qui ne presse pas.

Un bon manager **adapte** son style à la situation.
</details>

**4.** À quel **niveau de management** (stratégique, tactique, opérationnel) correspondent : décider de passer en cloud ; planifier la migration ; couper un switch ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Passer en cloud : **stratégique**. Planifier la migration : **tactique**. Couper un switch : **opérationnel**.
</details>

**5.** Calculez le **coût actuel** du support et le coût après amélioration. Quelle est l'**économie** ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

- Actuel : N1 840 × 12 = 10 080 ; N2 264 × 45 = 11 880 ; N3 96 × 130 = 12 480 ; **total 34 440 €** (28,70 € par ticket).
- Après : N1 960 × 12 = 11 520 ; N2 192 × 45 = 8 640 ; N3 48 × 130 = 6 240 ; **total 26 400 €** (22 € par ticket).
- Économie : **8 040 € par mois**, soit **23,3 %**.
</details>

**6.** Pourquoi le **coût total baisse-t-il** alors que le N1 traite plus de tickets ? Quelle **condition** doit être remplie pour que l'objectif de 80 % soit réaliste ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Un ticket résolu en N1 coûte **beaucoup moins** qu'en N3 (12 € contre 130 €) : déplacer des tickets vers le bas fait baisser le coût moyen. La condition : le N1 doit avoir les **moyens de résoudre** (procédures, base de connaissances, **formation**), et la **qualité** doit rester bonne (mesurée par la **satisfaction** et le taux de **réouverture**) : un N1 qui « résout » trop vite pourrait gonfler artificiellement le taux.
</details>

**7.** Pourquoi le **point de contact unique** est-il important ? Que fait-il perdre quand on le contourne ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Il garantit que **toute demande est enregistrée**, priorisée et suivie. Quand on appelle directement un technicien, la demande n'est **pas tracée**, les **statistiques** sont faussées, la charge est mal répartie et la **connaissance** n'est pas capitalisée.
</details>

**8.** **Proposez une organisation** (cinq lignes) : règles pour le service desk, niveaux, escalade, indicateurs.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Réponse type : (1) **Tout** passe par le portail ou le numéro unique ; (2) **N1** : enregistrement et résolution des cas à procédure ; (3) **N2** : cas techniques ; **N3** : expert ; (4) **escalade** fonctionnelle selon un délai défini (par exemple, passage en N2 au bout d'une heure) et **hiérarchique** pour les incidents majeurs ; (5) **indicateurs** : taux de résolution par niveau, délai de résolution, satisfaction, réouvertures.
</details>


## Je sais faire

Coche honnêtement ; ce que tu ne coches pas se reprend avant la séance suivante.

- [ ] Classer des ressources en tangibles, intangibles, humaines, financières
- [ ] Citer trois mécanismes de coordination
- [ ] Associer un style de management à une situation
- [ ] Décrire les rôles de N1, N2, N3
- [ ] Calculer un coût par niveau et une économie

**Ce que je dois reprendre :** ______________________

**Ma question à poser à l'enseignant :** ______________________
