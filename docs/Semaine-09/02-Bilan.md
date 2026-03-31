---
author: YLP
title: 📌 FICHE BILAN & MÉMO
---

# 📌 FICHE BILAN & MÉMO
## Article 32 RGPD : L'Essentiel Sécurité des Données

---

## 🎯 Synthèse de la Séance

| **Élément** | **Détail** |
|-------------|-----------|
| **Thème** | Article 32 RGPD : Obligation légale de sécurité |
| **Durée** | 4 heures |
| **Approche** | Juridique + Technique (TP chiffrement + RBAC) |
| **Compétences** | B1.4, B2.2, B3.4 |

---

## ✅ Objectifs Atteints

- ✅ Maîtriser le **texte Article 32** et ses 4 mesures
- ✅ Comprendre **CIA + Résilience**
- ✅ Mettre en œuvre **chiffrement** (BitLocker/VeraCrypt)
- ✅ Configurer **RBAC** dans Active Directory
- ✅ Connaître **sanctions** (10 M€ ou 2% CA)
- ✅ Analyser **conformité** d'une infrastructure

---

## 🔑 L'Article 32 en 1 Minute

```
╔════════════════════════════════════════════════════╗
║         ARTICLE 32 RGPD - L'ESSENTIEL              ║
╠════════════════════════════════════════════════════╣
║                                                    ║
║  TITRE : Sécurité du traitement                   ║
║                                                    ║
║  PRINCIPE :                                        ║
║  Garantir un NIVEAU DE SÉCURITÉ                   ║
║  ADAPTÉ AU RISQUE                                 ║
║                                                    ║
║  4 MESURES OBLIGATOIRES :                         ║
║  a) CHIFFREMENT et pseudonymisation               ║
║  b) CONFIDENTIALITÉ, INTÉGRITÉ, DISPONIBILITÉ     ║
║  c) RÉTABLIR disponibilité (sauvegardes, PCA)     ║
║  d) TESTER régulièrement les mesures              ║
║                                                    ║
║  SANCTION : 10 M€ ou 2% CA mondial                ║
║  (Article 83.4 RGPD)                              ║
║                                                    ║
╚════════════════════════════════════════════════════╝
```

---

## 📊 Les 4 Mesures en Tableau

| Mesure | Objectif | Exemples techniques | Exemples organisationnels |
|--------|----------|---------------------|---------------------------|
| **a) Chiffrement** | Protéger données au repos | BitLocker, LUKS, VeraCrypt | Politique mots de passe, gestion clés |
| **b) CIA+R** | Protéger traitement | RBAC, MFA, pare-feu, IDS | Procédures accès, formation, audit |
| **c) Restauration** | Garantir continuité | Sauvegardes 3-2-1, RAID, cluster | PCA/PRA, procédures restauration |
| **d) Tests** | Vérifier efficacité | Pentest, scan vulnérabilités | Exercices, revue logs, audits |

---

## 🎯 Le Modèle CIA + R

```
┌─────────────────────────────────────────────┐
│ C - CONFIDENTIALITÉ                         │
│     Seules personnes autorisées accèdent    │
│     → Chiffrement, RBAC, VPN, MFA           │
├─────────────────────────────────────────────┤
│ I - INTÉGRITÉ                               │
│     Données non altérées                    │
│     → Hash, signature numérique, logs       │
├─────────────────────────────────────────────┤
│ A - DISPONIBILITÉ                           │
│     Données accessibles quand nécessaire    │
│     → Sauvegardes, redondance, monitoring   │
├─────────────────────────────────────────────┤
│ R - RÉSILIENCE                              │
│     Capacité à résister et récupérer        │
│     → PCA/PRA, tests, documentation         │
└─────────────────────────────────────────────┘
```

---

## 🔐 Checklist Conformité Article 32

**Utilisez cette checklist pour auditer votre infrastructure :**

### Mesure a) Chiffrement

- ☐ Disques serveurs chiffrés (BitLocker/LUKS)
- ☐ Sauvegardes chiffrées
- ☐ Communications chiffrées (HTTPS, VPN)
- ☐ Données sensibles chiffrées en base
- ☐ Gestion sécurisée des clés

### Mesure b) CIA + R

**Confidentialité :**
- ☐ RBAC configuré (groupes AD)
- ☐ Principe moindre privilège appliqué
- ☐ MFA activée (comptes admin minimum)
- ☐ VPN pour accès distant
- ☐ Pare-feu activé et configuré

**Intégrité :**
- ☐ Hash des fichiers critiques
- ☐ Journalisation activée
- ☐ Signature code/mises à jour

**Disponibilité :**
- ☐ Sauvegardes quotidiennes automatisées
- ☐ Règle 3-2-1 respectée
- ☐ Redondance (RAID, cluster)
- ☐ Monitoring actif

**Résilience :**
- ☐ PCA/PRA documenté
- ☐ RTO et RPO définis
- ☐ Sites de secours (si applicable)

### Mesure c) Restauration

- ☐ Tests de restauration trimestriels
- ☐ Procédure restauration documentée
- ☐ Sauvegardes testées et validées
- ☐ Temps de restauration < RTO

### Mesure d) Tests et évaluation

- ☐ Pentest annuel
- ☐ Scan vulnérabilités mensuel
- ☐ Audit sécurité annuel
- ☐ Exercice PCA/PRA annuel
- ☐ Revue logs hebdomadaire
- ☐ Formation sécurité annuelle

---

## 📐 Schémas Récapitulatifs

### Schéma 1 : Triangle de la Sécurité RGPD

**[ILLUSTRATION À INSÉRER]**
**Légende :** Triangle équilatéral. Sommet : "Évaluation des Risques". Base gauche : "Mesures Techniques" (chiffrement, RBAC, sauvegardes). Base droite : "Mesures Organisationnelles" (procédures, formation, tests). Au centre du triangle : "Article 32 RGPD". Flèches bidirectionnelles reliant les 3 sommets.

---

### Schéma 2 : Flux de Conformité

```
1. ANALYSE DE RISQUES
   ↓
   Identifier données sensibles
   Évaluer probabilité × gravité
   ↓
2. MISE EN ŒUVRE MESURES
   ↓
   Techniques (chiffrement, RBAC...)
   + Organisationnelles (procédures, formation...)
   ↓
3. TESTS RÉGULIERS
   ↓
   Pentest, restauration, exercices
   ↓
4. AMÉLIORATION CONTINUE
   ↓
   Corriger failles détectées
   Mettre à jour procédures
   ↓
   [Retour à l'étape 1]
```

---

## 💻 Mise en Œuvre Technique

### Chiffrement en Pratique

**Chiffrer un disque Windows :**
```powershell
# Activer BitLocker
Enable-BitLocker -MountPoint "C:" -EncryptionMethod XtsAes256

# Sauvegarder clé de récupération
Backup-BitLockerKeyProtector -MountPoint "C:" -KeyProtectorId $KeyID
```

**Chiffrer un fichier avec VeraCrypt :**
1. Créer volume chiffré (AES-256)
2. Monter volume avec mot de passe
3. Copier fichiers sensibles
4. Démonter volume

**Chiffrer sauvegarde avec 7-Zip :**
```bash
7z a -p -mhe=on sauvegarde.7z dossier_a_sauvegarder/
# -p : demander mot de passe
# -mhe=on : chiffrer noms fichiers
```

---

### RBAC en Active Directory

**Étapes de mise en œuvre :**

```
1. CRÉER GROUPES PAR RÔLE
   New-ADGroup "GRP_Comptabilite" -GroupScope Global
   New-ADGroup "GRP_IT" -GroupScope Global

2. AFFECTER UTILISATEURS
   Add-ADGroupMember "GRP_Comptabilite" -Members "jdupont"

3. CONFIGURER ACL SUR DOSSIERS
   \\serveur\Compta\ 
   → GRP_Comptabilite : Lecture/Écriture
   → Autres : Aucun accès

4. APPLIQUER MOINDRE PRIVILÈGE
   Retirer droits Admin local non nécessaires
```

---

## 🚨 Sanctions et Jurisprudence

### Montants Sanctions Article 32

**Maximum légal :** 10 M€ ou 2% CA mondial (le plus élevé)

**Exemples réels :**

| Entreprise | Année | Amende | Manquement |
|------------|-------|--------|------------|
| British Airways | 2020 | 22 M€ | Défaut chiffrement + monitoring |
| Marriott | 2020 | 20 M€ | Faille système non corrigée |
| H&M | 2020 | 35 M€ | Surveillance excessive + défaut sécurité |
| EasyJet | 2020 | 0,5 M€ | Cyberattaque (mais mesures présentes) |

**Observation :** Même avec mesures, amende possible si insuffisantes. MAIS amende réduite si bonne foi démontrée.

---

### Facteurs Aggravants

- Caractère intentionnel du manquement
- Absence totale de mesures
- Récidive
- Non-coopération avec CNIL
- Données sensibles (santé, enfants)

### Facteurs Atténuants

- Mesures déjà en place (même insuffisantes)
- Coopération avec CNIL
- Notification rapide de la violation
- Mesures correctives immédiates
- Absence de précédent

---

## 📝 Auto-Évaluation Finale

### Je maîtrise...

**Connaissances juridiques :**
- ☐ Expliquer Article 32 et son obligation
- ☐ Citer les 4 mesures (a, b, c, d)
- ☐ Connaître sanction (10 M€ ou 2% CA)
- ☐ Distinguer Art. 32 (sécurité) vs Art. 33-34 (violations)

**Compétences techniques :**
- ☐ Chiffrer disque (BitLocker/LUKS)
- ☐ Chiffrer fichier (VeraCrypt/7-Zip)
- ☐ Configurer RBAC dans AD
- ☐ Appliquer principe moindre privilège
- ☐ Automatiser sauvegardes
- ☐ Tester restauration

**Posture professionnelle :**
- ☐ Analyser conformité infrastructure
- ☐ Proposer plan d'action sécurité
- ☐ Documenter mesures mises en œuvre
- ☐ Justifier choix techniques par Article 32

**Si < 10 cases cochées sur 12, revoir la fiche cours.**

---

## 🔗 Liens avec Autres Séances

| Séance | Lien avec S9 |
|--------|--------------|
| **S6 (RGPD Fondamentaux)** | Art. 32 = mise en œuvre principe 6 (sécurité) |
| **S3 (Charte)** | Charte = mesure organisationnelle Art. 32 |
| **Bloc 1 - AD** | RBAC = mesure technique Art. 32.1.b |
| **Bloc 1 - Sauvegarde** | Disponibilité = Art. 32.1.c |
| **Bloc 1 - Cybersécurité** | Toutes mesures techniques Art. 32 |

---

## 📚 Ressources Complémentaires

**Guides officiels :**
- **CNIL** : Guide sécurité des données personnelles (104 pages)
- **ANSSI** : Guide d'hygiène informatique (42 mesures)
- **ISO 27001** : Norme internationale sécurité

**Outils pratiques :**
- **BitLocker** (Windows) / **LUKS** (Linux) : Chiffrement disques
- **VeraCrypt** : Chiffrement fichiers/conteneurs
- **Veeam** / **Acronis** : Sauvegardes automatisées
- **Nessus** / **OpenVAS** : Scan vulnérabilités

**Formation continue :**
- Certification ISO 27001 Lead Implementer
- Certification CISSP (Certified Information Systems Security Professional)
- Formation ANSSI "SecNumCloud"

---

## 💡 Points Clés pour l'Examen

**À retenir PAR CŒUR :**

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
│   (Art. 83.4 - moins que Art. 83.5)           │
│                                                │
│ • CIA = Confidentialité, Intégrité,           │
│         Availability (Disponibilité)           │
│                                                │
│ • Règle 3-2-1 : 3 copies, 2 supports,         │
│                 1 hors site                    │
│                                                │
│ • RBAC = Contrôle accès par rôles             │
│                                                │
│ • Tests réguliers = OBLIGATOIRES (Art. 32.1.d)│
│                                                │
│ • British Airways : 22 M€ (2020)              │
│   Défaut chiffrement + monitoring             │
└────────────────────────────────────────────────┘
```

---

## 🎯 Message Final

**L'Article 32 = Colonne vertébrale de la sécurité RGPD**

```
Sans Article 32 :
• Pas de protection données
• Violations inévitables
• Sanctions maximales

Avec Article 32 bien appliqué :
• Protection effective données
• Conformité RGPD
• Réduction risques cyber
• Confiance clients
• Valorisation compétences
```

**En tant que technicien SISR, vous êtes l'ACTEUR principal de la mise en œuvre de l'Article 32.**

---

## 📅 Prochaines Séances

**S10 : Violations de Données (Art. 33-34 RGPD)**
- Notification CNIL (72h)
- Communication personnes concernées
- Procédure de gestion incident
- Registre des violations

**S11 : PIA (Privacy Impact Assessment)**
- Analyse d'impact protection données
- Méthode CNIL
- Cas pratiques

---

## 🔧 Aide-Mémoire Technique

### Commandes Utiles

**Windows - BitLocker :**
```powershell
# Vérifier statut BitLocker
Get-BitLockerVolume

# Chiffrer disque C:
Enable-BitLocker -MountPoint "C:" -EncryptionMethod XtsAes256

# Sauvegarder clé
Backup-BitLockerKeyProtector -MountPoint "C:" -KeyProtectorId $KeyID
```

**Linux - LUKS :**
```bash
# Chiffrer partition
cryptsetup luksFormat /dev/sdb1

# Ouvrir volume chiffré
cryptsetup open /dev/sdb1 backup_chiffre

# Créer système fichiers
mkfs.ext4 /dev/mapper/backup_chiffre
```

**Active Directory - RBAC :**
```powershell
# Créer groupe
New-ADGroup "GRP_Compta" -GroupScope Global

# Ajouter membre
Add-ADGroupMember "GRP_Compta" -Members "jdupont"

# Lister membres
Get-ADGroupMember "GRP_Compta"
```


---
