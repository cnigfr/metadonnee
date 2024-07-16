## II.7. Encodage

**EXIGENCE INSPIRE :**
Description du ou des concepts en langage machine spécifiant la représentation des objets de données dans un enregistrement, un fichier, un message, un dispositif de stockage ou un canal de transmission.
- Cet élément est obligatoire et répétable.

**_Commentaire :_**  
Les formats d’encodage par défaut d’INSPIRE sont ISO 19136 (GML 3.2.1) et les formats associés. Les formats d’encodage courants sont Shape, MIF-MID, etc…
Cet élément de métadonnée fait écho des spécifications de données INSPIRE, qui peuvent définir un encodage particulier selon les thèmes.

**RECOMMANDATIONS NATIONALES :**
1. Préciser en priorité le format d’échange (c'est-à-dire le format de distribution).
2. Il est obligatoire de fournir le nom et la version du format. Par exemple : nom : GML, version : 3.2.1. Si le numéro de version n’est pas connu, la valeur par défaut sera « inconnue ».
3. Des données produites selon les spécifications de données INSPIRE seront par défaut encodées selon ISO 19136 (GML) ou ISO/TS 19139. Les spécifications de données spécifieront si d’autres formats d’encodage sont acceptables selon les thèmes.
4. Dans le cadre de la mise en place des métadonnées, il est reconnu que les données décrites ne sont pas nécessairement déjà encodées selon les règles des spécifications de données INSPIRE. Dans ce cas, le format utilisé doit être décrit selon la recommandation 2.
5. Si la version est inconnue ou n’existe pas, utiliser les mots-clé “inapplicable” et “unknown”.

**Exemples :**
| Format                 |     versions       | inapplicable       |
|------------------------|--------------------|--------------------|
| nom : SHP              |   version          |                    |
| nom : MIF/MID          |   version : 4.5    |                    |
| nom : DXF              |   version : 2010   |                    |
| nom : DWG              |   version : 8      |                    |
| nom : GeoTIFF          |   version : 1.0    |                    | 


**Recommandation aux éditeurs**  
Il est recommandé que les outils d’édition des métadonnées mettent à disposition des utilisateurs un choix de formats (la liste sera établie dans le guide administrateur) pour lesquels les informations de nom et de version soient remplies automatiquement.

