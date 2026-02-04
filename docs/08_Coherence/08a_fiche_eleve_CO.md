---
author: ELP
title: 08 📝 Fiche élève – CORRIGÉ
---

# S08 – Cohérence des résultats : valider ou écarter une donnée ?
## CORRIGÉ ENSEIGNANT

---

## Travail 1 – Vérification par les unités

### 1.1 – Identifier les erreurs

| Calcul | Formule utilisée | Unité obtenue | Attendue | Correct ? |
|--------|------------------|:-------------:|:--------:|:---------:|
| Concentration | Cm = m × V | g·L | g/L | ☒ **Non** |
| Masse volumique | ρ = V / m | mL/g | g/mL | ☒ **Non** |
| Facteur de dilution | F = Vm / Vf | sans unité | sans unité | ☒ **Non** (F = Ci/Cf ou Vf/Vi) |
| Volume à prélever | Vm = Cf × Vf / Cm | mL | mL | ☑ **Oui** |

### 1.2 – Corrections

**Calcul 1 :** Cm = m / V = 5 / 0,1 = **50 g/L**

**Calcul 2 :** ρ = m / V = 45 / 50 = **0,90 g/mL**

**Calcul 3 :** F = Cm / Cf ou F = Vf / Vm (pas Vi/Vf)
Si Vm = 10 mL et Vf = 100 mL, alors F = 100/10 = **10**

---

## Travail 2 – Ordres de grandeur

### 2.1 – Valeurs suspectes

| Mesure | Résultat | Cohérent ? | Erreur probable |
|--------|----------|:----------:|-----------------|
| pH savon | 85 | ☒ **Non** | Erreur de virgule : probablement **8,5** |
| Concentration vitamine C | 150 g/L | ☑ **Oui** | Dans l'intervalle typique |
| Densité huile | 0,0092 | ☒ **Non** | Erreur de virgule : probablement **0,92** |
| Masse volumique eau | 1000 g/mL | ☒ **Non** | Erreur d'unité : **1,00 g/mL** ou **1000 g/L** |
| Volume prélevé | 2500 mL | ☒ **Non** | Erreur de facteur 100 : probablement **25 mL** |

### 2.2 – Explications

- pH 85 : erreur de virgule (oubli du point décimal)
- Densité 0,0092 : erreur de virgule (facteur 100)
- Masse volumique 1000 : confusion d'unité (g/L au lieu de g/mL)
- Volume 2500 : erreur de conversion ou de lecture (facteur 100)

---

## Travail 3 – Analyser une série de mesures

### 3.1 – Moyenne avec toutes les valeurs

$$\bar{x} = \frac{5,8 + 5,9 + 12,4 + 5,7 + 5,8}{5} = \frac{35,6}{5} = 7,12$$

### 3.2 – Observation

1. Cette moyenne (7,12) n'est **PAS** dans [5,5 ; 6,5] → ☒ Non

2. La valeur 12,4 n'est **PAS** cohérente → ☒ Non

3. *Justification : La valeur 12,4 est très éloignée des autres mesures (5,7 à 5,9). Elle est probablement due à une erreur de manipulation (mauvais rinçage de l'électrode, mesure dans un autre produit, erreur de lecture). De plus, un pH de 12,4 serait très basique et incohérent avec une crème hydratante.*

### 3.3 – Moyenne sans la valeur aberrante

$$\bar{x}_{corrigée} = \frac{5,8 + 5,9 + 5,7 + 5,8}{4} = \frac{23,2}{4} = 5,80$$

### 3.4 – Décision

1. La moyenne corrigée (5,80) EST dans [5,5 ; 6,5] → ☑ Oui

2. Décision : ☑ **L'écarter comme valeur aberrante** (ou refaire la mesure)

3. *Justification : La valeur 12,4 est manifestement aberrante car elle s'écarte de plus de 6 unités des autres valeurs qui sont toutes comprises entre 5,7 et 5,9. Cette valeur est probablement due à une erreur de manipulation. En l'écartant, la moyenne (5,80) devient conforme au cahier des charges.*

---

## Travail 4 – Dispersion simple : min, max, étendue (sans écart-type)

### 4.1 – Moyenne

$$\bar{d} = \frac{0,912 + 0,915 + 0,910 + 0,914 + 0,911 + 0,913}{6} = \frac{5,475}{6} = 0,9125$$

### 4.2 – Extrêmes

- $d_{min}$ = **0,910**  
- $d_{max}$ = **0,915**

### 4.3 – Étendue

$$E = 0,915 - 0,910 = 0,005$$

### 4.4 – Interprétation contrôle qualité

1) Série répétable si E ≤ 0,005 ?  
☑ **Oui** (E = 0,005 → limite acceptée)

2) **Conclusion attendue (exemple 2–3 lignes) :**  
*L’étendue vaut 0,005, ce qui respecte la tolérance interne (E ≤ 0,005). Les mesures sont donc suffisamment regroupées : la série est jugée répétable. Je peux valider la mesure de densité et reporter la valeur moyenne au responsable qualité.*

### 4.5 – Bonus “présentation de résultat”

Deux réponses possibles :

- **Format min–max :**  
*d̄ = 0,9125 ; min = 0,910 ; max = 0,915 (E = 0,005).*

- **Format moyenne ± (E/2) :**  
*d̄ = 0,9125 ± 0,0025 (dispersion simple basée sur E/2).*

---

## Travail 5 – Exercice de synthèse

### 5.1 – Moyennes

- Lot A : x̄ = (118 + 122 + 119 + 121) / 4 = 480 / 4 = **120 g/L**
- Lot B : x̄ = (115 + 180 + 117 + 116) / 4 = 528 / 4 = **132 g/L**
- Lot C : x̄ = (125 + 128 + 126 + 124) / 4 = 503 / 4 = **125,75 g/L**

### 5.2 – Valeur aberrante

Le **lot B** présente une valeur aberrante : **180 g/L** (très éloignée des autres valeurs 115-117).

### 5.3 – Moyenne corrigée lot B

$$\bar{x}_{B,corrigée} = \frac{115 + 117 + 116}{3} = \frac{348}{3} = 116 \text{ g/L}$$

### 5.4 – Tableau de synthèse

| Lot | Moyenne | Valeur aberrante ? | Moyenne corrigée | Conforme ? |
|:---:|:-------:|:------------------:|:----------------:|:----------:|
| A | 120 g/L | ☐ Non | — | ☑ **Oui** |
| B | 132 g/L | ☑ **Oui (180)** | **116 g/L** | ☑ **Oui** |
| C | 125,75 g/L | ☐ Non | — | ☑ **Oui** |

### 5.5 – Recommandation pour le lot B

> *Le lot B présente une valeur aberrante de 180 g/L, nettement supérieure aux trois autres mesures (115, 117 et 116 g/L). Cette valeur est probablement due à une erreur de manipulation (erreur de dilution, confusion d'échantillon).*
>
> *Je recommande d'écarter cette mesure et de la refaire pour confirmation. En excluant la valeur aberrante, la moyenne corrigée est de 116 g/L, ce qui est conforme au cahier des charges [110 ; 130 g/L].*
>
> *Sous réserve de confirmer cette mesure, le lot B peut être validé.*

---

## Travail 6 – Approfondissement

**Question :** Pourquoi un histogramme est-il utile ?

*Un histogramme permet de visualiser la distribution des mesures et d'identifier rapidement :*

- *La valeur centrale (mode)*
- *La dispersion (largeur de la distribution)*
- *Les valeurs isolées (barres éloignées du groupe principal)*
- *La symétrie de la distribution*

*Une valeur aberrante apparaît comme une barre isolée, loin du groupe principal.*

---

## Synthèse – Exemple de réponse attendue

> *Pour vérifier la cohérence d'un résultat expérimental, on procède en plusieurs étapes. D'abord, on vérifie que l'unité du résultat est correcte (analyse dimensionnelle). Ensuite, on compare la valeur obtenue aux ordres de grandeur typiques pour détecter une erreur grossière. Si plusieurs mesures sont disponibles, on calcule la moyenne et l'écart-type pour évaluer la reproductibilité. Une valeur aberrante s'écarte significativement des autres (plus de 2-3 écarts-types). Si une valeur est incohérente, on peut la rejeter ou refaire la mesure avant de valider le résultat final.*

---

## 📊 Barème global

| Travail | Points |
|---------|:------:|
| Travail 1 – Vérification par les unités | /3 |
| Travail 2 – Ordres de grandeur | /3 |
| Travail 3 – Analyse série (moyenne, aberrant) | /4 |
| Travail 4 – Écart-type | /3 |
| Travail 5 – Exercice de synthèse E2 | /4 |
| Synthèse personnelle | /3 |
| **TOTAL** | **/20** |

---

## 💡 Erreurs fréquentes

| Erreur | Correction |
|--------|------------|
| Ne pas vérifier les unités | Toujours faire l'analyse dimensionnelle |
| Garder une valeur aberrante sans justification | Argumenter la décision |
| Confondre moyenne et écart-type | Moyenne = valeur centrale, écart-type = dispersion |
| Oublier de recalculer sans la valeur aberrante | La moyenne corrigée peut changer la conclusion |
