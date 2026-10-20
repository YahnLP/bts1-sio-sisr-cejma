# Cours – RGPD : droits des personnes, cookies, prospection et transferts

*BTS SIO SISR 1re année – CEJMA – S14 – à lire avant l'[étude de cas](02-etude-de-cas.md)*

> [!NOTE] Ce que tu dois savoir déjà
> - **Prérequis :** S13

## À la fin de ce cours tu sauras

- [ ] Citer les **droits** des personnes
- [ ] Appliquer les **délais** de réponse
- [ ] Évaluer une **bannière cookies**
- [ ] Distinguer les règles de **prospection**
- [ ] Repérer un **transfert hors UE**

## I. Les droits des personnes

Le RGPD donne aux personnes des **droits** que l'organisation doit **faciliter**.

| Droit | Article | Contenu |
|---|---|---|
| **Information** | 13, 14 | Savoir qui traite quoi, pourquoi, combien de temps |
| **Accès** | 15 | Obtenir **copie** de ses données et des informations sur le traitement |
| **Rectification** | 16 | Faire corriger des données inexactes |
| **Effacement** (« droit à l'oubli ») | 17 | Faire supprimer, dans certains cas |
| **Limitation** | 18 | Geler temporairement le traitement |
| **Portabilité** | 20 | Récupérer ses données dans un format **structuré** et courant, et les transmettre à un autre responsable |
| **Opposition** | 21 | S'opposer, notamment à la **prospection** (sans condition) |
| **Décision automatisée** | 22 | Ne pas subir une décision fondée **uniquement** sur un traitement automatisé produisant des effets importants |

> [!NOTE]
> Certains droits ont des **conditions** : le droit à l'effacement n'est pas absolu (obligation légale de conserver, exercice de droits en justice…) ; la portabilité ne vise que les données **fournies par la personne** traitées sur la base du **consentement** ou du **contrat**.

## II. Répondre à une demande

| Étape | Règle |
|---|---|
| **Réception** | Toute demande est valable, **sans formalisme** (courriel, courrier, formulaire) |
| **Vérification d'identité** | Raisonnable et proportionnée (éviter de demander trop de pièces) |
| **Délai** | **Un mois** à compter de la réception ; prolongeable de **deux mois** si la demande est complexe ou nombreuse, avec information de la personne |
| **Gratuité** | En principe **gratuit** (frais raisonnables si demande manifestement infondée ou excessive) |
| **Réponse** | Claire, compréhensible, dans un format accessible |
| **Refus** | Motivé, avec rappel du droit de **réclamation** auprès de la CNIL et du recours juridictionnel |
| **Traçabilité** | Registre des demandes et des réponses |

## III. Cookies et traceurs

La directive « **ePrivacy** » (transposée en France) et le RGPD exigent, pour déposer un traceur non nécessaire au service (publicité, mesure d'audience non exemptée), le **consentement préalable** de l'utilisateur.

| Exigence | Détail |
|---|---|
| **Information** | Finalités claires avant le dépôt |
| **Consentement** | Libre, éclairé, univoque, **avant** le dépôt |
| **Refuser aussi simple qu'accepter** | Bouton « tout refuser » aussi visible que « tout accepter » |
| **Retrait** | Possible à tout moment |
| **Exemptés** | Traceurs strictement nécessaires (panier, session, sécurité) |

## IV. La prospection commerciale

| Cible | Règle |
|---|---|
| **Particuliers** (courriel, SMS) | **Consentement préalable** (« opt-in ») en principe ; exception pour clients existants et produits analogues |
| **Professionnels** (courriel professionnel) | Possible sans consentement préalable si le message est **en rapport avec leur fonction**, avec information et **opposition** facile |
| **Tous** | Droit d'**opposition** et lien de **désinscription** dans chaque message |

## V. Transferts hors de l'Union européenne

Transférer des données hors UE n'est possible que si le pays offre un niveau de protection **adéquat** (décision d'adéquation de la Commission) ou si l'on utilise des **garanties** (clauses contractuelles types, règles d'entreprise contraignantes). Les prestataires **cloud** sont concernés : vérifier le **lieu de traitement** et les **sous-traitants ultérieurs**.

## Comprendre pas à pas

### Traiter une demande d'accès : un calendrier

Une cliente écrit le **3 mars** : « Je veux une copie de mes données. »

| Étape | Ce que tu fais | Échéance |
|---|---|---|
| **Réception** | Accuser réception ; demande valable **sans formalisme** | 3 mars |
| **Identité** | Vérifier **proportionnellement** (pas trop de pièces) | Dès que possible |
| **Collecte** | Rechercher dans tous les systèmes (CRM, messagerie, sauvegardes concernées) | Avant la fin de la période |
| **Réponse** | Envoyer la copie et les informations demandées | **3 avril** (un mois) |
| **Si la demande est complexe** | Informer la personne de la prolongation avant l'échéance | Jusqu'au **3 juin** (deux mois en plus) |

> [!WARNING]
> **Ne pas répondre** n'est pas une option : la personne peut saisir la **CNIL**. Garde la **trace** de la demande et de la réponse.

### Cookies : lire une bannière comme un auditeur

| Critère | Conforme | Non conforme |
|---|---|---|
| Dépôt avant le choix | Aucun traceur non nécessaire déposé | Cookies publicitaires déposés dès l'arrivée |
| Boutons | « Tout accepter » **et** « Tout refuser » de même niveau | « Refuser » caché dans un sous-menu |
| Libellés | Clairs | Ambigus (« Continuer », « OK ») |
| Retrait | Lien permanent pour changer d'avis | Impossible sans vider le navigateur |

### Prospection : l'arbre de décision

1. **La cible est-elle un particulier ?** Oui → **consentement préalable** (sauf clients existants et produits analogues).
2. **Un professionnel, message en rapport avec sa fonction ?** Oui → possible **sans** consentement préalable, avec **information** et **opposition** facile.
3. **Dans tous les cas** : lien de **désinscription** dans chaque message, et **opposition** respectée sans condition.

Un cas réel est détaillé dans [Cookies : Google et Facebook](04-cas-reels.md).

## À retenir

- Droits : information, accès, rectification, effacement, limitation, portabilité, opposition, décision automatisée.
- Réponse sous **un mois** (prolongeable de deux), gratuite en principe, sans formalisme.
- Cookies : **consentement avant dépôt**, refuser aussi simple qu'accepter.
- Prospection des particuliers : **opt-in** ; opposition toujours possible.
- Transferts hors UE : décision d'**adéquation** ou **garanties**.
