---
author: YLP
title: 🖥️ Article 32 RGPD
---

# 🖥️ CArticle 32 RGPD : Obligation Légale de Sécurité des Données

---

## 🎯 Objectifs

À la fin de cette séance, je serai capable de :

✅ Expliquer l'**Article 32 RGPD** et son obligation  
✅ Identifier les **4 mesures de sécurité** obligatoires  
✅ Mettre en œuvre le **chiffrement** et la **pseudonymisation**  
✅ Configurer les **contrôles d'accès** (RBAC)  
✅ Comprendre **CIA+R** (Confidentialité, Intégrité, Disponibilité, Résilience)  
✅ Connaître les **sanctions** en cas de manquement


## 📚 Vocabulaire Technique Clé

| **Terme** | **Définition** |
|-----------|----------------|
| **Chiffrement** | Transformation données lisibles → illisibles sans clé |
| **Pseudonymisation** | Remplacer identifiants directs par pseudonymes |
| **RBAC** | Role-Based Access Control (contrôle accès par rôles) |
| **CIA** | Confidentiality, Integrity, Availability (sécurité) |
| **Résilience** | Capacité à résister et récupérer d'un incident |
| **PCA** | Plan de Continuité d'Activité |
| **Hash** | Empreinte numérique unique (SHA-256) |
| **ACL** | Access Control List (liste contrôle accès) |
---

## 1️⃣ L'ARTICLE 32 RGPD : TEXTE ET ANALYSE

### Texte Officiel (Article 32.1)

> *"Compte tenu de l'état des connaissances, des coûts de mise en œuvre et de la nature, de la portée, du contexte et des finalités du traitement ainsi que des risques, dont le degré de probabilité et de gravité varie, pour les droits et libertés des personnes physiques, le responsable du traitement et le sous-traitant mettent en œuvre les **mesures techniques et organisationnelles appropriées** afin de garantir un **niveau de sécurité adapté au risque**."*

---

### Décryptage Juridique

**Qui est concerné ?**
- **Responsable de traitement** (entreprise qui collecte)
- **Sous-traitant** (hébergeur, prestataire)
- → En tant que technicien SISR, vous êtes concerné !

**Quoi faire ?**
- Mettre en œuvre **mesures techniques ET organisationnelles**
- Niveau de sécurité **adapté au risque**

**Principe clé :**
```
Sécurité ≠ Absolu
Sécurité = Proportionné au RISQUE

Risque = Probabilité × Gravité
```

---

## 2️⃣ LES 4 MESURES OBLIGATOIRES (Art. 32.1)

```
╔════════════════════════════════════════════════════╗
║   4 MESURES ARTICLE 32.1 (a, b, c, d)              ║
╠════════════════════════════════════════════════════╣
║                                                    ║
║  a) PSEUDONYMISATION et CHIFFREMENT               ║
║                                                    ║
║  b) CONFIDENTIALITÉ, INTÉGRITÉ, DISPONIBILITÉ     ║
║     et RÉSILIENCE des systèmes                     ║
║                                                    ║
║  c) RÉTABLIR disponibilité et accès               ║
║     en cas d'incident physique ou technique        ║
║                                                    ║
║  d) TESTER, ANALYSER, ÉVALUER régulièrement       ║
║     l'efficacité des mesures                       ║
║                                                    ║
╚════════════════════════════════════════════════════╝
```

**[ILLUSTRATION À INSÉRER]**
**Légende :** Schéma en 4 quadrants représentant les 4 mesures. Quadrant 1 (a) : cadenas (chiffrement). Quadrant 2 (b) : bouclier (CIA). Quadrant 3 (c) : flèche circulaire (restauration). Quadrant 4 (d) : loupe (tests). Couleur code pour chaque quadrant.

---

## 3️⃣ MESURE A : PSEUDONYMISATION ET CHIFFREMENT

### Pseudonymisation (Art. 4.5 RGPD)

**Définition :**
> *"Traitement de données de telle façon que les données ne puissent plus être attribuées à une personne concernée sans information supplémentaire."*

**Exemple pratique :**

| Donnée originale | Pseudonymisée |
|------------------|---------------|
| Jean DUPONT | Utilisateur_4523 |
| marie.durand@mail.com | user_8f7a3b@domain.com |
| 192.168.1.45 | IP_hash_3a8f |

**Intérêt :**
- Réidentification possible (pas anonymisation totale)
- Mais nécessite information supplémentaire (table de correspondance)
- Réduit risque en cas de fuite

---

### Chiffrement

**Définition :** Transformation données lisibles → illisibles sans clé secrète.

**Types de chiffrement :**

```
┌────────────────────────────────────────────────┐
│ CHIFFREMENT SYMÉTRIQUE                         │
│ (Même clé pour chiffrer et déchiffrer)         │
├────────────────────────────────────────────────┤
│ • AES-256 (standard actuel)                    │
│ • Rapide, performant                           │
│ • Usage : Chiffrement disques, fichiers        │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ CHIFFREMENT ASYMÉTRIQUE                        │
│ (Clé publique pour chiffrer, privée déchiffrer)│
├────────────────────────────────────────────────┤
│ • RSA, ECC                                     │
│ • Plus lent                                    │
│ • Usage : HTTPS, emails chiffrés (PGP)         │
└────────────────────────────────────────────────┘
```

---

### Mise en Œuvre Technique

**Chiffrement de disques :**
- **Windows** : BitLocker
- **Linux** : LUKS
- **Macintosh** : FileVault

**Chiffrement de fichiers/dossiers :**
- **VeraCrypt** (multiplateforme)
- **7-Zip** (avec mot de passe AES-256)

**Chiffrement de bases de données :**
- **TDE** (Transparent Data Encryption) - SQL Server, Oracle
- **Chiffrement colonnes** sensibles (salaires, santé)

**Chiffrement communications :**
- **HTTPS** (TLS 1.3)
- **VPN** (OpenVPN, IPSec)

---

## 4️⃣ MESURE B : CONFIDENTIALITÉ, INTÉGRITÉ, DISPONIBILITÉ, RÉSILIENCE

### Le Modèle CIA + R

```
┌────────────────────────────────────────────────┐
│ C - CONFIDENTIALITÉ                            │
│     Seules personnes autorisées accèdent       │
├────────────────────────────────────────────────┤
│ Mesures techniques :                           │
│ • Chiffrement                                  │
│ • Contrôle d'accès (RBAC, ACL)                 │
│ • Authentification (MFA)                       │
│ • VPN                                          │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ I - INTÉGRITÉ                                  │
│     Données non modifiées/altérées             │
├────────────────────────────────────────────────┤
│ Mesures techniques :                           │
│ • Hash (SHA-256, SHA-512)                      │
│ • Signature numérique                          │
│ • Sommes de contrôle (checksum)                │
│ • Journalisation (logs)                        │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ A - DISPONIBILITÉ                              │
│     Données accessibles quand nécessaire       │
├────────────────────────────────────────────────┤
│ Mesures techniques :                           │
│ • Sauvegardes (3-2-1 rule)                     │
│ • Redondance (RAID, cluster)                   │
│ • Plan de continuité (PCA/PRA)                 │
│ • Monitoring                                   │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ R - RÉSILIENCE                                 │
│     Capacité à résister et récupérer           │
├────────────────────────────────────────────────┤
│ Mesures techniques :                           │
│ • Systèmes tolérants aux pannes                │
│ • Récupération rapide (RTO, RPO)               │
│ • Tests réguliers                              │
│ • Documentation procédures                     │
└────────────────────────────────────────────────┘
```

**[ILLUSTRATION À INSÉRER]**
**Légende :** Diagramme en croix des 4 piliers CIA+R. Au centre "Sécurité des données". 4 axes partant du centre vers chaque pilier avec icônes : cadenas (C), bouclier avec coche (I), serveurs multiples (A), flèche circulaire (R).

---

### Focus : RBAC (Role-Based Access Control)

**Principe :** Attribuer droits selon le **rôle** de l'utilisateur.

**Exemple dans Active Directory :**

```
┌──────────────────────────────────────────────┐
│ RÔLE : Comptable                             │
├──────────────────────────────────────────────┤
│ Accès autorisés :                            │
│ • \\serveur\Compta\ (Lecture/Écriture)       │
│ • \\serveur\Direction\ (Lecture seule)       │
│                                              │
│ Accès refusés :                              │
│ • \\serveur\RH\ (Aucun accès)                │
│ • \\serveur\IT\ (Aucun accès)                │
└──────────────────────────────────────────────┘

┌──────────────────────────────────────────────┐
│ RÔLE : Technicien IT                         │
├──────────────────────────────────────────────┤
│ Accès autorisés :                            │
│ • \\serveur\IT\ (Lecture/Écriture)           │
│ • \\serveur\Logs\ (Lecture seule)            │
│ • Droits Admin local (uniquement sur serveurs)│
│                                              │
│ Accès refusés :                              │
│ • \\serveur\Compta\ (Aucun accès)            │
│ • \\serveur\RH\Salaires\ (Aucun accès)       │
└──────────────────────────────────────────────┘
```

**Mise en œuvre :**
1. Créer groupes AD par rôle (GRP_Compta, GRP_IT)
2. Affecter utilisateurs aux groupes
3. Configurer ACL (NTFS) dossiers partagés
4. Appliquer principe **moindre privilège**

---

## 5️⃣ MESURE C : RÉTABLIR DISPONIBILITÉ ET ACCÈS

### Stratégie de Sauvegarde : Règle 3-2-1

```
┌────────────────────────────────────────────────┐
│ RÈGLE 3-2-1                                    │
├────────────────────────────────────────────────┤
│                                                │
│ 3 - Au moins 3 COPIES des données             │
│     (Production + 2 sauvegardes)               │
│                                                │
│ 2 - Sur 2 SUPPORTS différents                 │
│     (Disque dur + NAS OU Bande magnétique)     │
│                                                │
│ 1 - 1 copie HORS SITE (externalisée)          │
│     (Cloud, coffre, site distant)              │
│                                                │
└────────────────────────────────────────────────┘
```

**Exemple conforme :**
- Copie 1 : Serveur production (RAID 5)
- Copie 2 : NAS local (sauvegarde incrémentielle quotidienne)
- Copie 3 : Cloud (AWS S3, Azure Blob) - sauvegarde hebdomadaire

---

### Plan de Continuité (PCA) et Plan de Reprise (PRA)

**PCA (Plan de Continuité d'Activité) :**
- Objectif : **Maintenir** activité pendant incident
- Mesures : Redondance, basculement automatique

**PRA (Plan de Reprise d'Activité) :**
- Objectif : **Restaurer** activité après incident
- Mesures : Procédures de restauration, sites de secours

**Indicateurs clés :**

| Indicateur | Définition | Exemple |
|------------|------------|---------|
| **RTO** (Recovery Time Objective) | Temps maximum d'interruption acceptable | 4 heures |
| **RPO** (Recovery Point Objective) | Perte de données maximum acceptable | 1 heure (dernière sauvegarde) |

---

## 6️⃣ MESURE D : TESTER ET ÉVALUER RÉGULIÈREMENT

### Tests de Sécurité Obligatoires

```
┌────────────────────────────────────────────────┐
│ TYPES DE TESTS                                 │
├────────────────────────────────────────────────┤
│                                                │
│ 1. TEST DE RESTAURATION                       │
│    Vérifier que sauvegardes fonctionnent      │
│    Fréquence : Trimestriel minimum            │
│                                                │
│ 2. TEST DE PÉNÉTRATION (Pentest)              │
│    Simuler attaque externe                     │
│    Fréquence : Annuel minimum                  │
│                                                │
│ 3. AUDIT DE SÉCURITÉ                          │
│    Vérifier conformité procédures              │
│    Fréquence : Annuel                          │
│                                                │
│ 4. EXERCICE PCA/PRA                           │
│    Simuler incident majeur                     │
│    Fréquence : Annuel                          │
│                                                │
│ 5. REVUE DES LOGS                             │
│    Analyser événements sécurité                │
│    Fréquence : Hebdomadaire                    │
│                                                │
└────────────────────────────────────────────────┘
```

**Documentation obligatoire :**
- Rapport de tests (date, résultats, actions correctives)
- Registre des incidents sécurité
- Mises à jour procédures

---

## 7️⃣ MESURES ORGANISATIONNELLES

### Au-delà de la Technique

**L'Article 32 exige AUSSI des mesures organisationnelles :**

```
┌────────────────────────────────────────────────┐
│ POLITIQUE DE SÉCURITÉ                          │
│ Document écrit définissant :                   │
│ • Objectifs sécurité                           │
│ • Rôles et responsabilités                     │
│ • Procédures à suivre                          │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ FORMATION DES UTILISATEURS                     │
│ • Sensibilisation phishing                     │
│ • Bonnes pratiques mots de passe               │
│ • Gestion données personnelles                 │
│ Fréquence : Annuelle minimum                   │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ GESTION DES INCIDENTS                          │
│ • Procédure de signalement                     │
│ • Équipe dédiée (CERT/CSIRT)                   │
│ • Notification CNIL (72h si breach)            │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ CONTRÔLE DES SOUS-TRAITANTS                   │
│ • Clauses RGPD dans contrats                   │
│ • Audits réguliers                             │
│ • Garanties de sécurité                        │
└────────────────────────────────────────────────┘
```

---

## 8️⃣ SANCTIONS ET RESPONSABILITÉS

### Sanctions CNIL (Article 83.4)

**Montant maximum :**
- **10 M€** OU
- **2% du chiffre d'affaires annuel mondial**
- (Le montant le PLUS ÉLEVÉ)

**Critères d'évaluation de la sanction :**
- Gravité violation
- Caractère intentionnel
- Mesures prises pour atténuer
- Coopération avec autorité

---

### Exemples Réels de Sanctions

| Entreprise | Année | Amende | Motif |
|------------|-------|--------|-------|
| **British Airways** | 2020 | 22 M€ | Défaut sécurité site web → Vol 500 000 clients |
| **Marriott** | 2020 | 20 M€ | Faille système réservations → 339 M clients |
| **H&M** | 2020 | 35 M€ | Surveillance excessive + défaut sécurité |
| **EasyJet** | 2020 | 0,5 M€ | Cyberattaque → 9 M clients (mais mesures OK) |

---

### Responsabilité Personnelle

**Attention :** En tant que technicien SISR, vous pouvez être tenu **personnellement responsable** :

**Responsabilité pénale (Code pénal) :**
- Atteinte STAD (Art. 323-1) : 5 ans + 150 000€
- Non-sécurisation données : Mise en danger (Art. 223-1)

**Responsabilité civile :**
- Dommages et intérêts aux victimes

**Responsabilité professionnelle :**
- Licenciement pour faute grave
- Interdiction exercer

---

## 📝 Points Clés à Retenir

### Pour l'Examen

**À connaître PAR CŒUR :**

```
┌────────────────────────────────────────────────┐
│ • Article 32 = Sécurité du traitement         │
│                                                │
│ • 4 mesures : a) Chiffrement                  │
│               b) CIA + Résilience              │
│               c) Rétablir accès                │
│               d) Tester régulièrement          │
│                                                │
│ • Sanction : 10 M€ ou 2% CA                   │
│                                                │
│ • CIA = Confidentialité, Intégrité,           │
│         Availability (Disponibilité)           │
│                                                │
│ • RBAC = Contrôle accès par rôles             │
│                                                │
│ • Règle 3-2-1 sauvegardes                     │
│                                                │
│ • Tests réguliers = OBLIGATOIRES              │
└────────────────────────────────────────────────┘
```

---

### Pour la Vie Professionnelle

**Checklist technicien SISR :**

✅ **Chiffrement :**
- Disques serveurs (BitLocker/LUKS)
- Sauvegardes chiffrées
- Communications (VPN, HTTPS)

✅ **Contrôle d'accès :**
- RBAC dans Active Directory
- Principe moindre privilège
- MFA sur comptes admin

✅ **Sauvegardes :**
- Automatisées quotidiennes
- Règle 3-2-1 respectée
- Tests restauration trimestriels

✅ **Tests et audits :**
- Logs consultés régulièrement
- Pentest annuel
- Exercice PCA/PRA annuel

---

## 🎯 Auto-Évaluation

### Je sais...

- ☐ Expliquer l'Article 32 RGPD
- ☐ Citer les 4 mesures (a, b, c, d)
- ☐ Définir CIA + Résilience
- ☐ Chiffrer un disque (BitLocker/VeraCrypt)
- ☐ Configurer RBAC dans AD
- ☐ Expliquer règle 3-2-1 sauvegardes
- ☐ Connaître sanction Art. 32 (10 M€ ou 2%)
- ☐ Distinguer PCA vs PRA
- ☐ Identifier mesures techniques vs organisationnelles
- ☐ Expliquer RTO et RPO

**Si < 8 cases cochées, revoir la fiche cours.**

---
