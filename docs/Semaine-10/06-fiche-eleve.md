---
author: YLP
title: 📚 FICHE DE COURS ÉLÈVE 6 
---

# 📚 FICHE DE COURS ÉLÈVE
## RGPD (4) : Contrôle & Sanctions — Pouvoirs de la CNIL et Risques Financiers

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 10 — CEJMA*

---
## 📖 PARTIE VI — Prévention et Rôle du Technicien SISR

### VI.A. Les 10 Actions Prioritaires pour Éviter une Sanction

| **Action** | **Objectif** | **Responsable** |
|---|---|---|
| **1. Désigner un DPO** (si obligatoire) | Pilote de la conformité | Direction |
| **2. Tenir un registre des traitements** | Cartographier les données | DPO + Métiers |
| **3. Informer les personnes** | Politique de confidentialité claire | DPO + Communication |
| **4. Recueillir le consentement** | Cookies, newsletters, marketing | **Technicien SISR** + Dev |
| **5. Sécuriser les données** | Chiffrement, sauvegardes, MFA | **Technicien SISR** |
| **6. Répondre aux droits** | Accès, effacement, portabilité | **Technicien SISR** + DPO |
| **7. Limiter la conservation** | Purger les données anciennes | **Technicien SISR** |
| **8. Encadrer les sous-traitants** | Contrats RGPD | Juridique + Achats |
| **9. Notifier les violations** | Sous 72h à la CNIL | **Technicien SISR** + DPO |
| **10. Former les employés** | Sensibilisation RGPD | DPO + RH |

> 💡 **Rôle clé du technicien SISR :** Actions 4, 5, 6, 7, 9 = **responsabilité technique directe**.

### VI.B. Check-list de Sécurité pour Éviter les Sanctions

**Côté Infrastructure :**
- ✅ Serveurs à jour (patchs de sécurité)
- ✅ Pare-feu activé et configuré
- ✅ Antivirus/EDR à jour
- ✅ Sauvegardes quotidiennes (testées régulièrement)
- ✅ Chiffrement des données sensibles (en transit et au repos)
- ✅ Logs d'accès activés et conservés

**Côté Accès :**
- ✅ Authentification forte (MFA)
- ✅ Mots de passe robustes (≥12 caractères, politique appliquée)
- ✅ Principe du moindre privilège (pas d'admin pour tous)
- ✅ Révocation des accès des anciens employés

**Côté Applications :**
- ✅ Bandeau cookies conforme (bouton "tout refuser" visible)
- ✅ Formulaires sans cases pré-cochées
- ✅ Procédure d'exercice des droits (formulaire ou email dédié)
- ✅ Politique de confidentialité accessible et à jour

---

### VI.C. Que Faire en Cas de Violation de Données ?

**Procédure d'urgence (Incident Response) :**

```
1. DÉTECTION (monitoring, alerte, signalement)
   ↓
2. CONFINEMENT (bloquer l'attaque, isoler les serveurs)
   ↓
3. ÉVALUATION (gravité ? données concernées ? nombre de personnes ?)
   ↓
4. NOTIFICATION CNIL (sous 72h si risque pour les droits et libertés)
   ↓
5. NOTIFICATION PERSONNES (si risque élevé)
   ↓
6. INVESTIGATION (cause racine, logs, forensic)
   ↓
7. CORRECTION (patch, changement mots de passe, renforcement sécu)
   ↓
8. DOCUMENTATION (rapport d'incident, leçons apprises)
```

**Délais critiques :**
- **72 heures** pour notifier la CNIL (à partir de la prise de connaissance)
- **Sans délai** pour notifier les personnes (si risque élevé)

**Modèle de notification CNIL :** Disponible sur [cnil.fr](https://www.cnil.fr/fr/notifier-une-violation-de-donnees-personnelles)

---

![Schéma de prévention : 3 piliers - 1. Technique (sécurité, chiffrement, sauvegardes), 2. Organisationnel (DPO, registre, procédures), 3. Juridique (consentement, information, contrats). Au centre : "Conformité RGPD".]

*Légende : Les 3 piliers de la prévention RGPD*

---