---
author: YLP
title: 📚 FICHE DE COURS
---

# 📚 FICHE DE COURS ÉLÈVE
## Identité Numérique : E-réputation, Usurpation d'Identité et Cadre e-IDAS

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 15 — CEJMA*

---

## 🎯 Objectifs de Cette Fiche

À la fin de ce cours, vous serez capable de :
- ✅ Définir l'identité numérique et ses trois composantes
- ✅ Expliquer l'e-réputation et ses enjeux professionnels
- ✅ Identifier les risques d'usurpation d'identité et les protections
- ✅ Comprendre le règlement e-IDAS et les signatures électroniques
- ✅ Appliquer les bonnes pratiques de protection de votre identité numérique

---

## 📖 PARTIE I — L'Identité Numérique

### I.A. Définition

**Identité numérique :** Ensemble des traces et données qu'une personne laisse sur Internet, volontairement ou involontairement, et qui forment sa représentation en ligne.

**Formule :**
```
Identité Numérique = Identité Civile + Traces Numériques + Données Calculées
```

**Différence avec identité civile :**
- **Identité civile** : nom, prénom, date de naissance, nationalité (état civil)
- **Identité numérique** : représentation en ligne (profils, posts, commentaires, likes, historique...)

---

### I.B. Les 3 Composantes de l'Identité Numérique

#### 1. Identité Déclarative (Ce que JE dis de moi)

**Définition :** Informations que vous fournissez **volontairement** lors de la création de comptes ou de publications.

**Exemples :**
- Profil Facebook : nom, photo, ville, école, entreprise
- CV sur LinkedIn : expériences, formations, compétences
- Bio Instagram : description personnelle
- Formulaires d'inscription : email, téléphone, adresse

**Caractéristiques :**
- ✅ **Contrôlable** : vous choisissez ce que vous partagez
- ⚠️ **Permanente** : difficile à effacer une fois publiée
- 🔓 **Souvent publique** : visible par défaut sur réseaux sociaux

---

#### 2. Identité Agissante (Ce que JE fais en ligne)

**Définition :** Traces laissées par vos **actions** sur Internet.

**Exemples :**
- Posts, commentaires, likes sur réseaux sociaux
- Avis sur TripAdvisor, Google Maps, Amazon
- Historique de navigation (cookies, logs)
- Téléchargements, achats en ligne
- Géolocalisation (photos, check-ins)

**Caractéristiques :**
- ⚠️ **Partiellement contrôlable** : vous choisissez d'agir, mais les traces persistent
- 🕵️ **Traçable** : historique conservé par les plateformes
- 📊 **Analysable** : peut être agrégée pour créer un profil

---

#### 3. Identité Calculée (Ce que les ALGORITHMES disent de moi)

**Définition :** Données **inférées** ou **calculées** par des algorithmes à partir de votre comportement.

**Exemples :**
- Score de crédit (Crédit Agricole, BNP...)
- Profil publicitaire (Google Ads, Facebook Ads)
- Recommandations Netflix, Spotify (basées sur historique)
- Score de fiabilité (Uber, Airbnb)
- Catégorisation (Amazon : "client premium", "client à risque")

**Caractéristiques :**
- ❌ **NON contrôlable** : vous ne choisissez pas ce que les algorithmes calculent
- 🔒 **Opaque** : vous ne savez souvent pas comment vous êtes catégorisé
- 📊 **Discriminante** : peut mener à des discriminations (refus de crédit, prix différenciés...)

---

![Schéma : Identité numérique = 3 cercles concentriques - au centre "Identité déclarative" (ce que je dis), couche intermédiaire "Identité agissante" (ce que je fais), couche externe "Identité calculée" (ce que les algorithmes déduisent)]

*Légende : Les trois composantes de l'identité numérique*

---

### I.C. Les Données Personnelles (RGPD)

**Rappel RGPD :** Toute information se rapportant à une personne physique **identifiée ou identifiable**.

**Données d'identité numérique :**
- **Directement identifiantes** : nom, prénom, email, téléphone, photo
- **Indirectement identifiantes** : adresse IP, cookies, identifiants de session
- **Données sensibles** : religion, santé, orientation sexuelle (protection renforcée)

**Principe de minimisation (RGPD art. 5) :**
> *"Les données à caractère personnel doivent être adéquates, pertinentes et limitées à ce qui est nécessaire."*

**Application pratique :**
- ❌ Ne PAS publier : adresse postale, numéro de sécurité sociale, copie carte identité
- ⚠️ Limiter : téléphone, email, date de naissance complète
- ✅ OK : nom, prénom, ville, entreprise (si profil professionnel)

---

## 📖 PARTIE II — L'E-réputation

### II.A. Définition

**E-réputation (ou réputation numérique) :** Image qu'une personne ou une organisation projette sur Internet, résultant de ce qu'elle dit d'elle-même ET de ce que les autres disent d'elle.

**Formule :**
```
E-réputation = Mon identité déclarative + Avis des autres + Algorithmes de recherche
```

**Différence avec réputation classique :**
- **Réputation classique** : bouche-à-oreille, local, éphémère
- **E-réputation** : mondiale, permanente (archives, caches), indexée (Google)

---

### II.B. Enjeux de l'E-réputation

#### 1. Enjeux Personnels

| **Domaine** | **Impact** | **Exemple** |
|---|---|---|
| **Recrutement** | 70% des recruteurs googlent les candidats | Refus après découverte de photos de soirée |
| **Rencontres** | Vérification des profils avant rendez-vous | Date annulé après Google |
| **Relations** | Découverte d'informations embarrassantes | Conflit familial suite à post Facebook |

**Statistiques :**
- **93% des recruteurs** regardent les profils sociaux des candidats (CareerBuilder, 2022)
- **55% des recruteurs** ont rejeté un candidat à cause de son profil social

---

#### 2. Enjeux Professionnels

| **Domaine** | **Impact** | **Exemple** |
|---|---|---|
| **Carrière** | Promotion refusée | Post politique controversé |
| **Relations professionnelles** | Perte de confiance | Commentaire négatif sur ancien employeur |
| **Business** | Perte de clients | Avis négatifs sur Google Maps |

**Cas réel :**
> En 2013, Justine Sacco, directrice communication, poste un tweet raciste avant un vol long-courrier. À son atterrissage, elle est virée et son nom est devenu synonyme de "bad buzz".

---

### II.C. Droit à l'Oubli (RGPD Art. 17)

**Définition :** Droit de demander l'effacement de données personnelles dans certains cas (voir S8 RGPD).

**Application à l'e-réputation :**
- ✅ **Possible** : demander à un site de supprimer un article vous concernant (si conditions réunies)
- ⚠️ **Limité** : Google peut déréférencer (retirer des résultats de recherche), mais l'article reste en ligne
- ❌ **Impossible** : effacer TOUTES les traces (caches, archives, captures d'écran)

**Jurisprudence clé : Google Spain vs AEPD (2014)**

**Faits :**
- Mario Costeja González (Espagnol) avait des dettes dans les années 90
- Un article de journal parlait de la vente de sa maison aux enchères
- 15 ans plus tard, cet article apparaissait toujours en 1er résultat Google
- Il demande le déréférencement

**Décision CJUE (Cour de Justice de l'UE) :**
- ✅ Google doit déréférencer l'article (ne plus l'afficher dans les résultats)
- ⚠️ MAIS l'article reste en ligne (pas supprimé du site du journal)
- 🌍 Déréférencement limité à l'UE (toujours visible depuis les USA)

**Depuis 2014 :** Google a reçu +1 million de demandes de déréférencement en Europe, accepté ~50%.

---

### II.D. Gestion de l'E-réputation

#### 1. Surveiller son E-réputation

**Outils :**
- **Google Alerts** : alerte email quand votre nom apparaît
- **Google Search Console** : voir quelles pages vous mentionnent
- **Mention, Brandwatch** : outils pros de veille (payants)

**Fréquence :** Recherche Google sur son nom **1 fois par mois** minimum.

---

#### 2. Nettoyer son E-réputation

**Actions possibles :**

| **Action** | **Difficulté** | **Efficacité** |
|---|:---:|:---:|
| **Supprimer ses propres posts** | Facile | Élevée (si fait rapidement) |
| **Paramétrer profils en privé** | Facile | Élevée |
| **Demander suppression à un site** | Moyenne | Moyenne (dépend du site) |
| **Demander déréférencement Google** | Difficile | Moyenne (50% accepté) |
| **Noyer les résultats négatifs** | Difficile | Élevée (créer contenu positif) |

**Technique du "Name Flooding" :**
- Créer du contenu positif (LinkedIn, blog, GitHub) pour noyer les résultats négatifs dans Google
- Exemple : si "Pierre Dupont problème" apparaît page 1, créer "Pierre Dupont professionnel" pour passer page 2

---

## 📖 PARTIE III — Usurpation d'Identité Numérique

### III.A. Définition Juridique

**Code pénal — Article 226-4-1 :**
> *"Le fait d'usurper l'identité d'un tiers ou de faire usage d'une ou plusieurs données de toute nature permettant de l'identifier en vue de troubler sa tranquillité ou celle d'autrui, ou de porter atteinte à son honneur ou à sa considération, est puni d'un an d'emprisonnement et de 15 000 euros d'amende."*

**En clair :**
- Utiliser le nom, la photo, l'email, ou toute donnée d'une autre personne
- Dans le but de lui nuire ou de tromper
- = **1 an de prison + 15 000 € d'amende**

---

### III.B. Formes d'Usurpation d'Identité

#### 1. Phishing (Hameçonnage)

**Définition :** Email frauduleux se faisant passer pour un organisme officiel (banque, impôts, Sécurité sociale) pour voler des identifiants.

**Exemple typique :**
```
De : "Crédit Agricole" <support@credait-agricole.fr>  [Notez la faute]
Objet : Votre compte a été bloqué pour activité suspecte

Cher client,

Nous avons détecté une activité suspecte sur votre compte.
Veuillez confirmer votre identité en cliquant ici :
https://credit-agricole-verification.xyz  [Faux site]

Cordialement,
Le service sécurité
```

**Signaux d'alerte :**
- ❌ Fautes d'orthographe
- ❌ Expéditeur suspect (domaine différent)
- ❌ Urgence, menace ("compte bloqué !")
- ❌ Lien vers site externe (pas le vrai site banque)
- ❌ Demande de mot de passe (JAMAIS par email)

---

#### 2. Faux Profils sur Réseaux Sociaux

**Technique :**
- Vol de photo de profil + nom
- Création d'un faux compte
- Ajout d'amis/contacts de la victime
- Escroquerie (demander argent, obtenir infos)

**Exemple réel :**
> Faux profil LinkedIn d'un DRH pour piéger des candidats et voler leurs données personnelles (CV, copie pièce identité).

---

#### 3. SIM Swapping

**Technique :**
- Pirate obtient infos personnelles (date naissance, adresse...)
- Appelle opérateur télécom (Orange, SFR...) en se faisant passer pour la victime
- Demande transfert du numéro vers une nouvelle SIM
- Reçoit SMS de validation 2FA → accès aux comptes bancaires, emails

**Victime célèbre :** Jack Dorsey (fondateur Twitter) victime en 2019.

---

#### 4. Deepfakes

**Définition :** Vidéos ou audios **générés par IA** imitant une personne réelle.

**Usages malveillants :**
- Fausse vidéo compromettante d'une personnalité
- Faux appel vocal d'un CEO pour ordonner un virement (fraude au président)
- Pornographie non consentie (visage de la victime sur corps d'acteur/actrice)

**Exemple réel :**
> 2020 : Deepfake audio du CEO d'une entreprise britannique → employé vire 243 000$ aux pirates.

---

### III.C. Sanctions et Recours

**Sanctions pénales :**
- **Usurpation d'identité** (art. 226-4-1) : 1 an + 15 000 €
- **Escroquerie** (art. 313-1) : 5 ans + 375 000 €
- **Atteinte système informatique** (art. 323-1) : 2 ans + 60 000 €

**Recours possibles :**
1. **Plainte au commissariat** (ou gendarmerie)
2. **Signalement sur la plateforme** (Facebook, Twitter, LinkedIn → bouton "signaler")
3. **Plateforme officielle** : [internet-signalement.gouv.fr](https://www.internet-signalement.gouv.fr)
4. **Avocat** : pour action civile (dommages et intérêts)

---

### III.D. Prévention de l'Usurpation

| **Bonne Pratique** | **Efficacité** | **Difficulté** |
|---|:---:|:---:|
| **Mots de passe forts + uniques** | ⭐⭐⭐⭐⭐ | Moyenne |
| **2FA (double authentification)** | ⭐⭐⭐⭐⭐ | Facile |
| **Gestionnaire de mots de passe** | ⭐⭐⭐⭐ | Moyenne |
| **Ne PAS cliquer liens suspects** | ⭐⭐⭐⭐⭐ | Facile |
| **Vérifier expéditeur emails** | ⭐⭐⭐⭐ | Facile |
| **Limiter infos publiques** | ⭐⭐⭐ | Facile |
| **Surveiller comptes (HaveIBeenPwned)** | ⭐⭐⭐⭐ | Facile |

---

## 📖 PARTIE IV — Le Cadre e-IDAS

### IV.A. Qu'est-ce que e-IDAS ?

**e-IDAS :** Règlement européen (UE n°910/2014) sur l'**identification électronique et les services de confiance** pour les transactions électroniques dans le marché intérieur (electronic IDentification, Authentication and trust Services).

**Objectif :** Créer un **cadre de confiance numérique** harmonisé dans toute l'UE pour :
- ✅ Sécuriser les transactions en ligne
- ✅ Faciliter les échanges transfrontaliers
- ✅ Reconnaître les signatures électroniques entre pays UE

**Date d'application :** 1er juillet 2016

---

### IV.B. Les 3 Niveaux d'Identification Électronique

| **Niveau** | **Exigences** | **Exemples** |
|---|---|---|
| **Faible** | Simple identifiant + mot de passe | Compte Gmail, Facebook |
| **Substantiel** | 2FA (2 facteurs) | SMS + mot de passe, App authentificatrice |
| **Élevé** | Certificat qualifié + dispositif sécurisé | Carte d'identité électronique, FranceConnect |

**Application :** Les services publics européens doivent accepter les identités électroniques de niveau substantiel ou élevé des autres pays UE.

**Exemple :** Un Français peut utiliser FranceConnect pour accéder à un service public allemand.

---

### IV.C. Les 3 Niveaux de Signature Électronique

#### 1. Signature Électronique Simple

**Définition :** Données sous forme électronique jointes à d'autres données et servant de méthode d'authentification.

**Exemples :**
- Scan d'une signature papier (⚠️ faible sécurité)
- Case à cocher "J'accepte les CGU"
- Signature tactile sur tablette (Chronopost, banque)

**Valeur juridique :**
- ✅ Valide juridiquement (Code civil art. 1367)
- ⚠️ MAIS facilement contestable (pas de preuve d'identité)

---

#### 2. Signature Électronique Avancée

**Définition :** Signature qui répond aux exigences suivantes :
- ✅ **Liée uniquement** au signataire
- ✅ **Permet d'identifier** le signataire
- ✅ **Créée avec des moyens** que le signataire contrôle exclusivement
- ✅ **Liée aux données signées** (si modification, signature invalide)

**Moyens techniques :** Certificat numérique + clés cryptographiques (RSA, ECDSA)

**Exemples :**
- DocuSign (niveau avancé)
- Adobe Sign (niveau avancé)
- Universign

**Valeur juridique :**
- ✅ Valide et difficilement contestable
- ✅ Preuve d'identité (certificat)
- ⚠️ Pas de présomption de fiabilité absolue

---

#### 3. Signature Électronique Qualifiée

**Définition :** Signature électronique avancée + **certificat qualifié** délivré par un **PSCE (Prestataire de Services de Confiance Électronique) qualifié**.

**Exigences supplémentaires :**
- ✅ Certificat délivré par organisme **agréé par l'ANSSI** (France) ou équivalent UE
- ✅ Création par **dispositif sécurisé** (carte à puce, token USB)
- ✅ Respect normes techniques (ETSI, ISO)

**Exemples :**
- Carte Vitale (signature actes médicaux)
- CPS (Carte de Professionnel de Santé)
- Certificats Certigna, IDsign

**Valeur juridique :**
- ✅ **Équivalence avec signature manuscrite** (Règlement e-IDAS art. 25)
- ✅ **Présomption de fiabilité** (opposable juridiquement)
- ✅ **Reconnue dans toute l'UE**

---

**Tableau Comparatif :**

| **Critère** | **Simple** | **Avancée** | **Qualifiée** |
|---|:---:|:---:|:---:|
| **Identification signataire** | ⚠️ Faible | ✅ Forte | ✅ Très forte |
| **Lien avec données signées** | ❌ Faible | ✅ Oui | ✅ Oui |
| **Certificat qualifié** | ❌ Non | ❌ Non | ✅ Oui |
| **Dispositif sécurisé** | ❌ Non | ⚠️ Optionnel | ✅ Obligatoire |
| **Valeur juridique** | ⚠️ Contestable | ✅ Solide | ✅ Équivalence manuscrite |
| **Reconnaissance UE** | ❌ Non | ⚠️ Partielle | ✅ Totale |
| **Coût** | Gratuit | 5-20€/doc | 50-200€/an |

---

### IV.D. Les Prestataires de Services de Confiance (PSCO)

**Définition :** Organismes qui fournissent des services de confiance numérique (signatures, certificats, horodatages, archivage).

**Services fournis :**
- Délivrance de certificats qualifiés
- Signature électronique (simple, avancée, qualifiée)
- Cachet électronique (pour entreprises)
- Horodatage électronique (preuve de date)
- Recommandé électronique (équivalent lettre recommandée)

**Exemples de PSCO qualifiés (France) :**
- **Certigna** (Docaposte, La Poste)
- **IDsign** (Atos)
- **Universign**
- **ChamberSign** (Chambres de Commerce)

**Liste officielle :** [esignature.ec.europa.eu/efda/tl-browser](https://esignature.ec.europa.eu/efda/tl-browser)

---

### IV.E. FranceConnect et Identité Numérique

**FranceConnect :** Système d'identification français permettant d'accéder à +1000 services publics avec un seul compte (impots.gouv.fr, ameli.fr, pole-emploi.fr...).

**Fonctionnement :**
1. Vous avez un compte sur un **fournisseur d'identité** (Impôts, La Poste, Ameli...)
2. Vous cliquez "Se connecter avec FranceConnect" sur un service public
3. Vous choisissez votre fournisseur d'identité
4. Vous vous authentifiez (identifiant + mot de passe + éventuellement 2FA)
5. FranceConnect transmet vos données d'identité au service

**Avantages :**
- ✅ Un seul compte pour tous les services publics
- ✅ Pas besoin de créer 50 comptes différents
- ✅ Sécurisé (niveau substantiel e-IDAS)

**Projet France Identité Numérique (2024) :**
- Application mobile officielle
- Identité numérique de **niveau élevé** (e-IDAS)
- Basée sur pièce d'identité biométrique
- Permet signature électronique qualifiée

---

## 🔑 VOCABULAIRE CLÉ À MAÎTRISER

| **Terme** | **Définition Simple** |
|---|---|
| **Identité numérique** | Ensemble des traces qu'une personne laisse sur Internet |
| **Identité déclarative** | Ce que je dis de moi (profils, bio...) |
| **Identité agissante** | Ce que je fais en ligne (posts, likes, achats...) |
| **Identité calculée** | Ce que les algorithmes déduisent de moi |
| **E-réputation** | Image qu'une personne projette sur Internet |
| **Droit à l'oubli** | Droit de demander effacement de données (RGPD art. 17) |
| **Usurpation d'identité** | Utiliser l'identité d'un tiers pour lui nuire (1 an + 15k€) |
| **Phishing** | Email frauduleux pour voler identifiants |
| **Deepfake** | Vidéo/audio faux générée par IA |
| **2FA** | Double authentification (mot de passe + code SMS/app) |
| **e-IDAS** | Règlement UE sur confiance numérique (signatures, certificats) |
| **Signature électronique** | Données électroniques pour authentifier un document |
| **Signature qualifiée** | Signature avec certificat qualifié = équivalence manuscrite |
| **FranceConnect** | Système d'identification unique pour services publics français |

---

## ✅ Points Clés à Retenir

1. **Identité numérique = 3 composantes** : déclarative (je dis), agissante (je fais), calculée (algorithmes déduisent).

2. **E-réputation = crucial pour carrière** : 70% recruteurs googlent candidats, 55% rejettent à cause profil social.

3. **Droit à l'oubli ≠ effacement total** : Google peut déréférencer, mais contenu reste en ligne.

4. **Usurpation = 1 an + 15 000€** : phishing, faux profils, SIM swapping, deepfakes.

5. **2FA = protection essentielle** : réduit 90% des risques de piratage.

6. **e-IDAS = confiance numérique UE** : signatures électroniques (simple, avancée, qualifiée).

7. **Signature qualifiée = équivalence manuscrite** : certificat qualifié + dispositif sécurisé.

8. **FranceConnect = 1 compte, 1000 services** : identification unique services publics français.

9. **Surveiller e-réputation** : Google Alerts sur son nom 1×/mois minimum.

10. **Protéger identité** : mots de passe forts + uniques, 2FA, limiter infos publiques, vérifier emails.

---

## 📚 Pour Aller Plus Loin

**Outils pratiques :**
- [HaveIBeenPwned](https://haveibeenpwned.com) — Vérifier fuites de données
- [Google Alerts](https://www.google.com/alerts) — Surveiller son nom
- [FranceConnect](https://franceconnect.gouv.fr) — Identité numérique publique

**Textes de référence :**
- [Règlement e-IDAS](https://eur-lex.europa.eu/legal-content/FR/TXT/?uri=CELEX:32014R0910)
- [Code pénal art. 226-4-1](https://www.legifrance.gouv.fr/codes/article_lc/LEGIARTI000042193593)

**Questions de réflexion :**
- Faut-il créer des profils séparés (perso vs pro) sur réseaux sociaux ?
- Le droit à l'oubli est-il vraiment efficace ?
- Les deepfakes représentent-ils une menace majeure pour la démocratie ?

---
