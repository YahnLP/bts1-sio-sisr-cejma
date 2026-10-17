# Conventions de rédaction du site (à relire avant toute modification)

1. **Tout changement de contenu est validé par l'enseignant** avant publication sur `main`.
2. **Gabarit d'une séance** (`docs/phase-N-nom/Sxx-nom/`) : `README.md` (fiche séance), `01-cours.md`, `02-etude-de-cas.md`, `03-aide-memoire.md`. Les corrigés sont dans `corriges/Sxx-corrige.md`, hors du dossier `docs/` (non publiés).
3. **Étude de cas :** dossier documentaire **fictif** (annoncé comme tel), questions numérotées, réponses attendues dans des blocs `<details markdown="1"><summary>Voir la réponse attendue</summary>`. Chaque corrigé contient un **barème sur 20**, une **grille de capacités A à E**, les **erreurs fréquentes** et la **vérification des calculs**.
4. **Chiffres :** tout chiffre d'un cas est recalculé avant d'être écrit. Les statistiques ne sont citées qu'avec leur source et leur année.
5. **Textes juridiques :** articles, durées et montants cités de mémoire sont signalés dans les « Notes pour l'enseignant » de la séance pour relecture sur Légifrance, EUR-Lex ou le site de la CNIL.
6. **Épreuve :** E4, écrit de 4 h, coefficient 3 (arrêté du 8 juillet 2024). Tous les examens sont traités en forme terminale.
7. **Numérotation :** séances S01 à S19, colonne « Semaine » (01 à 19) sans date : les 19 semaines d'alternance sont réparties sur l'année et ne sont pas consécutives.
8. **Titres :** pas d'emoji. Page d'accueil signée « Yahn LE PRETTRE - Formateur », sans référence à un établissement.
9. **Génération :** les pages de séances sont générées depuis un générateur extérieur au dépôt ; le glossaire se régénère par `python3 scripts/gen_glossaire.py` (produit `docs/ressources/glossaire.md` et `includes/abbr.md`).
10. **Vérification avant commit :** `mkdocs build --strict` doit passer.
