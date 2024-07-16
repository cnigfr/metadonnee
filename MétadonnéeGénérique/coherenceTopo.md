## VII.3. Cohérence topologique
**EXIGENCE INSPIRE :**  
Exactitude des caractéristiques topologiques explicitement encodées de la série de données, telles que décrites dans le champ d’application.
- Cet élément n'est obligatoire que si la série de données comprend des types issus du modèle générique de réseau («Generic Network Model») et n’assure pas la topologie du réseau (c'est-à-dire à la connectivité des lignes centrales).

**_Commentaires :_**    
En pratique, ne sont concernées que les données respectant les spécifications de données INSPIRE et rentrant dans un cas de modèle de réseau (hydrographie, transport, services d’utilité publique). Les guides accompagnant les guides techniques des thèmes INSPIRE définissent les mesures à appliquer, selon les thèmes. Par exemples :
- nombre de superpositions invalides,
- nombre de noeuds pendants (undershoot, overshoot),
- nombre d’auto-intersections,
- nombre d’auto-superpositions.
La plupart des séries de données ne seront donc pas concernées.

**_Exemple :_**    
Par exemple, pour une série de données du thème Hydrographie, le résultat de la mesure qualité « Number of faulty point-curve connections » (nombre de connexions point-courbe erronées) sera exprimé ainsi (selon une traduction du premier tableau de la clause 7.2.3 du guide technique du thème Hydrographie) :
- Nom de la mesure : nombre de connexions point-courbe erronées (number of faulty point-curve connections)
- Identifiant de la mesure : 21 (ISO 19157)
- Description de la mesure : Il existe une connexion point-courbe là où différentes courbes entrent en contact. Ces courbes ont une relation topologique intrinsèque qui doit refléter la véritable constellation. Si la connexion point-courbe contredit l’univers du discours, la connexion point-courbe est erronée en ce qui concerne cette mesure de qualité. La mesure de qualité comptabilise le nombre d’erreurs de ce type.
- Résultat:
  - Type de valeur : Integer
  - Unité de mesure : unity
  - valeur: 12
