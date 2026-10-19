# Cours – Contrat de prestation, validité et sanctions ; cadre du salarié d'ESN

*BTS SIO SISR 1re année – CEJMA – S04 – à lire avant l'[étude de cas](02-etude-de-cas.md)*

> [!NOTE] Ce que tu dois savoir déjà
> - **Prérequis :** S01 (régie, forfait, obligations de moyens et de résultat)

## À la fin de ce cours tu sauras

- [ ] Énoncer les **conditions de validité** d'un contrat et les **vices du consentement**
- [ ] Identifier les **clauses clés** d'un contrat de prestation informatique
- [ ] Appliquer les règles sur la **clause limitative**, la **clause pénale** et le **déséquilibre significatif**
- [ ] Citer les **sanctions** de l'inexécution
- [ ] Situer le **contrat de travail** en ESN (Syntec) et le **portage salarial**

## I. Qu'est-ce qu'un contrat ?

Un **contrat** est un **accord de volontés** entre deux ou plusieurs personnes, destiné à **créer, modifier, transmettre ou éteindre des obligations** (Code civil, article 1101). Un contrat **légalement formé** s'impose aux parties **comme une loi** (article 1103) : on l'appelle la **force obligatoire** du contrat.

Les parties doivent négocier, conclure et exécuter le contrat **de bonne foi** (article 1104).

| Classement | Définition | Exemple |
|---|---|---|
| **Synallagmatique** | Chaque partie s'oblige envers l'autre | Prestation contre prix |
| **Onéreux** | Chacun reçoit un avantage en échange | Vente de matériel |
| **De gré à gré** | Les clauses sont **négociées** | Contrat d'infogérance sur mesure |
| **D'adhésion** | Les clauses sont **imposées** par une partie et non négociables | Conditions générales d'un service en ligne |
| **Consensuel** | Il suffit d'un échange de consentements | La plupart des contrats |

## II. La formation du contrat

### Les conditions de validité

Selon l'article 1128 du Code civil, trois conditions sont **nécessaires** à la validité d'un contrat :

1. le **consentement** des parties ;
2. leur **capacité** de contracter (un mineur non émancipé, par exemple, ne peut pas contracter seul pour les actes qui dépassent la vie courante) ;
3. un **contenu licite et certain**.

### Les vices du consentement

Le consentement est **vicié** s'il est donné par **erreur**, obtenu par **dol** ou extorqué par **violence**.

| Vice | Définition | Exemple dans l'informatique |
|---|---|---|
| **Erreur** | Fausse idée sur une **qualité essentielle** de la prestation | Le client croit acheter une solution compatible avec son système, ce qui n'est pas le cas |
| **Dol** | **Manœuvre ou mensonge** (ou silence) destiné à obtenir le consentement | Le prestataire annonce 99,99 % de disponibilité alors qu'il sait ne pas pouvoir la garantir |
| **Violence** | Pression qui conduit à s'engager par crainte | Menace de couper un service critique pour imposer un contrat |

Un contrat vicié peut être **annulé** (nullité) et les parties sont **remises dans la situation d'origine**.

### Le devoir d'information

Avant de signer, la partie qui détient une **information déterminante** pour l'autre doit la lui **donner** (article 1112-1). Un prestataire doit donc informer sur les limites techniques de sa solution.

## III. Le contrat de prestation de services informatiques

C'est le contrat le plus courant pour une ESN. Ses **clauses essentielles** :

| Clause | À quoi elle sert | Point de vigilance |
|---|---|---|
| **Objet et périmètre** | Décrire précisément la mission, ce qui est **inclus** et **exclu** | Un périmètre flou crée des litiges |
| **Durée et reconduction** | Fixer la durée et les conditions de renouvellement | **Tacite reconduction**, préavis de résiliation |
| **Prix et facturation** | Prix, périodicité, révision | Forfait, régie, redevance mensuelle |
| **Niveaux de service (SLA)** | Engagements mesurables : disponibilité, délais de prise en charge et de rétablissement | Définir **comment** on mesure |
| **Obligation de moyens ou de résultat** | Fixer l'intensité de l'engagement | Voir séance 1 et séance 7 |
| **Recette** | Procédure de **validation** par le client | Critères objectifs, délai |
| **Pénalités** | Sanctions automatiques en cas de manquement | Plafond |
| **Responsabilité** | Limite de la réparation (plafond) | Voir ci-dessous |
| **Confidentialité et données** | Secret des informations ; **sous-traitance des données personnelles** | Annexe RGPD (séance 13) |
| **Propriété intellectuelle** | Qui possède les livrables ? | Séance 16 |
| **Réversibilité** | Récupération des données et du service en fin de contrat | Indispensable en cloud |
| **Résiliation** | Cas de fin anticipée | Manquement grave |

### La clause limitative de responsabilité

Les parties peuvent **plafonner** les dommages-intérêts (par exemple : douze mois de redevances). Cette clause **n'est pas toujours efficace** : elle ne couvre pas la **faute lourde** ni le **dol**, et elle ne peut pas **priver de sa substance** l'obligation essentielle du contrat, sinon elle est **réputée non écrite** (article 1170).

### La clause pénale

La **clause pénale** fixe **à l'avance** le montant de la pénalité en cas d'inexécution (article 1231-5). Le juge peut **modérer** ou **augmenter** la pénalité si elle est manifestement excessive ou dérisoire.

### Un contrat d'adhésion peut être déséquilibré

Dans un contrat d'**adhésion**, toute clause qui crée un **déséquilibre significatif** entre les droits et obligations des parties est **réputée non écrite** (article 1171). C'est une protection contre les conditions générales abusives.

## IV. Quand le contrat n'est pas respecté

Si une partie n'exécute pas (ou mal) son obligation, l'autre peut (article 1217) :

- refuser d'exécuter à son tour (**exception d'inexécution**) ;
- demander l'**exécution forcée** ;
- demander une **réduction du prix** ;
- provoquer la **résolution** (fin du contrat) ;
- demander des **dommages-intérêts**.

On peut **cumuler** certaines de ces sanctions. Avant d'agir, on envoie en général une **mise en demeure** écrite.

## V. Un autre contrat : le contrat de travail dans les ESN

L'alternant, le technicien et le consultant sont liés par un **contrat de travail** : le salarié travaille sous l'**autorité** de l'employeur, contre une **rémunération**. Les ESN sont dans le champ de la **convention collective** des bureaux d'études techniques, cabinets d'ingénieurs-conseils et sociétés de conseils, dite **Syntec**.

### Les trois modalités de durée du travail (Syntec)

| Modalité | Pour qui | Durée du travail |
|---|---|---|
| **1 – Horaire standard** | Cas général | **35 heures** par semaine |
| **2 – Réalisation de missions** | Salariés avec une certaine autonomie | Jusqu'à **38 h 30** par semaine, dans la limite de **219 jours** par an, avec une rémunération d'au moins **115 %** du minimum conventionnel |
| **3 – Forfait annuel en jours** | **Cadres autonomes** | **218 jours** par an, sans décompte en heures |

> [!NOTE]
> Les seuils et conditions exacts évoluent : on les vérifie dans le texte de la convention en vigueur avant de les utiliser dans un document officiel.

### Le portage salarial

Le **portage salarial** est une relation à **trois** : un **professionnel** autonome (le **salarié porté**) trouve lui-même ses clients ; une **entreprise de portage** le salarie et facture le client ; l'**entreprise cliente** paie la prestation. Le porté bénéficie du **statut de salarié** (assurance chômage, protection sociale) tout en gardant son autonomie commerciale. Le Code du travail l'encadre aux articles **L1254-1 et suivants**.

| | **Salarié d'ESN** | **Salarié porté** | **Indépendant** |
|---|---|---|---|
| Qui trouve les clients ? | L'ESN | Le porté | L'indépendant |
| Statut | Salarié | Salarié (de la société de portage) | Non salarié |
| Protection sociale | Celle des salariés | Celle des salariés | Régime des indépendants |
| Liberté | Moindre | Forte | Très forte |
| Risque | Faible | Modéré | Élevé |

## À retenir

- Le contrat est un **accord de volontés** qui **s'impose** aux parties ; on l'exécute de **bonne foi**.
- Trois conditions de validité : **consentement**, **capacité**, **contenu licite et certain** ; vices du consentement : **erreur, dol, violence**.
- Clauses clés d'un contrat de prestation : **périmètre, durée, prix, SLA, recette, pénalités, responsabilité, données, propriété intellectuelle, réversibilité**.
- Une clause **limitative de responsabilité** est écartée en cas de **faute lourde** ou de dol ; une clause **abusive** d'un contrat d'adhésion est **réputée non écrite**.
- Sanctions de l'inexécution : **exception d'inexécution, exécution forcée, réduction du prix, résolution, dommages-intérêts**.
- Le salarié d'une ESN relève de la convention **Syntec** (trois modalités de durée du travail) ; le **portage salarial** est une relation à trois.
