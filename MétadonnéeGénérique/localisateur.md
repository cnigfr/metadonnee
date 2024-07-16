## II.4. Localisateur de la ressource

**EXIGENCE INSPIRE :**
Cet élément de métadonnée fournit un lien vers la ressource décrite elle-même, et/ou vers des informations complémentaires la concernant.
- Le domaine de valeur de cet élément est une chaîne de caractères couramment exprimée sous forme d’un localisateur uniforme de la ressource (URL).
- Cet élément répétable est obligatoire s’il existe une URL permettant d’obtenir davantage d’informations sur la ressource et/ou un accès à des services connexes.

**_Commentaires_**
Ce champ n’est pas optionnel mais conditionnel. Il devrait être considéré comme obligatoire. Un lien vers une page spécifique du site institutionnel de l’organisme responsable est un moyen de permettre d’accéder à plus d’informations sur la ressource si elle n’est pas accessible en ligne, par exemple en application d'une restriction d'accès public. S’il n’existe pas d’information complémentaire spécifique à la ressource accessible en ligne, un lien vers le site institutionnel est un pis-aller.
Il est également possible de fournir ici l’URL vers la série de données en téléchargement simple, ou la requête permettant le téléchargement de la ressource.

**RECOMMANDATIONS NATIONALES :**
1. Au moins un des liens doit être public (et non pointer vers un intranet).
2. Il est recommandé de renseigner cet élément avec un lien sur un enregistrement de métadonnées décrivant plus complètement la ressource ou à défaut, avec un lien sur une page dédiée du site institutionnel d’un organisme responsable de la ressource. Les deux types de lien peuvent être fournis en profitant du caractère répétable de l’élément.
3. Il est recommandé de fournir un lien vers les services de visualisation et de téléchargement si ces services sont connus.

**_Exemples :_**
- https://geobretagne.fr/geoserver/dreal_b/wfs?SERVICE=WFS&REQUEST=GetCapabilities
- http://www.geocatalogue.fr/Detail.do?id=1775

- **Cas particulier du lien vers les services**  
Quand il est connu, le localisateur de la ressource mentionne le lien vers les services diffusant la ressource.

**RECOMMANDATIONS NATIONALES :**
Le lien vers le service doit comporter les éléments suivants:
- **URL** : lien vers le service. A minima, renseigner le lien vers le point d’entrée/les capacités du service (GetCapabilities par exemple).
- **protocole** : le protocole doit préciser le type de service concerné selon une liste de valeurs prédéfinie (cf. tableau ci-dessous)
- **profil d’application** : permet de préciser le type de service INSPIRE
- **description** : fixée à « access point » (point d’accès).

**_Liste de valeurs pour la description :_**
| Identifiant                                                                       | Valeur                   |
|-----------------------------------------------------------------------------------|--------------------------|
| http://inspire.ec.europa.eu/metadata-codelist/OnLineDescriptionCode/accessPoint   | Access point             |
| http://inspire.ec.europa.eu/metadata-codelist/OnLineDescriptionCode/endPoint      | End point                |

**_Liste de valeurs pour le protocole :_**
| Identifiant                                                         | Valeur                             |
|---------------------------------------------------------------------|------------------------------------|
| http://www.opengis.net/def/serviceType/ogc/csw                      | OGC Catalogue Service for the Web  |
| http://www.opengis.net/def/serviceType/ogc/sos                      | OGC Sensor Observation Service     |
| http://www.opengis.net/def/serviceType/ogc/wcs                      | OGC Web Coverage Service           |
| http://www.opengis.net/def/serviceType/ogc/wfs                      | OGC Web Feature Service            |
| http://www.opengis.net/def/serviceType/ogc/wms                      | OGC Web Map Service                |
| http://www.opengis.net/def/serviceType/ogc/wmts                     | OGC Web Map Tile Service           |
| http://tools.ietf.org/html/rfc5023                                  | ATOM Syndication Format            |

**_Liste de valeurs possibles pour le profil d’application :_**
| Identifiant                                                                     | Valeur          |
|---------------------------------------------------------------------------------|------------------|
| http://inspire.ec.europa.eu/metadata-codelist/SpatialDataServiceType/download   | Download Service |
| http://inspire.ec.europa.eu/metadata-codelist/SpatialDataServiceType/view       | View Service     |


