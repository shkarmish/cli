---

copyright:

  years: 2018


lastupdated: "2018-08-30"
---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:tip: .tip}

# {{site.data.keyword.Bluemix_notm}}-Infrastruktur - Image

Verwenden Sie die folgenden Befehle, um Images der {{site.data.keyword.Bluemix_notm}}-Infrastruktur zu verwalten.
{: shortdesc}

<table summary="Alphabetisch geordnete Image-Befehle der {{site.data.keyword.Bluemix_notm}}-Infrastruktur mit Links zu weiteren Informationen über den Befehl">
 <tbody>
 <tr>
 <td>[ibmcloud sl image delete](/docs/cli/reference/ibmcloud/cli_image.html#sl_image_delete)</td>
 <td>[ibmcloud sl image detail](/docs/cli/reference/ibmcloud/cli_image.html#sl_image_detail)</td>
 <td>[ibmcloud sl image edit](/docs/cli/reference/ibmcloud/cli_image.html#sl_image_edit)</td>
 <td>[ibmcloud sl image list](/docs/cli/reference/ibmcloud/cli_image.html#sl_image_list)</td>
 </tr>
   </tbody>
 </table>

 ## ibmcloud sl image delete
{: #sl_image_delete}

Image löschen.
```
ibmcloud sl image delete IDENTIFIER
```
**Beispiele**:
```
   ibmcloud sl image delete 12345678
```
Dieser Befehl löscht das Image mit der ID `12345678`.

## ibmcloud sl image detail
{: #sl_image_detail}

Details zu einem Image abrufen.
```
ibmcloud sl image detail IDENTIFIER
```
**Beispiele**:
```
 ibmcloud sl image detail 12345678
```
Dieser Befehl ruft Details zu dem Image mit der ID 12345678 ab.

## ibmcloud sl image edit
{: #sl_image_edit}

Details zu einem Image bearbeiten.
```
ibmcloud sl image edit IDENTIFIER [OPTIONEN]
```

<strong>Befehlsoptionen</strong>:
<dl>
<dt>--name</dt>
<dd>Name des Images.</dd>
<dt>--note</dt>
<dd>Zusätzliche Anmerkung für das Image.</dd>
<dt>--tag</dt>
<dd>Tags für das Image.</dd>
</dl>

*Beispiele**:
```  
ibmcloud sl image edit 12345678 --name ubuntu16 --note testing --tag staging
```
Dieser Befehl bearbeitet ein Image mit der ID `12345678` und legt den Namen auf `ubuntu16`, die Anmerkung auf `testing` und den Tag auf `staging` fest.

## ibmcloud sl image list
{: #sl_image_list}

Alle Images für eigenes Konto auflisten.
```
ibmcloud sl image list [OPTIONEN]
```

<strong>Befehlsoptionen</strong>:
<dl>
<dt>--name</dt>
<dd>Nach Imagename filtern.</dd>
<dt>--public</dt>
<dd>Nur öffentliche Images anzeigen.</dd>
<dt>--private</dt>
<dd>Nur private Images anzeigen.</dd>
</dl>
