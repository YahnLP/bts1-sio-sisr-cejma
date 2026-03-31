---
author: YLP
title: 📚 FICHE DE COURS
---

# 📌 FICHE BILAN & MÉMO
## S14 — Droit de la Preuve : L'Essentiel à Retenir

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 14*

---
## 🎯 Synthèse de la Séance

| **Élément** | **Détail** |
|-------------|-----------|
| **Thème** | Valeur juridique logs, signature électronique, horodatage |
| **Durée** | 4 heures |
| **Approche** | Juridique + Technique (hash, signature, TSA) |
| **Compétences** | B1.4, B2.2, B3.1 |

---

## ✅ Objectifs Atteints

- ✅ Comprendre **Article 1366** (identification + intégrité)
- ✅ Maîtriser **conditions recevabilité logs**
- ✅ Distinguer **3 niveaux signature** (eIDAS)
- ✅ Expliquer **horodatage qualifié** (RFC 3161)
- ✅ Mettre en œuvre **hash SHA-256**
- ✅ Gérer **logs comme preuves**

---


## 🔑 Le Principe Fondamental

```
╔════════════════════════════════════════════════════╗
║     ARTICLE 1366 CODE CIVIL (PAR CŒUR)             ║
╠════════════════════════════════════════════════════╣
║                                                    ║
║  "L'écrit électronique a la MÊME FORCE PROBANTE   ║
║   que l'écrit sur support papier,                 ║
║   SOUS RÉSERVE que puisse être :                  ║
║                                                    ║
║   1. Dûment IDENTIFIÉE la personne                ║
║      dont il émane                                 ║
║                                                    ║
║   2. ÉTABLI et CONSERVÉ dans des conditions       ║
║      de nature à garantir son INTÉGRITÉ"          ║
║                                                    ║
╚════════════════════════════════════════════════════╝
```

---

## 📊 Les Logs : Conditions de Recevabilité

### Checklist Conformité

```
Pour qu'un log soit RECEVABLE comme preuve :

☑ INTÉGRITÉ PROUVÉE
  ├─ Hash SHA-256 calculé immédiatement
  ├─ Stockage immuable (append-only)
  └─ Signature numérique (optionnel mais recommandé)

☑ HORODATAGE FIABLE
  ├─ Synchronisation NTP (minimum)
  └─ Horodatage qualifié TSA (si contentieux prévisible)

☑ IDENTIFICATION
  ├─ Qui a généré le log ? (système, user)
  └─ Traçabilité (IP, login, certificat)

☑ CONSERVATION SÉCURISÉE
  ├─ Logs non modifiables localement
  ├─ Centralisation (serveur syslog distant)
  └─ Durée légale respectée (6 mois à 10 ans)

☑ DOCUMENTATION
  ├─ Politique de logs écrite
  ├─ Procédure de collecte
  └─ Chaîne de traçabilité
```

---

## 🔐 Signature Électronique : Les 3 Niveaux

```
┌────────────────────────────────────────────────┐
│         SIMPLE                                 │
│ • Email, case cochée, scan signature          │
│ • Valeur probante : FAIBLE                    │
│ • Usage : < 1 500€                             │
├────────────────────────────────────────────────┤
│         AVANCÉE                                │
│ • Certificat non qualifié                     │
│ • Détection modification                      │
│ • Valeur probante : MOYENNE                   │
│ • Usage : 1 500 - 50 000€                      │
├────────────────────────────────────────────────┤
│         QUALIFIÉE                              │
│ • Certificat PSCo (autorité confiance)        │
│ • Dispositif sécurisé (carte, clé USB)        │
│ • Valeur probante : MAXIMALE                  │
│ • = SIGNATURE MANUSCRITE (eIDAS Art. 27)      │
│ • Usage : > 50 000€, actes notariés           │
└────────────────────────────────────────────────┘
```

**[ILLUSTRATION À INSÉRER]**
**Légende :** Pyramide à 3 niveaux. Base (large) : Signature Simple. Milieu : Signature Avancée. Sommet (étroit) : Signature Qualifiée. Flèche montante annotée "Force probante croissante". Couleur vert (simple) → orange (avancée) → rouge (qualifiée).

---

## ⏰ Horodatage Qualifié (RFC 3161)

### Principe

```
HORODATAGE = Preuve qu'une donnée existait à un instant T

Horodatage SIMPLE (timestamp serveur)
├─ Modifiable (admin peut changer date)
└─ Valeur juridique : FAIBLE

Horodatage QUALIFIÉ (TSA + eIDAS)
├─ TSA certifiée (ChamberSign, Universign...)
├─ Source temps légale
├─ Signature numérique TSA
└─ Valeur juridique : MAXIMALE (présomption légale)
```

### Workflow RFC 3161

```
1. Client calcule HASH du document (SHA-256)
2. Client envoie hash à TSA
3. TSA appose TIMESTAMP + SIGNE
4. TSA retourne JETON (.tsr)
5. Archivage jeton avec document
```

---

## 🔢 Hash SHA-256 : Mode d'Emploi

### Principe

**Hash = Empreinte numérique unique**

**Propriétés :**
- Même fichier → Même hash
- Modification 1 bit → Hash complètement différent
- Irréversible (impossible retrouver fichier)

### Commandes Pratiques

**Linux :**
```bash
# Calculer hash
sha256sum /var/log/auth.log

# Stocker hash
sha256sum /var/log/auth.log > auth.log.sha256

# Vérifier intégrité ultérieure
sha256sum -c auth.log.sha256
```

**Windows (PowerShell) :**
```powershell
Get-FileHash C:\Logs\security.log -Algorithm SHA256
```

---

## ⚖️ Jurisprudence Clé

### CAS 1 : Logs RECEVABLES (2019)

**Faits :** Licenciement usage abusif Internet (sites pornographiques)
**Preuve :** Logs serveur proxy

**Décision :** ✅ LOGS RECEVABLES

**Motifs :**
- Horodatage fiable (NTP)
- Intégrité garantie (stockage centralisé)
- Identification salarié (login unique)
- Conservation sécurisée

→ Licenciement **CONFIRMÉ**

---

### CAS 2 : Logs REJETÉS (2020)

**Faits :** Administration présente logs connexion agent
**Preuve :** Fichier Excel avec recopie logs

**Décision :** ❌ LOGS IRRECEVABLES

**Motifs :**
- Pas de preuve intégrité (pas de hash)
- Format modifiable (Excel)
- Horodatage non fiable (modifiable)

→ Preuve **REJETÉE**

---

## 📐 Schéma Récapitulatif : Force Probante

```
MAXIMALE
   ↑
   │ • Log syslog + Hash SHA-256 + TSA qualifiée
   │ • Signature électronique qualifiée
   │ • Constat huissier
   │
   │ • Log syslog + Hash SHA-256
   │ • Signature avancée
   │ • Base données audit (append-only)
   │
   │ • Log fichier texte simple
   │ • Email avec signature simple
   │
   │ • Fichier Excel modifiable
   │ • Screenshot
   ↓
FAIBLE/NULLE
```

---

## 🔧 Mise en Œuvre Technique

### Sécuriser les Logs (5 Étapes)

```
ÉTAPE 1 : CENTRALISATION
├─ Serveur syslog distant (rsyslog, Graylog)
└─ Logs inaccessibles localement

ÉTAPE 2 : HASH AUTOMATIQUE
├─ Calcul SHA-256 à la rotation
└─ Stockage hash en base sécurisée

ÉTAPE 3 : HORODATAGE
├─ NTP (minimum)
└─ TSA qualifiée (si critique)

ÉTAPE 4 : STOCKAGE IMMUABLE
├─ Append-only (pas de modification)
└─ Chiffrement + Sauvegardes

ÉTAPE 5 : DOCUMENTATION
├─ Politique écrite
├─ Procédure export justice
└─ Formation équipe
```

---

### Implémenter Signature Électronique

**Plateformes conformes eIDAS :**
- **DocuSign** (signature avancée/qualifiée)
- **Adobe Sign** (signature avancée/qualifiée)
- **ChamberSign** (signature qualifiée, Chambres Commerce)
- **Universign** (signature qualifiée, banques)

**Workflow type :**
1. Upload document PDF
2. Définir signataires
3. Envoi invitations (email + OTP)
4. Signature avec certificat
5. Archivage document signé + certificats

---

## 📝 Auto-Évaluation Finale

### Je maîtrise...

**Connaissances juridiques :**
- ☐ Expliquer Article 1366 (2 conditions)
- ☐ Citer jurisprudence logs (2019, 2020)
- ☐ Définir 3 niveaux signature (eIDAS)
- ☐ Expliquer équivalence qualifiée = manuscrite

**Compétences techniques :**
- ☐ Calculer hash SHA-256 (commande)
- ☐ Expliquer RFC 3161 (workflow TSA)
- ☐ Configurer logs centralisés (rsyslog)
- ☐ Vérifier intégrité fichier (sha256sum -c)

**Posture professionnelle :**
- ☐ Reconnaître log recevable vs irrecevable
- ☐ Conseiller niveau signature selon montant
- ☐ Documenter procédure conservation logs
- ☐ Préparer export logs pour justice

**Si < 10 cases cochées sur 12, revoir la fiche cours.**

---

## 🔗 Liens avec Autres Séances

| Séance | Lien avec S14 |
|--------|---------------|
| **S9 (Article 32)** | Logs = mesure sécurité → Ici : valeur juridique |
| **S6 (RGPD)** | Conservation logs = traitement données perso |
| **Bloc 1 - Syslog** | Configuration serveur logs centralisés |
| **Bloc 1 - Cybersécurité** | Logs = détection → Preuve en cas attaque |

---

## 💡 Points Clés pour l'Examen

**À retenir PAR CŒUR :**

```
┌────────────────────────────────────────────────┐
│ • Article 1366 : Identification + Intégrité    │
│                                                │
│ • Hash SHA-256 = Preuve intégrité             │
│                                                │
│ • 3 signatures : Simple < Avancée < Qualifiée │
│                                                │
│ • Qualifiée = Manuscrite (eIDAS Art. 27)     │
│                                                │
│ • Horodatage qualifié = TSA + RFC 3161        │
│   → Présomption légale date                   │
│                                                │
│ • Logs recevables SI :                         │
│   - Hash SHA-256                               │
│   - Horodatage fiable                          │
│   - Stockage immuable                          │
│   - Conservation sécurisée                     │
│                                                │
│ • Jurisprudence 2019 : Logs OK → Licenciement │
│ • Jurisprudence 2020 : Excel KO → Preuve rejetée│
└────────────────────────────────────────────────┘
```

---

## 🎯 Message Final

**Logs = Preuves Juridiques Potentielles**

```
Mal gérés :
❌ Irrecevables en justice
❌ Contentieux perdus
❌ Licenciements annulés
❌ Responsabilité engagée

Bien gérés :
✅ Preuve décisive
✅ Licenciement validé
✅ Attaque prouvée
✅ Conformité légale
✅ Valorisation compétences SISR
```

**En tant que technicien SISR, vous générez des PREUVES quotidiennement. Votre responsabilité juridique est engagée.**

---

## 📅 Prochaine Séance

**S15 : Contrats Informatiques**
- Contrat licence (CLUF)
- Contrat maintenance (SLA)
- Contrat cloud (SaaS, IaaS)
- Responsabilités et garanties

---

## 📚 Ressources Complémentaires

**Textes officiels :**
- Code civil Article 1366
- Règlement eIDAS (UE 910/2014)
- RFC 3161 (Time-Stamp Protocol)

**Outils pratiques :**
- OpenSSL (hash, certificats)
- rsyslog (centralisation logs)
- DocuSign, Adobe Sign (signature)

**Formation :**
- ANSSI : Guide juridique logs
- CNIL : Logs et RGPD
- Certification eIDAS (PSCo)

---
