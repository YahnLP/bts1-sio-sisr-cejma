---
author: YLP
title: 📖 FICHE DE COURS ÉLÈVE
---

# FICHE COURS ÉLÈVE - S20 Année 1 - CEJMA
## Synthèse des Enjeux Juridiques en IT — Méthode d'Analyse

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 20*

---

## 🎯 Compétences Travaillées

| **Code** | **Compétence** |
|----------|---------------|
| **B1.6** | Organiser son développement professionnel |
| **Transversal** | Analyser les enjeux juridiques d'une situation professionnelle |
| **Transversal** | Mobiliser les connaissances juridiques en contexte |
| **E6** | Argumenter juridiquement une décision technique |

---

## PARTIE I — Les 6 Grandes Familles d'Enjeux Juridiques en IT

Au cours de l'Année 1, vous avez étudié **19 thèmes juridiques**. Ces thèmes se regroupent en **6 grandes familles** qui couvrent l'essentiel des enjeux juridiques rencontrés par un technicien système et réseau.

![Cartographie des 6 familles juridiques IT](image_placeholder_1)
<!-- PROMPT IMAGE 1 : "Schéma circulaire professionnel montrant 6 grandes familles d'enjeux juridiques IT : 1. RGPD & Données personnelles (icône cadenas vert), 2. Propriété intellectuelle (icône copyright bleu), 3. Responsabilité & Sécurité (icône bouclier rouge), 4. Droit du travail IT (icône personne jaune), 5. Organisation & Support (icône engrenages orange), 6. Économie & Régulation (icône balance violet). Style : infographie moderne, couleurs distinctes par famille, design corporate clair." -->

---

### Famille 1 : 🟢 RGPD & Protection des Données Personnelles

**Définition :** Ensemble des règles encadrant la collecte, le traitement, le stockage et la suppression des données personnelles.

| **Thèmes A1 concernés** | **Questions juridiques typiques** |
|-------------------------|-----------------------------------|
| **S6-S10 : RGPD complet** | • Puis-je créer un compte utilisateur sans consentement ?<br>• Combien de temps conserver les logs ?<br>• Dois-je chiffrer la base de données clients ?<br>• Que faire si un client demande l'effacement de ses données ? |

**Textes de référence :**
- Règlement UE 2016/679 (RGPD) — Articles clés : 5, 6, 32, 33, 34, 35
- Loi Informatique et Libertés (1978, modifiée 2018)

**Situations professionnelles types :**
- Création de comptes utilisateurs (AD, GLPI, applications métier)
- Sauvegarde de données contenant des informations personnelles
- Accès aux logs système (qui contiennent des données personnelles : IP, identifiants)
- Demandes d'exercice de droits (accès, rectification, effacement)
- Mise en conformité suite à un audit CNIL

**Critère de reconnaissance :** Dès qu'une **donnée personnelle** est impliquée (nom, prénom, email, IP, identifiant unique), le RGPD s'applique.

---

### Famille 2 : 🔵 Propriété Intellectuelle & Licences Logicielles

**Définition :** Règles protégeant les créations intellectuelles (code source, logiciels, bases de données) et encadrant leur utilisation.

| **Thèmes A1 concernés** | **Questions juridiques typiques** |
|-------------------------|-----------------------------------|
| **S11 : Droit d'auteur sur le code**<br>**S12-S13 : Licences logicielles** | • Puis-je installer ce logiciel sans acheter de licence ?<br>• Quelle différence entre GPL et MIT ?<br>• Puis-je modifier un logiciel open source ?<br>• Que risque l'entreprise en cas de piratage logiciel ? |

**Textes de référence :**
- Code de la Propriété Intellectuelle (CPI) — Articles L122-1 à L122-7
- Licences : GPL v2/v3, MIT, BSD, Apache, Licences propriétaires (EULA)

**Situations professionnelles types :**
- Installation de logiciels sur le parc informatique
- Gestion des licences (inventaire, conformité)
- Choix entre logiciel propriétaire et open source
- Développement de scripts/outils (qui détient les droits ?)
- Audit de conformité par la BSA (Business Software Alliance)

**Critère de reconnaissance :** Dès qu'un **logiciel** est installé, utilisé, modifié ou distribué, la propriété intellectuelle s'applique.

---

### Famille 3 : 🔴 Responsabilité & Sécurité Informatique

**Définition :** Obligations légales de sécurisation des systèmes d'information et responsabilité pénale/civile en cas de négligence ou d'intrusion.

| **Thèmes A1 concernés** | **Questions juridiques typiques** |
|-------------------------|-----------------------------------|
| **S9 : Obligation légale de sécurité (RGPD Art. 32)**<br>**S14 : Droit de la preuve**<br>**S16 : Responsabilité pénale de l'admin** | • Suis-je responsable si une faille n'est pas corrigée ?<br>• Que faire en cas de ransomware ?<br>• Les logs ont-ils une valeur juridique ?<br>• Dois-je notifier la CNIL en cas d'incident ? |

**Textes de référence :**
- RGPD Articles 32 (sécurité), 33 (notification incident), 34 (information personnes)
- Code Pénal Art. 323-1 à 323-7 (Loi Godfrain — STAD)
- Code Civil Art. 1240 (responsabilité civile)

**Situations professionnelles types :**
- Gestion d'une faille de sécurité (CVE critique)
- Ransomware / Cyberattaque
- Accès non autorisé à un système
- Perte ou vol de données
- Logs système comme preuve d'une intrusion

**Critère de reconnaissance :** Dès qu'il y a un **risque de sécurité** (faille, intrusion, incident), la responsabilité est engagée.

---

### Famille 4 : 🟡 Droit du Travail IT

**Définition :** Règles encadrant la relation de travail spécifique aux métiers de l'informatique (statut, conditions de travail, droits et devoirs).

| **Thèmes A1 concernés** | **Questions juridiques typiques** |
|-------------------------|-----------------------------------|
| **S2 : Convention Syntec**<br>**S3 : Charte informatique** | • Quelle est ma classification Syntec ?<br>• Puis-je utiliser ma messagerie pro à titre personnel ?<br>• Mon employeur peut-il surveiller mon activité ?<br>• Ai-je le droit de télétravailler ? |

**Textes de référence :**
- Convention Collective Syntec (IDCC 1486)
- Code du Travail (Art. L1121-1 : respect vie privée)
- Charte informatique de l'entreprise (document contractuel)

**Situations professionnelles types :**
- Signature de la charte informatique en arrivant
- Utilisation de la messagerie professionnelle
- Télétravail (mise en place technique : VPN, accès à distance)
- Surveillance de l'activité (logs, monitoring)
- Classification du poste (Etam, cadre)

**Critère de reconnaissance :** Dès qu'il s'agit de **votre statut** ou de **l'utilisation des outils IT par les salariés**, le droit du travail s'applique.

---

### Famille 5 : 🟠 Organisation & Management du Support IT

**Définition :** Règles et bonnes pratiques d'organisation du service informatique (ITIL, gestion des incidents, contrats de service).

| **Thèmes A1 concernés** | **Questions juridiques typiques** |
|-------------------------|-----------------------------------|
| **S17-S18 : ITIL, Gestion incidents** | • Comment formaliser un incident ?<br>• Quelle différence entre incident et demande ?<br>• Que contient un SLA (contrat de service) ?<br>• Qui est responsable en cas de non-respect du SLA ? |

**Textes de référence :**
- Référentiel ITIL (bonnes pratiques, non juridiquement contraignant)
- Contrats de service (SLA, OLA) — Droit des contrats (Code Civil)
- Norme ISO/IEC 20000 (management des services IT)

**Situations professionnelles types :**
- Gestion de tickets dans GLPI ou autre outil ITSM
- Rédaction de procédures de support
- Définition des niveaux de support (N1/N2/N3)
- Engagement sur un délai de résolution (GTR/GTI)
- Escalade d'un incident critique

**Critère de reconnaissance :** Dès qu'il s'agit d'**organisation du support** ou de **relation client/fournisseur IT**, cette famille s'applique.

---

### Famille 6 : 🟣 Économie Numérique & Régulation

**Définition :** Règles encadrant le marché du numérique, la concurrence, les acteurs et les pratiques commerciales.

| **Thèmes A1 concernés** | **Questions juridiques typiques** |
|-------------------------|-----------------------------------|
| **S1 : Écosystème numérique**<br>**S4 : Économie du hardware**<br>**S5 : Neutralité du net** | • Quelle différence entre ESN et DSI ?<br>• Puis-je acheter du matériel reconditionné ?<br>• Un FAI peut-il bloquer certains contenus ?<br>• Un hébergeur est-il responsable des contenus hébergés ? |

**Textes de référence :**
- Règlement UE 2015/2120 (neutralité du net)
- LCEN (Loi pour la Confiance dans l'Économie Numérique, 2004)
- Directive DEEE (Déchets d'Équipements Électriques et Électroniques)

**Situations professionnelles types :**
- Choix d'un fournisseur (ESN, éditeur, intégrateur)
- Achat de matériel (neuf, reconditionné, recyclé)
- Hébergement de contenus (responsabilité du prestataire)
- Obsolescence programmée vs durabilité

**Critère de reconnaissance :** Dès qu'il s'agit de **marché**, **acteurs économiques** ou **régulation**, cette famille s'applique.

---

## PARTIE II — Méthode d'Analyse Juridique : QQOQCP Juridique

### Qu'est-ce que le QQOQCP ?

**QQOQCP** est une méthode d'analyse utilisée en gestion de projet, en résolution de problèmes et en analyse de situations. Elle consiste à poser 6 questions systématiques pour **décrire complètement une situation**.

En adaptant cette méthode au **droit**, on obtient une grille d'analyse puissante pour identifier et traiter les enjeux juridiques.

![Méthode QQOQCP Juridique](image_placeholder_2)
<!-- PROMPT IMAGE 2 : "Infographie représentant la méthode QQOQCP juridique avec 6 questions en cercle autour d'une situation centrale : QUI (icône personne), QUOI (icône document), OÙ (icône lieu), QUAND (icône horloge), COMMENT (icône processus), POURQUOI (icône point d'interrogation). Style : design moderne, couleurs corporate, schéma clair et pédagogique avec flèches montrant la progression de l'analyse." -->

---

### Grille QQOQCP Juridique

| **Question** | **Objectif juridique** | **Exemple de réponse** |
|--------------|------------------------|------------------------|
| **QUI ?** | Identifier les **acteurs** et leurs **rôles juridiques** | • Qui est impliqué ? (salarié, entreprise, client, prestataire)<br>• Qui est responsable ? (responsable de traitement, DPO, admin système)<br>• Qui a l'autorité ? (hiérarchie, délégation) |
| **QUOI ?** | Identifier les **faits** et les **enjeux juridiques** | • Quelle est la situation concrète ?<br>• Quels enjeux juridiques ? (RGPD, licences, responsabilité, contrat)<br>• Quelles données/ressources sont concernées ? |
| **OÙ ?** | Identifier le **périmètre** et la **juridiction** | • Où se passe la situation ? (entreprise, cloud, serveur distant)<br>• Quelle juridiction s'applique ? (droit français, droit UE)<br>• Où sont localisées les données ? (France, UE, hors-UE) |
| **QUAND ?** | Identifier les **délais** et les **obligations temporelles** | • Quand la situation s'est-elle produite ?<br>• Y a-t-il des délais légaux ? (RGPD : notification 72h)<br>• Quelle est l'urgence ? (critique, importante, normale) |
| **COMMENT ?** | Identifier les **procédures** et les **moyens techniques** | • Comment la situation s'est-elle produite ? (processus)<br>• Comment est-ce encadré ? (procédure, contrat, règlement)<br>• Quels moyens techniques ? (logs, sauvegardes, chiffrement) |
| **POURQUOI ?** | Identifier les **causes** et les **objectifs juridiques** | • Pourquoi cette situation est-elle un enjeu juridique ?<br>• Quel est l'objectif de la règle de droit ? (protection, conformité)<br>• Pourquoi agir (ou ne pas agir) ? |

---

### Exemple d'Application : Analyse d'une Situation Vécue

**Situation :** "Mon tuteur m'a demandé d'installer le logiciel Adobe Photoshop sur 10 postes, mais il n'y a qu'une seule licence."

#### Analyse QQOQCP Juridique

| **Question** | **Réponse** |
|--------------|-------------|
| **QUI ?** | • **Acteurs** : Moi (apprenti), mon tuteur (responsable IT), l'entreprise (personne morale)<br>• **Responsabilité juridique** : L'entreprise (personne morale) est responsable pénalement. Le tuteur (donneur d'ordre) engage sa responsabilité. Moi (exécutant) : responsabilité limitée si j'ai alerté. |
| **QUOI ?** | • **Faits** : Installation d'un logiciel propriétaire sur 10 postes avec 1 seule licence<br>• **Enjeu juridique** : **Propriété intellectuelle** (contrefaçon de logiciel)<br>• **Données concernées** : Licence logicielle Adobe |
| **OÙ ?** | • **Lieu** : Entreprise (locaux)<br>• **Juridiction** : Droit français (Code de la Propriété Intellectuelle) |
| **QUAND ?** | • **Date** : [Date de la demande]<br>• **Urgence** : Non critique (pas de délai légal), mais risque d'audit BSA à tout moment<br>• **Prescription** : Contrefaçon = délit prescrit après 3 ans |
| **COMMENT ?** | • **Processus** : Installation manuelle via clé USB<br>• **Encadrement** : Contrat de licence Adobe EULA (End-User License Agreement) — stipule "1 licence = 1 poste"<br>• **Traçabilité** : Logs d'installation, inventaire parc (OCS Inventory) |
| **POURQUOI ?** | • **Cause** : Probablement méconnaissance de la loi ou budget insuffisant<br>• **Enjeu** : Protection du droit d'auteur de l'éditeur (Adobe)<br>• **Risque** : Sanction pénale (Code PI Art. L335-2 : jusqu'à 300 000€ d'amende et 3 ans de prison) + sanctions civiles (dommages et intérêts) |

#### Conclusion de l'Analyse

**Qualification juridique :** Contrefaçon de logiciel (Code de la Propriété Intellectuelle Art. L122-6 et L335-2)

**Action recommandée :**
1. **Alerter le tuteur** de l'illégalité de la demande (par écrit : email)
2. **Proposer des alternatives** : 
   - Achat de 9 licences supplémentaires
   - Utilisation d'un logiciel open source (GIMP, Krita)
   - Abonnement Adobe Creative Cloud entreprise (licences flottantes)
3. **Refuser d'exécuter** si le tuteur maintient sa demande illégale
4. **Documenter** : conserver l'email d'alerte (preuve de bonne foi)

---

## PARTIE III — Mobiliser ses Connaissances Juridiques à l'Examen E6

### Pourquoi le Droit à l'Examen E6 ?

L'épreuve E6 (Cybersécurité des services informatiques) contient **systématiquement des questions juridiques** car :
- La cybersécurité est **encadrée par le droit** (RGPD, Loi Godfrain, NIS 2)
- Un admin système doit **argumenter juridiquement** ses choix techniques
- La conformité légale est un **critère de décision** aussi important que la performance technique

### Exemples de Questions E6 avec Dimension Juridique

**Question type 1 — Incident de sécurité**

> "L'entreprise XYZ a subi une cyberattaque. Des données clients ont été compromises. Quelles sont les obligations légales de l'entreprise ?"

**Mobilisation juridique attendue :**
- RGPD Art. 33 : Notification CNIL sous 72h
- RGPD Art. 34 : Information des personnes concernées si risque élevé
- Loi Godfrain : Dépôt de plainte recommandé
- Code du Travail : Information du CSE

**Question type 2 — Mise en conformité**

> "L'entreprise souhaite déployer un système de vidéosurveillance dans ses locaux. Quelles démarches juridiques sont nécessaires ?"

**Mobilisation juridique attendue :**
- RGPD Art. 35 : Analyse d'Impact (AIPD) obligatoire
- Code du Travail : Information/consultation du CSE
- CNIL : Notification si surveillance continue
- Affichage obligatoire (information des personnes filmées)

---

### Méthode de Réponse E6 avec Enjeu Juridique

**Structure de réponse recommandée (en 4 étapes) :**

#### Étape 1 : IDENTIFIER l'enjeu juridique (1 phrase)

> "Cette situation soulève un enjeu de **[Famille juridique]** car **[raison]**."

**Exemple :** "Cette situation soulève un enjeu de **protection des données personnelles** car la vidéosurveillance collecte des images de salariés et visiteurs."

#### Étape 2 : CITER les textes applicables (liste)

> "Les textes de référence sont : **[liste des textes]**."

**Exemple :** "Les textes de référence sont : RGPD Art. 35 (AIPD), Code du Travail Art. L2312-8 (consultation CSE), Délibération CNIL n°2010-112."

#### Étape 3 : EXPLIQUER les obligations (paragraphe)

> "Selon ces textes, l'entreprise doit **[obligations concrètes]**."

**Exemple :** "Selon ces textes, l'entreprise doit : (1) réaliser une analyse d'impact avant tout déploiement, (2) consulter le CSE et recueillir son avis, (3) limiter la durée de conservation des images à 30 jours maximum, (4) afficher une signalétique informant de la vidéosurveillance."

#### Étape 4 : PROPOSER des actions techniques (liste numérotée)

> "Techniquement, je recommande de : **[actions concrètes]**."

**Exemple :** "Techniquement, je recommande de : (1) choisir un système avec purge automatique à J+30, (2) chiffrer les flux vidéo et le stockage, (3) limiter les accès aux seules personnes habilitées (matrice de droits), (4) tenir un registre des consultations des images."

---

## 📌 Points Clés à Retenir

✅ **6 grandes familles** d'enjeux juridiques en IT : RGPD, Propriété intellectuelle, Responsabilité & Sécurité, Droit du travail, Organisation & Support, Économie & Régulation

✅ **Méthode QQOQCP juridique** = grille d'analyse systématique de toute situation professionnelle

✅ **Reconnaître l'enjeu** juridique dans une situation technique = compétence clé de l'admin système

✅ **Mobiliser le droit à l'examen E6** = identifier + citer + expliquer + proposer (4 étapes)

✅ **Le droit n'est pas séparé de la technique** — c'est un outil de travail quotidien pour un professionnel

---

## 🔗 Tableau Récapitulatif : De la Situation au Texte de Loi

| **Situation Professionnelle** | **Famille Juridique** | **Texte de Loi Applicable** |
|-------------------------------|-----------------------|-----------------------------|
| Créer des comptes utilisateurs | 🟢 RGPD | RGPD Art. 5 et 6 (licéité) |
| Installer un logiciel | 🔵 Propriété intellectuelle | CPI Art. L122-6 (licence) |
| Ne pas corriger une faille connue | 🔴 Responsabilité | RGPD Art. 32 + CP Art. 323-1 |
| Signer la charte informatique | 🟡 Droit du travail | Code du Travail + Charte |
| Gérer un ticket GLPI | 🟠 Organisation | ITIL (bonnes pratiques) |
| Choisir un hébergeur | 🟣 Économie & Régulation | LCEN (responsabilité hébergeur) |

---
