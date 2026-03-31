---
author: YLP
title: 🖥️ FICHE Bilan
---

# 📌 FICHE BILAN & MÉMO
## Licences Logicielles : L'Essentiel à Retenir

## 🎯 Synthèse de la Séance

| **Élément** | **Détail** |
|-------------|-----------|
| **Thème** | Licences logicielles propriétaires (OEM, Retail, Volume) |
| **Durée** | 4 heures |
| **Approche** | Juridique + Économique + Gestion de parc |
| **Compétences** | B1.1, B1.4, B3.4 |

---

## ✅ Objectifs Atteints

- ✅ Comprendre **nature juridique** d'une licence (droit d'usage ≠ propriété)
- ✅ Maîtriser **3 modèles Microsoft** (OEM, Retail, Volume)
- ✅ Calculer **CAL Windows Server** (User vs Device)
- ✅ Estimer **coût total** d'un parc de licences
- ✅ Gérer **conformité** et éviter audits
- ✅ Conseiller selon **contexte** (PME, startup, grande entreprise)

---

## 🔑 Le Principe Fondamental

```
╔════════════════════════════════════════════════════╗
║           LICENCE ≠ PROPRIÉTÉ                      ║
╠════════════════════════════════════════════════════╣
║                                                    ║
║  Vous n'ACHETEZ PAS le logiciel                   ║
║                                                    ║
║  Vous achetez un DROIT D'UTILISATION              ║
║  limité par un contrat (CLUF)                     ║
║                                                    ║
║  L'éditeur reste PROPRIÉTAIRE du code             ║
║                                                    ║
║  Violation = CONTREFAÇON (3 ans + 300 000€)      ║
║                                                    ║
╚════════════════════════════════════════════════════╝
```

---

## 📊 Les 3 Modèles Microsoft

### Tableau Comparatif Express

| | OEM | Retail | Volume |
|---|-----|--------|--------|
| **Prix** | 💰 Bas (140€) | 💰💰 Moyen (259€) | 💰💰💰 Dégressif (180-220€) |
| **Transfert** | ❌ NON (lié PC) | ✅ OUI | ✅ OUI |
| **Support** | Constructeur | Microsoft | Microsoft Pro |
| **Idéal pour** | PME budget serré | Particuliers, TPE | Entreprises ≥5 PC |

---

### OEM (Original Equipment Manufacturer)

```
┌────────────────────────────────────────────────┐
│ • LIÉ AU HARDWARE (PC)                         │
│ • Pas transférable sur nouveau PC             │
│ • Moins cher (-30 à -50%)                      │
│ • Support par constructeur (pas Microsoft)     │
│ • Autocollant COA sur PC                       │
│                                                │
│ Cas d'usage :                                  │
│ • Budget limité                                │
│ • Pas de changement PC prévu                   │
│ • PME/TPE                                      │
└────────────────────────────────────────────────┘
```

---

### Retail (Boîte commerciale)

```
┌────────────────────────────────────────────────┐
│ • INDÉPENDANT du hardware                      │
│ • Transférable sur nouveau PC                  │
│ • Plus cher                                    │
│ • Support Microsoft direct                     │
│ • Boîte avec clé USB/COA                       │
│                                                │
│ Cas d'usage :                                  │
│ • Particuliers                                 │
│ • TPE < 5 PC                                   │
│ • Besoin flexibilité                           │
└────────────────────────────────────────────────┘
```

---

### Volume (Entreprise ≥5 licences)

```
┌────────────────────────────────────────────────┐
│ • GESTION CENTRALISÉE (KMS, MAK)               │
│ • Prix dégressif selon volume                  │
│ • Support professionnel                        │
│ • Droits downgrade étendus                     │
│ • Software Assurance (mises à jour)            │
│                                                │
│ Types :                                        │
│ • Open License (5-250)                         │
│ • Open Value (5+, engagement 3 ans)            │
│ • Enterprise Agreement (>500)                  │
│                                                │
│ Activation :                                   │
│ • KMS (serveur interne, ≥25 clients)          │
│ • MAK (clé multi-activations)                  │
└────────────────────────────────────────────────┘
```

---

## 🎯 Les CAL en 1 Minute

### Principe

```
Windows Server = 2 éléments obligatoires

1. LICENCE SERVEUR (1 070€)
   → Droit d'installer le serveur

2. CAL (45€ / unité)
   → Droit d'accéder au serveur
```

**SANS CAL = Serveur inutilisable légalement**

---

### User CAL vs Device CAL

```
USER CAL
├─ 1 personne → N appareils
├─ Commercial avec PC + portable = 1 CAL suffit
└─ Idéal si : Utilisateurs < Appareils

DEVICE CAL
├─ 1 appareil → N personnes
├─ PC atelier 3×8 = 1 CAL suffit
└─ Idéal si : Appareils < Utilisateurs
```

**[ILLUSTRATION À INSÉRER]**
**Légende :** Schéma balance. Gauche : icônes utilisateurs. Droite : icônes appareils. Fléau au centre indiquant "Comparer pour choisir". Si utilisateurs < appareils → flèche vers "User CAL". Si appareils < utilisateurs → flèche vers "Device CAL".

---

### Formule de Choix

```
IF (Nombre_Utilisateurs < Nombre_Appareils)
    → User CAL (moins cher)
ELSE IF (Nombre_Appareils < Nombre_Utilisateurs)
    → Device CAL (moins cher)
ELSE
    → Équivalent (même prix)
```

**Exemple :**
- 50 users, 30 devices → 30 Device CAL (1 350€)
- 20 users, 35 devices → 20 User CAL (900€)

---

## 🔧 Aide-Mémoire Calcul CAL

### Étapes de Calcul

```
ÉTAPE 1 : Identifier qui accède au serveur
├─ Compter utilisateurs (personnes physiques)
└─ Compter appareils (PC, portables, tablettes)

ÉTAPE 2 : Comparer les nombres
├─ IF Users < Devices → User CAL
└─ ELSE → Device CAL

ÉTAPE 3 : Calculer le coût
├─ Nombre CAL × 45€ = Coût CAL
└─ + Licence serveur (1 070€) = Coût total
```

---

### Exemple Complet

**Entreprise :** 40 salariés, 50 PC (dont 10 portables)

```
Utilisateurs : 40
Appareils : 50

40 < 50 → User CAL plus économique

Calcul :
• 40 User CAL × 45€ = 1 800€
• Licence serveur = 1 070€
• TOTAL = 2 870€ HT

Si Device CAL :
• 50 Device CAL × 45€ = 2 250€
• Licence serveur = 1 070€
• TOTAL = 3 320€ HT

Économie avec User CAL : 450€
```

---

## ⚖️ Conformité et Audits

### Checklist Conformité

**✅ À FAIRE obligatoirement :**

- ☐ Tenir inventaire licences à jour (CMDB)
- ☐ Conserver factures d'achat
- ☐ Vérifier COA présents sur PC OEM
- ☐ Documenter installations
- ☐ Former utilisateurs (pas de copie illégale)
- ☐ Audit interne annuel
- ☐ Prévoir budget renouvellement

---

### Préparer un Audit Microsoft

**Microsoft peut auditer SANS préavis** (clause contrats Volume).

**Documents à préparer :**

```
┌────────────────────────────────────────────────┐
│ DOSSIER AUDIT                                  │
├────────────────────────────────────────────────┤
│ ✓ Inventaire complet (Excel ou outil)         │
│ ✓ Factures d'achat licences                   │
│ ✓ Contrats Volume (si applicable)             │
│ ✓ COA photos (licences OEM)                   │
│ ✓ Historique installations                    │
│ ✓ Documentation CAL                           │
│ ✓ Procédure gestion licences                  │
└────────────────────────────────────────────────┘
```

**Coût audit non-conforme :**
- Régularisation licences manquantes
- Dommages et intérêts (3-10× prix)
- Frais audit (15-50 k€)

---

### Sanctions Contrefaçon

**Code propriété intellectuelle (Art. L335-2) :**

```
╔════════════════════════════════════════════════════╗
║       SANCTIONS CONTREFAÇON LOGICIEL               ║
╠════════════════════════════════════════════════════╣
║                                                    ║
║  PÉNAL :                                           ║
║  • 3 ans de prison                                ║
║  • 300 000 € d'amende                             ║
║                                                    ║
║  CIVIL :                                           ║
║  • Dommages et intérêts                           ║
║  • 3 à 10× prix licences manquantes               ║
║                                                    ║
║  EXEMPLES :                                        ║
║  • PME 20 licences : 80 000 €                     ║
║  • Entreprise 150 licences : 500 000 €            ║
║                                                    ║
╚════════════════════════════════════════════════════╝
```

---

## 💡 Situations Pratiques

### Cas 1 : Remplacement PC avec OEM

```
SITUATION :
PC Dell (2020) avec Windows 10 Pro OEM
PC tombe en panne → Remplacement

QUESTION : Puis-je transférer la licence ?

RÉPONSE : ❌ NON
• OEM = lié au PC Dell
• PC change → Licence perdue
• Doit racheter nouvelle licence

SOLUTION :
• Racheter OEM (140€, économique)
• OU Retail (259€, transférable futur)
• OU Volume si ≥5 PC (gestion centralisée)
```

---

### Cas 2 : Windows Home en Entreprise

```
SITUATION :
10 PC avec Windows 11 Home (achat grand public)
Besoin rejoindre domaine AD

QUESTION : Home suffit-il ?

RÉPONSE : ❌ NON
• Home ne peut pas rejoindre domaine
• Pas de GPO
• Pas de BitLocker

SOLUTION :
• Upgrade Home → Pro (99€/PC)
• Total : 10 × 99€ = 990€
• Économie vs Pro complet : 1 600€
```

---

### Cas 3 : Calcul CAL Complexe

```
SITUATION :
• 30 salariés fixes (1 PC chacun)
• 10 commerciaux (PC fixe + portable chacun)
• 5 stagiaires rotatifs (5 PC partagés)

CALCUL :
Utilisateurs : 30 + 10 + 5 = 45
Appareils : 30 + (10×2) + 5 = 55

45 < 55 → User CAL

COÛT :
• 45 User CAL × 45€ = 2 025€
• Serveur = 1 070€
• TOTAL = 3 095€ HT
```

---

## 📝 Auto-Évaluation Finale

### Je maîtrise...

**Connaissances :**
- ☐ Expliquer licence = droit d'usage ≠ propriété
- ☐ Définir OEM, Retail, Volume
- ☐ Comparer avantages/inconvénients modèles
- ☐ Expliquer obligation CAL pour serveur

**Calculs :**
- ☐ Calculer nombre CAL nécessaires
- ☐ Choisir User vs Device CAL
- ☐ Estimer coût total (licences + CAL)
- ☐ Calculer TCO sur plusieurs années

**Gestion :**
- ☐ Tenir inventaire licences
- ☐ Préparer audit Microsoft
- ☐ Documenter conformité
- ☐ Conseiller choix selon contexte

**Si < 10 cases cochées sur 12, revoir la fiche cours.**

---

## 🔗 Liens avec Autres Séances

| Séance | Lien avec S12 |
|--------|---------------|
| **S4 (Économie hardware)** | Licences = partie TCO matériel |
| **S13 (Open Source)** | Comparaison modèles propriétaires vs libres |
| **Bloc 1 - Gestion parc** | Inventaire licences = CMDB ITIL |
| **Bloc 1 - Windows Server** | CAL obligatoires pour AD, partages |

---

## 📚 Ressources Complémentaires

**Officielles :**
- **Microsoft Volume Licensing** : microsoft.com/licensing
- **Microsoft Product Terms** : Document contractuel officiel
- **VLSC** (Volume Licensing Service Center) : Gestion licences

**Outils :**
- **PDQ Inventory** : Inventaire automatisé
- **GLPI** : Gestion parc open source
- **SpiceWorks** : Inventaire gratuit
- **Excel** : Template inventaire (PME)

**Formation :**
- **Microsoft Learn** : Modules licensing
- **SAM** (Software Asset Management) : Certification

---

## 💡 Points Clés pour l'Examen

**À retenir PAR CŒUR :**

```
┌────────────────────────────────────────────────┐
│ • Licence = Droit d'usage ≠ Propriété         │
│                                                │
│ • OEM = Lié PC, 140€, pas transférable        │
│                                                │
│ • Retail = Transférable, 259€, boîte          │
│                                                │
│ • Volume = ≥5 lic, KMS/MAK, gestion centralisée│
│                                                │
│ • CAL obligatoire pour accès serveur          │
│   Serveur seul = inutilisable                 │
│                                                │
│ • User CAL : 1 personne, N devices            │
│ • Device CAL : 1 device, N personnes          │
│                                                │
│ • Règle : Choisir MIN(users, devices)         │
│                                                │
│ • Contrefaçon = 3 ans + 300 000€              │
│                                                │
│ • Inventaire = OBLIGATOIRE                    │
│   (preuve conformité si audit)                │
└────────────────────────────────────────────────┘
```

---

## 🎯 Message Final

**Les licences = Enjeu stratégique, pas juste "acheter Windows"**

```
Mal gérer les licences :
❌ Surcoûts (achats inutiles)
❌ Sous-licence (amendes)
❌ Audits (stress, temps, argent)
❌ Non-conformité juridique

Bien gérer les licences :
✅ Optimisation budgétaire
✅ Conformité juridique
✅ Audits sans problème
✅ Crédibilité professionnelle
✅ Valorisation compétences SISR
```

**⚠️ En tant que technicien SISR, vous êtes le GARANT de la conformité licences.**

---
