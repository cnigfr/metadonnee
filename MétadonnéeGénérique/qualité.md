## VII.4. Eléments de qualité complémentaires
En complément des éléments de qualité décrits ci-dessus, d’autres résultats de mesure qualité peuvent être décrits. Ces résultats ne présentant aucune obligation dans le cadre de la Directive INSPIRE.    
Des fiches méthodologiques réalisées par le groupe QuadoGeo décrivent quelles mesures de qualité sont pertinentes en fonction du type de données [Note : Non publiées au jour de rédaction du guide.] Ces mesures constituent un registre national de mesures qualité





## VIII. Conformité
Les exigences de conformité seront remplies au moyen des éléments de métadonnées « spécification » et « degré ».

**_Commentaires :_**    
La conformité est une déclaration de la seule responsabilité du producteur et il n’est pas prévu de contrôler, en France, cette déclaration. Une série de données conforme remplit toutes les conditions posées par la spécification visée (voir VIII.1 Spécification). Le degré et la spécification de référence forment un couple. Ces deux éléments de métadonnées (spécification et degré) expriment la conformité des données (et non des métadonnées !) à une spécification. La première exigence de conformité vise la mise en oeuvre des règlements européens dits d’interopérabilité. La référence à des spécifications différentes comme celles du CNIG (PLU...) ou de la COVADIS est possible en complément. Concrètement, cela revient à créer une série de données à partir du gabarit de série de données fourni, par exemple, par la COVADIS, ou à comparer une série de données particulière au dit gabarit. Dans ce cas de figure, la conformité au règlement Interopérabilité est à décrire comme "conforme" (par nature).

**RECOMMANDATIONS NATIONALES :**  
1. Le règlement Interopérabilité INSPIRE doit obligatoirement faire partie des spécifications visées. Il sera renseigné comme décrit en Annexe A
2. Il est recommandé d’exprimer la conformité vis-à-vis du guide technique du thème considéré, selon l’Annexe B. La spécification référencée ici doit correspondre au thème INSPIRE indiqué dans les mots-clés.
3. En règle générale, il est conseillé de découper sa ressource en thèmes, afin de ne devoir se conformer qu’à un modèle de données INSPIRE à la fois (Par exemple, la BD Carto de l’IGN a été découpé en plusieurs ensembles de séries : BD Carto – Hydrographie, BD Carto – Réseau routier, BD Carto – Parcelles cadastrales, etc.).





## VIII.1. Spécification
**EXIGENCE INSPIRE :**  
Cet élément donne la référence des règles de mise en oeuvre adoptées en vertu de l’article 7, paragraphe 1, de la directive 2007/2/CE ou des autres spécifications auxquelles la ressource est conforme.
1. Il est possible de renseigner la conformité à plusieurs spécifications de données.
2. Cette indication inclut au moins le titre et une date de référence (date de publication, date de dernière révision ou de création) des spécifications auxquelles la ressource est conforme.

**_Commentaire :_**    
L’article 7, paragraphe 1, de la directive 2007/2/CE correspond aux modalités techniques de l’interopérabilité : il s’agit du règlement relatif à l’interopérabilité : règlement n°1253/2013 du 21 octobre 2013 modifiant et complétant le règlement n°1089/2010 du 23 novembre 2010. Dans le cas où une spécification autre qu’INSPIRE est citée, il est conseillé, si elle est disponible en ligne, d’ajouter l’URL menant à la spécification dans le champ ISO « explanation » (cf exemple XML ci-dessous).

**_Exemples :_**    
- Titre : Règlement n°1253/2013 date : 2013-10-21 type de date : publication 
- Titre : INSPIRE Data Specification on Cadastral Parcels - Guidelines v3.0.1 date : 2010-04-26 type de date : publication 
- Exemple pour un PLU conforme au règlement interopérabilité INSPIRE et au Géostandard CNIG.
  - Titre : Règlement n°1253/2013 date : 2013-10-21 type de date : publication
  - Titre : Standard de données COVADIS PLU et POS version 2.0 date : 2012-06-13 type de date : publication






## VIII.2. Degré
**EXIGENCE INSPIRE :**  
C’est le degré de conformité de la ressource par rapport à la spécification citée dans le précédent élément de métadonnées.

**RECOMMANDATION NATIONALE :**  
1. Pour chaque spécification visée en Annexe A et Annexe B, le degré de conformité (conforme/non conforme5) doit être indiqué.

**_Commentaire_**  
Les délais légaux de mise en oeuvre étant dépassés, la valeur "non évaluée” n'est plus utilisable.

