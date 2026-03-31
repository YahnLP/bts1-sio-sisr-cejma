---
author: YLP
title: 📚 FICHE DE COURS
---

# 📚 FICHE DE COURS ÉLÈVE
## RGPD (3) : Droits des Personnes et Mise en Œuvre Technique

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 8*

---

## 🎯 Objectifs de Cette Fiche

À la fin de ce cours, vous serez capable de :
- ✅ Lister les 8 droits des personnes selon le RGPD
- ✅ Expliquer les droits d'accès, d'effacement et de portabilité
- ✅ Répondre techniquement à une demande d'exercice de droit (SQL, export, suppression)
- ✅ Distinguer anonymisation, pseudonymisation, suppression, archivage
- ✅ Respecter les délais, la gratuité, les exceptions

---

## 📖 PARTIE I — Les 8 Droits des Personnes (Vue d'Ensemble)

### I.A. Principes Généraux

Le RGPD confère aux **personnes concernées** (les individus dont les données sont traitées) **8 droits fondamentaux** pour **maîtriser leurs données personnelles**.

Ces droits s'exercent **gratuitement** (sauf abus) et le responsable de traitement doit y répondre sous **1 mois** (extensible à 3 mois si complexité).

### I.B. Tableau des 8 Droits

| **Droit** | **Article** | **Description Courte** | **Exemple** |
|---|:---:|---|---|
| **1. Droit d'information** | Art. 13-14 | Être informé de la collecte et du traitement | Politique de confidentialité |
| **2. Droit d'accès** | Art. 15 | Obtenir une copie de ses données | Export de l'historique de commandes |
| **3. Droit de rectification** | Art. 16 | Corriger des données inexactes | Modifier son adresse postale |
| **4. Droit à l'effacement** | Art. 17 | Demander la suppression de ses données | Supprimer son compte |
| **5. Droit à la limitation** | Art. 18 | Geler temporairement le traitement | "Ne plus utiliser mes données le temps de vérifier leur exactitude" |
| **6. Droit à la portabilité** | Art. 20 | Récupérer ses données dans un format structuré | Télécharger ses données Facebook en JSON |
| **7. Droit d'opposition** | Art. 21 | S'opposer à un traitement | Se désabonner des newsletters |
| **8. Décision automatisée** | Art. 22 | Ne pas subir une décision uniquement automatisée | Refus de crédit par algorithme → demande d'examen humain |

> 📌 **Focus de cette séance :** Les droits **2 (accès)**, **4 (effacement)** et **6 (portabilité)** qui nécessitent des **compétences techniques** pour être mis en œuvre.

---

## 📖 PARTIE II — Le Droit d'Accès (Article 15)

### II.A. Définition

Le droit d'accès permet à toute personne de demander au responsable de traitement :
- ✅ **Si** ses données sont traitées
- ✅ **Quelles** données sont traitées
- ✅ **Pourquoi** (finalités du traitement)
- ✅ **Combien de temps** elles seront conservées
- ✅ **Qui** y a accès (destinataires)
- ✅ **D'où** viennent les données (si collecte indirecte)

### II.B. Contenu de la Réponse

Le RT doit fournir **une copie** des données personnelles traitées. Cette copie peut être :
- Format **PDF** (pour les particuliers, lisible par humain)
- Format **CSV / JSON / XML** (pour portabilité, si demandé)
- Format **papier** (si demande par courrier)

**Contenu minimal :**
- Identité (nom, prénom, email, adresse...)
- Historique des actions (commandes, connexions, avis...)
- Données générées (logs, préférences, consentements...)

### II.C. Mise en Œuvre Technique

**Étapes pour répondre à une demande d'accès :**

#### Étape 1 : Vérifier l'Identité

⚠️ **SÉCURITÉ CRITIQUE** : Avant de communiquer des données, vérifier que le demandeur est bien la personne concernée.

**Méthodes de vérification :**
- Envoi d'un code de confirmation par email (si email vérifié)
- Demande de copie de pièce d'identité
- Questions de sécurité (date de naissance, dernière commande...)
- Double authentification (2FA)

#### Étape 2 : Extraire les Données (SQL)

**Exemple de requête SQL :**

```sql
-- Extraire les données utilisateur
SELECT * FROM users WHERE email = 'john.doe@example.com';

-- Extraire l'historique des commandes
SELECT * FROM orders WHERE user_id = 123;

-- Extraire les avis laissés
SELECT * FROM reviews WHERE user_id = 123;

-- Extraire les logs de connexion (3 derniers mois)
SELECT * FROM access_logs 
WHERE user_id = 123 
AND timestamp >= DATE_SUB(NOW(), INTERVAL 3 MONTH);
```

#### Étape 3 : Anonymiser les Données Tierces

Si les données extraites contiennent des **informations sur d'autres personnes**, il faut les anonymiser.

**Exemple :** Un avis produit mentionne le nom d'un autre utilisateur dans les commentaires → remplacer par "Utilisateur anonymisé".

#### Étape 4 : Exporter dans un Format Structuré

**Export CSV :**

```csv
id,email,name,phone,address,created_at
123,john.doe@example.com,John Doe,0612345678,12 rue de Paris,2022-01-15
```

**Export JSON :**

```json
{
  "user": {
    "id": 123,
    "email": "john.doe@example.com",
    "name": "John Doe",
    "phone": "0612345678",
    "address": "12 rue de Paris",
    "created_at": "2022-01-15"
  },
  "orders": [
    {
      "id": 456,
      "product": "Laptop HP",
      "amount": 799.99,
      "order_date": "2023-05-20"
    }
  ],
  "reviews": [...]
}
```

#### Étape 5 : Envoyer la Réponse

- Email avec pièce jointe sécurisée (zip chiffré, mot de passe communiqué séparément)
- Lien de téléchargement temporaire (24-48h) avec authentification
- Courrier postal si demande papier

### II.D. Délais et Exceptions

**Délai :** 1 mois à compter de la réception de la demande (art. 12-3)  
**Extension possible :** +2 mois si complexité (mais informer sous 1 mois)  
**Gratuité :** 1ère demande gratuite, demandes abusives peuvent être facturées

**Exceptions :** Le droit d'accès peut être **limité** si :
- Secret des affaires
- Sécurité publique, défense nationale
- Procédure judiciaire en cours
- Atteinte aux droits d'autrui

---

![Schéma du processus droit d'accès : 1. Demande reçue, 2. Vérification identité, 3. Extraction BDD (SQL), 4. Export CSV/JSON, 5. Envoi sécurisé sous 1 mois]

*Légende : Processus de traitement d'une demande de droit d'accès*

---

## 📖 PARTIE III — Le Droit à l'Effacement (Article 17)

### III.A. Définition

Le droit à l'effacement (ou **"droit à l'oubli"**) permet à une personne de demander la **suppression** de ses données personnelles.

> ⚠️ **Attention :** Ce droit n'est **PAS absolu**. Il existe de nombreuses exceptions.

### III.B. Motifs d'Effacement

La personne peut demander l'effacement si :
- Les données ne sont **plus nécessaires** au regard des finalités initiales
- Elle **retire son consentement** (et aucune autre base légale)
- Elle s'**oppose** au traitement (et pas de motif légitime impérieux)
- Les données ont été traitées **illégalement**
- Obligation légale de suppression (ex : CNIL ordonne)
- Données collectées sur un **mineur** dans le cadre de services en ligne

### III.C. Exceptions — Quand le RT Peut Refuser

Le RT peut **refuser** l'effacement si :
- ✅ **Obligation légale de conservation** (ex : facturation = 10 ans, comptabilité, archives fiscales)
- ✅ **Intérêt public** (santé publique, archives historiques...)
- ✅ **Exercice du droit à la liberté d'expression** (journalisme, recherche...)
- ✅ **Constatation, exercice ou défense de droits en justice** (litige en cours)
- ✅ **Intérêt public en matière de santé** (épidémiologie, alertes sanitaires...)

### III.D. Mise en Œuvre Technique — Suppression vs Anonymisation

Le RT a **3 options** selon le contexte :

#### Option 1 : Suppression Physique (DELETE)

**Quand ?** Données vraiment inutiles, aucune obligation de conservation.

```sql
-- Supprimer l'utilisateur et toutes ses données liées (attention aux contraintes)
DELETE FROM reviews WHERE user_id = 123;
DELETE FROM orders WHERE user_id = 123;
DELETE FROM access_logs WHERE user_id = 123;
DELETE FROM users WHERE id = 123;
```

⚠️ **Attention :**
- Vérifier les **contraintes de clés étrangères** (ON DELETE CASCADE ou SET NULL)
- Penser aux **sauvegardes** (doivent aussi être purgées ou anonymisées)
- **Tracer l'action** dans un log RGPD (preuve de suppression)

#### Option 2 : Anonymisation (UPDATE)

**Quand ?** Obligation de conserver certaines données (ex : commandes pour comptabilité), mais pas besoin d'identifier la personne.

```sql
-- Anonymiser l'utilisateur (remplacer données identifiantes par des valeurs génériques)
UPDATE users 
SET 
    name = 'Utilisateur supprimé',
    email = NULL,
    phone = NULL,
    address = NULL,
    password_hash = NULL,
    deleted_at = NOW()
WHERE id = 123;
```

**Résultat :** Les commandes existent toujours (pour la compta), mais impossible d'identifier la personne.

#### Option 3 : Pseudonymisation (HASH)

**Quand ?** Besoin de conserver des statistiques, mais anonymiser l'identité.

```sql
-- Remplacer les identifiants par des hash
UPDATE users 
SET 
    email = SHA256(email),
    name = SHA256(name)
WHERE id = 123;
```

### III.E. Cas Particulier : Les Avis et Commentaires Publics

**Problème :** Un utilisateur demande l'effacement, mais il a laissé 50 avis produits sur le site. Faut-il supprimer les avis ?

**Réponse :**
- Si avis **identifiants** (nom complet, photo) → **anonymiser** ("Utilisateur anonyme")
- Si avis **anonymes** (pseudo, pas de photo) → **conserver** (liberté d'expression, intérêt public)
- Si avis **illicites** (diffamation, haine) → **supprimer** (obligation légale)

### III.F. Notification aux Tiers

Si les données ont été **transmises à des tiers** (sous-traitants, partenaires), le RT doit les **informer** de la demande d'effacement (art. 19).

**Exemple :** ShopOnline a transmis les données à Google Analytics → informer Google de supprimer aussi.

---

![Schéma des 3 options d'effacement : Suppression physique (DELETE, données vraiment inutiles), Anonymisation (UPDATE, obligation conservation mais anonymat OK), Pseudonymisation (HASH, stats anonymisées)]

*Légende : Les 3 techniques d'effacement selon le contexte*

---

## 📖 PARTIE IV — Le Droit à la Portabilité (Article 20)

### IV.A. Définition

Le droit à la portabilité permet à une personne de **récupérer ses données** dans un **format structuré, couramment utilisé et lisible par machine** pour :
- Les conserver
- Les transférer à un autre RT

> 💡 **Objectif :** Faciliter le changement de fournisseur (interopérabilité).

### IV.B. Conditions d'Application

Le droit à la portabilité s'applique **SEULEMENT** si :
- ✅ Le traitement est fondé sur le **consentement** ou un **contrat**
- ✅ Le traitement est **automatisé** (pas de traitement manuel)

**Données concernées :**
- ✅ Données **fournies par la personne** (nom, email, adresse...)
- ✅ Données **générées par son activité** (historique de navigation, likes, playlists...)
- ❌ Données **inférées/dérivées** (score de crédit, profil publicitaire...) → **NON portables**

### IV.C. Formats d'Export

**Formats couramment utilisés :**
- **CSV** : Simple, universel, lisible par Excel
- **JSON** : Structuré, utilisé par les API
- **XML** : Structuré, ancien standard
- **PDF** : Lisible par humain (mais pas idéal pour portabilité machine)

**Exemple JSON (export Spotify) :**

```json
{
  "user": {
    "username": "john_doe",
    "email": "john.doe@example.com",
    "created_at": "2018-05-12"
  },
  "playlists": [
    {
      "name": "My Favorite Songs",
      "songs": [
        {"title": "Song 1", "artist": "Artist A", "duration": 210},
        {"title": "Song 2", "artist": "Artist B", "duration": 180}
      ]
    }
  ],
  "listening_history": [...]
}
```

### IV.D. Mise en Œuvre Technique

#### Étape 1 : Identifier les Données Portables

**Requête SQL (exemple) :**

```sql
-- Données fournies par l'utilisateur
SELECT id, email, name, phone, address, birthdate 
FROM users 
WHERE id = 123;

-- Données générées par l'activité
SELECT product_name, amount, order_date 
FROM orders 
WHERE user_id = 123;

SELECT product_id, rating, comment, review_date 
FROM reviews 
WHERE user_id = 123;
```

#### Étape 2 : Exporter en Format Structuré

**Script Python (exemple) :**

```python
import json
import mysql.connector

# Connexion BDD
conn = mysql.connector.connect(host="localhost", user="root", password="", database="shoponline")
cursor = conn.cursor(dictionary=True)

# Extraction données utilisateur
cursor.execute("SELECT * FROM users WHERE id = 123")
user_data = cursor.fetchone()

# Extraction commandes
cursor.execute("SELECT * FROM orders WHERE user_id = 123")
orders_data = cursor.fetchall()

# Création du JSON
export = {
    "user": user_data,
    "orders": orders_data
}

# Export JSON
with open("user_123_export.json", "w") as f:
    json.dump(export, f, indent=2, default=str)

print("Export terminé : user_123_export.json")
```

#### Étape 3 : Envoyer l'Export

- Email avec pièce jointe
- Lien de téléchargement sécurisé (temporaire, authentifié)
- API directe (si transmission à un autre RT)

### IV.E. Différence avec le Droit d'Accès

| **Critère** | **Droit d'Accès (Art. 15)** | **Droit à la Portabilité (Art. 20)** |
|---|---|---|
| **Objectif** | Consulter, vérifier | Transférer, changer de fournisseur |
| **Format** | Tout format (PDF OK) | Format structuré, lisible machine (CSV, JSON) |
| **Données** | **Toutes** les données | **Uniquement** fournies/générées, pas inférées |
| **Base légale** | Toujours applicable | Seulement si consentement ou contrat |

---

## 📖 PARTIE V — Les Autres Droits (Aperçu)

### V.A. Droit de Rectification (Article 16)

**Définition :** Corriger des données **inexactes** ou **incomplètes**.

**Mise en œuvre :**

```sql
-- Corriger l'adresse email
UPDATE users SET email = 'new.email@example.com' WHERE id = 123;

-- Corriger l'adresse postale
UPDATE users SET address = '24 rue Victor Hugo, Lyon' WHERE id = 123;
```

**Délai :** 1 mois

---

### V.B. Droit à la Limitation (Article 18)

**Définition :** **Geler** temporairement le traitement (ne plus utiliser les données, mais les conserver).

**Cas d'usage :**
- Contestation de l'exactitude des données (temps de vérifier)
- Traitement illicite, mais la personne préfère limiter plutôt qu'effacer
- Données nécessaires pour défendre des droits en justice

**Mise en œuvre :**

```sql
-- Marquer le compte comme "gelé"
UPDATE users SET status = 'frozen', frozen_at = NOW() WHERE id = 123;

-- Interdire l'envoi d'emails, l'analyse des données...
```

---

### V.C. Droit d'Opposition (Article 21)

**Définition :** S'opposer à un traitement pour des **raisons tenant à sa situation particulière**.

**Cas d'usage :**
- Opposition au **marketing direct** (newsletters, pub ciblée)
- Opposition au **profilage**

**Mise en œuvre :**

```sql
-- Désabonner des newsletters
UPDATE users SET marketing_consent = FALSE WHERE id = 123;

-- Supprimer du CRM marketing
DELETE FROM marketing_list WHERE user_id = 123;
```

**Différence avec l'effacement :** On ne supprime pas le compte, juste on arrête un traitement spécifique.

---

### V.D. Droit de Notification (Article 19)

**Définition :** Lorsque le RT rectifie, efface ou limite des données, il doit **notifier les destinataires** (sous-traitants, partenaires) sauf si impossible ou disproportionné.

**Exemple :** ShopOnline a transmis les données à Google Analytics → informer Google de la rectification/effacement.

---

### V.E. Droit de Ne Pas Faire l'Objet d'une Décision Automatisée (Article 22)

**Définition :** Ne pas subir une décision **uniquement automatisée** (sans intervention humaine) produisant des **effets juridiques** ou **affectant de manière significative**.

**Exemples :**
- Refus de crédit bancaire par algorithme
- Licenciement décidé par IA
- Refus d'admission universitaire par algorithme

**Droit :** Demander un **examen humain** de la décision.

---

## 📖 PARTIE VI — Procédure Générale de Traitement des Demandes

### VI.A. Étapes Communes à Tous les Droits

```
1. RÉCEPTION de la demande (email, courrier, formulaire web)
   ↓
2. IDENTIFICATION du demandeur (vérifier identité)
   ↓
3. VÉRIFICATION de la légitimité (droit applicable ? exceptions ?)
   ↓
4. TRAITEMENT technique (extraction, suppression, rectification...)
   ↓
5. TRAÇABILITÉ (log de l'action RGPD)
   ↓
6. RÉPONSE à la personne (sous 1 mois, avec confirmation)
```

### VI.B. Outils de Traçabilité

**Table SQL pour tracer les demandes RGPD :**

```sql
CREATE TABLE rgpd_requests (
    id INT PRIMARY KEY AUTO_INCREMENT,
    user_id INT,
    request_type ENUM('access', 'rectification', 'erasure', 'portability', 'opposition', 'limitation'),
    request_date DATETIME,
    identity_verified BOOLEAN,
    processed_by VARCHAR(255), -- Nom du technicien
    processed_date DATETIME,
    status ENUM('pending', 'completed', 'rejected', 'in_progress'),
    response_sent_date DATETIME,
    notes TEXT,
    FOREIGN KEY (user_id) REFERENCES users(id)
);
```

**Pourquoi tracer ?**
- Prouver la conformité en cas de contrôle CNIL
- Suivre les délais de traitement
- Identifier les demandes répétitives/abusives

---

## 🔑 VOCABULAIRE CLÉ À MAÎTRISER (pour l'examen)

| **Terme** | **Définition Simple** |
|---|---|
| **Droit d'accès** | Obtenir une copie de ses données personnelles |
| **Droit à l'effacement** | Demander la suppression de ses données (droit à l'oubli) |
| **Droit à la portabilité** | Récupérer ses données dans un format structuré pour les transférer |
| **Droit de rectification** | Corriger des données inexactes ou incomplètes |
| **Droit d'opposition** | Refuser un traitement (ex : marketing, profilage) |
| **Droit à la limitation** | Geler temporairement le traitement (ne plus utiliser, mais conserver) |
| **Anonymisation** | Rendre impossible l'identification (irréversible) |
| **Pseudonymisation** | Remplacer les identifiants directs par des pseudos/hash (réversible) |
| **Suppression physique** | DELETE en BDD (effacement total) |
| **Format structuré** | CSV, JSON, XML (lisible par machine) |
| **Délai RGPD** | 1 mois (extensible à 3 mois si complexité) |

---

## ✅ Points Clés à Retenir

1. **Le RGPD confère 8 droits fondamentaux** aux personnes : information, accès, rectification, effacement, limitation, portabilité, opposition, décision automatisée.

2. **Les droits les plus techniques** (nécessitant des compétences SISR) sont : accès, effacement, portabilité.

3. **Droit d'accès** → Extraction SQL + export CSV/JSON/PDF.

4. **Droit à l'effacement** → 3 options selon contexte : suppression physique (DELETE), anonymisation (UPDATE), pseudonymisation (HASH).

5. **Droit à la portabilité** → Export format structuré (CSV, JSON) des données fournies/générées uniquement (pas les données inférées).

6. **Délai de réponse : 1 mois** (extensible à 3 mois). Gratuité (sauf abus). Vérifier l'identité avant de communiquer.

7. **En tant que technicien SISR, vous serez directement impliqué** dans le traitement technique de ces demandes : extraction BDD, scripts, exports, suppressions, traçabilité.

---

## 📚 Pour Aller Plus Loin

**Textes de référence :**
- [RGPD — Articles 15-22](https://www.cnil.fr/fr/reglement-europeen-protection-donnees) (droits des personnes)
- [Guide CNIL — Exercer ses droits](https://www.cnil.fr/fr/les-droits-pour-maitriser-vos-donnees-personnelles)

**Outils techniques :**
- [Mockaroo](https://www.mockaroo.com) — Générateur de données fictives pour tester
- [jq](https://stedolan.github.io/jq/) — Outil CLI pour manipuler du JSON
- [csvkit](https://csvkit.readthedocs.io) — Outils CLI pour manipuler du CSV

**Questions de réflexion :**
- Comment gérer un droit à l'effacement si la personne a des dettes impayées (obligation de conservation comptable) ?
- Faut-il anonymiser ou supprimer les avis produits quand un utilisateur demande l'effacement ?
- Comment automatiser le traitement des demandes RGPD dans une entreprise de 100 000 clients ?

---
