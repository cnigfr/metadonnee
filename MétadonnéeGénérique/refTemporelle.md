## VI. Référence temporelle
Après un paragraphe général explicitant les exigences INSPIRE en matière de Référence Temporelle, ce chapitre décrit plus en détail l’élément de métadonnées Etendue temporelle (VI.1), puis les Dates de référence (Date de publication (VI.2.1), Date de création (VI.2.2) et Date de dernière révision (VI.2.3)), et enfin le Système de référence temporel (VI.3).

**EXIGENCE INSPIRE :**
- INSPIRE impose la fourniture d’au moins une référence temporelle qui peut être une date de création, de dernière révision, de publication ou une étendue temporelle.
- Le système de référence par défaut est le calendrier grégorien.
- Les dates sont exprimées conformément à la norme ISO 8601 (c’est-à-dire aaaa-mm-jj).
- Il est possible de définir plusieurs références temporelles mais :
  - Il peut y avoir plus d’une date de publication.
  - Il ne doit pas y avoir plus d’une date de dernière révision.
  - Il ne doit pas y avoir plus d’une date de création.

*Commentaire :*
Une date de référence de la ressource est une information représentative de la vie de la ressource (création, publication, révision), tandis que l’étendue temporelle fournit une indication de la période de temps couverte par la ressource, ce qui est un indicateur de l’actualité de la ressource.
La date de dernière révision n’a de sens que si elle se distingue de la date de création.

**_Exemple :_**
- Exemple 1, donnée mise à jour en continu : par exemple une donnée de la Banque du sous-sol qui est actualisée au fil de l’eau – techniquement tous les jours – verra le champ « Etendue temporelle » sous la forme : “1956 à maintenant”. La banque du sous-sol peut être publiée tous les ans, auquel cas sa date de publication sera celle de l’année en cours.
- Exemple 2, exemple de date de création : comment remplir la date d’un jeu de données créé à partir d’une numérisation d’une photo aérienne d’une date donnée? Il faudra saisir la date de numérisation comme date de création. Le champ généalogie fournira la date de la donnée de référence, ie. la photo-aérienne, et les explications de gestion de la mise à jour.
- Il est également possible de fournir un couple date/heure à la place d’une date. Dans ce cas, ce couple s’exprime sous la forme aaaa-mm-jjThh:mi:ss+hh:mi, où les quatre derniers chiffres correspondent au décalage avec l’heure UTC. En France métropolitaine, ces derniers chiffres sont donc +01:00 pendant l’heure d’hiver, et +02:00 pendant l’heure d’été.
  - Exemple : 2011-08-24T12:12:00+02:00 (c'est-à-dire, midi douze minutes, 0 secondes, le 24 août 2011, zone UTC+2)

**RECOMMANDATIONS NATIONALES :**
1. Il est recommandé de fournir au moins une date de référence (date de création, de dernière révision, ou de publication). (cf. VI.2 Dates de référence)
2. L’étendue temporelle (cf. VI.1) est un élément optionnel
