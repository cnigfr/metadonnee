

## IX. Contraintes en matière d’accès et d’utilisation
Ce chapitre présente les différents types de contrainte pouvant être décrits dans une métadonnée. Un premier paragraphe détaille les exigences INSPIRE (IX.1), ce chapitre précise les valeurs attendues pour le champ Restrictions de l’accès public, et pour le champ conditions à l’accès et à l’utilisation. Un second paragraphe décrit d’autres types de contraintes qui peuvent être utilisées. Enfin des exemples sont fournis :
- Cas le plus simple
- Cas des données sous licence ouverte
- Cas des données tarifées
- Cas des données présentant une autre restriction d’accès public
- Ajout de restrictions d’usage
- Cas des données présentant des contraintes de type « sécurité »






### IX.1. Contraintes INSPIRE
**EXIGENCES INSPIRE :**
- Une contrainte en matière d’accès et d’utilisation est composée des deux éléments suivants :
  - Les conditions d’accès et d’utilisation décrivant les conditions applicables à l’accès et à l’utilisation des séries et des services de données géographiques, et, le cas échéant, les frais correspondants. Si aucune condition ne s’applique à l’accès à la ressource et à son utilisation, on utilisera la mention «aucune condition ne s’applique». Si les conditions sont inconnues, on utilisera la mention «conditions inconnues».
  - Les restrictions d’accès public c’est-à-dire les informations sur les restrictions à l’accès public et les raisons de ces restrictions lorsque les États membres restreignent l’accès public aux séries et aux services de données géographiques au titre de l'article L127-6 du code de l’environnement. S’il n’y a pas de restrictions concernant l’accès public, cet élément de métadonnées l’indiquera.
- Il doit y avoir au moins une condition contrainte en matière d’accès et d’utilisation exprimée pour chaque ressource.
- Au travers des différentes contraintes exprimées, il doit y avoir au moins l’expression d’une condition d’accès et d’utilisation et d’une indication sur les restrictions d’accès public.

**RECOMMANDATIONS NATIONALES :**
1. Il est recommandé de se conformer aux instructions du tableau ci-dessous.

**Tableau 1 Instructions pour renseigner les champs de métadonnées relatifs aux contraintes en matière d’accès et d’utilisation**

| Champs de Métadonnées                             |Contraintes de type légal                            | 
|---------------------------------------------------|-----------------------------------------------------|
| Condition d’accès et d’utilisation|Si une condition s’applique, par exemple les frais : une ou plusieurs chaînes de caractères. Si aucune condition ne s’applique, « aucune condition ne s’applique ».|
| Restriction d’accès public                        |Au moins une des valeurs proposées dans le Tableau 2 |








## IX.1.1. Restrictions d’accès public
**EXIGENCE INSPIRE :**  
- Cet élément exprime l’absence de restriction ou les restrictions lorsque les États membres restreignent l’accès public aux séries et aux services de données géographiques au titre de l'article L127-6 du code de l’environnement.
- Il doit prendre une des valeurs du Tableau 2.
- Selon le cas, il peut s’exprimer sous forme d’un ensemble d’éléments qui sont résumés dans le logigramme ci-dessous.

| N° | Valeur à saisir dans les métadonnées | Valeur à afficher dans l’interface |
|----|--------------------------------------|------------------------------------|
| 0  | Pas de restriction d’accès public    | Aucun des articles de la loi ne peut être invoqué pour justifier d’une restriction d’accès public. |
| 1  | L124-4-I-1 du code de l’environnement (Directive 2007/2/CE (INSPIRE), Article 13.1.a) | La confidentialité des travaux des autorités publiques, lorsque cette confidentialité est prévue par la loi. |
| 2  | L124-5-II-1 du code de l’environnement (Directive 2007/2/CE (INSPIRE), Article 13.1.b) | Les relations internationales, la sécurité publique ou la défense nationale. |
| 3  | L124-5-II-2 du code de l’environnement (Directive 2007/2/CE (INSPIRE), Article 13.1.c) | La bonne marche de la justice, la possibilité pour toute personne d’être jugée équitablement ou la capacité d’une autorité publique d’effectuer une enquête d’ordre pénal ou disciplinaire. |
| 4  | L124-4-I-1 du code de l’environnement (Directive 2007/2/CE (INSPIRE), Article 13.1.d) | La confidentialité des informations commerciales ou industrielles, lorsque cette confidentialité est prévue par la législation nationale ou communautaire afin de protéger un intérêt économique légitime, notamment l’intérêt public lié à la préservation de la confidentialité des statistiques et du secret fiscal. |
| 5  | L124-5-II-3 du code de l’environnement (Directive 2007/2/CE (INSPIRE), Article 13.1.e) | Les droits de propriété intellectuelle. |
| 6  | L124-4-I-1 du code de l’environnement (Directive 2007/2/CE (INSPIRE), Article 13.1.f) | La confidentialité des données à caractère personnel et/ou des fichiers concernant une personne physique lorsque cette personne n’a pas consenti à la divulgation de ces informations au public, lorsque la confidentialité de ce type d’information est prévue par la législation nationale ou communautaire. |
| 7  | L124-4-I-3 du code de l’environnement (Directive 2007/2/CE (INSPIRE), Article 13.1.g) | Les intérêts ou la protection de toute personne qui a fourni les informations demandées sur une base volontaire sans y être contrainte par la loi ou sans que la loi puisse l’y contraindre, à moins que cette personne n’ait consenti à la divulgation de ces données. |
| 8  | L124-4-I-2 du code de l’environnement (Directive 2007/2/CE (INSPIRE), Article 13.1.h) | La protection de l’environnement auquel ces informations ont trait, comme par exemple la localisation d’espèces rares. |

Attention, l’article L 124-4-I du code de l’environnement (cas n° 1, 4, 6, 7 et 8) ne peut pas être invoqué pour justifier une restriction d’accès public à des informations concernant des émissions dans l’environnement (article L 127-6 du même code). Selon L127-8-IV du code de l’environnement, une restriction d’accès public au titre de l’article L124-5-II 1er ou 2ème alinéa du code de l’environnement (i.e. cas n°2 ou 3) induit une restriction de partage de la ressource entre autorités publiques.







## IX.1.2. Conditions applicables à l’accès et à l’utilisation
**EXIGENCE INSPIRE :**  
Cet élément de métadonnées définit les conditions applicables à l’accès et à l’utilisation des séries et des services de données géographiques, et, le cas échéant, les frais correspondants.
- Au fil des différents ensembles de contraintes en matière d’accès et d’utilisation, il doit y avoir au moins une instance de cet élément.
- Cet élément doit avoir une valeur textuelle. Les valeurs suivantes sont imposées dans les cas particuliers prévus par INSPIRE :
  - aucune condition ne s’applique si aucune condition ne s’applique à l’accès à la ressource et à son utilisation ;
  - conditions inconnues si les conditions sont inconnues.
- Cet élément fournira aussi des informations sur tout frais éventuel à acquitter pour avoir accès à la ressource et l’utiliser, le cas échéant, ou fera référence à un localisateur de ressource uniforme (Uniform Resource Locator, URL) où il sera possible de trouver des informations sur les frais.

**RECOMMANDATIONS NATIONALES :**
1. Lorsqu’elles existent, il est obligatoire de diffuser les conditions applicables à l’accès et à l’utilisation de la ressource.
2. Pour les administrations, l'article 1er de la loi "Pour une République numérique" impose l'ouverture des données publiques. Elles sont gratuites au sein de l’État, entre l’État et ses EPA ou entre EPA. Cela conduira à retenir la valeur “aucune condition d’accès ne s’applique”. Il conviendra d'ajouter la mention “Utilisation libre sous réserve de mentionner la source (a minima le nom du producteur) et la date de sa dernière mise à jour.”
3. Il est recommandé d’éviter la valeur “conditions inconnues”.
4. Lorsqu’elles existent, il est recommandé d’exprimer les conditions financières d’accès et d’utilisation de la ressource.
5. Il est recommandé que les conditions financières d’accès et d’utilisation de la ressource soient documentées dans une instance dédiée de cet élément.






## IX.2. Autres contraintes
Il est possible de formuler 3 grandes familles de conditions d’accès et d’usage :
- Les contraintes légales, dont font partie les contraintes INSPIRE, qui peuvent aussi comprendre d’autres contraintes.
- Les contraintes de sécurité, dans le cas de la défense nationale. Par exemple, les métadonnées d'une série de données réalisée dans le cadre d'un projet d'intervention des forces françaises sont non diffusables.
- Les contraintes d’usage (par exemple : données maritimes impropres à la navigation).

Les métadonnées d’une ressource peuvent donc exprimer tout un ensemble de contraintes en matière d’accès et d’utilisation couvrant ces 3 grandes familles de contraintes.

Contraintes de type légales (accès ou utilisation)|Contraintes de type sécurité| Information sur le type d’usage|
|-------------------------------------------------|----------------------------|--------------------------------|
Une ou plusieurs des valeurs proposées dans le Tableau 3 qui n’ont pas de base légale dans le cadre d’INSPIRE ou qui ne peuvent pas être interprétées comme telle ;Une ou plusieurs chaînes de caractères complémentaires apportant des précisions sur les restrictions. Une ou plusieurs chaînes de caractères complémentaires apportant des précisions sur les restrictions.|Une ou plusieurs chaînes de caractères explicitant les conditions à satisfaire pour accéder à la ressource.Dans le cas de la défense nationale, une des valeurs suivantes qui induit une restriction d’accès public : (Restreint, Confidentiel, Secret, Très secret) Dans ce cas, il est recommandé également d’expliciter la restriction d’accès public au travers d’une contrainte légale faisant référence à L124-5-II-1 du code de l’environnement (Cf. Erreur ! Source du renvoi introuvable., cas n°2).|Une ou plusieurs chaînes de caractères explicitant les restrictions d’accès et d’utilisation, par exemple, “impropre à la navigation”.|

**Tableau 3 Valeurs pouvant apparaître dans les restrictions d’accès public mais insuffisantes à en établir la base légale**

| Valeur à indiquer dans les métadonnées | Nature de la restriction |
|----------------------------------------|--------------------------|
| Copyright                              | Il existe un copyright associé à la ressource. |
| Brevet                                 | Il existe un brevet lié à la ressource. |
| Brevet en cours                        | Un dépôt de brevet lié à la ressource a été réalisé mais le brevet n’a pas encore été obtenu. |
| Marque déposée                         | Il existe une marque déposée liée à la ressource. |
| Licence                                | L’accès à la ressource est soumis à licence. |
| Droit de propriété intellectuelle      | Les droits de propriété intellectuelle peuvent contraindre l’accès à la ressource. |
| Restreint                              | Il existe une restriction d’accès à la ressource. Cette valeur est à utiliser dès qu’une restriction d’accès public est exprimée au travers d’une des valeurs proposées dans le Tableau 2. |






## IX.3. Exemples et mise en oeuvre
Selon l’outil éditeur de métadonnées utilisé, deux approches sont possibles :
- Soit l’éditeur utilisé propose une interface basée sur INSPIRE. Dans ce cas, deux champs s’offrent à l’utilisateur, « Condition d’accès et d’utilisation » et « Restriction d’accès public ». Le champ « Condition d’accès et d’utilisation » pourra être rempli selon les recommandations du paragraphe IX.2 Conditions applicables à l’accès et à l’utilisation. Le champ « Restriction d’accès public » sera rempli avec une des valeurs du Tableau 2.
- Soit l’éditeur utilisé propose une interface de type ISO. Dans ce cas, 3 familles de contraintes s’offrent à l’utilisateur : les contraintes légales (MD_LegalConstraint), contraintes de sécurité (MD_SecurityConstraint) et autres contraintes (MD_Constraint) (cf. les colonnes du Tableau 1). Pour chacune de ces familles, plusieurs champs de métadonnées sont possibles. Les exemples ci-dessous précisent comment remplir ces champs.

| Type de contrainte ISO | Champ ISO utilisé | Elément de MD INSPIRE correspondant | Exemple de Valeur |
|------------------------|--------------------|-------------------------------------|-------------------|
|Contraintes légales(MD_LegalConstraints). Contraintes légales (MD_LegalConstraints)|Contrainte d’usage useConstraints (CharacterString) Limitations d’usage. otherConstraints (CharacterString). Contraintes d’accès accessConstraints (CharacterString). Autres contraintes otherConstraints (CharacterString)|Conditions applicable à l’accès et l’utilisation A remplir selon les instructions du paragraphe IX.2. Conditions applicable à l’accès et l’utilisation. A remplir selon les instructions du paragraphe IX.2. Restriction d’accès public. Restriction d’accès public|otherRestrictions. aucune condition ne s’applique. otherRestrictions. Pas de restriction d’accès public|

Le champ « accesConstraint » est fixé à « otherRestrictions » pour pouvoir débloquer le champ « otherConstraints » 






## IX.3.1. Cas le plus simple
Dans ce cas, il n’y a pas de restrictions d’accès public à la donnée. L’élément INSPIRE « Conditions applicable à l’accès et l’utilisation » est fixé à « aucune condition ne s’applique»
7 Il est nécessaire d’invoquer l’article du code de l'environnement au travers de la valeur proposée au Tableau 2 (cas n°5) pour induire une restriction d’accès public liée à ce droit de propriété intellectuelle.
Guide de saisie des éléments de métadonnées INSPIRE – Appliqué aux données v2.0
CNIG Page 68/93
et on indique qu’il n’y a pas de restrictions à l’accès public en ajoutant la valeur correspondante du Tableau 2 (« Pas de restriction d’accès public»)




## IX.3.2. Cas des données sans licence ou sous licence ouverte
En cas d'absence de licence, la donnée est sous licence ouverte (d'Etalab).
Par exemple : un atlas de zone inondable réalisé par la DREAL Pays-de-Loire, sous licence ouverte.

Dans le cas des données ouvertes, il est recommandé d’ajouter à l’information « pas de restriction d’accès public » une description du type de licence (versionné) et un lien vers le texte de la licence lui-même. Enfin, il est recommandé d’ajouter une instance du champ useConstraints utilisant la valeur « license » de la liste de code.

| Type de contrainte ISO | Champ ISO utilisé | Elément de MD INSPIRE correspondant | Exemple de Valeur |
|------------------------|--------------------|-------------------------------------|-------------------|
|Contraintes légales(MD_LegalConstraints). Contraintes légales (MD_LegalConstraints)|Contrainte d’usage useConstraints (CharacterString) Limitations d’usage. otherConstraints (CharacterString). Contraintes d’accès accessConstraints (CharacterString). Autres contraintes otherConstraints (CharacterString)|Conditions applicable à l’accès et l’utilisation Conditions applicable à l’accès et l’utilisation. Restriction d’accès public. Restriction d’accès public. Restriction d’accès public|otherRestrictions. Licence OdBL + version et/ou date + URL vers le texte de la license. license. otherRestrictions. Pas de restriction d’accès public|






## IX.3.3. Cas des données tarifées  
Dans ce cas, la « restriction à l’accès public » est soumise à des « conditions d’accès et d’utilisation » précisant comment se procurer les données, à quel tarif, sous quelles conditions et quelles en sont les conditions d’utilisation.

| Type de contrainte ISO | Champ ISO utilisé | Elément de MD INSPIRE correspondant | Exemple de Valeur |
|------------------------|--------------------|-------------------------------------|-------------------|
|Contraintes légales(MD_LegalConstraints).|Contrainte d’usage useConstraints (CharacterString) Limitations d’usage. otherConstraints (CharacterString). Contraintes d’accès accessConstraints (CharacterString). Autres contraintes otherConstraints (CharacterString)|Conditions applicable à l’accès et l’utilisation Conditions applicable à l’accès et l’utilisation. Restriction d’accès public. Restriction d’accès public. Restriction d’accès public|otherRestrictions. Données soumises à une tarification du droit d’utilisation. Ces deux éléments (tarifs et restrictions) sont décrits dans le document disponible ici : [url]. license. otherRestrictions. L124-5-II-3 du code de l’environnement (Directive 2007/2/CE (INSPIRE), Article 13.1.e)|





## IX.3.4. Cas des données présentant une autre restriction d’accès public
Par exemple : les relevés des traces des ours des Pyrénées.

Dans ce cas, une instance du champ ISO «MD_LegalConstraint>accessConstraint » est fixé à « restreint ». Une autre instance de ce même champ est fixée à « autres restrictions », et la valeur appropriée de la liste du tableau 2 est ajoutée dans le champ « otherConstraint ». Un champ otherConstraints (correspondant à l’élément INSPIRE « Conditions applicable à l’accès et l’utilisation » doit être ajouté pour préciser sous quelle conditions il est possible d’accéder à la donnée.)

| Type de contrainte ISO | Champ ISO utilisé | Elément de MD INSPIRE correspondant | Exemple de Valeur |
|------------------------|--------------------|-------------------------------------|-------------------|
|Contraintes légales(MD_LegalConstraints). Contraintes légales (MD_LegalConstraints)|Contraintes d’accès accessConstraints (CharacterString). Autres contraintes otherConstraints (CharacterString). Contraintes d’accès accessConstraints (CharacterString). Contraintes d’accès accessConstraints (CharacterString). Autres contraintes otherConstraints (CharacterString)|Conditions applicable à l’accès et l’utilisation Conditions applicable à l’accès et l’utilisation. Restriction d’accès public. Restriction d’accès public. Restriction d’accès public|otherRestrictions. Seules les conditions suivantes peuvent permettre l’accès à la ressource : <conditions>. restricted. otherRestrictions. L124-4-I-2 du code de l’environnement (Directive 2007/2/CE (INSPIRE), Article 13.1.h)|





## IX.3.5. Ajout de restrictions d’usage  
Aux deux exemples précédents, on peut ajouter l’expression de restrictions d’usage. (Par exemple : « données impropres à la navigation » ou « Limites d'utilisation dues à l'échelle de saisie (1:1000)”). Dans ce cas, et pour distinguer ce type de restrictions des limitations légales ou contractuelles, on utilise une instance du champ MD_Constraint>useLimitation.  

Ce cas ne peut pas exister seul, mais s’ajoute nécessairement à un des autres exemples.

| Type de contrainte ISO | Champ ISO utilisé | Elément de MD INSPIRE correspondant | Exemple de Valeur |
|------------------------|--------------------|-------------------------------------|-------------------|
Contraintes générales  (MD_Constraints)| Limitations d’usage  useLimitation (CharacterString)|Conditions applicable à l’accès et l’utilisation|Seules les conditions suivantes peuvent permettre l’accès à la ressource : <conditions>|
