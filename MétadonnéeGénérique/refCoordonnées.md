## V.2. Référentiel de coordonnées
### V.2.1. Cas général : système de référence spatial
**EXIGENCE INSPIRE :**
- Description du ou des référentiels de coordonnées utilisés dans la série de données
- Cet élément est obligatoire et répétable.

**_Commentaires :_**
Le système de référence cité est celui des données accessibles par l’utilisateur.
Il est recommandé de se fixer sur un système de référence disponible indépendamment de tel ou tel logiciel.
Dans le cas de données indirectement géoréférencées (données statistiques), on ne peut pas remplir ce système de référence. C’est le système de référence des données géométriques associées qui permettra de remplir ce champ.

**RECOMMANDATIONS NATIONALES :**
1. L’identifiant du système de référence doit être fourni. Cet identifiant peut comporter un code et un espace de nommage.
2. Les codes à utiliser sont les codes EPSG.
3. Pour faciliter la compréhension de l’utilisateur, il est recommandé de fournir également le libellé descriptif du système de référence de coordonnées (ex : RGF 93).
4. Une URL doit être fournie pour permettre à l’utilisateur d’accéder à la description du code dans le registre EPSG. C’est cette URL qui fait référence. Elle peut être complétée par une information textuelle, dans le contenu du code.

**_Commentaires :_**
Une URL doit être fournie pour permettre à l’utilisateur d’accéder à la description du code dans le registre EPSG (ex : http://www.opengis.net/def/crs/EPSG/0/4258). C’est cette URL qui fait référence. Elle peut être complétée par une information textuelle, dans le contenu du code.
Le champ code est donc implémenté sous forme d’un élément Anchor, permettant de stocker l’URL d’accès au système de coordonnées dans le registre EPSG (http://www.opengis.net/def/crs/EPSG/0/4258), un libellé dans le code lui-même. L’espace de nommage (EPSG) est inutile dans ce cas.

**Exemple :**
- URL : http://www.opengis.net/def/crs/EPSG/0/4258
- Code : EPSG:4258





## V.2.2. Cas particulier : système de référence par identifiants géographiques
Pour les données référencées indirectement à un lieu (statistiques, etc…), les données qui servent de références spatiales (par exemple les communes, les adresses) doivent être renseignées comme système de référence spatial. Il est conseillé de préciser une date ou une version.

**_Exemple :_**
- Pour des données de qualité de l’air qui sont référencées via un code INSEE de commune :
  - URL : https://www.data.gouv.fr/fr/datasets/code-officiel-geographique-cog/
  - Code : COG 2019-03-14
- Pour des données de trafic référencées au tronçon :
  - URL : http://professionnels.ign.fr/bdtopo
  - Code : BDTopo ® Edition mars 2019
- Pour des données d’établissements recevant du public qui sont référencées via une adresse :
  - URL : https://adresse.data.gouv.fr
  - Code : BAN 2018-11-26

