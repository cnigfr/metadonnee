<h3><a name="md-on-md">Qualité</a></h3>
<p>Les commentaires sont à faire ici : https://github.com/cnigfr/metadonnee/issues/4</p>

<table>
  <thead>
    <tr>
      <th colspan="2" rowspan="2">Elément de métadonnée (ISO 19115 / INSPIRE)</th>
      <th colspan="2">Mappings</th>
      <th rowspan="2">Statut</th>
      <th rowspan="2">Commentaire</th>
    </tr>
    <tr>
      <th>Propriété et/ou attribut</th>
      <th>Valeurs</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td colspan="2">Généalogie</td>
      <td><code>dcat:Dataset/dct:provenance</code></td>
      <td><code>dct:ProvenanceStatement</code></td>
      <td>stable</td>
      <td></td>
    </tr>
<tr>
      <td colspan="2"><a href="#mapping-spatial-resolution" title="see details">Résolution spatiale</a></td>
      <td><strong><code>dcat:Dataset/rdfs:comment</code></strong></td>
      <td><strong><code>rdf:PlainLiteral</code></strong></td>
      <td><strong>unstable</strong></td>
      <td>Seulement pour le profil étendu. A discuter</td>
    </tr>
 <tr>
      <td>Cohérence topologique</td>
      <td><em>no candidate available</em></td>
      <td><em>no candidate available</em></td>
      <td>pending</td>
      <td>Des travaux globaux pourraient être à mener avec le groupe Quadogéo. </td>
    </tr>
<tr>
      <td rowspan="4"><a href="#mapping-conformance-result" title="see details">Conformité des données</a></td>
      <td><em>Conforme ou non conforme</em></td>
      <td><strong><code>dcat:Dataset/prov:wasUsedBy</code></strong></td>
      <td><strong><code>prov:Activity</code></strong></td>
      <td><em>testing</em></td>
      <td>Seulement pour le profil étendu.</td>
    </tr>
    <tr>
      <td>Conforme</td>
      <td><code>dcat:Dataset/dct:conformsTo</code></td>
      <td><code>dct:Standard</code></td>
      <td>stable</td>
      <td></td>
    </tr>
    <tr>
      <td>Non conforme</td>
      <td>-</td>
      <td>-</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>Non évalué</td>
      <td>-</td>
      <td>-</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
  </tbody>
</table>

<h4><a name="mapping-spatial-resolution">Spatial resolution</a></h4>

This is currently mapped to a free text field (namely, `rdfs:comment`).

The text is built by using the following pattern:

* If spatial resolution is specified with a distance:

    `Spatial resolution (distance): <distance> <uom>`

* If spatial resolution is specified with an equivalent scale:

    `Spatial resolution (equivalent scale): 1:<denominator>`

Examples:

````xml
  <rdfs:comment xml:lang="en">
    Spatial resolution (distance): 5 km
  </rdfs:comment>
````

````xml
  <rdfs:comment xml:lang="en">
    Spatial resolution (equivalent scale): 1:10000
  </rdfs:comment>
````

<h4><a name="mapping-conformance-result">Conformance result / Conformity (Data quality)</a></h4>

GeoDCAT-AP provides only a partial mapping for data quality information, limited to the component "conformance result".

#### GeoDCAT-AP core profile

````xml
  <dct:conformsTo rdf:parseType="Resource">
    <dct:title xml:lang="en">COMMISSION REGULATION (EU) No 1089/2010 of 23 November 2010 implementing Directive 2007/2/EC of the European Parliament and of the Council as regards interoperability of spatial data sets and services</dct:title>
    <dct:issued rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2010-12-08</dct:issued>
  </dct:conformsTo>
````

If the conformity specification is specified with an HTTP URI ([see how](./HTTP-URIs.md#uri-conformity-specification))

````xml
  <dct:conformsTo rdf:resource="http://eur-lex.europa.eu/LexUriServ/LexUriServ.do?uri=CELEX:32010R1089:EN:NOT"/>
````

#### GeoDCAT-AP extended profile

````xml
  <prov:wasUsedBy>
    <prov:Activity>
      <prov:qualifiedAssociation rdf:parseType="Resource">
        <prov:hadPlan rdf:parseType="Resource">
<!-- Specification -->
          <prov:wasDerivedFrom>
            <rdf:Description rdf:about="http://eur-lex.europa.eu/LexUriServ/LexUriServ.do?uri=CELEX:32010R1089:EN:NOT">
              <dct:title xml:lang="en">COMMISSION REGULATION (EU) No 1089/2010 of 23 November 2010 implementing Directive 2007/2/EC of the European Parliament and of the Council as regards interoperability of spatial data sets and services</dct:title>
              <dct:issued rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2010-12-08</dct:issued>
            </rdf:Description>
          </prov:wasDerivedFrom>
        </prov:hadPlan>
      </prov:qualifiedAssociation>
<!-- Conformance result / conformity degree -->      
      <prov:generated rdf:parseType="Resource">
        <dct:type rdf:resource="http://inspire.ec.europa.eu/metadata-codelist/DegreeOfConformity/conformant"/>
        <dct:description xml:lang="en">See the referenced specification</dct:description>
      </prov:generated>
    </prov:Activity>
  </prov:wasUsedBy>
````

If the conformity specification is specified with an HTTP URI ([see how](./HTTP-URIs.md#uri-conformity-specification))

````xml
  <prov:wasUsedBy>
    <prov:Activity>
      <prov:qualifiedAssociation rdf:parseType="Resource">
        <prov:hadPlan rdf:parseType="Resource">
<!-- Specification -->
          <prov:wasDerivedFrom rdf:resource="http://eur-lex.europa.eu/LexUriServ/LexUriServ.do?uri=CELEX:32010R1089:EN:NOT"/>
        </prov:hadPlan>
      </prov:qualifiedAssociation>
<!-- Conformance result / conformity degree -->      
      <prov:generated rdf:parseType="Resource">
        <dct:type rdf:resource="http://inspire.ec.europa.eu/metadata-codelist/DegreeOfConformity/conformant"/>
        <dct:description xml:lang="en">See the referenced specification</dct:description>
      </prov:generated>
    </prov:Activity>
  </prov:wasUsedBy>
````
