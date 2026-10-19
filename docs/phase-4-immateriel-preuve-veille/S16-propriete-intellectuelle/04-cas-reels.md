# Cas réel – Oracle contre Google : peut-on copier des interfaces de programmation ?

*BTS SIO SISR 1re année – CEJMA – S16*

> [!NOTE]
> **Comment travailler.** Lis chaque cas réel et ses sources, réponds par écrit aux questions, puis ouvre « Voir la réponse attendue ». Les faits viennent des sources citées en fin de page ; en cas de doute, **retourne à la source**. Ces cas complètent l'étude de cas fictive de la séance.

## Le dossier

**Les faits.** Google a utilisé, pour son système Android, des éléments de l'**interface de programmation (API) du langage Java**, développée par Oracle. Oracle a soutenu que ce code était **protégé par le droit d'auteur** et que Google l'avait copié sans autorisation. Google a répondu que cet usage était légitime.

**La procédure (États-Unis).**

| Date | Étape |
|---|---|
| 9 mai 2014 | La cour d'appel fédérale juge que les API Java sont protégées par le droit d'auteur |
| 26 mai 2016 | Un jury de Californie estime que l'usage par Google relève du **fair use** (usage loyal) |
| Mars 2018 | La cour d'appel fédérale infirme : l'usage n'est pas un fair use |
| 5 avril 2021 | **La Cour suprême donne raison à Google**, par 6 voix contre 2 |

**La décision.** La Cour suprême suppose, « pour les besoins de l'argumentation », que le code d'Oracle est protégeable. Elle juge que **les quatre critères du fair use** jouent en faveur de Google. Elle décrit les éléments repris comme les seules lignes nécessaires pour permettre aux programmeurs de **réutiliser leurs compétences** dans un nouveau programme.

> [!WARNING]
> C'est du **droit américain** (notion de *fair use*). En France, le droit d'auteur fonctionne autrement : il liste des **exceptions précises** (par exemple la courte citation). Ne transpose pas la solution telle quelle ; sers-t'en pour comprendre **la question posée**.

## Pourquoi ce cas est utile

Il montre que la **frontière entre ce qui est protégé et ce qui ne l'est pas** n'est pas évidente pour un logiciel : le code est une création, mais les **interfaces** permettent à d'autres logiciels de dialoguer. Il illustre aussi la durée d'un litige : de 2014 à 2021 au moins, avec plusieurs renversements de décisions.

## Questions

**1.** Quelle **œuvre** Oracle prétendait-il protéger, et sur quel fondement ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Le **code déclarant de l'API Java** (la partie du code qui nomme et organise les fonctions utilisables), comme œuvre protégée par le **droit d'auteur**. Oracle reprochait une **copie sans autorisation**, donc une **contrefaçon** au sens du cours (partie V).
</details>

**2.** Pourquoi la solution a-t-elle changé plusieurs fois entre 2014 et 2021 ? Qu'en retiens-tu pour une entreprise qui développe un logiciel ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Parce que les juges ont **apprécié différemment** la même situation : la protection de l'API, puis le caractère « loyal » de la reprise. Pour une entreprise : **ne pas supposer** qu'une reprise de code ou d'interface est libre, **vérifier la licence**, **conserver la trace** de l'origine du code, et **anticiper** le coût d'un litige.
</details>

**3.** Dans quelle mesure ce raisonnement est-il transposable en France ? Cite une différence.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Peu directement. Le *fair use* est une notion **ouverte** du droit américain, appréciée au cas par cas ; en France, les **exceptions au droit d'auteur** sont **limitativement listées** par la loi (courte citation, copie privée, etc.). Un juge français ne raisonnerait donc pas en *fair use*.
</details>

## Sources

- [Copyright Alliance – Oracle America v. Google](https://copyrightalliance.org/copyright-cases/oracle-america-v-google/) : chronologie et décision, consultée pour cette page.
- [Wiley – Supreme Court Determines Copying of Software API Can Constitute Fair Use](https://www.wiley.law/alert-Supreme-Court-Determines-Copying-of-Software-API-Can-Constitute-Fair-Use) et [Winston & Strawn](https://www.winston.com/en/insights-news/supreme-court-rules-in-favor-of-google-in-multibillion-dollar-api-copyright-dispute) : analyses de la décision du 5 avril 2021.

> [!NOTE]
> **À valider :** dates et résumé repris de ces sources secondaires, à comparer avec le texte de la décision (*Google LLC v. Oracle America, Inc.*, Cour suprême des États-Unis, 2021) avant usage en évaluation.
