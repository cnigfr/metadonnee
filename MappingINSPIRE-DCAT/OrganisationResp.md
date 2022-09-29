<h3><a name="md-on-md">Organisations responsables</a></h3>

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
      <td rowspan="12"><a href="#mapping-responsible-party" title="see details">Organisation responsable</a></td>
      <td><em>N'importe quel rôle</em></td>
      <td><strong><code>dcat:Dataset/prov:qualifiedAttribution</code></strong></td>
      <td><strong><code>prov:Attribution</code></strong></td>
      <td><strong>unstable</strong></td>
      <td>Seulement pour le profil étendu.</td>
    </tr>
     <tr>
      <td>Propriétaire</td>
      <td><strong><code>dcat:Dataset/dct:rightsHolder</code></strong></td>
      <td><strong><code>foaf:Agent</code></strong></td>
      <td>stable</td>
      <td>Seulement pour le profil étendu.</td>
    </tr>
    <tr>
      <td>Gestionnaire</td>
      <td>-</td>
      <td>-</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>Point de contact</td>
      <td><code>dcat:Dataset/dcat:contactPoint</code></td>
      <td><code>vcard:Kind</code></td>
      <td>stable</td>
      <td></td>
    </tr>
     <tr>
      <td>Fournisseur</td>
      <td><code>dcat:Dataset/dct:publisher</code></td>
      <td><code>foaf:Agent</code></td>
      <td>stable</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>Auteur</td>
      <td><strong><code>dcat:Dataset/dct:creator</code></strong></td>
      <td><strong><code>foaf:Agent</code></strong></td>
      <td><em>testing</em></td>
      <td>Seulement pour le profil étendu.</td>
    </tr>
  </tbody>
</table>
