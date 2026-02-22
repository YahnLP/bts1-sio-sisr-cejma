---
author: YLP
title: 📚 FICHE DE COURS
---

# 📚 FICHE DE COURS ÉLÈVE
## "Méthodologie Épreuve E4 · Conseils · Grille d'Évaluation"

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 19*

---

## 🎯 Compétences Travaillées

| **Code** | **Compétence** |
|----------|---------------|
| **Épreuve E4** | Support et mise à disposition de services informatiques |
| **Transversal** | Communication orale, argumentation, gestion du stress |

---

## PARTIE I — Structure de l'Épreuve E4

### I.A. Format Officiel

```
ÉPREUVE E4 — DURÉE 40 MINUTES
═══════════════════════════════════════════════════════════════

PHASE 1 — PRÉSENTATION (20 minutes)
──────────────────────────────────────────────────────────────
Le candidat présente 2 situations professionnelles choisies
dans son portfolio.

Pour chaque situation (10 minutes) :
  • Contexte et problématique
  • Mission confiée
  • Réalisation technique
  • Résultats obtenus
  • Bilan et réflexion

Support autorisé :
  • Slides (PowerPoint, LibreOffice)
  • Schémas techniques
  • Démonstration sur ordinateur (si pertinent)


PHASE 2 — ENTRETIEN (20 minutes)
──────────────────────────────────────────────────────────────
Le jury pose des questions sur :
  • Les choix techniques effectués
  • Les difficultés rencontrées et résolutions
  • Les alternatives possibles
  • La veille technologique
  • Les compétences mobilisées

Le candidat doit :
  • Répondre de manière précise et argumentée
  • Utiliser le vocabulaire technique approprié
  • Faire preuve de recul critique
```

---

### I.B. Ce que le Jury Évalue

| **Critère** | **Description** | **Exemples** |
|---|---|---|
| **Compétences techniques** | Maîtrise des outils, procédures, normes | Configuration GLPI, droits NTFS, tickets ITIL |
| **Démarche professionnelle** | Méthodologie, documentation, suivi | Diagnostic structuré, RFC, wiki |
| **Résolution de problèmes** | Diagnostic, tests, solutions | Analyse des 3 tickets en S17 |
| **Communication** | Clarté, vocabulaire, argumentation | Explication technique accessible |
| **Réflexion critique** | Analyse, axes d'amélioration, veille | "Avec le recul, j'aurais pu..." |

---

## PARTIE II — Structure d'une Présentation Situation

### II.A. Plan Type (10 minutes par situation)

```
STRUCTURE RECOMMANDÉE POUR 1 SITUATION
═══════════════════════════════════════════════════════════════

1. CONTEXTE (2 minutes)
──────────────────────────────────────────────────────────────
"Je vais vous présenter une situation vécue lors de mon
alternance chez [Entreprise]."

• Présentation de l'entreprise (secteur, taille)
• Problématique ou besoin initial
• Enjeux pour l'entreprise

Exemple :
"SimIO SARL est une PME de 80 employés. L'entreprise
n'avait pas de système de support centralisé, ce qui
causait des pertes d'informations et des délais de
résolution longs."


2. MISSION (1 minute)
──────────────────────────────────────────────────────────────
"Ma mission était de..."

• Objectifs clairs et précis
• Périmètre (ce qui était demandé)
• Contraintes (temps, budget, ressources)

Exemple :
"J'ai été chargé d'installer et configurer GLPI pour
centraliser la gestion des incidents et OCS Inventory
pour automatiser l'inventaire du parc."


3. RÉALISATION (5 minutes)
──────────────────────────────────────────────────────────────
"Voici comment j'ai procédé..."

• Étapes de réalisation (3-5 étapes principales)
• Choix techniques justifiés
• Outils et technologies utilisés
• Difficultés rencontrées et solutions apportées

Exemple :
"1. Installation GLPI sur Ubuntu avec stack LAMP
 2. Configuration base de données et permissions
 3. Installation OCS Inventory Server
 4. Déploiement agents OCS sur 10 postes pilotes
 5. Synchronisation OCS → GLPI via plugin"

[Montrer schéma architecture si disponible]


4. RÉSULTATS (1 minute)
──────────────────────────────────────────────────────────────
"Voici les résultats obtenus..."

• Résultats quantitatifs (chiffres, métriques)
• Résultats qualitatifs (satisfaction, impact)
• Validation de la mission

Exemple :
"80 postes inventoriés automatiquement, système utilisé
par 80 utilisateurs, temps de résolution réduit de 40%,
retours positifs sur les guides utilisateur."


5. BILAN (1 minute)
──────────────────────────────────────────────────────────────
"Avec le recul..."

• Compétences mobilisées (référentiel)
• Ce qui a bien fonctionné
• Points d'amélioration identifiés
• Veille technologique effectuée

Exemple :
"Cette situation m'a permis de mobiliser les compétences
B1.4 (outils de gestion de parc) et B1.5 (mise à
disposition de services). Si c'était à refaire, je
configurerais l'authentification LDAP dès le début."
```

---

### II.B. Exemple de Slide Type

```
╔══════════════════════════════════════════════════════════════╗
║                   SLIDE 1 — TITRE                            ║
╠══════════════════════════════════════════════════════════════╣
║                                                              ║
║   Situation N°3 :                                            ║
║   Mise en Place Système de Support IT                        ║
║   (GLPI + OCS Inventory)                                     ║
║                                                              ║
║   SimIO SARL — Février 2025                                  ║
║                                                              ║
╚══════════════════════════════════════════════════════════════╝


╔══════════════════════════════════════════════════════════════╗
║                   SLIDE 2 — CONTEXTE                         ║
╠══════════════════════════════════════════════════════════════╣
║                                                              ║
║   ENTREPRISE                                                 ║
║   • SimIO SARL — Commerce informatique                       ║
║   • 80 employés, 4 services                                  ║
║                                                              ║
║   PROBLÉMATIQUE                                              ║
║   ❌ Pas d'inventaire centralisé                             ║
║   ❌ Gestion incidents via emails                            ║
║   ❌ Pas de suivi des demandes                               ║
║                                                              ║
║   ENJEUX                                                     ║
║   • Améliorer qualité du support                             ║
║   • Réduire temps de résolution                              ║
║                                                              ║
╚══════════════════════════════════════════════════════════════╝


╔══════════════════════════════════════════════════════════════╗
║                   SLIDE 3 — MISSION                          ║
╠══════════════════════════════════════════════════════════════╣
║                                                              ║
║   OBJECTIFS                                                  ║
║                                                              ║
║   ① Installer GLPI (helpdesk)                                ║
║   ② Installer OCS Inventory (inventaire auto)                ║
║   ③ Synchroniser OCS → GLPI                                  ║
║   ④ Créer catalogue de services                              ║
║   ⑤ Former les utilisateurs (guides)                         ║
║                                                              ║
║   CONTRAINTES                                                ║
║   • Délai : 2 semaines                                       ║
║   • Budget : Open source uniquement                          ║
║                                                              ║
╚══════════════════════════════════════════════════════════════╝


╔══════════════════════════════════════════════════════════════╗
║                SLIDE 4 — ARCHITECTURE                        ║
╠══════════════════════════════════════════════════════════════╣
║                                                              ║
║   [SCHÉMA TECHNIQUE]                                         ║
║                                                              ║
║   ┌─────────────┐                                            ║
║   │ CLIENTS (80)│                                            ║
║   │ Agent OCS   │                                            ║
║   └──────┬──────┘                                            ║
║          │                                                   ║
║          ↓                                                   ║
║   ┌─────────────────┐      ┌────────────┐                   ║
║   │ OCS INVENTORY   │─────→│   GLPI     │                   ║
║   │ (Serveur)       │      │ (Helpdesk) │                   ║
║   └─────────────────┘      └────────────┘                   ║
║          │                        │                          ║
║          ↓                        ↓                          ║
║   ┌─────────────┐          ┌─────────────┐                  ║
║   │   MySQL     │          │   MySQL     │                  ║
║   └─────────────┘          └─────────────┘                  ║
║                                                              ║
╚══════════════════════════════════════════════════════════════╝


╔══════════════════════════════════════════════════════════════╗
║               SLIDE 5 — RÉSULTATS                            ║
╠══════════════════════════════════════════════════════════════╣
║                                                              ║
║   QUANTITATIFS                                               ║
║   ✅ 80 postes inventoriés automatiquement                   ║
║   ✅ 80 utilisateurs actifs dans GLPI                        ║
║   ✅ 12 services IT catalogués                               ║
║   ✅ 3 incidents résolus et documentés                       ║
║                                                              ║
║   QUALITATIFS                                                ║
║   ✅ Temps de résolution : -40%                              ║
║   ✅ Traçabilité complète des tickets                        ║
║   ✅ Satisfaction utilisateurs (guides)                      ║
║                                                              ║
╚══════════════════════════════════════════════════════════════╝
```

---

## PARTIE III — Réussir l'Entretien (Phase Questions)

### III.A. Types de Questions du Jury

**① QUESTIONS D'APPROFONDISSEMENT TECHNIQUE**

```
Exemples :
"Comment avez-vous configuré exactement les droits NTFS ?"
"Pourquoi avoir choisi GLPI plutôt qu'un autre outil ?"
"Expliquez-nous le fonctionnement de la synchronisation OCS → GLPI."

Comment répondre :
• Être précis et technique
• Utiliser le vocabulaire approprié
• Montrer qu'on maîtrise le sujet
• Si on ne sait pas : le dire honnêtement et expliquer comment
  on trouverait la réponse
```

**② QUESTIONS SUR LES DIFFICULTÉS**

```
Exemples :
"Quelles difficultés avez-vous rencontrées ?"
"Comment avez-vous résolu le problème X ?"
"Qui vous a aidé ? Comment avez-vous trouvé la solution ?"

Comment répondre :
• Être honnête (tout le monde rencontre des difficultés)
• Décrire la méthodologie de résolution
• Montrer son autonomie ou sa capacité à chercher de l'aide
• Mettre en avant l'apprentissage
```

**③ QUESTIONS SUR LES ALTERNATIVES**

```
Exemples :
"Auriez-vous pu faire autrement ?"
"Quelles autres solutions avez-vous envisagées ?"
"Connaissez-vous d'autres outils qui auraient pu convenir ?"

Comment répondre :
• Montrer qu'on a réfléchi aux alternatives
• Justifier le choix fait
• Citer d'autres solutions (même si non retenues)
• Faire preuve de veille technologique
```

**④ QUESTIONS DE RECUL CRITIQUE**

```
Exemples :
"Avec le recul, que feriez-vous différemment ?"
"Quels sont les points d'amélioration de votre solution ?"
"Comment feriez-vous évoluer ce système ?"

Comment répondre :
• Faire preuve d'autocritique constructive
• Proposer des améliorations concrètes
• Montrer une vision évolutive
• Démontrer une démarche d'amélioration continue
```

**⑤ QUESTIONS SUR LES COMPÉTENCES**

```
Exemples :
"Quelles compétences du référentiel avez-vous mobilisées ?"
"En quoi cette situation illustre-t-elle la compétence B1.4 ?"
"Comment documentez-vous vos interventions ?"

Comment répondre :
• Citer les codes des compétences (B1.x, B2.x...)
• Faire le lien explicite entre action et compétence
• Donner des exemples concrets
```

---

### III.B. Les 10 Commandements de l'Oral E4

```
① Tu prépareras tes réponses aux questions types
② Tu maîtriseras ton temps (20 min max par phase)
③ Tu utiliseras le vocabulaire technique correct
④ Tu seras honnête (pas d'invention ou exagération)
⑤ Tu montreras ton portfolio et tes preuves
⑥ Tu feras preuve de recul critique
⑦ Tu citeras tes sources (veille technologique)
⑨ Tu garderas ton calme même si stressé
⑨ Tu écouteras la question avant de répondre
⑩ Tu demanderas de reformuler si tu ne comprends pas
```

---

## PARTIE IV — Conseils Pratiques

### IV.A. Avant l'Épreuve

**1 SEMAINE AVANT**
- ✅ Finaliser le portfolio (3 situations minimum)
- ✅ Préparer le support de présentation (slides)
- ✅ Répéter devant un miroir ou un proche
- ✅ Chronométrer la présentation (20 min max)

**LA VEILLE**
- ✅ Relire toutes les situations
- ✅ Vérifier le matériel (ordinateur, clé USB, câbles)
- ✅ Préparer les preuves (captures, schémas, documents)
- ✅ Se coucher tôt

**LE JOUR J**
- ✅ Arriver 15 minutes en avance
- ✅ Respirer profondément pour gérer le stress
- ✅ Saluer le jury avec professionnalisme
- ✅ Sourire et faire preuve d'assurance

---

### IV.B. Pendant l'Épreuve

**✅ À FAIRE**
- Regarder le jury (pas seulement l'écran)
- Parler clairement et à un rythme posé
- Utiliser le support visuel (pointer, montrer)
- Gérer le temps (timer)
- Répondre directement aux questions posées
- Dire "Je ne sais pas" si c'est le cas (puis expliquer comment trouver)

**❌ À ÉVITER**
- Lire ses notes ou slides intégralement
- Parler trop vite (signe de stress)
- Dépasser le temps imparti
- Inventer ou exagérer
- Répondre à côté de la question
- Être trop familier (vouvoyer le jury)
- Critiquer son entreprise ou son tuteur

---

## V. Vocabulaire Clé

| **Terme** | **Définition** |
|-----------|---------------|
| **Portfolio** | Recueil de situations professionnelles pour l'épreuve E4 |
| **Situation professionnelle** | Expérience vécue en entreprise mobilisant des compétences |
| **Jury** | Évaluateurs de l'épreuve (enseignant + professionnel) |
| **Entretien** | Phase de questions après la présentation |
| **Compétence** | Savoir-faire professionnel du référentiel (ex : B1.4) |
| **Preuve** | Document justifiant la réalisation (capture, schéma, attestation) |
| **Recul critique** | Capacité à analyser sa pratique et identifier des améliorations |

