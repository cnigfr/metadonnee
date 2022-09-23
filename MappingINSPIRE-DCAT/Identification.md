<h3><a name="md-on-md">Identification </a></h3>
<p>Le domaine du mapping est <code>dcat:Dataset</code>, sauf mention contraire.</p>

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
      <td colspan="2">Intitulé</td>
      <td><code>dct:title</code></td>
      <td><code>rdf:PlainLiteral</code></td>
      <td>stable</td>
      <td></td>
    </tr>
    <tr>
      <td colspan="2">Résumé</td>
      <td><code>dct:description</code></td>
      <td><code>rdf:PlainLiteral</code></td>
      <td>stable</td>
      <td></td>
    </tr>
    <tr>
      <td rowspan="5">Type de la ressource</td>
      <td><em>Any type</em></td>
      <td><strong><code>dct:type</code></strong></td>
      <td><strong><code>skos:Concept</code></strong></td>
      <td>stable</td>
      <td>Seulement pour le profil étendu</td>
    </tr>
    <tr>
      <td>Data set</td>
      <td rowspan="4"><code>rdf:type</code></td>
      <td rowspan="2"><code>dcat:Dataset</code></td>
      <td rowspan="2">stable</td>
      <td rowspan="2"></td>
    </tr>
    <tr>
      <td>Data set series</td>
    </tr>
    <tr>
      <td rowspan="2">Service</td>
      <td><code>dcat:Catalog</code></td>
      <td>stable</td>
      <td>Pour les catalogues</td>
    </tr>
    <tr>
      <td><strong><code>dctype:Service</code></strong></td>
      <td>stable</td>
      <td>Pour les autres types de services (profil étendu uniquement)</td>
    </tr>
<tr>
      <td rowspan="6">Localisateur de la ressource</td>
      <td>* Download</td>
      <td><code>dcat:accessURL</code></td>
      <td><code>rdfs:Resource</code></td>
      <td>stable</td>
      <td>Le domaine est <code>dcat:Distribution</code></td>
    </tr>
 <tr>
      <td>Information</td>
      <td><code>foaf:page</code></td>
      <td><code>foaf:Document</code></td>
      <td><em>testing</em></td>
      <td></td>
    </tr>
    <tr>
      <td>* Offline access</td>
      <td><code>dcat:accessURL</code></td>
      <td><code>rdfs:Resource</code></td>
      <td><em>testing</em></td>
      <td>Le domaine est <code>dcat:Distribution</code></td>
    </tr>
    <tr>
      <td>* Order</td>
      <td><code>dcat:accessURL</code></td>
      <td><code>rdfs:Resource</code></td>
      <td><em>testing</em></td>
      <td>Le domaine est <code>dcat:Distribution</code></td>
    </tr>
    <tr>
      <td>Search</td>
      <td><code>foaf:page</code></td>
      <td><code>foaf:Document</code></td>
      <td><em>testing</em></td>
      <td></td>
    </tr>
    <tr>
      <td><em>missing</em></td>
      <td><code>dcat:landingPage</code></td>
      <td><code>foaf:Document</code></td>
      <td>stable</td>
      <td></td>
    </tr>
    <tr>
      <td colspan="2">identificateur de ressource unique</td>
      <td><code>dct:identifier</code></td>
      <td><code>rdfs:Literal</code></td>
      <td><em>testing</em></td>
      <td></td>
    </tr>
    <tr>
      <td colspan="2">Langue</td>
      <td><code>dct:language</code></td>
      <td><code>dct:LinguisticSystem</code></td>
      <td>stable</td>
      <td></td>
    </tr>
 <tr>
      <td colspan="2">* Format / Encoding</td>
<!--      
      <td><code>dcat:mediaType</code></td>
-->      
      <td><code>dct:format</code></td>
      <td><code>dct:MediaTypeOrExtent</code></td>
      <td><em>testing</em></td>
      <td>Le domaine est <code>dcat:Distribution</code></td>
    </tr>
    <tr>
      <td colspan="2">* Character encoding</td>
      <td><strong><code>cnt:characterEncoding</code></strong></td>
      <td><strong><code>rdfs:Literal</code></strong></td>
      <td><em>testing</em></td>
      <td>Seulement pour le profil étendu. Le domaine est <code>dcat:Distribution</code></td>
    </tr>
<tr>
      <td colspan="2">* Type de représentation géographique</td>
      <td><strong><code>adms:representationTechnique</code></strong></td>
      <td><strong><code>rdfs:Resource</code></strong></td>
      <td><em>testing</em></td>
      <td>Seulement pour le profil étendu. Le domaine est <code>dcat:Distribution</code></td>
    </tr>
  </tbody>
</table>
