# Étude de cas – Le support de Transports Delorme

*BTS SIO SISR 1re année – CEJMA – S09*

> [!NOTE]
> **Comment travailler.** Lis le dossier, puis réponds **par écrit** à chaque question, avec une réponse **construite et argumentée** : une idée, sa justification, l'exemple tiré du dossier. Ouvre ensuite « Voir la réponse attendue » pour te corriger. À l'épreuve E4, une réponse sans justification n'est pas complète.

## Dossier : le support de Transports Delorme

> [!NOTE]
> L'entreprise, les tickets et les chiffres sont **fictifs**.

### Document 1 – La grille de priorité et le SLA

Mêmes règles que dans le cours (matrice impact × urgence ; GTR en heures ouvrées : **P1 4 h, P2 8 h, P3 24 h, P4 72 h**). Le service est ouvert **220 heures ouvrées** dans le mois.

### Document 2 – Les tickets du mois

| N° | Description | Impact | Urgence | Durée de rétablissement (h ouvrées) |
|---|---|---|---|---|
| T1 | L'ERP est inaccessible pour **tout l'entrepôt** | Élevé | Haute | 3,5 |
| T2 | La messagerie est très lente pour le service comptabilité (**12 personnes**) | Moyen | Moyenne | 30 |
| T3 | Un salarié a **oublié son mot de passe** et ne peut plus travailler | Faible | Haute | 2 |
| T4 | Le Wi-Fi du **dépôt** tombe par intermittence (**40 salariés**) | Élevé | Moyenne | 9 |
| T5 | Le poste de la directrice générale **ne démarre plus** | Faible | Haute | 5 |
| T6 | Un salarié demande un **écran supplémentaire** | – | – | 60 |

### Document 3 – Un extrait de ticket mal renseigné

> **Ticket 0412** : « Ça ne marche plus. Merci de régler vite. » (créé par téléphone, sans plus de détail)

### Questions

**1.** Parmi les tickets du document 2, lequel n'est **pas un incident** ? Pourquoi ? Comment doit-on le traiter ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

**T6** : c'est une **demande de service** (demande standard et prévue d'un équipement), pas une interruption ni une dégradation. On la traite par le processus de **demande** (validation, commande, livraison), pas par le processus d'incident.
</details>

**2.** Attribuez une **priorité** (P1 à P4) à chacun des **cinq incidents** avec la matrice.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

| Ticket | Impact / Urgence | Priorité | GTR |
|---|---|---|---|
| T1 | Élevé / Haute | **P1** | 4 h |
| T2 | Moyen / Moyenne | **P3** | 24 h |
| T3 | Faible / Haute | **P3** | 24 h |
| T4 | Élevé / Moyenne | **P2** | 8 h |
| T5 | Faible / Haute | **P3** | 24 h |
</details>

**3.** Calculez le **taux de respect du SLA** sur les cinq incidents. Quels tickets **dépassent** le délai ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

- T1 : 3,5 h pour 4 h : **respecté**.
- T2 : 30 h pour 24 h : **dépassé** de 6 h.
- T3 : 2 h pour 24 h : respecté.
- T4 : 9 h pour 8 h : **dépassé** de 1 h.
- T5 : 5 h pour 24 h : respecté.

Taux : 3 ÷ 5 = **60 %** (objectif visé : 90 % : **−30 points**). Les tickets **T2** et **T4** dépassent le délai.
</details>

**4.** Calculez le **MTTR** des cinq incidents. Calculez la **disponibilité de l'ERP** (T1) sur le mois.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

- MTTR : (3,5 + 30 + 2 + 9 + 5) ÷ 5 = 49,5 ÷ 5 = **9,9 heures**.
- Disponibilité de l'ERP : (220 − 3,5) ÷ 220 = 216,5 ÷ 220 = **98,41 %**.
</details>

**5.** Le MTTR est dominé par un ticket. Lequel ? Que **conclure** et que **faire** ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

**T2** (30 h sur un total de 49,5 h, soit plus de 60 %). Une **moyenne** peut masquer un cas extrême : sans T2, le MTTR serait (3,5 + 2 + 9 + 5) ÷ 4 = **4,875 h**. On analyse la **cause** de la lenteur (problème à traiter), on vérifie si une **escalade** aurait dû avoir lieu plus tôt, et on suit aussi la **médiane** ou les délais par priorité.
</details>

**6.** Le ticket 0412 est mal renseigné. **Listez** les informations à demander à l'utilisateur avant de poursuivre, puis **proposez une reformulation** correcte.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

À demander : **qui** (nom, service), **quoi** (équipement ou application, message d'erreur), **depuis quand**, **ce qui a changé** (mise à jour, déplacement), **combien de personnes** touchées, **ce qui a déjà été essayé**.

Reformulation : « Mme Lefèvre (comptabilité, poste PC-045) ne peut plus ouvrir le logiciel de facturation depuis ce matin 8 h 30, message “serveur introuvable” ; 3 collègues du service sont concernés ; un redémarrage n'a rien changé. »
</details>

**7.** Le service passe de **120** à **240** dépannages de même type par mois grâce à une procédure. Avec une **courbe d'expérience à 80 %** (base de 100 au premier dépannage), que devient le coût d'un dépannage après **un doublement** ? Pourquoi est-ce utile ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Après un doublement de la production cumulée, le coût unitaire est multiplié par 0,8 : **100 → 80**, soit **−20 %**. Après deux doublements : **64**. L'intérêt : en **capitalisant** l'expérience (procédures, base de connaissances), on **réduit durablement** le coût unitaire et le temps de traitement. C'est un **modèle**, non une loi exacte.
</details>

**8.** Après l'incident T1 (ERP indisponible pour tout l'entrepôt), dites **quatre éléments** d'un retour d'expérience utile.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(1) **Chronologie** précise ; (2) **cause** racine (problème) ; (3) **ce qui a bien fonctionné** et ce qui a **retardé** ; (4) **actions** d'amélioration avec un responsable et une échéance. On cherche à **améliorer le processus**, **pas à désigner un coupable**.
</details>


## Je sais faire

Coche honnêtement ; ce que tu ne coches pas se reprend avant la séance suivante.

- [ ] Distinguer incident, problème et demande de service
- [ ] Attribuer une priorité avec la matrice
- [ ] Calculer un taux de respect du SLA et un MTTR
- [ ] Calculer une disponibilité
- [ ] Écrire un ticket complet

**Ce que je dois reprendre :** ______________________

**Ma question à poser à l'enseignant :** ______________________
