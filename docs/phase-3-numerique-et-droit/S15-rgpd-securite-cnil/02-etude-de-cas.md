# Étude de cas – L'incident du cabinet Delorme

*BTS SIO SISR 1re année – CEJMA – S15*

> [!NOTE]
> **Comment travailler.** Lis le dossier, puis réponds **par écrit** à chaque question, avec une réponse **construite et argumentée** : une idée, sa justification, l'exemple tiré du dossier. Ouvre ensuite « Voir la réponse attendue » pour te corriger. À l'épreuve E4, une réponse sans justification n'est pas complète.

## Dossier : l'incident du cabinet Delorme

> [!NOTE]
> L'entreprise et les personnes sont **fictives**.

### Document 1 – Le contexte

Le **cabinet Delorme** (comptabilité, 22 salariés) gère les dossiers de **380 clients** (entreprises individuelles) : identité, adresses, numéros de sécurité sociale pour la paie, **IBAN**, bulletins de paie. Le poste de travail de chaque collaborateur contient les dossiers de ses clients ; seuls les serveurs sont sauvegardés.

### Document 2 – Chronologie

- **Vendredi 17 h 30** : Léa, collaboratrice, constate qu'elle ne peut plus ouvrir ses fichiers : une **demande de rançon** s'affiche. Elle prévient Karim, le technicien, qui isole le poste du réseau.
- **Vendredi 18 h** : Karim constate que **3 postes** sont chiffrés. Aucune trace de fuite n'est trouvée à ce stade ; les journaux montrent une connexion externe inhabituelle la **veille**.
- **Samedi** : le gérant, informé par SMS, décide d'« attendre lundi » pour voir si la rançon peut être évitée.
- Les **disques** des postes ne sont **pas chiffrés** ; le **dernier test de restauration** date de plus d'un an.

### Questions

**1.** Cet incident est-il une **violation de données** au sens du RGPD ? Quelle(s) propriété(s) (confidentialité, intégrité, disponibilité) est/sont touchée(s) ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Oui. Les données sont **indisponibles** (chiffrées) : atteinte à la **disponibilité** ; une atteinte à la **confidentialité** est probable (accès externe inhabituel, fuite possible non exclue) et l'**intégrité** peut être touchée. Il s'agit d'une violation, même sans preuve de fuite.
</details>

**2.** À quelle **date et heure** expire le délai de notification à la CNIL ? À partir de quand court-il ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Le délai de **72 heures** court à partir du moment où le responsable **a connaissance** de la violation, c'est-à-dire **vendredi vers 17 h 30** (au plus tard 18 h, constat par Karim). Il expire donc **lundi vers 17 h 30** (ou 18 h). Les jours de week-end **comptent** : attendre lundi matin laisse très peu de marge.
</details>

**3.** Faut-il **informer les clients** (les personnes concernées) ? Justifiez avec la nature des données.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Probablement **oui** si le **risque est élevé** : numéros de sécurité sociale, IBAN et bulletins de paie permettent **usurpation d'identité** et **fraude**. Si une fuite est possible mais non démontrée, l'évaluation doit être documentée ; le chiffrement des disques aurait pu réduire le risque, mais il est **absent**.
</details>

**4.** La décision du gérant d'« attendre lundi » est-elle acceptable ? Que faire **immédiatement** ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Non. Il faut **agir sans attendre** : contenir (isoler les postes, changer les mots de passe, couper les accès externes), **préserver les preuves** (ne pas éteindre sans réfléchir, copier les journaux), **alerter** le DPO ou le référent, **déposer plainte** (utile), contacter un prestataire d'assistance, **préparer la notification** CNIL, évaluer l'information des clients et **documenter** au registre des violations.
</details>

**5.** Faut-il **payer la rançon** ? Donnez deux arguments.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Le paiement est **déconseillé** par les autorités : (1) aucune **garantie** de récupérer les données ; (2) il **finance** la criminalité et expose à de nouvelles attaques. La priorité est la **restauration depuis des sauvegardes** saines. (Avis à confronter aux recommandations officielles.)
</details>

**6.** Relevez les **manquements** à l'article 32 du cabinet (quatre) et proposez une **mesure corrective** pour chacun.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(1) **Disques non chiffrés** → chiffrement des disques ; (2) **données sur les postes, non sauvegardées** → centraliser sur serveur + sauvegardes ; (3) **restauration non testée** → tests réguliers ; (4) **pas de supervision** (connexion externe vue la veille) → journalisation et alertes ; (5) possibles : authentification forte, mises à jour, sensibilisation.
</details>

**7.** Quelles **sanctions** le cabinet risque-t-il ? Expliquez ce qui jouera sur leur gravité.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Mise en demeure, **amende** (niveau 1 : jusqu'à 10 M€ ou 2 % du CA pour défaut de sécurité ou de notification), responsabilité **civile** envers les clients et dégâts d'**image**. Jouent : gravité des manquements, **nombre** et **sensibilité** des données, **réactivité**, **notification dans les délais**, mesures prises, coopération avec la CNIL.
</details>


## Je sais faire

Coche honnêtement ; ce que tu ne coches pas se reprend avant la séance suivante.

- [ ] Définir une violation de données
- [ ] Calculer le délai de 72 heures
- [ ] Dire quand informer les personnes
- [ ] Citer deux niveaux d'amende
- [ ] Lister des mesures de sécurité adaptées

**Ce que je dois reprendre :** ______________________

**Ma question à poser à l'enseignant :** ______________________
