# Étude de cas – Cobalt Services et la Maison Verdier

*BTS SIO SISR 1re année – CEJM et CEJMA – S19*

> [!NOTE]
> **Comment travailler.** Lis le dossier, puis réponds **par écrit** à chaque question, avec une réponse **construite et argumentée** : une idée, sa justification, l'exemple tiré du dossier. Ouvre ensuite « Voir la réponse attendue » pour te corriger. À l'épreuve E4, une réponse sans justification n'est pas complète.

## Dossier de synthèse : Cobalt Services et la Maison Verdier

> [!NOTE]
> Les entreprises et les personnes sont **fictives**. Ce sujet mobilise les trois champs (économie, droit, management) et prépare à l'épreuve E4.

### Document 1 – Le contexte

**Cobalt Services**, ESN de 40 salariés, propose à **Maison Verdier** (négoce de vins, 25 salariés) un contrat d'**infogérance** : supervision, support utilisateurs, sauvegardes, gestion des postes. Aujourd'hui, Maison Verdier emploie **un technicien** en interne.

### Document 2 – Comparatif de coûts annuels

| Poste de coût | Solution interne | Infogérance Cobalt |
|---|---|---|
| Coût employeur du technicien | 48 000 € | — |
| Licences logicielles | 6 000 € | — (incluses) |
| Matériel (amortissement annuel) | 9 000 € | — (inclus) |
| Formation | 2 000 € | — |
| Forfait mensuel | — | 3 200 € × 12 |
| Options (interventions sur site, projets) | — | 4 800 € / an |

### Document 3 – Extraits du contrat proposé

- **Disponibilité** de la supervision : engagement de **99,5 % par mois** (mois de 30 jours). En dessous, pénalité de **5 %** du forfait mensuel.
- Cobalt **traitera des données personnelles** de salariés et de clients de Maison Verdier.
- Durée : **3 ans**, reconduction tacite, résiliation avec **préavis de 6 mois**.
- Cobalt « utilisera ses propres outils, dont un logiciel sous licence **GPL** modifié par ses soins ».
- En cas d'incident, Cobalt « interviendra dans les meilleurs délais ».

### Document 4 – Mois de juin

Le service de supervision a été **indisponible 5 heures** au total (300 minutes) sur le mois de juin (30 jours).

### Questions

**1.** (Économie) Calculez le **coût annuel** de chaque solution et l'**écart** (en euros et en pourcentage du coût interne). Commentez.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Interne : 48 000 + 6 000 + 9 000 + 2 000 = **65 000 €**. Infogérance : 3 200 × 12 + 4 800 = 38 400 + 4 800 = **43 200 €**. Écart : 65 000 − 43 200 = **21 800 €**, soit 21 800 / 65 000 ≈ **33,5 %** du coût interne. L'infogérance est moins chère sur le papier, mais le **coût total** doit aussi intégrer la **dépendance** au prestataire, la perte de **compétence interne**, la qualité de service et les **coûts cachés** (pilotage du contrat, réversibilité).
</details>

**2.** (Management) Quels sont **deux avantages** et **deux risques** de l'externalisation pour Maison Verdier ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Avantages : **expertise** et **continuité** (équipe plutôt qu'une personne), **coûts** prévisibles, concentration sur le cœur de métier. Risques : **dépendance** envers Cobalt, **perte de maîtrise** du système d'information, **confidentialité** des données, difficulté de **réversibilité** (reprendre ou changer de prestataire).
</details>

**3.** (Droit) Le contrat parle d'« intervenir dans les meilleurs délais ». Pourquoi est-ce insuffisant ? Que proposer ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

La formule est **vague**, donc **inexécutable** et **difficile à sanctionner** (séances 4 et 9). Proposer un **SLA** chiffré : délai de **prise en charge** et de **rétablissement** selon la **priorité** (par exemple critique : prise en charge en 1 heure, rétablissement en 4 heures, à négocier), horaires de couverture, **pénalités** et indicateurs de suivi.
</details>

**4.** (Calcul) Calculez la **disponibilité** de juin, comparez-la à l'engagement et déterminez la **pénalité** éventuelle.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Minutes du mois : 30 × 24 × 60 = **43 200**. Indisponibilité tolérée à 99,5 % : 0,5 % × 43 200 = **216 minutes** (3 h 36). Constatée : **300 minutes**. Disponibilité : 1 − 300 / 43 200 ≈ **99,31 %**, inférieure à 99,5 %. L'engagement n'est **pas respecté** → pénalité de 5 % × 3 200 = **160 €**.
</details>

**5.** (Droit) Quelles **obligations RGPD** s'appliquent à Cobalt et à Maison Verdier ? Citez quatre points à prévoir.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Maison Verdier est **responsable de traitement**, Cobalt **sous-traitant** : **contrat de sous-traitance** (article 28), **instructions** documentées, **sécurité** des données, **notification** des violations (alerte rapide du responsable pour respecter les 72 h), **sous-traitants ultérieurs** soumis à autorisation, **restitution ou suppression** des données en fin de contrat, **registre**, éventuels **transferts** hors UE encadrés.
</details>

**6.** (Droit) Le logiciel **GPL modifié** : quel point d'attention pour le client ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Si Cobalt **redistribue** ou livre ce logiciel modifié à Maison Verdier, la GPL impose de fournir les **sources** et de respecter la licence. Maison Verdier doit **demander** la liste des composants, la licence et les conditions d'**utilisation** ; vérifier la **conformité** pour éviter un risque de contrefaçon.
</details>

**7.** (Management) Rédigez **cinq clauses** ou garanties à négocier avant de signer.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(1) **SLA** chiffré avec pénalités ; (2) **réversibilité** (restitution des données et documentation, aide à la transition) ; (3) **durée** et **préavis** raisonnables (préavis de 6 mois sur 3 ans est long : à négocier) ; (4) clause **RGPD** et sécurité ; (5) **responsabilité** et assurance du prestataire, plafonds de pénalités ; (6) **confidentialité** et propriété des données.
</details>

**8.** (Veille) Concevez une **veille** pour Maison Verdier sur le sujet : trois thèmes, trois sources, une fréquence.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Thèmes : **cybersécurité** (menaces, alertes), **RGPD/CNIL** (obligations, sanctions), **évolution des offres** et prix de l'infogérance. Sources : **CERT-FR / Cybermalveillance**, **CNIL**, presse spécialisée ou observatoire du secteur. Fréquence : **hebdomadaire** pour les alertes de sécurité, **mensuelle** pour le reste ; sortie : bulletin d'une page (fait, source, impact, action).
</details>


## Je sais faire

Coche honnêtement ; ce que tu ne coches pas se reprend avant la séance suivante.

- [ ] Décrire les étapes d'une veille
- [ ] Citer cinq sources fiables
- [ ] Rédiger un bulletin de veille
- [ ] Répondre en trois temps à une question
- [ ] Calculer un coût total et une disponibilité

**Ce que je dois reprendre :** ______________________

**Ma question à poser à l'enseignant :** ______________________
