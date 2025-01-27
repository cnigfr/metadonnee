Reference technique

Xpath ISO 19115	```identificationInfo[1]/*/descriptiveKeywords/*/keyword``` ```identificationInfo[1]/*/descriptiveKeywords/*/thesaurusName```

Exemple de XML :
```xml
<gmd:MD_Metadata>
  <gmd:identificationInfo>
    <gmd:MD_DataIdentification>
        …
      <gmd:descriptiveKeywords> <gmd:MD_Keywords>
          <gmd:keyword> <gmx:Anchor xlink:href=”ht tp://inspire.ec.europa.eu/metadata-codelist/PriorityDataset/Agglomerations-dir-2002-49”>Agglomérations (Directive Bruit)</gco:CharacterString> </gmd:keyword>
          <gmd:thesaurusName> <gmd:CI_Citation>
                    <gmd:title> <gmx:Anchor xlink:href=”http://inspire.ec.europa.eu/metadata-codelist/PriorityDataset”>INSPIRE priority data set</gco:CharacterString> </gmd:title>
                    <gmd:date> <gmd:CI_Date>
                        <gmd:date> <gco:Date>2010-01-13</gco:Date> </gmd:date>
                        <gmd:dateType> <gmd:CI_DateTypeCode codeList=http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/Codelist/ML_gmxCodelists.xml#CI_DateTypeCode codeListValue="publication">publication</gmd:CI_DateTypeCode> </gmd:dateType>
                  </gmd:CI_Date> </gmd:date>
          </gmd:CI_Citation> </gmd:thesaurusName>
      </gmd:MD_Keywords> </gmd:descriptiveKeywords>
</gmd:MD_DataIdentification>
</gmd:identificationInfo>
…
</gmd:MD_Metadata>
```
