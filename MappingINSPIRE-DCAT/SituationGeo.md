<h3><a name="md-on-md">Situation géographique</a></h3>

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
      <td colspan="2"><em>Etendue spatiale</em></td>
      <td><code>dcat:Dataset/dct:spatial</code></td>
      <td><code>dct:Location</code></td>
      <td>stable</td>
      <td>Spatial extent / coverage is specified as a geographic identifier and/or bounding box - see below</td>
    </tr>
  <tr>
      <td colspan="2"><a href="#mapping-bbox" title="see details">Etendue spatiale: emprise</a></td>
      <td><code>dct:Location/locn:geometry</code></td>
      <td><code>locn:Geometry</code> (<code>rdfs:Literal</code> or <code>rdfs:Class</code>)</td>
      <td>stable</td>
      <td>The recommendation is to use WKT or GML literals, encoded as per the GeoSPARQL specification.</td>
    </tr>
    <tr>
      <td rowspan="4"><a href="#mapping-geo-id" title="see details">Etendue spatiale: Geographic identifier</a></td>
      <td rowspan="3">Code</td>
      <td><code>dcat:Dataset/dct:spatial</code></td>
      <td><code>rdfs:Resource</code> (URI reference)</td>
      <td>stable</td>
      <td>If the geographic identifier is an HTTP URI.</code></td>
    </tr>
  </tbody>
</table>

<h4><a name="mapping-bbox">Geographic bounding box</a></h4>

The XSLT outputs a geographic bounding box in multiple encodings, namely, the ones recommended in GeoDCAT-AP (i.e., WKT and GML), and GeoJSON.

To denote the datatype of the GeoJSON literal, [the URL of the relevant IANA Media Type](https://www.iana.org/assignments/media-types/application/vnd.geo+json) is used.

````xml
  <dct:spatial rdf:parseType="Resource">
<!-- As WKT -->
    <locn:geometry rdf:datatype="http://www.opengis.net/ont/geosparql#wktLiteral"><![CDATA[POLYGON((-6.41736 55.7447,2.05827 55.7447,2.05827 49.8625,-6.41736 49.8625,-6.41736 55.7447))]]></locn:geometry>
<!- As GML -->
    <locn:geometry rdf:datatype="http://www.opengis.net/ont/geosparql#gmlLiteral"><![CDATA[<gml:Envelope srsName="http://www.opengis.net/def/crs/OGC/1.3/CRS84"><gml:lowerCorner>-6.41736 49.8625</gml:lowerCorner><gml:upperCorner>2.05827 55.7447</gml:upperCorner></gml:Envelope>]]></locn:geometry>
<!-- As GeoJSON -->
    <locn:geometry rdf:datatype="https://www.iana.org/assignments/media-types/application/vnd.geo+json"><![CDATA[{"type":"Polygon","crs":{"type":"name","properties":{"name":"urn:ogc:def:crs:OGC:1.3:CRS84"}},"coordinates":[[[-6.41736,55.7447],[2.05827,55.7447],[2.05827,49.8625],[-6.41736,49.8625],[-6.41736,55.7447]]]}]]></locn:geometry>
  </dct:spatial
````
<h4><a name="mapping-geo-id">Geographic identifier</a></h4>

If specified with an HTTP URI ([see how](./HTTP-URIs.md#uri-geo-id)):

````xml
  <dct:spatial rdf:resource="http://publications.europa.eu/resource/authority/continent/EUROPE"/>
````

If specified with a literal:

````xml
  <dct:spatial rdf:parseType="Resource">
<!-- Code -->
    <skos:prefLabel xml:lang="en">Location &gt; Continent &gt; Europe</skos:prefLabel>
    <skos:inScheme>
<!-- Authority -->
      <skos:ConceptScheme>
        <rdfs:label xml:lang="en">NASA/GCMD Location Keywords</rdfs:label>
        <dct:modified rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2009-01-01</dct:modified>
      </skos:ConceptScheme>
    </skos:inScheme>
  </dct:spatial>
````
