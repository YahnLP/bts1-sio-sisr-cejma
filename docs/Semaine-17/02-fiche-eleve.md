---
author: YLP
title: 📚 FICHE DE COURS
---

# 📚 FICHE DE COURS ÉLÈVE
## "GLPI + OCS Inventory · Catalogue de Services · Support IT"

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 17*

---

## 🎯 Compétences Travaillées

| **Code** | **Compétence** |
|----------|---------------|
| **B1.4** | Mettre en place et exploiter des outils de gestion de parc |
| **B1.5** | Mettre à disposition un service informatique |
| **B1.2** | Exploiter des référentiels ITIL |

---

## PARTIE I — GLPI (Rappels + Approfondissement)

### I.A. Rappel : Qu'est-ce que GLPI ?

**GLPI** (Gestion Libre de Parc Informatique) est un logiciel open source de :
- **Gestion de parc** (inventaire matériel et logiciel)
- **Helpdesk** (gestion des tickets d'incidents et demandes)
- **Gestion des actifs IT** (licences, contrats, fournisseurs)

```
   GLPI — FONCTIONNALITÉS PRINCIPALES
   ─────────────────────────────────────────────────────────────

   ① INVENTAIRE
      • Matériel (PC, serveurs, imprimantes, téléphones)
      • Logiciels (licences, versions)
      • Réseau (switches, routeurs, IP)

   ② HELPDESK
      • Tickets d'incidents
      • Tickets de demandes de service
      • Suivi et historique

   ③ GESTION ADMINISTRATIVE
      • Contrats (maintenance, support)
      • Fournisseurs
      • Budgets

   ④ BASE DE CONNAISSANCES
      • Articles de résolution
      • FAQ
      • Procédures
```

**Chiffres clés :**
- 15 000+ organisations utilisent GLPI
- Disponible en 45 langues
- 500+ plugins disponibles

---

### I.B. OCS Inventory — Inventaire Automatique

**OCS Inventory** est un outil d'inventaire automatique qui remonte les informations vers GLPI.

```
   FONCTIONNEMENT OCS + GLPI
   ─────────────────────────────────────────────────────────────

   ① AGENT OCS (sur chaque poste client)
      • S'exécute en tâche planifiée (ex : tous les jours à 9h)
      • Scanne le matériel (CPU, RAM, disques, réseau)
      • Scanne les logiciels installés
      • Envoie les données au serveur OCS

   ② SERVEUR OCS INVENTORY
      • Reçoit les données des agents
      • Stocke dans sa base de données
      • Met à disposition via API

   ③ GLPI
      • Se connecte au serveur OCS via plugin
      • Importe automatiquement les nouveaux ordinateurs
      • Met à jour l'inventaire existant
      • Affiche tout dans son interface
```

**Avantages :**
- ✅ Inventaire automatique (pas de saisie manuelle)
- ✅ Mise à jour en temps réel
- ✅ Détection des changements matériels/logiciels
- ✅ Conformité licences (détecter les logiciels non autorisés)

---

## PARTIE II — Le Catalogue de Services

### II.A. Définition

Un **catalogue de services IT** est la liste structurée de tous les services proposés par la DSI aux utilisateurs.

```
   CATALOGUE DE SERVICES = MENU DE LA DSI

   Comme un menu de restaurant :
   ────────────────────────────────────────────────────────────
   • Liste tous les plats disponibles (services)
   • Indique les ingrédients (prérequis)
   • Précise les délais de préparation (SLA)
   • Affiche les prix (coûts si applicable)

   Catalogue de services IT :
   ────────────────────────────────────────────────────────────
   • Liste tous les services IT disponibles
   • Décrit comment les demander
   • Indique les délais de livraison (SLA)
   • Précise les conditions d'accès
```

---

### II.B. Structure d'un Catalogue

**Organisation en 3 niveaux :**

```
NIVEAU 1 — CATÉGORIES PRINCIPALES
├── Support Utilisateur
├── Infrastructure & Réseau
├── Applications Métier
└── Sécurité

NIVEAU 2 — SOUS-CATÉGORIES
└── Support Utilisateur
    ├── Compte et Authentification
    ├── Poste de Travail
    ├── Messagerie
    └── Impression

NIVEAU 3 — SERVICES DÉTAILLÉS
└── Compte et Authentification
    ├── Création de compte utilisateur
    ├── Réinitialisation mot de passe
    ├── Déblocage de compte
    └── Modification droits d'accès
```

---

### II.C. Fiche de Service Type

Chaque service du catalogue doit avoir une **fiche descriptive** :

```
╔══════════════════════════════════════════════════════════════╗
║             FICHE DE SERVICE                                 ║
╠══════════════════════════════════════════════════════════════╣
║  Nom du service     : Réinitialisation mot de passe         ║
║  Catégorie          : Support > Compte et Authentification  ║
║  Type               : Demande de service                     ║
╠══════════════════════════════════════════════════════════════╣
║  Description :                                               ║
║  Réinitialiser le mot de passe d'un utilisateur bloqué ou   ║
║  oublié, conformément à la politique de sécurité.           ║
╠══════════════════════════════════════════════════════════════╣
║  Bénéficiaires      : Tous les employés                     ║
║  Prérequis          : Validation identité (manager ou RH)   ║
╠══════════════════════════════════════════════════════════════╣
║  SLA (Délai)        : 2 heures ouvrées                      ║
║  Disponibilité      : Lun-Ven 8h-18h                        ║
╠══════════════════════════════════════════════════════════════╣
║  Procédure de demande :                                      ║
║  1. Créer un ticket dans GLPI                               ║
║  2. Catégorie : Support > Compte                            ║
║  3. Fournir : nom, prénom, service                          ║
║  4. Validation manager (par email)                          ║
╠══════════════════════════════════════════════════════════════╣
║  Contact support    : support@simio.local                   ║
╚══════════════════════════════════════════════════════════════╝
```

---

### II.D. Avantages d'un Catalogue

**Pour les utilisateurs :**
- ✅ Savent quels services sont disponibles
- ✅ Connaissent les délais de livraison
- ✅ Savent comment demander un service
- ✅ Autonomie (self-service)

**Pour la DSI :**
- ✅ Standardisation des demandes
- ✅ Priorisation facilitée (SLA définis)
- ✅ Mesure de la qualité de service
- ✅ Réduction des demandes hors périmètre

---

## PARTIE III — Le Cycle de Vie d'un Ticket

### III.A. Les États d'un Ticket

```
   CYCLE DE VIE D'UN TICKET DANS GLPI
   ─────────────────────────────────────────────────────────────

   ① NOUVEAU
      • Ticket vient d'être créé
      • En attente d'affectation à un technicien

   ② EN COURS (ATTRIBUÉ)
      • Ticket affecté à un technicien
      • Technicien travaille sur la résolution

   ③ EN ATTENTE
      • Ticket mis en pause (en attente info utilisateur, commande...)
      • Timer SLA en pause

   ④ RÉSOLU
      • Technicien a trouvé et appliqué une solution
      • En attente validation utilisateur

   ⑤ CLOS
      • Utilisateur confirme que le problème est résolu
      • Ticket archivé

   ⑥ ANNULÉ (optionnel)
      • Demande retirée par l'utilisateur
      • Ou doublon d'un autre ticket
```

---

### III.B. Les Champs Essentiels d'un Ticket

| **Champ** | **Description** | **Exemple** |
|---|---|---|
| **Titre** | Résumé court du problème | "Impossible d'accéder au serveur fichiers" |
| **Demandeur** | Utilisateur ayant créé le ticket | Julie Dupont (Comptabilité) |
| **Catégorie** | Classification du problème | Réseau > Accès serveur |
| **Priorité** | Urgence × Impact | 3 (Moyenne) |
| **Description** | Détails du problème | "Depuis ce matin 9h, message d'erreur..." |
| **Technicien** | Personne assignée à la résolution | Marc Technician |
| **Statut** | État actuel | En cours |
| **Solution** | Description de la résolution | "Droits NTFS manquants → ajoutés" |

---

### III.C. Diagnostic d'un Incident (Méthodologie)

**Méthode en 5 étapes :**

```
ÉTAPE 1 — COLLECTER LES INFORMATIONS
─────────────────────────────────────────────────────────────
Questions à poser :
• Quand le problème est-il apparu ?
• Quel est le message d'erreur exact ?
• Le problème affecte-t-il d'autres utilisateurs ?
• Des changements récents ont-ils été effectués ?


ÉTAPE 2 — REPRODUIRE LE PROBLÈME
─────────────────────────────────────────────────────────────
• Tenter de reproduire le problème sur le poste de l'utilisateur
• Tester sur un autre poste (problème local ou global ?)


ÉTAPE 3 — FORMULER DES HYPOTHÈSES
─────────────────────────────────────────────────────────────
Exemples :
• H1 : Droits d'accès insuffisants
• H2 : Problème réseau (câble, switch)
• H3 : Service Windows arrêté


ÉTAPE 4 — TESTER LES HYPOTHÈSES
─────────────────────────────────────────────────────────────
• Vérifier les droits NTFS → OK, droits corrects
• Tester ping vers serveur → KO, pas de réponse
  → H2 confirmée : problème réseau


ÉTAPE 5 — APPLIQUER LA SOLUTION
─────────────────────────────────────────────────────────────
• Vérifier câble réseau → débranché
• Rebrancher le câble
• Tester ping → OK
• Utilisateur peut accéder au serveur → Résolu
```

---

## IV. Vocabulaire Clé

| **Terme** | **Définition** |
|-----------|---------------|
| **GLPI** | Gestion Libre de Parc Informatique — logiciel de gestion IT open source |
| **OCS Inventory** | Outil d'inventaire automatique de parc informatique |
| **Agent OCS** | Logiciel installé sur chaque poste qui remonte l'inventaire |
| **Catalogue de services** | Liste structurée des services IT proposés aux utilisateurs |
| **Fiche de service** | Description détaillée d'un service (SLA, procédure, prérequis) |
| **Ticket** | Demande de support ou signalement d'incident dans GLPI |
| **SLA** | Service Level Agreement — engagement sur délai de résolution |
| **Helpdesk** | Service d'assistance aux utilisateurs (synonyme : support) |
| **Base de connaissances** | Bibliothèque de solutions et procédures dans GLPI |
| **Inventaire** | Liste complète du matériel et logiciels du parc |

