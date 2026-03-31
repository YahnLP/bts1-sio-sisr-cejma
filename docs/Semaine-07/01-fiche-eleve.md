---
author: YLP
title: 📚 FICHE DE COURS
---

# 📚 FICHE DE COURS ÉLÈVE
## RGPD (2) : Les Acteurs — Rôle du DPO et du Responsable de Traitement

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 7*

---

## 🎯 Objectifs de Cette Fiche

À la fin de ce cours, vous serez capable de :
- ✅ Définir les rôles de responsable de traitement, sous-traitant, et DPO
- ✅ Distinguer les responsabilités de chacun
- ✅ Identifier qui est responsable dans des cas concrets
- ✅ Expliquer les missions d'un DPO
- ✅ Comprendre la chaîne de sous-traitance

---


## 📖 PARTIE I — Le Responsable de Traitement (RT)

### I.A. Définition (Article 4-7 du RGPD)

Le **responsable de traitement** (RT) est la personne physique ou morale, l'autorité publique, le service ou un autre organisme qui, **seul ou conjointement avec d'autres**, détermine les **finalités** et les **moyens** du traitement de données personnelles.

**En clair :** C'est celui qui **décide** :
- **POURQUOI** on collecte des données (la finalité)
- **COMMENT** on les traite (les moyens : outils, durée de conservation, sécurité...)

> 💡 **Mot-clé :** Le RT est le **décideur**, pas forcément celui qui exécute techniquement le traitement.

### I.B. Exemples de Responsables de Traitement

| **Organisme** | **Finalité** | **Données Traitées** |
|---|---|---|
| **Une banque** | Gérer les comptes clients | Identité, revenus, opérations bancaires |
| **Un hôpital** | Gérer les dossiers médicaux | Identité, pathologies, traitements |
| **Une ESN** | Gérer ses propres employés (RH) | Identité, CV, salaires, évaluations |
| **Un site e-commerce** | Vendre des produits en ligne | Identité, adresses, commandes, paiements |
| **Une collectivité** | Gérer l'état civil, les impôts locaux | Identité, situation familiale, revenus |

### I.C. Responsabilités du RT

Le RT est **responsable de la conformité RGPD**. Il doit :

| **Obligation** | **Détail** | **Article RGPD** |
|---|---|---|
| **1. Respecter les principes** | Licéité, loyauté, transparence, minimisation... | Art. 5 |
| **2. Obtenir le consentement** | Si nécessaire (ou autre base légale) | Art. 6 |
| **3. Informer les personnes** | Politique de confidentialité claire | Art. 13-14 |
| **4. Respecter les droits** | Accès, rectification, effacement, portabilité... | Art. 15-22 |
| **5. Sécuriser les données** | Mesures techniques et organisationnelles | Art. 32 |
| **6. Tenir un registre** | Registre des traitements | Art. 30 |
| **7. Notifier les violations** | À la CNIL sous 72h si risque | Art. 33 |
| **8. Faire une AIPD** | Si traitement à risque élevé | Art. 35 |
| **9. Désigner un DPO** | Si obligation (voir Partie III) | Art. 37 |
| **10. Encadrer les ST** | Contrat avec clauses RGPD | Art. 28 |

### I.D. Sanctions en Cas de Non-Respect

Le RT peut être sanctionné par la CNIL :

| **Type de Violation** | **Amende Maximale** | **Exemples** |
|---|---|---|
| **Violations graves** | **20 millions €** ou **4 % du CA mondial** | Absence de consentement, violation droits fondamentaux, pas de sécurité |
| **Violations administratives** | **10 millions €** ou **2 % du CA mondial** | Pas de registre, DPO non désigné, AIPD non réalisée |

**Exemples de sanctions réelles (France) :**
- Amazon Europe (746M€, 2021) — cookies sans consentement
- Google Ireland (90M€, 2024) — cookies, refus difficile
- Microsoft Ireland (60M€, 2022) — cookies publicitaires

### I.E. Qui Peut Être RT ?

**Tout organisme qui traite des données personnelles** :
- ✅ Entreprises privées (PME, ETI, grandes entreprises)
- ✅ Associations
- ✅ Administrations publiques (mairies, hôpitaux, universités...)
- ✅ Professions libérales (médecins, avocats, comptables...)

> ⚠️ **Attention :** Une entreprise peut être **à la fois RT et sous-traitant** selon les activités.  
> Exemple : Une ESN est **RT** pour ses propres employés (RH) ET **sous-traitant** pour ses clients (hébergement).

---

![Schéma du Responsable de Traitement : RT au centre, flèches sortantes vers : Personnes concernées (obligations d'information), CNIL (notification violations), Sous-traitants (contrats), DPO (consultation)]

*Légende : Le Responsable de Traitement et ses obligations*

---

## 📖 PARTIE II — Le Sous-Traitant (ST)

### II.A. Définition (Article 4-8 du RGPD)

Le **sous-traitant** (ST) est la personne physique ou morale qui **traite des données personnelles pour le compte du responsable de traitement**.

**En clair :** Le ST **exécute** les instructions du RT. Il ne décide pas de la finalité ni des moyens principaux.

> 💡 **Mot-clé :** Le ST est l'**exécutant**, pas le décideur.

### II.B. Exemples de Sous-Traitants

| **Sous-Traitant** | **Service Fourni** | **RT (Client)** |
|---|---|---|
| **OVH** | Hébergement de serveurs, bases de données | Entreprise qui héberge son site chez OVH |
| **Google Workspace** | Messagerie, stockage cloud (Gmail, Drive) | Entreprise qui utilise G Suite pour ses employés |
| **Salesforce** | CRM (gestion relation client) | Entreprise qui gère ses clients sur Salesforce |
| **ESN** | Maintenance, infogérance, développement | Entreprise qui confie sa DSI à une ESN |
| **Prestataire de paie** | Gestion des bulletins de salaire | Entreprise qui externalise la paie |

### II.C. Obligations du Sous-Traitant

Le ST doit (Article 28) :

| **Obligation** | **Détail** |
|---|---|
| **1. Suivre les instructions du RT** | Ne traiter les données **QUE** selon les instructions documentées du RT |
| **2. Confidentialité** | Les employés du ST doivent être tenus au secret |
| **3. Sécurité** | Mettre en place des mesures de sécurité appropriées |
| **4. Aider le RT** | Pour les demandes d'exercice de droits (accès, effacement...) |
| **5. Restituer ou effacer** | À la fin du contrat, restituer ou détruire les données |
| **6. Informer le RT** | En cas de violation de données |
| **7. Autorisation préalable** | Pour recourir à un sous-traitant ultérieur (sous-sous-traitant) |

### II.D. Le Contrat RT-ST (Article 28-3)

**Obligation légale :** Le RT et le ST doivent signer un **contrat écrit** (ou acte juridique) comportant des **clauses RGPD**.

**Clauses obligatoires :**

| **Clause** | **Contenu** |
|---|---|
| **Objet du traitement** | Nature des données, finalité, durée |
| **Obligations du ST** | Suivre les instructions du RT, sécuriser, confidentialité |
| **Durée** | Durée du contrat, sort des données à la fin |
| **Mesures de sécurité** | Chiffrement, contrôle d'accès, sauvegardes... |
| **Sous-traitance ultérieure** | Conditions d'autorisation |
| **Assistance au RT** | Pour répondre aux demandes d'exercice de droits |
| **Audit** | Le RT peut auditer le ST ou mandater un auditeur |

**Exemple de clause RGPD type (extrait) :**

```
Article X — Protection des Données Personnelles

Le Sous-Traitant s'engage à :
a) Ne traiter les données que selon les instructions documentées du RT
b) Garantir la confidentialité des données
c) Mettre en œuvre les mesures de sécurité suivantes : [liste]
d) Notifier au RT toute violation de données sous 24 heures
e) Restituer ou détruire les données à la fin du contrat
```

### II.E. La Chaîne de Sous-Traitance

Un sous-traitant peut lui-même recourir à un **sous-traitant ultérieur** (sous-sous-traitant), mais il doit :
- ✅ Obtenir l'**autorisation préalable** du RT (écrite ou générale)
- ✅ Imposer au sous-traitant ultérieur les **mêmes obligations** RGPD

**Exemple :**
```
RT : Banque ACME
  ↓ (contrat)
ST : ESN TechServices (infogérance)
  ↓ (contrat)
Sous-traitant ultérieur : OVH (hébergement des serveurs)
```

> ⚠️ **Important :** Le ST reste **responsable vis-à-vis du RT** même s'il sous-traite à un tiers.

### II.F. Sanctions du Sous-Traitant

Le ST peut être sanctionné **directement** par la CNIL s'il :
- ❌ Ne respecte pas ses obligations (art. 28)
- ❌ Traite les données sans instructions ou à d'autres fins
- ❌ Ne sécurise pas les données

**Amende maximale :** Même que le RT → **20 millions €** ou **4 % du CA mondial**

---

![Schéma de la chaîne de sous-traitance : RT en haut, flèche vers ST 1 (contrat RGPD), flèche vers ST ultérieur (contrat RGPD). Responsabilité : RT responsable global, ST responsable envers RT, ST ultérieur responsable envers ST.]

*Légende : La chaîne de sous-traitance RGPD*

---

## 📖 PARTIE III — Le Délégué à la Protection des Données (DPO)

### III.A. Définition (Article 37-39 du RGPD)

Le **DPO** (Data Protection Officer) ou **DPD** (Délégué à la Protection des Données) est une personne chargée de **conseiller et contrôler** le respect du RGPD au sein de l'organisme.

> 💡 **Mot-clé :** Le DPO est un **conseiller**, pas un responsable. Il n'a pas de pouvoir de décision.

### III.B. Missions du DPO (Article 39)

| **Mission** | **Détail** |
|---|---|
| **1. Informer et conseiller** | Le RT, le ST et les employés sur leurs obligations RGPD |
| **2. Contrôler le respect du RGPD** | Vérifier que les traitements sont conformes |
| **3. Conseiller sur les AIPD** | Analyses d'Impact sur la Protection des Données |
| **4. Coopérer avec la CNIL** | Point de contact entre l'organisme et l'autorité de contrôle |
| **5. Sensibiliser** | Former le personnel aux bonnes pratiques RGPD |
| **6. Gérer les demandes** | Aider à traiter les demandes d'exercice de droits |

### III.C. Désignation du DPO — Quand Est-Ce Obligatoire ?

**Obligation de désigner un DPO (Article 37-1) :**

| **Cas d'Obligation** | **Exemples** |
|---|---|
| **1. Autorité ou organisme public** | Mairies, conseils départementaux, hôpitaux publics, universités |
| **2. Traitement à grande échelle de données sensibles** | Hôpital privé, assurance santé, banque... |
| **3. Surveillance régulière et systématique à grande échelle** | Vidéosurveillance massive, géolocalisation d'employés, profilage publicitaire |

**Cas où le DPO est FACULTATIF mais recommandé :**
- PME sans traitement sensible ou à grande échelle
- Startup avec peu de données

> 📌 **En France :** Environ **25 000 DPO désignés** (2024).

### III.D. Statut et Indépendance du DPO

**Le DPO peut être :**
- ✅ **Interne** (employé de l'organisme) — CDI dédié à cette fonction
- ✅ **Externe** (prestataire) — Cabinet de conseil, avocat, consultant RGPD

**Garanties d'indépendance (Article 38) :**
- ❌ Le DPO **ne peut pas être licencié** ou sanctionné pour ses recommandations
- ✅ Le DPO **rend compte directement à la direction** (pas d'autorité hiérarchique intermédiaire)
- ❌ Le DPO **ne peut pas être en conflit d'intérêts** (ex : DSI ne peut pas être DPO, car il est juge et partie)
- ✅ Le DPO dispose de **ressources** (temps, budget, formation)

### III.E. DPO ≠ Responsable

**IDÉE REÇUE (FAUSSE) :** *"Le DPO est responsable en cas de violation RGPD"*

**RÉALITÉ :**
- ❌ Le DPO **n'est PAS responsable** juridiquement
- ✅ C'est le **Responsable de Traitement** qui est sanctionné
- ✅ Le DPO est un **conseiller** : il alerte, recommande, mais ne décide pas

**Exemple :**
- Un DPO recommande de chiffrer les bases de données
- La direction refuse pour des raisons budgétaires
- Il y a une fuite de données
- **Qui est sanctionné ?** → Le **RT** (la direction), PAS le DPO

### III.F. Comment Contacter le DPO ?

Le DPO doit être **facilement joignable** :
- ✅ Coordonnées publiées sur le site web de l'organisme
- ✅ Email dédié (ex : dpo@entreprise.fr)
- ✅ Déclaré à la CNIL (publication dans le registre public)

**Les personnes concernées peuvent contacter le DPO pour :**
- Exercer leurs droits (accès, rectification, effacement...)
- Poser des questions sur le traitement de leurs données
- Déposer une réclamation

---

![Schéma du positionnement du DPO : DPO au centre en tant que conseiller, flèches vers RT (conseille), vers CNIL (coopère), vers employés (forme), vers personnes concernées (répond). Note : DPO n'est PAS dans la chaîne hiérarchique opérationnelle.]

*Légende : Le rôle et le positionnement du DPO*

---

## 📖 PARTIE IV — La Coresponsabilité

### IV.A. Définition (Article 26 du RGPD)

Il y a **coresponsabilité** lorsque **deux organismes ou plus déterminent conjointement** les finalités et les moyens d'un traitement.

**En clair :** Deux RT pour un même traitement.

### IV.B. Exemples de Coresponsabilité

| **Cas** | **Coresponsables** | **Traitement Commun** |
|---|---|---|
| **Site e-commerce + Facebook** | Le site + Facebook | Pixel Facebook (suivi des visiteurs pour pub ciblée) |
| **Deux hôpitaux partenaires** | Hôpital A + Hôpital B | Dossier médical partagé d'un patient transféré |
| **Réseau de franchises** | Franchiseur + Franchisés | Base de données clients commune |
| **Événement organisé par 2 associations** | Association A + Association B | Inscription des participants |

### IV.C. Obligations en Cas de Coresponsabilité

Les coresponsables doivent :
- ✅ **Définir leurs responsabilités respectives** par un accord écrit (qui fait quoi ?)
- ✅ **Désigner un point de contact unique** pour les personnes concernées
- ✅ **Informer les personnes** de la coresponsabilité et de l'accord

**Exemple d'accord de coresponsabilité (simplifié) :**

```
Entreprise A (site e-commerce) et Facebook Inc. sont coresponsables
du traitement des données de navigation via le pixel Facebook.

Répartition des responsabilités :
- Entreprise A : Informer les visiteurs, recueillir le consentement
- Facebook : Sécuriser les données, respecter les droits d'accès

Point de contact : dpo@entreprise-a.com
```

### IV.D. Sanctions

En cas de violation, **les deux coresponsables** peuvent être sanctionnés solidairement :
- La CNIL peut sanctionner l'un ou les deux
- Les personnes concernées peuvent poursuivre l'un ou les deux

---

## 📖 PARTIE V — Tableau Récapitulatif des Acteurs

| **Acteur** | **Rôle** | **Responsabilité Juridique** | **Obligations Principales** |
|---|---|---|:---:|
| **Responsable de Traitement (RT)** | Décide finalités et moyens | ⭐⭐⭐⭐⭐ **TOTALE** | Conformité RGPD, sécurité, droits personnes, registre, notification |
| **Sous-Traitant (ST)** | Exécute pour le compte du RT | ⭐⭐⭐ **Limitée** (si faute) | Suivre instructions RT, sécurité, confidentialité, contrat RGPD |
| **DPO** | Conseille et contrôle | ❌ **AUCUNE** (conseiller) | Informer, conseiller, contrôler, coopérer avec CNIL |
| **Coresponsables** | Déterminent conjointement | ⭐⭐⭐⭐⭐ **Solidaire** | Accord écrit, répartition claire, point de contact unique |

---

## 🔑 VOCABULAIRE CLÉ À MAÎTRISER (pour l'examen)

| **Terme** | **Définition Simple** |
|---|---|
| **Responsable de Traitement (RT)** | Organisme qui décide des finalités et moyens du traitement |
| **Sous-Traitant (ST)** | Organisme qui traite des données pour le compte du RT |
| **DPO / DPD** | Délégué à la Protection des Données (conseiller RGPD) |
| **Finalité** | Objectif, raison pour laquelle on collecte des données |
| **Moyens** | Comment on traite les données (outils, durée, sécurité...) |
| **Sous-traitant ultérieur** | Sous-traitant du sous-traitant (sous-sous-traitant) |
| **Coresponsabilité** | Deux organismes ou plus déterminent conjointement finalités et moyens |
| **Registre des traitements** | Document listant tous les traitements de données de l'organisme |
| **AIPD** | Analyse d'Impact sur la Protection des Données (si traitement à risque) |
| **Notification à la CNIL** | Obligation d'informer la CNIL sous 72h en cas de violation de données |

---

## ✅ Points Clés à Retenir

1. **Le Responsable de Traitement (RT) est le principal responsable juridique.** C'est lui qui décide et qui est sanctionné en priorité.

2. **Le Sous-Traitant (ST) traite pour le compte du RT.** Il doit suivre les instructions du RT et signer un contrat RGPD. Il peut être sanctionné s'il commet une faute.

3. **Le DPO est un conseiller, PAS un responsable.** Il alerte, recommande, contrôle, mais ne décide pas. Il ne peut pas être sanctionné pour les violations RGPD.

4. **Un contrat écrit RT-ST est obligatoire** avec des clauses RGPD (instructions, sécurité, confidentialité, durée...).

5. **La coresponsabilité existe quand deux organismes déterminent conjointement** les finalités et moyens. Ils sont solidairement responsables.

6. **En tant que technicien SISR, vous serez souvent dans un rôle de sous-traitant** (si vous hébergez, maintenez, gérez des systèmes pour des clients). Vous devez respecter vos obligations contractuelles RGPD.

---

## 📚 Pour Aller Plus Loin

**Textes de référence :**
- [RGPD — Articles 24-28](https://www.cnil.fr/fr/reglement-europeen-protection-donnees) (RT et ST)
- [RGPD — Articles 37-39](https://www.cnil.fr/fr/reglement-europeen-protection-donnees) (DPO)
- [RGPD — Article 26](https://www.cnil.fr/fr/reglement-europeen-protection-donnees) (Coresponsabilité)

**Guides CNIL :**
- [Le responsable de traitement](https://www.cnil.fr/fr/guide-responsable-de-traitement)
- [Le sous-traitant](https://www.cnil.fr/fr/sous-traitant)
- [Le DPO](https://www.cnil.fr/fr/devenir-delegue-la-protection-des-donnees)

**Questions de réflexion :**
- Votre entreprise d'alternance est-elle RT, ST, ou les deux ?
- Si vous administrez un serveur hébergeant des données clients, êtes-vous ST ?
- Si votre entreprise a un DPO, quand devez-vous le solliciter ?


---
