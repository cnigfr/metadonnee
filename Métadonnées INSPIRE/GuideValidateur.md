# Intro

Le validateur national est disponible ici : https://validateur.geocatalogue.fr/validator/ 
![image](https://github.com/cnigfr/metadonnee/assets/12797943/2a6dc977-58e1-4e81-a7d2-eecd3de1fb55)

Le validateur européen est disponible ici : https://inspire.ec.europa.eu/validator/home/index.html
Pour tester une métadonnées de données le paramétrage suivant doit être sélectionné :
![image](https://github.com/cnigfr/metadonnee/assets/12797943/f18adde8-ca22-4f37-a8c7-34fde80e84cf)


# Comprendre les erreurs du validateur

Les erreurs couramment rencontrées sont les suivantes !
| CODE | LIBELLE | %ERREUR |
| --- | --- | --- |
| C1 | XML Schema | 26% |
| --- | --- | --- |
| C2 | Root Element | 0% |
| **C5** | **Language Code** | 20% |
| C6 | Metadata Point of Contact | 5% |
| C7 | Metadata Date | 0% |
| C8 | Ressource Title | 0% |
| C9 | Ressource Abstract | 0% |
| C10 | Responsible Organization | 6% |
| C11 | Temporal Reference | 10% |
| C12 | Max One Date of Creation | 0% |
| C13 | Not More than one Date of Last revision | 1% |
| C14 | Temporal Extent | 10% |
| C15 | Keyword Originating CV | 24% |
| C16 | Group Keyword by CV | 3% |
| **C17** | **Limitations on Public Access** | 30% |
| C18 | Conditions for Access and Use | 7% |
| **C19** | **Geographical Bounding Box** | 2% |
| **C20** | **Dataset Conformity** | 12% |
| **C21** | **Dataset Conformity Specifications** | 12% |
| **C22** | **Conformity Degree** | 12% |
| 1.1 | Resource Type | 0% |
| --- | --- | --- |
| 1.2 | Only One Data Identification | 0% |
| 1.3 | Dataset UID | 0% |
| 1.4 | INSPIRE Theme Keyword | 8% |
| 1.5 | Spatial Resolution | 0% |
| **1.6** | **Ressource Language** | 30% |
| 1.7 | Topic Category | 0% |
| 1.8 | Resource Locator | 0% |
| 1.9 | Data Quality Info Section | 0% |
| 1.10 | Dataset Conformity | 17% |
| 1.11 | Lineage | 0% |
| 3.1 | Resource Type | 27% |
| --- | --- | --- |
| 3.2 | Service Identification Element | 0% |
| 3.3 | Spatial Resolution | 0% |
| 3.4 | Spatial Data Service Category | 27% |
| 3.5 | Spatial Data Service Type | 18% |
| _ **3.6** _ | _ **Coupled Resource** _ | 55% |
| 3.7 | Resource Locator | 0% |
| 3.8 | Only One Data Quality Element | 27% |

## C1 XML SChema
![image](https://github.com/cnigfr/metadonnee/assets/12797943/c0e82b58-8d37-41cc-b371-f13323c80b16)

Problème de schéma. 

## C5 Language Code

![image](https://github.com/cnigfr/metadonnee/assets/12797943/21cbf91c-6906-4108-b914-cd4cb5d71176)

`<gmd:language>
<gco:CharacterString xmlns:gco="http://www.isotc211.org/2005/gco">fre</gco:CharacterString>
</gmd:language>`

A remplacer par 

`<gmd:language> <gmd:LanguageCode codeList="http://www.loc.gov/standards/iso639-2/" codeListValue="fre">fre</gmd:LanguageCode> </gmd:language>`

## C10 Responsible Organization
![image](https://github.com/cnigfr/metadonnee/assets/12797943/fd2b8b79-a234-4860-9062-7fa1a1c104b6)

Le rôle de la partie responsable doit être pris dans la liste des valeurs possibles (cf. [liste](https://inspire.ec.europa.eu/metadata-codelist/ResponsiblePartyRole))

## C17 Limitations on Public Access

![image](https://github.com/cnigfr/metadonnee/assets/12797943/e49e6a73-ce05-427b-a672-f537a963fdaa)

Les limitations d'accès publiques doivent être expréimées dans une contrainte supplémentaire comme ceci :

    <gmd:resourceConstraints>
            <gmd:MD_LegalConstraints>
               <gmd:accessConstraints>
                  <gmd:MD_RestrictionCode codeList="http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/codelist/ML_gmxCodelists.xml#MD_RestrictionCode" codeListValue="otherRestrictions"/>
               </gmd:accessConstraints>
               <gmd:otherConstraints xsi:type="gmd:PT_FreeText_PropertyType">
                  <gmx:Anchor xlink:href="http://inspire.ec.europa.eu/metadata-codelist/LimitationsOnPublicAccess/noLimitations">No public access restriction according to INSPIRE</gmx:Anchor>
                  <gmd:PT_FreeText>
                     <gmd:textGroup>
                        <gmd:LocalisedCharacterString locale="#FR">Pas de restriction d'accès public selon INSPIRE</gmd:LocalisedCharacterString>
                     </gmd:textGroup>
                  </gmd:PT_FreeText>
               </gmd:otherConstraints>
            </gmd:MD_LegalConstraints>
         </gmd:resourceConstraints>

## C19 Geographical Bounding Box
![image](https://github.com/cnigfr/metadonnee/assets/12797943/c6bc9507-393d-4ae1-9bdc-ddeaec648a05)

Les coordonnées doivent avoir 2 chiffres après la virgule, comme ceci :
south-bound latitude = '41.3 **0**'

## C20 Dataset Conformity

![image](https://github.com/cnigfr/metadonnee/assets/12797943/3473ab74-af66-4e0b-bdf1-cc449d927874)

La conformité au règlement INSPIRE doit être exprimée de la façon suivante : 

    <gmd:result> 
      <gmd:DQ_ConformanceResult> 
      <gmd:specification xlink:href="http://inspire.ec.europa.eu/id/citation/ir/reg-1089-2010"> 
          <gmd:CI_Citation> 
              <gmd:title><gmx:Anchor xlink:href="http://data.europa.eu/eli/reg/2010/1089">COMMISSION REGULATION (EU) No 1089/2010 of 23 November 2010 implementing Directive 2007/2/EC of the European Parliament and of the Council as regards interoperability of spatial data sets and services</gmx:Anchor> </gmd:title>
              <gmd:date> <gmd:CI_Date> 
                <gmd:date> <gco:Date>2010-12-08</gco:Date> </gmd:date>
                <gmd:dateType> <gmd:CI_DateTypeCode codeList="http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#CI_DateTypeCode" codeListValue="publication">publication</gmd:CI_DateTypeCode> </gmd:dateType> </gmd:CI_Date> </gmd:date> 
          </gmd:CI_Citation> 
      </gmd:specification> 
      <gmd:explanation> <gco:CharacterString>This data set is conformant with the INSPIRE Implementing Rules for the interoperability of spatial data sets and services</gco:CharacterString> </gmd:explanation> 
      <gmd:pass> <gco:Boolean>true</gco:Boolean> </gmd:pass> 
    </gmd:DQ_ConformanceResult> 
    </gmd:result>

## 1.4 INSPIRE Theme Keyword
![image](https://github.com/cnigfr/metadonnee/assets/12797943/4f0b98c7-c05a-4763-af8c-f02dfe043f90)
![image](https://github.com/cnigfr/metadonnee/assets/12797943/d112f0de-166f-4d90-b88b-24f6ffe40d2e)


Le mot-clé INSPIRE doit être exprimé comme suit : 

     <gmd:MD_Keywords>
                     <gmd:keyword>
                        <gmx:Anchor xmlns:gmx="http://www.isotc211.org/2005/gmx" xlink:href="http://inspire.ec.europa.eu/theme/pf" xlink:type="simple">Lieux de production et sites industriels</gmx:Anchor>
                     </gmd:keyword>
                     <gmd:type>
                        <gmd:MD_KeywordTypeCode codeList="http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#MD_KeywordTypeCode" codeListValue="theme"/>
                     </gmd:type>
                     <gmd:thesaurusName xlink:type="simple">
                        <gmd:CI_Citation>
                           <gmd:title>
                              <gco:CharacterString xmlns:gco="http://www.isotc211.org/2005/gco">GEMET - INSPIRE themes, version 1.0</gco:CharacterString>
                           </gmd:title>
                           <gmd:date xlink:type="simple">
                              <gmd:CI_Date>
                                 <gmd:date>
                                    <gco:Date xmlns:gco="http://www.isotc211.org/2005/gco">2008-06-01</gco:Date>
                                 </gmd:date>
                                 <gmd:dateType>
                                    <gmd:CI_DateTypeCode codeList="http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#CI_DateTypeCode" codeListValue="publication"/>
                                 </gmd:dateType>
                              </gmd:CI_Date>
                           </gmd:date>
                           <gmd:identifier xlink:type="simple">
                              <gmd:MD_Identifier>
                                 <gmd:code>
                                    <gmx:Anchor xmlns:gmx="http://www.isotc211.org/2005/gmx" xlink:href="http://inspire.ec.europa.eu/theme" xlink:type="simple">Registre de thème INSPIRE</gmx:Anchor>
                                 </gmd:code>
                              </gmd:MD_Identifier>
                           </gmd:identifier>
                        </gmd:CI_Citation>
                     </gmd:thesaurusName>
                  </gmd:MD_Keywords>

## 1.6 Ressource Language
![image](https://github.com/cnigfr/metadonnee/assets/12797943/9b0b7573-221e-4ba3-be0f-3d08b52690fb)

`<gmd:language>
<gco:CharacterString xmlns:gco="http://www.isotc211.org/2005/gco">fre</gco:CharacterString>
</gmd:language>`

A remplacer par 

`<gmd:language> <gmd:LanguageCode codeList="http://www.loc.gov/standards/iso639-2/" codeListValue="fre">fre</gmd:LanguageCode> </gmd:language>`

## 1.10 Dataset Conformity
Résoudre les C.20, C.21, C.22 doit permettre de résoudre cette erreur.

## M.1 Spatial scope

![image](https://github.com/cnigfr/metadonnee/assets/12797943/d9c041e2-440b-462e-85dc-fe120d605240)

#Option 1: avec gmx:Anchor

`<gmd:descriptiveKeywords>
    <gmd:MD_Keywords>
        <gmd:keyword>
            <gmx:Anchor xlink:href="http://inspire.ec.europa.eu/metadata-codelist/SpatialScope/national">National</gmx:Anchor>
        </gmd:keyword>
        <gmd:thesaurusName>
            <gmd:CI_Citation>
                <gmd:title>
                    <gmx:Anchor xlink:href="http://inspire.ec.europa.eu/metadata-codelist/SpatialScope">Spatial scope</gmx:Anchor>
                </gmd:title>
                <gmd:date>
                    <gmd:CI_Date>
                        <gmd:date>
                            <gco:Date>2019-05-22</gco:Date>
                        </gmd:date>
                        <gmd:dateType>
                            <gmd:CI_DateTypeCode codeList="http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#CI_DateTypeCode" codeListValue="publication">publication</gmd:CI_DateTypeCode>
                        </gmd:dateType>
                    </gmd:CI_Date>
                </gmd:date>
            </gmd:CI_Citation>
        </gmd:thesaurusName>
    </gmd:MD_Keywords>
</gmd:descriptiveKeywords>`

#Option 2: Avec gco:CharacterString

`<gmd:descriptiveKeywords>
    <gmd:MD_Keywords>
        <gmd:keyword>
            <gco:CharacterString>National</gco:CharacterString>
        </gmd:keyword>
        <gmd:thesaurusName>
            <gmd:CI_Citation>
                <gmd:title>
                    <gco:CharacterString>Spatial scope</gco:CharacterString>
                </gmd:title>
                <gmd:date>
                    <gmd:CI_Date>
                        <gmd:date>
                            <gco:Date>2019-05-22</gco:Date>
                        </gmd:date>
                        <gmd:dateType>
                            <gmd:CI_DateTypeCode codeList="http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/codelist/ML_gmxCodelists.xml#CI_DateTypeCode" codeListValue="publication">publication</gmd:CI_DateTypeCode>
                        </gmd:dateType>
                    </gmd:CI_Date>
                </gmd:date>
            </gmd:CI_Citation>
        </gmd:thesaurusName>
    </gmd:MD_Keywords>
</gmd:descriptiveKeywords>`
