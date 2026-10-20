# Cours – RGPD : définitions, acteurs, principes et bases légales

*BTS SIO SISR 1re année – CEJMA – S13 – à lire avant l'[étude de cas](02-etude-de-cas.md)*

> [!NOTE] Ce que tu dois savoir déjà
> - **Prérequis :** S11, S12

## À la fin de ce cours tu sauras

- [ ] Définir **donnée personnelle** et **donnée sensible**
- [ ] Distinguer **responsable**, **sous-traitant**, **DPO**, **CNIL**
- [ ] Citer les **principes** de l'article 5
- [ ] Associer une **base légale** à une finalité
- [ ] Lister les **outils** de conformité

## I. Pourquoi le RGPD ?

Le **règlement général sur la protection des données (RGPD)**, règlement (UE) 2016/679, est applicable depuis le **25 mai 2018**. Il complète la loi française **Informatique et Libertés** de 1978. Son but : protéger les **personnes** dont on traite les données, et responsabiliser les organisations.

### Les définitions clés

| Notion | Définition |
|---|---|
| **Donnée personnelle** | Toute information se rapportant à une personne **identifiée ou identifiable** (nom, adresse IP, identifiant, photo, numéro de client) |
| **Donnée sensible** | Santé, origine, opinions politiques ou religieuses, appartenance syndicale, vie sexuelle, données génétiques ou biométriques d'identification : **traitement interdit en principe**, avec exceptions (article 9) |
| **Traitement** | Toute opération sur des données : collecter, enregistrer, consulter, transmettre, conserver, effacer |
| **Personne concernée** | La personne dont les données sont traitées |

## II. Les acteurs

| Acteur | Rôle |
|---|---|
| **Responsable de traitement** | Décide des **finalités** et des **moyens** ; porte la responsabilité principale |
| **Sous-traitant** | Traite les données **pour le compte** du responsable, sur ses instructions (ex. : hébergeur, éditeur SaaS, ESN) |
| **Responsables conjoints** | Décident ensemble des finalités et des moyens |
| **DPO** (délégué à la protection des données) | Conseille, contrôle, point de contact de la CNIL ; **obligatoire** dans certains cas (autorités publiques, suivi régulier à grande échelle, données sensibles à grande échelle) |
| **CNIL** | Autorité de contrôle française : conseille, contrôle, **sanctionne** |

> [!NOTE]
> Un prestataire informatique est souvent **sous-traitant** : un **contrat** (article 28) fixe l'objet, la durée, les instructions, la sécurité, la sous-traitance ultérieure, l'aide au responsable, la restitution ou suppression des données.

## III. Les principes (article 5)

| Principe | Signification |
|---|---|
| **Licéité, loyauté, transparence** | Base légale, information claire |
| **Limitation des finalités** | Des finalités **déterminées, explicites, légitimes** |
| **Minimisation** | Seules les données **nécessaires** |
| **Exactitude** | Données à jour |
| **Limitation de conservation** | Durée **limitée**, adaptée à la finalité |
| **Intégrité et confidentialité** | **Sécurité** adaptée |
| **Responsabilité (*accountability*)** | Pouvoir **démontrer** sa conformité |

## IV. Les bases légales (article 6)

Tout traitement doit reposer sur **une** des six bases :

| Base | Exemple |
|---|---|
| **Consentement** | Newsletter commerciale |
| **Contrat** | Livraison d'une commande |
| **Obligation légale** | Conservation des factures |
| **Sauvegarde d'intérêts vitaux** | Urgence médicale |
| **Mission d'intérêt public** | Service public |
| **Intérêts légitimes** | Sécurité du système, prévention de la fraude (avec mise en balance) |

Le **consentement** doit être **libre, spécifique, éclairé et univoque** ; il se retire aussi facilement qu'il se donne.

## V. Les outils de conformité

| Outil | Rôle |
|---|---|
| **Registre des traitements** (article 30) | Liste des traitements : finalités, données, durées, destinataires, mesures de sécurité |
| **Information des personnes** (articles 13 et 14) | Mentions : identité, finalités, base légale, durée, droits, contact |
| **Privacy by design / by default** (article 25) | Protection intégrée dès la conception, paramètres protecteurs par défaut |
| **AIPD** (article 35) | Analyse d'impact pour les traitements **à risque élevé** |
| **Contrats de sous-traitance** (article 28) | Cadre de la relation avec les prestataires |

## Comprendre pas à pas

### Qui est responsable de traitement, qui est sous-traitant ?

| Situation | Qui décide des finalités et des moyens ? | Rôle |
|---|---|---|
| Une boutique collecte les adresses de ses clients pour livrer ses commandes | La boutique | **Responsable de traitement** |
| L'éditeur d'un logiciel en ligne héberge ces données pour le compte de la boutique | La boutique donne les instructions | **Sous-traitant** |
| Deux sociétés organisent ensemble un jeu-concours | Ensemble | **Responsables conjoints** |

> [!NOTE]
> Être **sous-traitant** ne dispense pas de **responsabilité** : le RGPD impose des **obligations directes** au sous-traitant (sécurité, instructions, contrat).

### Choisir la base légale : une méthode en trois questions

1. **Quel est le but du traitement ?** (livrer, facturer, envoyer des offres…)
2. **Qu'est-ce qui le justifie ?** (un contrat, une loi, l'intérêt légitime, le consentement…)
3. **Le consentement est-il vraiment nécessaire ?** Il n'est **pas** la base par défaut : pour livrer une commande, on s'appuie sur le **contrat**, pas sur une case à cocher.

### Exemple guidé : un formulaire d'inscription

Un club de sport demande nom, courriel, date de naissance, **numéro de sécurité sociale** et photo pour envoyer sa newsletter. Application des principes :

| Principe | Constat | Correction |
|---|---|---|
| **Minimisation** | Le numéro de sécurité sociale n'est **pas nécessaire** | Le supprimer |
| **Limitation des finalités** | La newsletter n'exige pas la date de naissance complète | Ne demander que ce qui sert |
| **Transparence** | Aucune mention d'information | Ajouter les mentions (articles 13 et 14) |
| **Base légale** | Newsletter commerciale | **Consentement**, case **non précochée** |

Pour une sanction réelle sur ces notions, voir [Google et la CNIL](04-cas-reels.md).

## À retenir

- RGPD : applicable depuis le **25 mai 2018** ; donnée personnelle = personne **identifiée ou identifiable**.
- **Responsable de traitement** / **sous-traitant** / **DPO** / **CNIL**.
- Sept principes : licéité, finalités, minimisation, exactitude, conservation limitée, sécurité, **responsabilité**.
- **Six bases légales**.
- Registre, information, AIPD, contrat de sous-traitance.
