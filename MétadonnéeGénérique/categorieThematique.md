### III.1. Catégorie thématique

**EXIGENCE INSPIRE :**
La catégorie thématique est un système de classification de haut niveau qui permet de regrouper et de chercher par thème les ressources de données géographiques disponibles.
- Une ou plusieurs valeurs parmi les 19 catégories thématiques ISO listées à <span style="text-decoration: underline; color: blue;">la partie D.2 du règlement</span> sur les métadonnées INSPIRE doivent être fournies (élément obligatoire et répétable).

| 	Nom de concept (en anglais)	| Code	| Définition |
|----------------------|-------------------------|-------------------------------------------------|
|	farming (élevage) |	farming	| élevage d'animaux et/ou culture de plantes EXEMPLES Agriculture, irrigation, aquaculture, plantations, élevage de troupeaux, nuisibles et maladies affectant les récoltes et le bétail. |
|	biota (biote) |	biota |	flore et/ou faune dans l'environnement naturel EXEMPLES Vie sauvage, végétation, biologie, écologie, lieux sauvages, vie marine, marécages, habitat |
|boundaries (limites)	|boundaries	|descriptions légales d'un pays, limites maritimes EXEMPLES Limites politiques et administratives, mers territoriales, zone économique exclusive, zones de sécurité portuaire|
|climatologyMeteorologyAtmosphere (climatologie, météorologie et atmosphère)	|climatologyMeteorologyAtmosphere	|processus et phénomènes dans l'atmosphèreEXEMPLES Couverture de nuages, météorologie, climat, conditions atmosphériques, changements climatiques, précipitation.|
|economy (économie)	|economy	|activités, conditions économiques et emploi EXEMPLES Production, main-d'œuvre, revenus, commerce, industrie, tourisme et écotourisme, industrie forestière, pêche, chasse commerciale ou de subsistance, exploration et exploitation des ressources telles que les minéraux, le pétrole et le gaz.|
|elevation (élévation)	|elevation	|hauteur au-dessus ou en dessous d'une référence verticale EXEMPLES Altitude, bathymétrie, modèles numériques d'élévation, pentes, produits dérivés.
|environment (environnement)	|environment	|ressources, protection et conservation de l'environnement EXEMPLES Pollution environnementale, stockage et traitement des déchets, évaluation de l'impact sur l'environnement, surveillance des risques pour l'environnement, réserves naturelles, paysage|
|geoscientificInformation (informations géoscientifiques)	|geoscientificInformation	|informations se rapportant aux sciences terrestres EXEMPLES Caractéristiques et processus géophysiques, géologie, minéraux, sciences traitant de la composition, de la structure et de l'origine des roches terrestres, risques de tremblements de terre, activité volcanique, glissement de terrains, informations sur la gravité, sols, pergélisol, hydrogéologie, érosion|
|health (santé)	|health	|santé, services de santé, écologie humaine et sécurité EXEMPLES Epidémies et maladies, facteurs affectant la santé, hygiène, abus de substance, santé physique et mentale, services de santé|
|imageryBaseMapsEarthCover (imagerie, cartes de base et occupation du sol	|imageryBaseMapsEarthCover	|cartes de base EXEMPLES Occupation du sol, cartes topographiques, imagerie, images non classées, annotations|
|intelligenceMilitary (intelligence militaire)	|intelligenceMilitary	|bases, structures, activités militaires EXEMPLES Casernes, champs de manœuvres, transport militaire, collecte d'informations|
|inlandWaters (eaux intérieures)	|inlandWaters	|caractéristiques des eaux intérieures, systèmes de drainage et leurs caractéristiques EXEMPLES Rivières et glaciers, lacs salés, plans d'utilisation de l'eau, barrages, courants, crues, qualité de l'eau, informations hydrologiques|
|location (position)	|location	|informations de position et services EXEMPLES Adresses, réseaux géodésiques, points de contrôle, zones et services postaux, noms de lieux|
|oceans (océans)	|oceans	|types et caractéristiques des eaux salées (à l'exception des eaux intérieures)EXEMPLES Marées, tsunamis, informations côtières, récifs|
|planningCadastre (planification et cadastre)	|planningCadastre	|informations utilisées pour des actions appropriées à une utilisation future du pays EXEMPLES Cartes d'aménagement, plans d'occupation des sols, levés cadastraux, propriétés foncières|
|society (société)	|society	|caractéristiques de sociétés et de culturesEXEMPLES Accords, anthropologie, archéologie, enseignement, croyances traditionnelles, us et coutumes, données démographiques, zones et activités de loisirs, évaluation des impacts sociaux, crime et justice, recensement|
|structure (structure)	|structure	|construction réalisée par l'hommeEXEMPLES Immeubles, musées, églises, usines, logements, monuments, magasins, tours|
|transportation (transport)	|transportation	|moyens et aides pour acheminer des personnes et/ou des biensEXEMPLES Routes, aéroports, pistes d'atterrissage, voies maritimes, tunnels, cartes nautiques, emplacements de véhicules ou de vaisseaux, cartes aéronautiques, voies ferrées|
|utilitiesCommunication (utilitaires de communication)	|utilitiesCommunication	|systèmes de distribution énergétique, d'eau et d'évacuation des eaux usées et infrastructure et services de communicationEXEMPLES Hydroélectricité, sources géothermiques, solaires et nucléaires d'énergie, purification et distribution de l'eau, collecte et mise au rebut des déchets, distribution d'électricité et de gaz, communication de données, télécommunication, radio, réseaux de communication|

**_Commentaires :_**  
Cet élément de métadonnées vient de la norme ISO 19115. Une correspondance entre les catégories thématiques ISO et les thèmes INSPIRE a été établie dans <span style="text-decoration: underline; color: blue;">la partie D.2 du règlement</span> Métadonnées.   
Le tableau ci-dessous « inverse » la clause D2 et présente pour chacun des thèmes INSPIRE les catégories ISO correspondantes. Cependant, ce tableau est fourni à titre indicatif et rien n’empêche de choisir d’autres valeurs de catégorie ISO si celle proposée pour le thème ne convient pas ou doit être complétée. Les valeurs à indiquer dans les métadonnées sont fournies dans la colonne « Catégorie ISO ».

| Thème INSPIRE                                 | Catégorie ISO                                   |
|-----------------------------------------------|-------------------------------------------------|
| Annexe 1                                                                                         |
| Référentiel de coordonnées                     | Au choix                                        |
| Système de maillage géographique               | Au choix                                        |
| Dénominations géographiques                    | Localisation (location)                         |
| Unités administratives                         | Limites (boundaries)                            |
| Adresses                                      | Localisation (location)                         |
| Parcelles cadastrales                          | Planification/Cadastre (planningCadastre)      |
| Réseaux de transport                           | Transport (transportation)                      |
| Hydrographie                                   | Eaux intérieures (inlandWaters)                 |
| Sites protégés                                 | Environnement (environment)                     |
| Annexe 2                                                                                         |
| Altitude                                      | Altitude (elevation)                            |
| Occupation des terres                          | Imagerie/Cartes de base/Occupation des terres (imageryBaseMapsEarthCover) |
| Ortho-imagerie                                | Imagerie/Cartes de base/Occupation des terres (imageryBaseMapsEarthCover) |
| Géologie                                      | Informations géoscientifiques (geoscientificInformation) |
| Annexe 3                                                                                                 |
| Unités statistiques                            | Limites (boundaries)                            |
| Bâtiments                                     | Structure (structure)                          |
| Sols                                          | Informations géoscientifiques (geoscientificInformation) |
| Usage des sols                                | Planification/Cadastre (planningCadastre)      |
| Santé et sécurité des personnes               | Santé (health)                                  |
| Services d’utilité publique et services publics | Services d’utilité publique/Communication (utilitiesCommunication) |
| Installations de suivi environnemental        | Structure (structure)                          |
| Lieux de production et sites industriels      | Structure (structure)                          |
| Installations agricoles et aquacoles           | Agriculture (farming)                          |
| Répartition de la population — Démographie    | Société (society)                              |
| Zones de gestion, de restriction ou de réglementation et unités de déclaration | Planification/Cadastre (planningCadastre) |
| Zones à risque naturel                         | Informations géoscientifiques (geoscientificInformation) |
| Conditions atmosphériques                      | Climatologie/Météorologie/Atmosphère (climatologyMeteorologyAtmosphere) |
| Caractéristiques géographiques météorologiques | Climatologie/Météorologie/Atmosphère (climatologyMeteorologyAtmosphere) |
| Caractéristiques géographiques océanographiques | Océans (oceans)                                |
| Régions maritimes                              | Océans (oceans)                                |
| Régions biogéographiques                       | Biote (biota)                                  |
| Habitats et biotopes                           | Biote (biota)                                  |
| Répartition des espèces                        | Biote (biota)                                  |
| Sources d’énergie                              | Économie (economy)                             |
| Ressources minérales                           | Économie (economy)                             |

**RECOMMANDATIONS NATIONALES :**
1. Il est important d’associer la ressource aux thématiques les plus pertinentes.



