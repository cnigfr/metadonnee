## IV. Mots clés

**EXIGENCE INSPIRE :**
La catégorie thématique étant trop imprécise pour des recherches détaillées, les mots clés permettent d’affiner la recherche en texte intégral et permettent une recherche structurée.
- Si le mot clé provient d’un vocabulaire contrôlé (thésaurus), le nom et la date de publication de celui-ci doivent être précisés.
- Il est obligatoire pour les données (séries et ensembles de séries) dans le champ d’INSPIRE de fournir au moins un mot clé précisant le thème INSPIRE concerné par la donnée, comme défini dans le thésaurus GEMET des thèmes INSPIRE (« GEMET – INSPIRE themes, version 1.0 », du 2008-06-01, cf. http://www.eionet.europa.eu/gemet/inspire_themes?langcode=fr).
- D’autres mots clés peuvent être fournis en complément.

*Commentaires :*
En résumé, il est donc demandé un jeu de mots-clés obligatoire : le ou les thèmes INSPIRE, et il est possible de fournir des mots complémentaires : un ou des mot(s)-clé(s) recommandé(s) issus de thésaurus métiers validés ou du thésaurus GEMET-Concepts, ou encore un ou des mot(s)-clé(s) libre(s).
Les thésaurus métiers validés permettent d'atteindre une meilleure interopérabilité sémantique, et donc d'être plus efficace, mais sont rarement mis à jour. Les mots-clés libres permettent ainsi de prendre en compte les nouveautés (ex. : permis éolien).

|Mot clé      | Thème INSPIRE (obligatoire)  | Mots-clés recommandés (facultatifs)| Mots-clés libres (facultatifs)|
|-------------|------------------------------|------------------------------------|-------------------------------|
Valeur du mot-clé| Thème INSPIRE, comme défini dans le thésaurus suivant| Autre mot-clé provenant d’un thésaurus|Tout autre mot clé|
Thésaurus (nom, date de publication)|Nom : [GEMET – INSPIRE themes](https://www.eionet.europa.eu/gemet/fr/inspire-themes/), version 1.0 Date de publication : 2008-06-01|Autre thésaurus dont est extrait le mot clé|
Exemple|Valeur du Mot-clé : Hydrologie Thésaurus : nom : GEMET – INSPIRE themes, version 1.0 Date de publication : 2008-06-01|Valeur du Mot-clé : hydrologie Thésaurus : nom : GEMET-Concepts, version 3.1, Date de publication : 2012-07-20|Valeur du Mot-clé : servitudes d'utilité publique|

*_Exemple pour un document d'urbanisme :_* 
  - Mot-clé obligatoire : (Thème INSPIRE) usage des sols
  - Mot-clé(s) complémentaire(s) : 
    - 54321 (thésaurus : Code officiel géographique au 1er janvier 2019)
    - PLU (thésaurus : Types de documents d’urbanisme)
    - document d’urbanisme (thésaurus : GEMET-Concepts, http://www.eionet.europa.eu/gemet/concept?cp=6285&langcode=fr&ns=1)
  - Mot-clé(s) libre(s) : « PLU Plan Local d’urbanisme » et « planification » (puisque le thésaurus ne propose ni ce niveau de détail ni les synonymes) et « données ouvertes ».

*_Exemple pour un Plan cadastral informatisé_*
  - Mot-clé obligatoire : (Thème INSPIRE) Parcelles cadastrales.
  - Mot-clé(s) complémentaire(s) : "bâtiment" (GEMET-Concepts, http://www.eionet.europa.eu/gemet/concept?cp=1029&langcode=fr&ns=1)





## IV.1. Mots clé obligatoire
### IV.1.1. Thème INSPIRE

**EXIGENCE INSPIRE :**
- Le thésaurus GEMET des thèmes INSPIRE est multilingue. Le langage dans lequel les thèmes INSPIRE sont exprimés doit donc concorder avec le ou les langages des métadonnées.
- Cet élément est répétable.

**_Commentaires :_**  
Les séries de données peuvent correspondre à plusieurs thèmes, et le règlement autorise les rattachements multiples. Toutefois, la conformité aux spécifications INSPIRE est établie thème par thème (cf. partie VIII). Cela incite à un rattachement à un thème unique.
Dans le cas d’une donnée concernant plusieurs thèmes, on pourra fournir plusieurs mots clés correspondant à ces thèmes à la condition de ne pas les associer au thésaurus GEMET– INSPIRE themes.
Attention, c’est la présence du thème INSPIRE, associé au thésaurus GEMET-INSPIRE themes, qui est prise en compte pour distinguer des métadonnées relevant de la Directive INSPIRE de métadonnées décrivant des ressources hors du champ d’INSPIRE. Dans le cas de données sortant du cadre d’INSPIRE il est donc indispensable de ne pas renseigner le thème INSPIRE, et donc de ne pas utiliser le thésaurus « GEMET – INSPIRE themes, version 1.0 » du 2008-06-01.

**RECOMMANDATIONS NATIONALES :**
1. Il est recommandé de ne rattacher une ressource qu’à un seul thème INSPIRE.
2. INSPIRE n’identifie pas explicitement d’élément de métadonnées « Thème INSPIRE » mais induit son existence par les exigences formulées de manière générale sur la présence de mots-clés. La recommandation est donc de considérer le thème INSPIRE comme un élément à part entière.
3. Il est recommandé de ne pas fournir cet élément de métadonnées pour les ressources qui ne sont pas dans le champ d’INSPIRE (des données d’accidentologie, par exemple) étant entendu que pour les ressources dans le champ d’INSPIRE, cet élément est obligatoire.

**Exemple :**
Zones à risque naturel




## IV.1.2. Données prioritaires

Les données prioritaires sont "des séries de données géographiques déjà utilisées par les États membres aux fins de la communication d’informations dans le cadre de la législation environnementale de l’Union recensées dans le rapport de la Commission «Mesures visant à rationaliser la communication d’informations relatives à l’environnement»". Concrètement, ce sont les données des rapportages européens.

**EXIGENCE INSPIRE :**
- Les données prioritaires doivent être documentées avec un mot-clé spécifique. Cet élément est obligatoire pour les jeux de données prioritaires et non répétable.
- Les valeurs possibles des mots clés pour les données prioritaires sont celles figurant dans un registre fourni par la Commission : http://inspire.ec.europa.eu/metadata-codelist/PriorityDataset

**_Exemple :_**
« Agglomérations (Directive Bruit) »




## IV.1.3. Données de couverture nationale/régionale
Les données de couverture nationale ou régionale [de référence] sont identifiées par le CNIG3.

**EXIGENCE INSPIRE :**
- Les données de couverture nationale ou régionale doivent être documentées avec un mot-clé spécifique. Cet élément est obligatoire pour ces jeux de données et non répétable.
- Les valeurs possibles des mots clés pour ces données sont celles figurant dans un registre fourni par la Commission : http://inspire.ec.europa.eu/metadata-codelist/SpatialScope

**_Exemple :_**
- « nationales »
- Les données prioritaires (cf. IV.1.2) sont également des données d’importance nationale. La métadonnées doit donc comporter les deux types de mots-clés




## IV.2. Mots clés complémentaires
Il est conseillé de fournir des mots-clés complémentaires. Ces mots-clés peuvent être associés à des vocabulaires contrôlés définissant ces mots-clés.

**EXIGENCE INSPIRE :**
- Les valeurs des mots clés sont du texte libre.

**RECOMMANDATIONS NATIONALES : FORMATAGE DES MOTS CLES**
1. Les mots-clés libres doivent être fournis en minuscule, accentués, au pluriel.
2. Il faut éviter les acronymes ou les sigles (ex : SUP) sauf s'ils viennent compléter les termes littéraux, et même s'ils sont courant dans la profession.
3. Dans le cas de données sous licence ouverte, il convient d’ajouter un mot-clé «données ouvertes».

**_Commentaires_**  
Des exemples de thésaurus métier ou de vocabulaires contrôlés sont : Ecoplanet pour les métiers de l'environnement, Urbamet pour l'urbanisme, glossaire EauFrance pour l'eau.
Il faut éviter les mots-clés trop génériques qui renverraient des réponses trop dispersées. Par exemple, pour "servitudes d'utilités publiques", éviter : Utilités, Publiques.
Quand les acronymes sont courants dans la profession, il est prudent de mettre l’expression littérale et l’acronyme, ne sachant pas ce que va rechercher l’utilisateur.
L’information « données ouvertes » servira à des fins d’indexation par les portails régionaux et nationaux (ex. : data.gouv.fr), il est donc important de conserver la casse proposée.

**_Exemple :_**
- « plan de développement urbain », « planification et développement urbain » provenant du thésaurus GEMET-Concept.
- « données ouvertes »
- « études et prévention des risques naturels »
