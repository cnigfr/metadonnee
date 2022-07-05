# Mapping INSPIRE DCAT
Ce dossier a pour vocation de rassembler des ressources utiles aux travaux de mise en correspondace entre les métadonnées INSPIRE ISO 19115 et GeoDCAT-AP. 
```mermaid
flowchart LR;
 classDef dcat fill:#f9f;
  classDef prov fill:#39f;
    
    ISO[METADONNE INSPIRE]-->A1;
    ISO-->A2;
    ISO-->A3;
    ISO-->A4;
    ISO-->A5;
    ISO-->A6;
    ISO-->A7;
    ISO-->A8;
    ISO-->A9;
    
    	A1[IDENTIFICATION DES DONNEES]-->B[INTITULE DE LA RESSOURCE];
		click A1 "https://github.com/cnigfr/metadonnee/issues/9"
    		B-->TITLE["dct:title"]:::dcat;
    		A1-->C[RESUME DE LA RESSOURCE];
		C-->DESC["dct:description"]:::dcat;
    		A1-->D[TYPE DE LA RESSOURCE];
	    	A1-->E[LOCALISATEUR DE LA RESSOURCE];
    		A1-->F[IDENTIFICATEUR DE RESSOURCE UNIQUE];
    		A1-->G[LANGUE DE LA RESSOURCE];
    		A1-->H[ENCODAGE];
    		A1-->I[ENCODAGE DES CARACTERES];
    		A1-->J[TYPE DE REPRESENTATION];
    	A2[CLASSIFICATION DES DONNEES ET SERVICES GEOGRAPHIQUES]-->B2[CATEGORIE THEMATIQUE];
		click A2 "https://github.com/cnigfr/metadonnee/issues/8"
    	A3[MOTS CLES]-->B3[MOTS CLE OBLIGATOIRE];
		click A3 "https://github.com/cnigfr/metadonnee/issues/7"
		B3-->B33[Thème INSPIRE];
		B3-->B34[Données prioritaires];
		B3-->B35[Données de couverture nationale/régionale];
		A3-->C3[MOTS CLES COMPLEMENTAIRES];
	A4[SITUATION GEOGRAPHIQUE]-->B4[RECTANGLE DE DELIMITATION GEOGRAPHIQUE];
		click A4 "https://github.com/cnigfr/metadonnee/issues/6"
		B4-->Z4["dct:spatial"]:::dcat;
		A4-->C4[REFERENTIEL DE COORDONNEES];
		C4-->C41[Cas général : système de référence spatial];
		C4-->C42[Cas particulier : système de référence par identifiants géographiques];
	A5[REFERENCE TEMPORELLE]-->B5[ETENDUE TEMPORELLE];
		click A5 "https://github.com/cnigfr/metadonnee/issues/5"
		A5-->C5[DATES DE REFERENCE];
		C5-->C51[Date de publication];
		C5-->C52[Date de création];
		C5-->C53[Date de dernière révision];
		A5-->D5[SYSTEME DE REFERENCE TEMPOREL];
	A6[QUALITE ET VALIDITE]-->B6[GENEALOGIE];
		click A6 "https://github.com/cnigfr/metadonnee/issues/4"
		A6-->C6[RESOLUTION SPATIALE];
		A6-->D6[COHERENCE TOPOLOGIQUE];
		A6-->E6[CONFORMITE];
		E6-->E61[SPECIFICATION];
		E6-->E62[DEGRE];
	A7[CONTRAINTES]-->B7[CONTRAINTES INSPIRE];
		click A7 "https://github.com/cnigfr/metadonnee/issues/3"
		B7-->B71[Restrictions];
		B7-->B72[Conditions applicable];
		A7-->C7[AUTRES CONTRAINTES];
	A8[ORGANISATIONS RESPONSABLES]-->B8[PARTIE RESPONSABLE];
		click A8 "https://github.com/cnigfr/metadonnee/issues/2"
		A8-->C8[ROLE DE LA PARTIE RESPONSABLE];
	A9[METADONNEES CONCERNANT LES METADONNEES]-->B9[POINT DE CONTACT DES METADONNEES];
		click A9 "https://github.com/cnigfr/metadonnee/issues/1"
		B9-->QUALATT["prov:qualifiedAttribution"]:::prov;
		B9-->CONTA["dcat:contactPoint"]:::dcat;
		A9-->C9[DATE DES METADONNEES];
		C9-->MODIF["dct:modified"]:::dcat;
		A9-->D9[LANGUE DES METADONNEES];
		D9-->LANG["dct:language"]:::dcat;
		A9-->E9[IDENTIFIANT DE LA METADONNEE];
		E9-->IDENT["dct:Identifier"]:::dcat;
		
    ""
```
