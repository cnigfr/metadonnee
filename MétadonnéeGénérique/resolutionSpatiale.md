## VII.2. Résolution spatiale
**EXIGENCE INSPIRE :**  
La résolution spatiale décrit le niveau de détail de la ressource.
- Elle est exprimée comme un ensemble de valeurs de distance de résolution allant de zéro à plusieurs valeurs ou exprimée en échelles équivalentes :
  - Une échelle équivalente :
    - est exprimée sous la forme d’une valeur entière correspondant au dénominateur de l’échelle.
    - est utilisée en général pour les cartes ou les produits dérivés de cartes.
  - Une distance de résolution :
    - est exprimée sous la forme d’une valeur associée à une unité de longueur.
    - est utilisée en général pour des données maillées et des produits dérivés d’imagerie.
- Cet élément répétable est obligatoire pour les séries de données et les ensembles de séries de données pour lesquels une échelle équivalente ou une distance de résolution peuvent être indiquées.

**_Commentaire :_**    
Extrait du document “La qualité des données géographiques”, CERTU, 2010 : “cette grandeur est exprimée soit par une échelle pour les données de type vecteur, soit par une distance pour les données de type raster. (...) La notion d’échelle proposée par INSPIRE pour qualifier la résolution spatiale d’un lot de données vecteur est également très subjective et sujette à interprétation.” La plupart du temps, pour une donnée vectorielle, cela revient à noter l’échelle de la série de données source. A défaut, il s’agit de l’échelle optimum d’emploi de la donnée.

**RECOMMANDATION NATIONALE :**  
1. La résolution spatiale doit être fournie pour toutes les données géographiques (séries et ensemble de séries). Une exception est faite pour les données statistiques.

**_Exemple :_**  
- pour une échelle équivalente :
  - dénominateur : 5000
- pour une distance de résolution :
  - valeur : 2
  - unité de mesure : m

**_Contre-exemples :_**    
- 1/50000  
- 50 000  
- 50000e  
- 50000eme  
- 2 mètres  
