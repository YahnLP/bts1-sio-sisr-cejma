# Étude de cas – L'incident de Domus Habitat

*BTS SIO SISR 1re année – CEJMA – S18*

> [!NOTE]
> **Comment travailler.** Lis le dossier, puis réponds **par écrit** à chaque question, avec une réponse **construite et argumentée** : une idée, sa justification, l'exemple tiré du dossier. Ouvre ensuite « Voir la réponse attendue » pour te corriger. À l'épreuve E4, une réponse sans justification n'est pas complète.

## Dossier : l'incident de Domus Habitat

> [!NOTE]
> L'entreprise et les personnes sont **fictives**.

### Document 1 – Le contexte

**Domus Habitat** est une agence immobilière de 14 salariés. Le **mardi 4 mars**, la responsable constate que des **fiches de clients** ont été modifiées sur le logiciel de gestion. Elle soupçonne **Julien**, un commercial qui a démissionné le 28 février. Le technicien, **Mehdi**, dispose des journaux du serveur et du poste de Julien.

### Document 2 – Éléments disponibles

- Journal du logiciel : modifications le **3 mars à 22 h 14**, compte de **Julien**.
- Julien dit que son **mot de passe** était noté sur un papier à côté du poste.
- Les **horloges** du serveur et du poste ne sont **pas synchronisées** (écart de plusieurs minutes).
- Mehdi **redémarre** le poste de Julien et **supprime** les fichiers temporaires « pour faire de la place ».
- Un client a reçu un **courriel** de Julien lui proposant de passer par son nouvel employeur ; le client a **transféré** le message à Domus Habitat sans les en-têtes.
- Le contrat de travail de Julien comporte une **clause de confidentialité**.

### Questions

**1.** Les journaux prouvent-ils que **Julien** est l'auteur des modifications ? Relevez deux faiblesses.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Pas avec certitude. Le compte est celui de Julien, mais : (1) son **mot de passe** était **accessible** à d'autres (papier) ; (2) les **horloges** non synchronisées affaiblissent la **fiabilité** de l'horodatage. Autres faiblesses possibles : pas d'authentification forte, journaux non protégés en écriture. Un compte désactivé depuis le 28 février aurait dû empêcher l'accès.
</details>

**2.** Mehdi a-t-il bien agi en redémarrant et en supprimant des fichiers ? Quelles conséquences ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Non : il a **altéré** des éléments de preuve potentiels (mémoire vive, fichiers temporaires). Il faut **préserver** : ne pas redémarrer sans nécessité, **copier** les journaux, faire une **image disque** avec **empreinte**. Les conséquences : preuve **affaiblie** ou **écartée**, et soupçon sur la **loyauté** du technicien.
</details>

**3.** Décrivez la **procédure correcte** de préservation, en cinq étapes.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(1) **Isoler** le poste sans l'altérer ; (2) **copier** les journaux (serveur et poste) ; (3) réaliser une **image disque** et calculer une **empreinte** (SHA-256) ; (4) conserver l'**original** scellé et travailler sur la **copie** ; (5) tenir la **chaîne de conservation** (qui, quand, pourquoi) et rédiger un **rapport**.
</details>

**4.** Le **courriel transféré** par le client est-il une preuve solide ? Que faire ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Faible : sans **en-têtes** ni original, on ne prouve ni l'**expéditeur** ni l'**intégrité**. Il faut demander au client l'**original** (ou un export complet), conserver les **en-têtes**, éventuellement faire constater par un **commissaire de justice**.
</details>

**5.** Quelles **règles de loyauté** Domus Habitat doit-elle respecter en réunissant ses preuves ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Se limiter aux **données professionnelles**, respecter la **vie privée** (pas de lecture de messages personnels, séance 11), s'appuyer sur des dispositifs **déclarés** aux salariés, rester **proportionné**, ne pas faire pression pour obtenir des aveux. Une preuve obtenue de façon **déloyale** peut être écartée.
</details>

**6.** Quelles **mesures préventives** auraient évité la situation (quatre) ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(1) **Désactiver** le compte au départ (procédure de départ, séance 11) ; (2) **authentification forte** et mots de passe non notés ; (3) **synchronisation NTP** et centralisation des journaux ; (4) **droits d'accès** limités et journaux protégés ; (5) rappel de la **clause de confidentialité** à la sortie.
</details>

**7.** Que doit faire Domus Habitat pour **réagir** (actions juridiques et techniques) ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

**Restaurer** les fiches depuis la sauvegarde, **évaluer** la violation de données (séance 15 : notification si risque), **documenter**, **mettre en demeure** Julien, éventuellement **déposer plainte** (accès ou maintien frauduleux, article 323-1 du Code pénal, selon les faits) ou saisir le conseil de prud'hommes, et **renforcer** la sécurité.
</details>


## Je sais faire

Coche honnêtement ; ce que tu ne coches pas se reprend avant la séance suivante.

- [ ] Dire quand un écrit électronique vaut preuve
- [ ] Citer trois niveaux de signature
- [ ] Décrire la chaîne de conservation
- [ ] Distinguer identification et authentification
- [ ] Citer des règles de loyauté

**Ce que je dois reprendre :** ______________________

**Ma question à poser à l'enseignant :** ______________________
