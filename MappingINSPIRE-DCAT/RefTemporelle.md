<h3><a name="md-on-md">Référence temporelle</a></h3>

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
      <td rowspan="4">Référence temporelle</td>
      <td>Etendue temporelle</td>
      <td><code>dcat:Dataset/dct:temporal</code></td>
      <td><code>dct:PeriodOfTime</code></td>
      <td>stable</td>
      <td></td>
    </tr>   
 <tr>
      <td>Date de publication</td>
      <td><code>dcat:Dataset/dct:issued</code></td>
      <td><code>xsd:date</code></td>
      <td>stable</td>
      <td></td>
    </tr>
    <tr>
      <td>Date de dernière révision</td>
      <td><code>dcat:Dataset/dct:modified</code></td>
      <td><code>xsd:date</code></td>
      <td>stable</td>
      <td></td>
    </tr>
    <tr>
      <td>Date de création</td>
      <td><strong><code>V/dct:created</code></strong></td>
      <td><strong><code>xsd:date</code></strong></td>
      <td>stable</td>
      <td>Seulement pour le profil étendu</td>
    </tr>  
<tr>
      <td colspan="2">Système de référence temporel</td>
      <td><strong><code>dcat:Dataset/dct:conformsTo</code></strong></td>
      <td><strong><code>rdfs:Resource</code></strong></td>
      <td><strong>unstable</strong></td>
      <td>Seulement pour le profil étendu. A discuter</td>
    </tr>
  </tbody>
</table>
