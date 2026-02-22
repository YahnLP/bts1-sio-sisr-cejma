---
author: YLP
title: 📝 DOCUMENTATION
---

# 📝 DOCUMENTATION DANS LE WIKI

*Durée : 30 minutes — Collectif*

---

## Objectif

Documenter le Projet 1 (partie S17) dans le wiki d'équipe créé en S16.

---

## Pages à Créer

### 1. Page "Projet 1 — Architecture Globale"

```wiki
====== Projet 1 — Infrastructure SimIO SARL ======

**Date de réalisation :** S17-S18 (Février 2025)
**Équipe :** [Noms des membres]

===== Architecture Générale =====

[Insérer schéma réseau]

===== Composants Déployés =====

^ Composant ^ Serveur ^ IP ^ Rôle ^
| Active Directory | SRV-DC01 | 192.168.10.20 | Contrôleur de domaine |
| GLPI | SRV-GLPI | 192.168.10.30 | Gestion parc + Helpdesk |
| OCS Inventory | SRV-GLPI | 192.168.10.30 | Inventaire automatique |
| Serveur Fichiers | SRV-FILES | 192.168.10.40 | Partages réseau |

===== Documentation Technique =====

  * [[projet_1:installation_glpi|Installation GLPI + OCS]]
  * [[projet_1:catalogue_services|Catalogue de Services]]
  * [[projet_1:incidents_resolus|Incidents Résolus]]
```

---

### 2. Page "Installation GLPI + OCS"

```wiki
====== Procédure : Installation GLPI + OCS Inventory ======

**Auteur :** [Nom]
**Date :** 2025-02-XX
**Version :** 1.0

===== Prérequis =====

  * Ubuntu Server 22.04
  * LAMP installé (Apache, MySQL, PHP 8.1+)
  * Accès sudo

===== Installation GLPI =====

==== 1. Télécharger GLPI ====

<code bash>
cd /tmp
wget https://github.com/glpi-project/glpi/releases/download/10.0.12/glpi-10.0.12.tgz
tar -xzf glpi-10.0.12.tgz
sudo mv glpi /var/www/
</code>

[Suite de la procédure...]

===== Installation OCS Inventory =====

[Procédure détaillée...]

===== Synchronisation OCS → GLPI =====

[Procédure détaillée...]
```

---

### 3. Page "Incidents Résolus"

```wiki
====== Base d'Incidents Résolus — Projet 1 ======

===== Incident #1 : Accès Serveur Refusé =====

**Date :** 2025-02-XX
**Utilisateur :** Julie Dupont (Comptabilité)
**Symptôme :** Accès refusé au dossier \\SRV-FILES\Comptabilite

**Diagnostic :**
Droits NTFS du groupe Comptabilite supprimés.

**Résolution :**
Ajout du groupe Comptabilite avec droits "Modification".

**Temps de résolution :** 15 minutes

===== Incident #2 : Application GestCom =====

[Idem pour les 2 autres incidents...]
```

