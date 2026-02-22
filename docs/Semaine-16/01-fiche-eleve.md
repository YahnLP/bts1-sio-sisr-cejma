---
author: YLP
title: 📚 FICHE DE COURS
---

# 📚 FICHE DE COURS ÉLÈVE
## "Travail Collaboratif · Outils · Bonnes Pratiques"

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 16*

---

## 🎯 Compétences Travaillées

| **Code** | **Compétence** |
|----------|---------------|
| **B3.3** | Participer à la gestion et au suivi d'un projet |
| **B1.5** | Mettre à disposition un service informatique |

---

## PARTIE I — Les Enjeux du Travail Collaboratif

### I.A. Pourquoi Collaborer ?

En IT, **personne ne travaille seul** :
- Les projets impliquent plusieurs personnes (techniciens, responsables, utilisateurs)
- Les connaissances sont dispersées (chacun a son expertise)
- Les outils évoluent (veille collective plus efficace)

```
   TRAVAIL ISOLÉ                    vs        TRAVAIL COLLABORATIF
   ─────────────────────                     ────────────────────────
   • Chacun dans son coin                    • Équipe synchronisée
   • Documentation personnelle               • Documentation partagée
   • Connaissances perdues si départ         • Connaissances capitalisées
   • Réinventer la roue                      • Réutiliser l'existant
   • Erreurs répétées                        • Apprentissage collectif
```

**Statistiques (Atlassian 2023) :**
- 86% des DSI considèrent la collaboration comme critique
- 75% des échecs de projets IT sont dus à une mauvaise communication
- 60% du temps d'un technicien est perdu à chercher de l'information

---

### I.B. Les 4 Piliers de la Collaboration IT

**① DOCUMENTATION PARTAGÉE**

Centraliser la connaissance technique dans un espace accessible à tous.

**Outils :** Wiki (DokuWiki, MediaWiki, Confluence), Base de connaissances (SharePoint, Notion)

**② VERSIONING ET GESTION DE CODE**

Suivre les modifications des fichiers (scripts, configurations, code).

**Outils :** Git, SVN, GitLab, GitHub

**③ COMMUNICATION ASYNCHRONE**

Communiquer sans nécessiter de réponse immédiate (vs téléphone, réunion).

**Outils :** Slack, Microsoft Teams, Mattermost, email structuré

**④ GESTION DE TÂCHES**

Organiser le travail, attribuer des tâches, suivre l'avancement.

**Outils :** Jira, Trello, Monday, GLPI (tickets)

---

### I.C. Bonnes Pratiques

**① NOMMER LES FICHIERS CORRECTEMENT**

```
❌ MAUVAIS EXEMPLES
─────────────────────────────────────────────────────────────
• doc.txt (quoi comme doc ?)
• nouveau.docx (nouveau quoi ?)
• Copie de Copie de rapport.pdf (quelle version ?)
• IMG_3847.jpg (contenu ?)

✅ BONS EXEMPLES
─────────────────────────────────────────────────────────────
• 2024-02-16_Procedure_Installation_Apache.pdf (date + description)
• Config_Switch_Principal_v2.3.txt (nom + version)
• Schema_Reseau_Projet1_Final.png (projet + état)
```

**Convention de nommage recommandée :**
```
[Date]_[Type]_[Description]_[Version].[ext]

Exemples :
• 2024-02-16_Procedure_Backup_v1.0.pdf
• 2024-02-15_Schema_Infra_SimIO.png
• 2024-02-14_Config_Firewall_v2.1.txt
```

**② VERSIONNER LES DOCUMENTS**

Utiliser un système de versions explicites :
- v1.0 → version initiale
- v1.1 → corrections mineures
- v2.0 → refonte majeure

**③ TOUJOURS DATER**

Un document sans date est un document mort (on ne sait pas s'il est à jour).

**④ UTILISER UN SEUL OUTIL PAR USAGE**

Ne pas multiplier les outils pour le même besoin :
- ❌ Documentation dans : emails + Word + Google Docs + papier
- ✅ Documentation dans : wiki uniquement

---

## PARTIE II — Le Wiki Technique

### II.A. Qu'est-ce qu'un Wiki ?

Un **wiki** est un site web collaboratif où chaque page peut être modifiée par plusieurs utilisateurs.

```
   CARACTÉRISTIQUES D'UN WIKI
   ─────────────────────────────────────────────────────────────
   ✅ Éditable par plusieurs personnes
   ✅ Historique des modifications (qui, quand, quoi)
   ✅ Recherche intégrée
   ✅ Liens entre pages (navigation fluide)
   ✅ Syntaxe simple (markdown ou équivalent)
   ✅ Pas besoin de coder HTML
```

**Exemples de wikis connus :**
- **Wikipedia** : encyclopédie collaborative mondiale
- **ArchWiki** : documentation Linux Arch (référence dans la communauté)
- **Wiki interne** : documentation d'équipe (IT, projets, procédures)

---

### II.B. Cas d'Usage d'un Wiki IT

| **Usage** | **Contenu typique** | **Exemple** |
|---|---|---|
| **Base de connaissances** | Procédures techniques, FAQ | "Comment créer un utilisateur AD" |
| **Documentation projet** | Architecture, schémas, décisions | "Projet SimIO — Architecture réseau" |
| **Onboarding** | Guide pour nouveaux arrivants | "Bienvenue dans l'équipe IT" |
| **Troubleshooting** | Incidents connus et résolutions | "Serveur mail ne démarre pas → solution" |
| **Inventaire** | Liste des serveurs, IP, comptes | "Serveurs production — tableau récapitulatif" |
| **Veille techno** | Synthèses de veille, nouveautés | "Nouveautés Windows Server 2025" |

---

### II.C. Comparatif des Solutions de Wiki

| **Wiki** | **Technicité** | **Hébergement** | **Coût** | **Points forts** | **Usage type** |
|---|---|---|---|---|---|
| **DokuWiki** | ★☆☆ | Auto-hébergé | Gratuit | Pas de BDD, fichiers texte, plugins | PME, labo, école |
| **MediaWiki** | ★★☆ | Auto-hébergé | Gratuit | Même moteur que Wikipedia, puissant | DSI, projets complexes |
| **BookStack** | ★☆☆ | Auto-hébergé | Gratuit | Interface moderne, organisation livres/chapitres | Équipes < 20 personnes |
| **Confluence** | ★☆☆ | Cloud ou auto | 10 users = 10 $/mois | Intégration Jira, professionnel | Entreprises structurées |
| **Notion** | ★☆☆ | Cloud | Gratuit/payant | Moderne, tout-en-un (wiki+tâches+bases) | Startups, petites équipes |
| **Wiki.js** | ★★☆ | Auto-hébergé | Gratuit | Moderne, markdown natif, open source | Équipes techniques |

> 📌 **Choix S16 BLOC 1 :** DokuWiki — simple, sans base de données, parfait pour apprendre.

---

### II.D. DokuWiki — Présentation

**DokuWiki** est un wiki open source créé en 2004, très utilisé dans les environnements IT.

**Caractéristiques :**
- ✅ Pas de base de données (tout en fichiers texte)
- ✅ Installation en 5 minutes
- ✅ Syntaxe wiki simple
- ✅ 1000+ plugins disponibles
- ✅ Gestion des droits (ACL)
- ✅ Historique des modifications
- ✅ Recherche full-text

**Stockage :**
```
/var/www/dokuwiki/
├── data/
│   ├── pages/           ← Contenu des pages (fichiers .txt)
│   ├── media/           ← Images, fichiers joints
│   └── attic/           ← Historique des versions
├── conf/                ← Configuration
└── lib/                 ← Plugins
```

---

## PARTIE III — Git (Introduction)

### III.A. Le Problème du Versioning

**Situation classique sans Git :**

```
Mon_Projet/
├── script.sh
├── script_v2.sh
├── script_v2_final.sh
├── script_v2_final_VRAI.sh
├── script_v2_final_VRAI_corrigé.sh
└── script_OK.sh            ← Lequel est le bon ?
```

**Problèmes :**
- On ne sait plus quelle est la bonne version
- Impossible de savoir ce qui a changé entre les versions
- Si erreur, difficile de revenir en arrière
- Impossible de travailler à plusieurs sur le même fichier

---

### III.B. Git — La Solution

**Git** est un système de **gestion de versions** (version control system — VCS).

```
   GIT EN UNE PHRASE
   ─────────────────────────────────────────────────────────────
   Git enregistre l'historique complet de toutes les modifications
   d'un projet, permettant de :
   • Revenir à n'importe quelle version
   • Voir qui a modifié quoi et quand
   • Travailler en parallèle sur le même projet
```

**Avantages :**
- ✅ Historique complet de tous les changements
- ✅ Chaque modification est datée et attribuée à son auteur
- ✅ Possibilité de revenir en arrière à n'importe quel moment
- ✅ Branches pour travailler sur des fonctionnalités séparées
- ✅ Collaboration sans conflit

---

### III.C. Git vs GitHub

**Confusion fréquente :** Git ≠ GitHub

| **Aspect** | **Git** | **GitHub** |
|---|---|---|
| **Nature** | Logiciel (installé sur votre PC) | Site web (service en ligne) |
| **Fonction** | Gérer les versions localement | Héberger le code en ligne |
| **Utilisation** | Ligne de commande | Interface web + Git |
| **Coût** | Gratuit | Gratuit (public) / payant (privé) |

**Analogie :**
- **Git** = Word (logiciel pour écrire)
- **GitHub** = Google Drive (endroit pour stocker et partager)

**Alternatives à GitHub :** GitLab, Bitbucket, Gitea

---

### III.D. Les 4 Commandes de Base

**① git init** — Initialiser un dépôt Git

```bash
cd /home/user/mon-projet
git init
# Résultat : Création d'un dossier caché .git
```

**② git add** — Ajouter des fichiers au suivi

```bash
git add script.sh          # Ajouter un fichier
git add .                  # Ajouter tous les fichiers modifiés
```

**③ git commit** — Enregistrer une version

```bash
git commit -m "Ajout de la fonction de backup automatique"
# -m = message décrivant les modifications
```

**④ git log** — Voir l'historique

```bash
git log
# Affiche la liste des commits avec date, auteur, message
```

**Workflow typique :**

```bash
# 1. Créer un projet
mkdir mon-script
cd mon-script
git init

# 2. Créer un fichier
echo "#!/bin/bash" > backup.sh
echo "echo 'Backup en cours...'" >> backup.sh

# 3. Ajouter au suivi Git
git add backup.sh

# 4. Enregistrer la version
git commit -m "Version initiale du script de backup"

# 5. Modifier le fichier
echo "tar -czf backup.tar.gz /data" >> backup.sh

# 6. Enregistrer la modification
git add backup.sh
git commit -m "Ajout de la commande tar pour compresser"

# 7. Voir l'historique
git log
```

---

## PARTIE IV — Partage Documentaire

### IV.A. Solutions de Partage

| **Solution** | **Principe** | **Avantages** | **Inconvénients** | **Usage** |
|---|---|---|---|---|
| **Serveur fichiers (SMB/NFS)** | Dossiers partagés sur serveur local | Contrôle total, rapide, local | Pas d'accès distant facile | PME, réseau local |
| **NAS** | Boîtier dédié partage fichiers | Simple, fiable, RAID | Coût initial | PME/TPE |
| **Cloud public** | Google Drive, Dropbox, OneDrive | Accessible partout, facile | Dépendance, confidentialité | Petites équipes |
| **Cloud privé** | Nextcloud, ownCloud auto-hébergé | Contrôle total, souveraineté | Installation, maintenance | DSI structurées |
| **SharePoint** | Solution Microsoft intégrée Office 365 | Intégration MS, workflow | Complexité, coût | Grandes entreprises |

---

### IV.B. Critères de Choix

**① SÉCURITÉ ET CONFIDENTIALITÉ**

```
   DONNÉES SENSIBLES                     → Hébergement local ou cloud privé
   DONNÉES PUBLIQUES OU PEU SENSIBLES    → Cloud public acceptable
```

**② ACCESSIBILITÉ**

```
   ÉQUIPE NOMADE / TÉLÉTRAVAIL           → Cloud impératif
   ÉQUIPE SUR SITE UNIQUEMENT            → Serveur local suffisant
```

**③ COÛT**

```
   Budget limité                          → Serveur local (coût matériel)
   Budget flexible                        → Cloud public (abonnement)
```

**④ VOLUMÉTRIE**

```
   < 100 Go                               → Cloud public
   100 Go - 1 To                          → NAS ou cloud privé
   > 1 To                                 → Serveur fichiers dédié
```

---

## V. Vocabulaire Clé

| **Terme** | **Définition** |
|-----------|---------------|
| **Travail collaboratif** | Méthodes et outils permettant à une équipe de travailler ensemble efficacement |
| **Wiki** | Site web collaboratif éditable par plusieurs utilisateurs |
| **DokuWiki** | Solution de wiki open source sans base de données |
| **Git** | Système de gestion de versions (VCS) |
| **Commit** | Enregistrement d'une version dans Git avec un message descriptif |
| **Dépôt (repository)** | Projet suivi par Git (contient l'historique des versions) |
| **GitHub** | Service d'hébergement de code en ligne utilisant Git |
| **Versioning** | Suivi des modifications successives d'un fichier |
| **NAS** | Network Attached Storage — boîtier de stockage réseau |
| **Cloud privé** | Service cloud hébergé et contrôlé par l'organisation |
| **Nextcloud** | Solution open source de cloud privé (équivalent Dropbox auto-hébergé) |

---

## ✅ Auto-évaluation

- [ ] J'explique les enjeux du travail collaboratif en IT
- [ ] J'identifie les 4 piliers de la collaboration (documentation, versioning, communication, tâches)
- [ ] Je définis ce qu'est un wiki et liste 3 cas d'usage
- [ ] Je compare DokuWiki, MediaWiki, Confluence
- [ ] J'installe DokuWiki sur Ubuntu Server
- [ ] Je crée une structure documentaire cohérente dans un wiki
- [ ] J'explique à quoi sert Git (versioning, collaboration)
- [ ] Je distingue Git et GitHub
- [ ] J'exécute les 4 commandes de base (init, add, commit, log)
- [ ] Je compare les solutions de partage documentaire

