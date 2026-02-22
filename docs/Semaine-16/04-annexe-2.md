---
author: YLP
title: 📄 ANNEXE 2
---

# 📄 ANNEXE 2 — CHEAT SHEET GIT (COMMANDES DE BASE)

```
═══════════════════════════════════════════════════════════════
                    GIT CHEAT SHEET — BASES
═══════════════════════════════════════════════════════════════

INITIALISATION
──────────────────────────────────────────────────────────────
git init                    # Créer un nouveau dépôt Git
git config --global user.name "Nom"     # Configurer nom
git config --global user.email "email"  # Configurer email


COMMANDES ESSENTIELLES
──────────────────────────────────────────────────────────────
git status                  # Voir l'état des fichiers
git add fichier.txt         # Ajouter un fichier au suivi
git add .                   # Ajouter tous les fichiers modifiés
git commit -m "Message"     # Enregistrer une version
git log                     # Voir l'historique des commits
git log --oneline           # Historique compact


VOIR LES MODIFICATIONS
──────────────────────────────────────────────────────────────
git diff                    # Voir les modifications non ajoutées
git diff fichier.txt        # Voir modifs d'un fichier précis
git show <commit-id>        # Voir le contenu d'un commit


ANNULER DES MODIFICATIONS
──────────────────────────────────────────────────────────────
git checkout fichier.txt    # Annuler les modifs d'un fichier
git reset HEAD fichier.txt  # Retirer un fichier du staging
git revert <commit-id>      # Annuler un commit (crée un nouveau)


WORKFLOW TYPIQUE
──────────────────────────────────────────────────────────────
1. Modifier des fichiers
2. git status               # Voir ce qui a changé
3. git add .                # Ajouter les modifications
4. git commit -m "..."      # Enregistrer la version
5. git log                  # Vérifier que le commit est là

═══════════════════════════════════════════════════════════════
```
