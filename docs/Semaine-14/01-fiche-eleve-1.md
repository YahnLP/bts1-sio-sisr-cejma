---
author: YLP
title: 📚 FICHE DE COURS
---

# 📖 FICHE DE COURS ÉLÈVE
## S14 — Droit de la Preuve : Logs, Signature Électronique, Horodatage

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 14*

---

## 🎯 Objectifs

À la fin de cette séance, je serai capable de :

✅ Expliquer la **valeur juridique** d'un écrit électronique (Art. 1366)  
✅ Identifier les **conditions de recevabilité** des logs  
✅ Distinguer les **3 niveaux de signature électronique** (eIDAS)  
✅ Comprendre l'**horodatage qualifié** (RFC 3161)  
✅ Mettre en œuvre **hash SHA-256** pour garantir intégrité  
✅ Gérer les logs comme **preuves juridiques**

---


## 📚 Vocabulaire Juridique et Technique

| **Terme** | **Définition** |
|-----------|----------------|
| **Preuve** | Élément établissant la réalité d'un fait juridique |
| **Force probante** | Valeur juridique d'une preuve devant un tribunal |
| **Intégrité** | Garantie qu'un document n'a pas été modifié |
| **Hash** | Empreinte numérique unique d'un fichier (SHA-256) |
| **Signature électronique** | Procédé cryptographique d'authentification |
| **eIDAS** | Règlement UE sur l'identification électronique |
| **Horodatage** | Preuve de l'existence d'une donnée à un instant T |
| **TSA** | Time Stamping Authority (autorité d'horodatage) |

---

## 1️⃣ VALEUR JURIDIQUE DE L'ÉCRIT ÉLECTRONIQUE

### Article 1366 du Code Civil

**Texte intégral :**

> *"L'écrit électronique a la même force probante que l'écrit sur support papier, sous réserve que puisse être dûment identifiée la personne dont il émane et qu'il soit établi et conservé dans des conditions de nature à en garantir l'intégrité."*

**Principe fondamental :**

```
╔════════════════════════════════════════════════════╗
║  ÉCRIT ÉLECTRONIQUE = ÉCRIT PAPIER                 ║
║  (même valeur juridique)                           ║
╠════════════════════════════════════════════════════╣
║                                                    ║
║  MAIS 2 CONDITIONS OBLIGATOIRES :                  ║
║                                                    ║
║  1. IDENTIFICATION de la personne                 ║
║     → Qui a créé le document ?                     ║
║                                                    ║
║  2. INTÉGRITÉ du document                         ║
║     → Document non modifié depuis création ?       ║
║                                                    ║
╚════════════════════════════════════════════════════╝
```

**[ILLUSTRATION À INSÉRER]**
**Légende :** Balance équilibrée. Plateau gauche : document papier avec signature manuscrite. Plateau droite : document électronique avec certificat + hash. Annotation "Valeur probante égale SI conditions respectées".

---

### Les 2 Conditions Détaillées

**CONDITION 1 : Identification**

Moyens d'identification acceptés :
- Login + mot de passe (si traçabilité)
- Certificat électronique
- Signature électronique (simple, avancée, qualifiée)
- Adresse email (si authentifiée)

**CONDITION 2 : Intégrité**

Moyens de garantir l'intégrité :
- Hash cryptographique (SHA-256)
- Signature numérique
- Stockage immuable (blockchain, WORM)
- Horodatage qualifié

---

## 2️⃣ LES LOGS COMME PREUVE JURIDIQUE

### Qu'est-ce qu'un Log ?

**Définition technique :**
> Enregistrement automatique d'un événement système (connexion, modification, accès fichier, erreur).

**Définition juridique :**
> Écrit électronique traçant une action, pouvant servir de preuve si conditions Art. 1366 respectées.

---

### Conditions de Recevabilité des Logs

**Pour qu'un log soit recevable comme preuve :**

```
┌────────────────────────────────────────────────┐
│ 1. INTÉGRITÉ PROUVÉE                           │
│    → Hash SHA-256 du fichier log               │
│    → Stockage immuable (append-only)           │
│    → Signature numérique                       │
├────────────────────────────────────────────────┤
│ 2. HORODATAGE FIABLE                          │
│    → Timestamp NTP synchronisé                 │
│    → Horodatage qualifié (TSA) si critique     │
├────────────────────────────────────────────────┤
│ 3. IDENTIFICATION AUTEUR                       │
│    → Quel utilisateur/système a généré ?       │
│    → Traçabilité (login, IP, certificat)       │
├────────────────────────────────────────────────┤
│ 4. CONSERVATION SÉCURISÉE                      │
│    → Logs non modifiables                      │
│    → Stockage centralisé (serveur syslog)      │
│    → Durée légale respectée                    │
├────────────────────────────────────────────────┤
│ 5. PROCÉDURE DOCUMENTÉE                        │
│    → Politique de logs écrite                  │
│    → Procédure de collecte                     │
│    → Chaîne de traçabilité                     │
└────────────────────────────────────────────────┘
```

---

### Jurisprudence sur les Logs

**Cour de cassation, Chambre sociale (2019) :**

**Faits :**
- Salarié licencié pour usage abusif Internet (sites pornographiques)
- Employeur présente logs serveur proxy

**Question juridique :**
Les logs sont-ils recevables comme preuve du comportement fautif ?

**Décision :**
✅ **Logs RECEVABLES**

**Motifs :**
- Logs horodatés de manière fiable (serveur NTP)
- Intégrité garantie (stockage centralisé, pas de modification)
- Identification claire du salarié (login unique)
- Conservation sécurisée conforme

→ Licenciement pour faute grave **CONFIRMÉ**

---

**Conseil d'État (2020) - Contre-exemple :**

**Faits :**
- Administration présente logs pour prouver connexion agent

**Question :**
Logs recevables ?

**Décision :**
❌ **Logs REJETÉS**

**Motifs :**
- Pas de preuve d'intégrité (pas de hash)
- Logs présentés sous format Excel (modifiable)
- Horodatage non fiable (timestamp serveur modifiable)

→ Preuve **IRRECEVABLE**

---

## 3️⃣ HASH CRYPTOGRAPHIQUE (SHA-256)

### Principe du Hash

**Définition :**
> Fonction mathématique qui transforme un fichier en une empreinte numérique unique de longueur fixe.

**Analogie :** Le hash = empreinte digitale du fichier.

**Propriétés :**
- **Déterministe** : Même fichier = même hash
- **Unique** : 2 fichiers différents = 2 hash différents (collision quasi impossible)
- **Irréversible** : Impossible retrouver fichier depuis hash
- **Sensible** : Modification 1 bit → hash complètement différent

---

### Exemple Pratique

```
Fichier original : /var/log/auth.log (15 Mo)
Hash SHA-256 : 8f3a2b1c9d4e5f6a7b8c9d0e1f2a3b4c5d6e7f8a9b0c1d2e3f4a5b6c7d8e9f0a

Modification : 1 caractère changé dans le fichier
Nouveau hash : 2a1b3c4d5e6f7a8b9c0d1e2f3a4b5c6d7e8f9a0b1c2d3e4f5a6b7c8d9e0f1a2b

→ Hash complètement différent
```

**Usage juridique :**
1. Calculer hash du log au moment de la collecte
2. Stocker hash séparément (base de données, TSA)
3. Lors du procès : recalculer hash du log présenté
4. Comparer : hash identique = fichier non modifié ✅

---

### Commandes Pratiques

**Linux :**
```bash
sha256sum /var/log/auth.log > auth.log.sha256
# Vérification ultérieure
sha256sum -c auth.log.sha256
```

**Windows (PowerShell) :**
```powershell
Get-FileHash C:\Logs\security.log -Algorithm SHA256
```

---

## 4️⃣ SIGNATURE ÉLECTRONIQUE (RÈGLEMENT eIDAS)

### Règlement eIDAS (UE 910/2014)

**Définition officielle (Art. 3) :**
> *"Signature électronique : données sous forme électronique, jointes ou associées à d'autres données électroniques et utilisées par le signataire pour signer."*

---

### Les 3 Niveaux de Signature

```
┌────────────────────────────────────────────────┐
│ SIGNATURE SIMPLE (Art. 25)                     │
├────────────────────────────────────────────────┤
│ Exemples :                                     │
│ • Scan de signature manuscrite                 │
│ • Email (champ "From:")                        │
│ • Case "J'accepte" cochée                     │
│ • SMS de confirmation                          │
│                                                │
│ Valeur juridique :                             │
│ • Faible force probante                       │
│ • Facilement contestable                       │
│ • OK pour actes de faible valeur (< 1 500€)   │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ SIGNATURE AVANCÉE (Art. 26)                    │
├────────────────────────────────────────────────┤
│ Caractéristiques obligatoires :                │
│ • Liée UNIQUEMENT au signataire               │
│ • Permet IDENTIFICATION du signataire          │
│ • Créée par moyens sous contrôle signataire    │
│ • Permet DÉTECTION de toute modification       │
│                                                │
│ Moyens techniques :                            │
│ • Certificat électronique (non qualifié)       │
│ • Clé privée sur ordinateur                    │
│ • DocuSign, Adobe Sign (mode avancé)           │
│                                                │
│ Valeur juridique :                             │
│ • Bonne force probante                         │
│ • Acceptable pour actes moyens (< 50 000€)     │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ SIGNATURE QUALIFIÉE (Art. 28)                  │
├────────────────────────────────────────────────┤
│ Exigences supplémentaires :                    │
│ • Certificat délivré par Autorité de confiance │
│   (PSCo = Prestataire Services Confiance)      │
│ • Dispositif sécurisé (carte à puce, clé USB)  │
│ • Vérification identité physique signataire    │
│                                                │
│ Autorités françaises :                         │
│ • ChamberSign (Chambres de Commerce)           │
│ • Certigna (Dhimyotis)                         │
│ • DocuSign (mode qualifié)                     │
│                                                │
│ Valeur juridique :                             │
│ • ÉQUIVALENT signature manuscrite (Art. 27)    │
│ • Force probante MAXIMALE                      │
│ • Obligatoire pour actes > 1 500€ notariés     │
│ • Recommandé pour actes > 50 000€              │
└────────────────────────────────────────────────┘
```

---

### Tableau Comparatif

| Critère | Simple | Avancée | Qualifiée |
|---------|--------|---------|-----------|
| **Exemple** | Email, checkbox | Certificat non qualifié | Certificat PSCo |
| **Valeur juridique** | Faible | Moyenne | Maximale |
| **Équivalence manuscrite** | ❌ Non | ❌ Non | ✅ Oui (Art. 27) |
| **Coût** | Gratuit | 0-50€ | 50-200€/an |
| **Usage recommandé** | < 1 500€ | 1 500-50 000€ | > 50 000€ |

---

## 5️⃣ HORODATAGE QUALIFIÉ (RFC 3161)

### Définition

**Horodatage électronique qualifié (Art. 41 eIDAS) :**
> Preuve qu'une donnée existait à un instant précis, délivrée par une autorité de confiance (TSA).

**Analogie :** Horodatage = huissier numérique qui certifie la date.

---

### RFC 3161 (Internet Timestamp Protocol)

**Standard technique :**
- **TSA** (Time Stamping Authority) = Autorité d'horodatage
- Processus :
  1. Client calcule hash du document
  2. Client envoie hash à la TSA
  3. TSA appose timestamp + signe avec son certificat
  4. TSA retourne jeton d'horodatage (.tsr)

**Garanties :**
- Date/heure certifiées par TSA (source temps fiable)
- Hash du document inclus (intégrité)
- Signature TSA (authenticité)

---

### Horodatage Simple vs Qualifié

```
┌────────────────────────────────────────────────┐
│ HORODATAGE SIMPLE (timestamp serveur)          │
├────────────────────────────────────────────────┤
│ • Horloge locale serveur                       │
│ • Modifiable (admin peut changer date)         │
│ • Pas de tiers de confiance                    │
│                                                │
│ Valeur juridique : FAIBLE                      │
│ → Facilement contestable                       │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ HORODATAGE QUALIFIÉ (RFC 3161 + eIDAS)        │
├────────────────────────────────────────────────┤
│ • TSA certifiée (ChamberSign, Universign)      │
│ • Source temps légale (observatoire)           │
│ • Signature numérique TSA                      │
│ • Non modifiable                               │
│                                                │
│ Valeur juridique : MAXIMALE (Art. 41 eIDAS)    │
│ → Présomption légale de date                   │
└────────────────────────────────────────────────┘
```

---

### TSA Françaises Qualifiées

| TSA | Éditeur | Usage |
|-----|---------|-------|
| **ChamberSign** | Chambres de Commerce | Entreprises, PME |
| **Universign** | Cryptolog | Banques, assurances |
| **DocuSign** | DocuSign Inc. | International |
| **Certinomis** | La Poste | Collectivités, administrations |

---

## 6️⃣ MISE EN ŒUVRE TECHNIQUE

### Sécuriser les Logs (Checklist)

```
☐ 1. JOURNALISATION CENTRALISÉE
   → Serveur syslog distant (rsyslog, Graylog)
   → Logs inaccessibles localement

☐ 2. HASH AUTOMATIQUE
   → Calcul SHA-256 à la rotation logs
   → Stockage hash en base sécurisée

☐ 3. HORODATAGE FIABLE
   → Synchronisation NTP (pool.ntp.org)
   → Horodatage qualifié si critique (TSA)

☐ 4. STOCKAGE IMMUABLE
   → Append-only (pas de modification)
   → WORM (Write Once Read Many)
   → OU Blockchain (si besoin extrême)

☐ 5. CONSERVATION LÉGALE
   → Durée légale respectée (6 mois à 10 ans)
   → Accès restreint (chiffrement)
   → Procédure export pour justice

☐ 6. DOCUMENTATION
   → Politique de logs écrite
   → Procédure de collecte
   → Chaîne de traçabilité
```

---

### Exemple Procédure Signature Électronique

**Workflow signature qualifiée d'un contrat :**

```
1. PRÉPARATION
   ├─ Rédaction contrat (PDF)
   ├─ Upload sur plateforme PSCo (DocuSign, ChamberSign)
   └─ Identification signataires

2. ENVOI
   ├─ Notification signataires (email)
   ├─ Accès sécurisé (lien unique + OTP)
   └─ Lecture contrat

3. SIGNATURE
   ├─ Authentification forte (SMS, carte)
   ├─ Validation signature
   └─ Certificat qualifié appliqué

4. ARCHIVAGE
   ├─ Document signé + certificats
   ├─ Horodatage qualifié (TSA)
   ├─ Hash SHA-256
   └─ Archivage électronique (10 ans)
```

---

## 📝 Points Clés à Retenir

### Pour l'Examen

**À connaître PAR CŒUR :**

```
┌────────────────────────────────────────────────┐
│ • Article 1366 : 2 conditions                  │
│   1. Identification                            │
│   2. Intégrité                                 │
│                                                │
│ • 3 niveaux signature (eIDAS) :                │
│   Simple < Avancée < Qualifiée                │
│                                                │
│ • Signature qualifiée = Manuscrite            │
│   (Art. 27 eIDAS)                              │
│                                                │
│ • Hash SHA-256 = Preuve intégrité             │
│                                                │
│ • Horodatage qualifié = RFC 3161 + TSA        │
│   → Présomption légale de date                │
│                                                │
│ • Logs recevables SI :                         │
│   Intégrité + Horodatage + Conservation        │
└────────────────────────────────────────────────┘
```

---

### Pour la Vie Professionnelle

**Réflexe du technicien SISR :**

✅ **Logs = Preuves juridiques potentielles**
- Centraliser (serveur syslog)
- Hash automatique (SHA-256)
- Horodatage fiable (NTP minimum)
- Conservation sécurisée (durée légale)

✅ **Signature électronique = Selon enjeux**
- < 1 500€ : Simple (email) acceptable
- 1 500-50 000€ : Avancée recommandée
- > 50 000€ : Qualifiée obligatoire

✅ **Horodatage qualifié = Si critique**
- Contentieux prévisible
- Montants élevés
- Propriété intellectuelle (dépôt, antériorité)

---

## 🎯 Auto-Évaluation

### Je sais...

- ☐ Expliquer Article 1366 (2 conditions)
- ☐ Lister conditions recevabilité logs
- ☐ Distinguer 3 niveaux signature électronique
- ☐ Expliquer équivalence qualifiée = manuscrite
- ☐ Calculer hash SHA-256 d'un fichier
- ☐ Expliquer RFC 3161 et rôle TSA
- ☐ Configurer logs sécurisés (append-only)
- ☐ Citer 2 TSA françaises qualifiées
- ☐ Conseiller niveau signature selon montant

**Si < 7 cases cochées, revoir la fiche cours.**


---
