<h3><a name="md-on-md">Métadonnées sur les métadonnées</a></h3>

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
      <td colspan="2" rowspan="2">Point de contact des métadonnées</td>
      <td><strong><code>dcat:CatalogRecord/prov:qualifiedAttribution</code></strong></td>
      <td><strong><code>prov:Attribution</code></strong></td>
      <td><em>testing</em></td>
      <td>Profil étendu uniquement</td>
    </tr>
    <tr>
      <td><strong><code>dcat:CatalogRecord/dcat:contactPoint</code></strong></td>
      <td><strong><code>vcard:Kind</code></strong></td>
      <td><em>testing</em></td>
      <td>Profil étendu uniquement</td>
    </tr>
    <tr>
      <td colspan="2">Date des métadonnées</td>
      <td><code>dcat:CatalogRecord/dct:modified</code></td>
      <td><code>xsd:date</code></td>
      <td><em>testing</em></td>
      <td></td>
    </tr>
    <tr>
      <td colspan="2">Langue des métadonnées</td>
      <td><code>dcat:CatalogRecord/dct:language</code></td>
      <td><code>dct:LinguisticSystem</code></td>
      <td>stable</td>
      <td></td>
    </tr>
    <tr>
      <td colspan="2">Identifiant des métadonnées</td>
      <td><strong><code>dcat:CatalogRecord/dct:identifier</code></strong></td>
      <td><strong><code>rdfs:Literal</code></strong></td>
      <td>stable</td>
      <td>Profil étendu uniquement</td>
    </tr>
    <tr>
      <td colspan="2">Encodage des métadonnées</td>
      <td><strong><code>dcat:CatalogRecord/cnt:characterEncoding</code></strong></td>
      <td><strong><code>rdfs:Literal</code></strong></td>
      <td>stable</td>
      <td>Profil étendu uniquement</td>
    </tr>
    <tr>
      <td colspan="2"><em>Standard des métadonnées</em></td>
      <td><code>dct:conformsTo</code></td>
      <td><code>dct:Standard</code></td>
      <td>stable</td>
      <td>Le standard de métadonnées est modélisé avec <code>dct:Standard</code>, et est décrit par un titre et une version (cf. ci-dessous)</td>
    </tr>
    <tr>
      <td colspan="2">* Nom du standard</td>
      <td><code>dct:Standard/dct:title</code></td>
      <td><code>rdf:PlainLiteral</code></td>
      <td>stable</td>
      <td></td>
    </tr>
    <tr>
      <td colspan="2">* Version du standard</td>
      <td><code>dct:Standard/owl:versionInfo</code></td>
      <td><code>rdf:PlainLiteral</code></td>
      <td>stable</td>
      <td></td>
    </tr>
  </tbody>
</table>
