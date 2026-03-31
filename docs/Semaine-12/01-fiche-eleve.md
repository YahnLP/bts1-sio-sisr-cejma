---
author: YLP
title: 📚 FICHE DE COURS
---

# 📖 FICHE DE COURS ÉLÈVE
## Licences Logicielles (1) : Modèles Propriétaires

---

## 🎯 Objectifs

À la fin de cette séance, je serai capable de :

✅ Expliquer la **nature juridique** d'une licence logicielle  
✅ Distinguer les **modèles Microsoft** (OEM, Retail, Volume)  
✅ Calculer le nombre de **CAL Windows Server** nécessaires  
✅ Choisir entre **User CAL** et **Device CAL**  
✅ Estimer le **coût total** d'un parc de licences  
✅ Gérer la **conformité** et éviter les audits

---

## 📚 Vocabulaire Clé

| **Terme** | **Définition** |
|-----------|----------------|
| **Licence** | Contrat autorisant l'utilisation d'un logiciel (≠ propriété) |
| **OEM** | Original Equipment Manufacturer (licence liée au hardware) |
| **Retail** | Licence boîte, transférable entre PC |
| **Volume** | Licence entreprise (≥5 licences), gestion centralisée |
| **CAL** | Client Access License (droit d'accès à Windows Server) |
| **KMS** | Key Management Service (activation centralisée Volume) |
| **MAK** | Multiple Activation Key (clé multi-activations) |
| **CLUF** | Contrat de Licence Utilisateur Final (conditions d'usage) |

---


## 1️⃣ NATURE JURIDIQUE D'UNE LICENCE

### Qu'est-ce qu'une Licence Logicielle ?

**Définition juridique :**

> *"Contrat par lequel le titulaire des droits d'auteur autorise un tiers à **utiliser** le logiciel, sans transférer la **propriété** du code."*

**Principe fondamental :**

```
╔════════════════════════════════════════════════════╗
║     VOUS N'ACHETEZ PAS LE LOGICIEL                 ║
╠════════════════════════════════════════════════════╣
║                                                    ║
║  Vous achetez un DROIT D'USAGE                    ║
║                                                    ║
║  L'éditeur reste PROPRIÉTAIRE du code source      ║
║                                                    ║
║  Vous avez des droits LIMITÉS par le contrat     ║
║  (CLUF = Contrat de Licence Utilisateur Final)    ║
║                                                    ║
╚════════════════════════════════════════════════════╝
```

**[ILLUSTRATION À INSÉRER]**
**Légende :** Schéma avec 2 colonnes. Gauche "Propriété" : maison avec titre de propriété (total). Droite "Licence logicielle" : maison en location avec contrat (usage limité). Flèches montrant les différences.

---

### Conséquences Pratiques

**Ce que vous POUVEZ faire (généralement) :**
- ✅ Installer le logiciel sur votre PC
- ✅ Utiliser le logiciel selon les termes du contrat
- ✅ Faire des copies de sauvegarde (usage personnel)

**Ce que vous NE POUVEZ PAS faire :**
- ❌ Revendre le logiciel (sauf Retail sous conditions)
- ❌ Modifier le code source (sauf licence le permettant)
- ❌ Installer sur plusieurs PC avec 1 licence (sauf précisé)
- ❌ Prêter/louer la licence (sauf conditions spécifiques)

---

### Sanctions en Cas de Contrefaçon

**Violation de licence = Contrefaçon**

**Code de la propriété intellectuelle (Art. L335-2) :**
- **3 ans de prison**
- **300 000€ d'amende**

**Sanctions civiles :**
- Dommages et intérêts (jusqu'à 10× le prix des licences manquantes)
- Frais d'audit

**Exemples réels :**
- PME : 80 000€ (20 licences manquantes)
- Entreprise industrielle : 500 000€ (150 licences Windows)

---

## 2️⃣ LES MODÈLES DE LICENCES MICROSOFT

### Vue d'Ensemble

```
┌────────────────────────────────────────────────┐
│ OEM (Original Equipment Manufacturer)          │
│ • Lié au hardware (PC)                         │
│ • Moins cher                                   │
│ • Pas transférable                             │
│ • Support limité                               │
├────────────────────────────────────────────────┤
│ RETAIL (Boîte commerciale)                     │
│ • Indépendant du hardware                      │
│ • Transférable                                 │
│ • Support Microsoft direct                     │
│ • Plus cher                                    │
├────────────────────────────────────────────────┤
│ VOLUME (Entreprise ≥5 licences)               │
│ • Gestion centralisée (KMS, MAK)              │
│ • Prix dégressif                               │
│ • Support professionnel                        │
│ • Droits de downgrade                          │
└────────────────────────────────────────────────┘
```

---

### Modèle OEM (Original Equipment Manufacturer)

**Définition :** Licence **liée au PC** sur lequel elle est installée.

**Caractéristiques :**

| Critère | OEM |
|---------|-----|
| **Prix** | 💰 Moins cher (-30 à -50% vs Retail) |
| **Transfert** | ❌ Non transférable (lié au PC) |
| **Support** | ⚠️ Par le constructeur (pas Microsoft) |
| **Downgrade** | ❌ Non (sauf Volume) |
| **Packaging** | Autocollant COA sur PC |

**Utilisation typique :**
- PC pré-assemblés (Dell, HP, Lenovo)
- Intégrateurs systèmes
- Budget serré + pas de changement PC prévu

**Exemple concret :**
```
PC Dell acheté avec Windows 11 Pro = OEM
→ Si PC tombe en panne et remplacé
→ Licence Windows PERDUE (liée au PC)
→ Doit racheter nouvelle licence pour nouveau PC
```

---

### Modèle Retail (Boîte commerciale)

**Définition :** Licence **indépendante** du hardware, transférable.

**Caractéristiques :**

| Critère | Retail |
|---------|--------|
| **Prix** | 💰💰 Plus cher |
| **Transfert** | ✅ Transférable sur nouveau PC |
| **Support** | ✅ Microsoft direct |
| **Downgrade** | ✅ Oui (ex: Win 11 → Win 10) |
| **Packaging** | Boîte avec clé USB |

**Utilisation typique :**
- Particuliers
- TPE (< 5 licences)
- PC assemblés maison

**Exemple concret :**
```
Achat Windows 11 Pro Retail à la FNAC : 259€
→ Installation sur PC 1
→ PC 1 remplacé par PC 2
→ Désinstallation PC 1, installation PC 2 : OK
→ Licence transférée légalement
```

---

### Modèle Volume (Entreprise)

**Définition :** Licences **groupées** pour entreprises (minimum 5 licences).

**Caractéristiques :**

| Critère | Volume |
|---------|--------|
| **Prix** | 💰💰💰 Prix dégressif (volume) |
| **Transfert** | ✅ Flexible selon contrat |
| **Support** | ✅✅ Support entreprise prioritaire |
| **Downgrade** | ✅✅ Droits étendus |
| **Gestion** | KMS (activation centralisée) |

**Types de contrats Volume :**

1. **Open License** (5-250 licences)
   - Pas d'engagement durée
   - Licence perpétuelle
   - Prix unitaire fixe

2. **Open Value** (5+ licences)
   - Engagement 3 ans
   - Paiements annuels
   - Software Assurance incluse

3. **Enterprise Agreement** (>500 licences)
   - Grandes entreprises
   - Engagement 3 ans
   - Prix négocié

**Activation Volume :**

```
┌────────────────────────────────────────────────┐
│ KMS (Key Management Service)                   │
│ • Serveur interne activation                   │
│ • Clients s'activent automatiquement           │
│ • Minimum 25 clients (Windows Desktop)         │
│ • Réactivation tous les 180 jours             │
├────────────────────────────────────────────────┤
│ MAK (Multiple Activation Key)                  │
│ • Clé unique multi-activations                 │
│ • Quota d'activations (ex: 50, 100...)        │
│ • Activation via Internet ou téléphone         │
└────────────────────────────────────────────────┘
```

---

## 3️⃣ LES CAL (CLIENT ACCESS LICENSE)

### Définition

**CAL = Droit d'accéder à Windows Server.**

**Principe CRUCIAL :**
```
Licence Windows Server = Droit d'installer le serveur
CAL = Droit pour un utilisateur/appareil d'y accéder

Serveur SANS CAL = INUTILISABLE légalement
```

**Exemple :**
```
Serveur Windows Server 2022 : 1 070€
+ 50 utilisateurs qui doivent y accéder
→ Il faut 50 CAL (50 × 45€ = 2 250€)

TOTAL : 1 070€ + 2 250€ = 3 320€
```

---

### User CAL vs Device CAL

**2 types de CAL, 2 logiques différentes :**

```
┌────────────────────────────────────────────────┐
│ USER CAL (par utilisateur)                     │
├────────────────────────────────────────────────┤
│ • 1 personne peut utiliser N appareils         │
│ • Exemple : Commercial avec PC + portable      │
│              → 1 User CAL suffit               │
│                                                │
│ Cas d'usage :                                  │
│ • Utilisateurs nomades                         │
│ • Plusieurs devices par personne               │
│ • Télétravail                                  │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ DEVICE CAL (par appareil)                      │
├────────────────────────────────────────────────┤
│ • 1 appareil peut être utilisé par N personnes │
│ • Exemple : PC atelier utilisé par 3 équipes   │
│              → 1 Device CAL suffit             │
│                                                │
│ Cas d'usage :                                  │
│ • Postes partagés (3×8, hôpital...)           │
│ • Kiosques, bornes                             │
│ • Moins d'appareils que d'utilisateurs         │
└────────────────────────────────────────────────┘
```

**[ILLUSTRATION À INSÉRER]**
**Légende :** Schéma comparatif. Gauche : 1 personne (icône) → 3 appareils (PC, laptop, tablette) = 1 User CAL. Droite : 1 appareil (PC) ← 3 personnes (icônes) = 1 Device CAL. Serveur au centre recevant les connexions.

---

### Formule de Choix

**Règle simple :**

```
IF (Nombre_Utilisateurs < Nombre_Appareils)
    → User CAL (moins cher)
ELSE IF (Nombre_Appareils < Nombre_Utilisateurs)
    → Device CAL (moins cher)
ELSE
    → Indifférent (même prix)
```

**Exemple 1 :**
- 50 utilisateurs
- 30 PC
- **User CAL** : 50 × 45€ = 2 250€
- **Device CAL** : 30 × 45€ = 1 350€
- → **Choisir Device CAL** (économie 900€)

**Exemple 2 :**
- 20 utilisateurs
- 25 PC (dont 5 portables)
- **User CAL** : 20 × 45€ = 900€
- **Device CAL** : 25 × 45€ = 1 125€
- → **Choisir User CAL** (économie 225€)

---

### CAL Cumulatives

**ATTENTION : Les CAL sont cumulatives selon les services.**

```
Windows Server 2022 Standard : 1 CAL
+ SQL Server 2022 : 1 CAL supplémentaire
+ Exchange Server : 1 CAL supplémentaire

Utilisateur accédant aux 3 services = 3 CAL nécessaires
```

**Tableau récapitulatif :**

| Service | CAL nécessaire | Prix unitaire (indicatif) |
|---------|----------------|---------------------------|
| Windows Server | Oui | 45€ |
| SQL Server Standard | Oui | 230€ |
| Exchange Server | Oui | 90€ |
| SharePoint Server | Oui | 85€ |
| Remote Desktop Services (RDS) | Oui | 130€ |

---

## 4️⃣ COMPARAISON DES MODÈLES

### Tableau Comparatif Complet

| Critère | OEM | Retail | Volume |
|---------|-----|--------|--------|
| **Prix unitaire** | 140€ | 259€ | 180-220€ (dégressif) |
| **Transfert PC** | ❌ Non | ✅ Oui | ✅ Oui (selon contrat) |
| **Support** | Constructeur | Microsoft | Microsoft Pro |
| **Downgrade** | ❌ Non | ✅ 1 version | ✅ 2+ versions |
| **Activation** | COA (autocollant) | Clé produit | KMS ou MAK |
| **Gestion centralisée** | ❌ Non | ❌ Non | ✅ Oui |
| **Mise à jour gratuite** | ⚠️ Limitée | ⚠️ Limitée | ✅ Software Assurance |
| **Idéal pour** | PME budget serré | Particuliers, TPE | Entreprises ≥5 PC |

---

### TCO (Total Cost of Ownership) sur 5 ans

**Exemple : 50 PC**

```
┌────────────────────────────────────────────────┐
│ MODÈLE OEM                                     │
├────────────────────────────────────────────────┤
│ Achat initial : 50 × 140€ = 7 000€            │
│ Remplacement 20 PC (an 3) : 20 × 140€ = 2 800€│
│ Support externe : 500€/an × 5 = 2 500€        │
│ TCO 5 ans : 12 300€                           │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ MODÈLE VOLUME                                  │
├────────────────────────────────────────────────┤
│ Achat initial : 50 × 200€ = 10 000€           │
│ Remplacement 20 PC : 0€ (licence transférée)  │
│ Software Assurance : 1 000€/an × 5 = 5 000€   │
│ Support inclus : 0€                            │
│ TCO 5 ans : 15 000€                           │
└────────────────────────────────────────────────┘
```

**Observation :** OEM plus économique SI pas de remplacement PC. Sinon, Volume devient rentable.

---

## 5️⃣ GESTION DE LA CONFORMITÉ

### Inventaire des Licences (CMDB)

**Obligation légale :** Documenter toutes les licences.

**Informations à conserver :**

```
┌────────────────────────────────────────────────┐
│ FICHE LICENCE (par PC)                         │
├────────────────────────────────────────────────┤
│ • Nom PC / Utilisateur                         │
│ • Logiciel (Windows, Office...)                │
│ • Type licence (OEM, Retail, Volume)           │
│ • N° série / Clé produit                       │
│ • Date d'achat                                 │
│ • Facture / Bon de livraison                   │
│ • Date d'installation                          │
│ • Version installée                            │
└────────────────────────────────────────────────┘
```

**Outils d'inventaire :**
- **Microsoft Volume Licensing Service Center** (VLSC)
- **PDQ Inventory**
- **GLPI** (open source)
- **Excel** (PME, acceptable)

---

### Préparer un Audit

**Microsoft peut auditer SANS préavis** (clause contrat Volume).

**Checklist de préparation :**

- ☐ Inventaire à jour (PC + logiciels + licences)
- ☐ Factures d'achat conservées
- ☐ Licences OEM = COA présents sur PC
- ☐ Licences Retail = boîtes/clés conservées
- ☐ Contrats Volume disponibles
- ☐ Nombre de CAL documenté
- ☐ Désinstallations documentées (si PC remplacé)

**Coût d'un audit non-conforme :**
- Régularisation licences manquantes
- Dommages et intérêts (3-10× prix licences)
- Frais d'audit (15 000-50 000€)

---

## 📝 Points Clés à Retenir

### Pour l'Examen

**À connaître PAR CŒUR :**

```
┌────────────────────────────────────────────────┐
│ • Licence = Droit d'usage ≠ Propriété         │
│                                                │
│ • OEM = Lié PC, pas transférable              │
│                                                │
│ • Retail = Transférable, plus cher            │
│                                                │
│ • Volume = ≥5 licences, gestion centralisée   │
│                                                │
│ • CAL obligatoire pour accès serveur          │
│                                                │
│ • User CAL = 1 personne, N appareils          │
│ • Device CAL = 1 appareil, N personnes        │
│                                                │
│ • Règle choix : Comparer Nb users vs devices  │
│                                                │
│ • Contrefaçon = 3 ans + 300 000€              │
└────────────────────────────────────────────────┘
```

---

### Pour la Vie Professionnelle

**Réflexe du technicien SISR :**

✅ **AVANT installation :**
- Vérifier licence disponible
- Documenter dans inventaire
- Conserver facture/preuve d'achat

✅ **PENDANT utilisation :**
- Inventaire régulier (trimestriel)
- Anticiper renouvellements
- Former utilisateurs (pas de copie illégale)

✅ **APRÈS remplacement PC :**
- Si OEM : Licence perdue, racheter
- Si Retail/Volume : Transférer, documenter
- MAJ inventaire

---

## 🎯 Auto-Évaluation

### Je sais...

- ☐ Expliquer droit d'usage vs propriété
- ☐ Définir OEM, Retail, Volume
- ☐ Identifier avantages/inconvénients de chaque modèle
- ☐ Calculer nombre CAL nécessaires
- ☐ Choisir entre User CAL et Device CAL
- ☐ Calculer coût total (licences + CAL)
- ☐ Expliquer sanctions contrefaçon
- ☐ Gérer inventaire de licences
- ☐ Préparer audit Microsoft

**Si < 7 cases cochées, revoir la fiche cours.**

---
