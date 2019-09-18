---
description: Exemplos de algumas combinações de macro HTTP comumente usadas.
seo-description: Exemplos de algumas combinações de macro HTTP comumente usadas.
seo-title: ' Exemplos de macro de formato HTTP'
title: ' Exemplos de macro de formato HTTP'
uuid: a81a2e2a-de7e-4b6a-8771-fcfa0dc74570
translation-type: tm+mt
source-git-commit: 4c6d1752ff10d2d3d12cab88e823f25f5ef4fcd0

---


# Exemplos de macro de formato HTTP {#http-format-macro-examples}

Exemplos de algumas combinações de [!DNL HTTP] macro comumente usadas.

Consulte Macros [de formato](../formats/web-formats.md) HTTP para obter uma lista de macros e suas definições.

<table id="table_D5FAC5D056ED49D79FA883197EF8F42E"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Exemplos de macro </th> 
   <th colname="col2" class="entry"> Formato de saída </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>&lt;PID_ALIAS&gt;|&lt;DP_UUID&gt;|&lt;TRAITALIAS_LIST; separator=","&gt;</code> </p> </td> 
   <td colname="col2"> <p> <code>pid_alias|dp_uid|trait_1,trait_2</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>&lt;PID_ALIAS&gt;|count:&lt;NUM_USERS&gt;|users:[&lt;USER_LIST:{user|&lt;user.aamUuid&gt;:&lt;user.dpUuid&gt;}; separator=", "&gt;]</code> </p> </td> 
   <td colname="col2"> <p> <code>"pid_alias|count:2|users:[uuid1:dpuuid1, uuid2:dpuuid2]"</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>&lt;USER_AGENT&gt;|&lt;IP&gt;|&lt;TIMESTAMP&gt;|&lt;RANDOM&gt;</code> </p> </td> 
   <td colname="col2"> <p> <code>"Firefox|255.255.255.255|1395758143|42341"</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>&lt;USER_LIST:{u|&lt;u.userAgent&gt;|&lt;u.ip&gt;|&lt;u.timestamp&gt;|&lt;u.random&gt;}; separator=", "&gt;</code> </p> </td> 
   <td colname="col2"> <p> <code>"Firefox|255.255.255.255|1395758143|42341"</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>&lt;DP_UUIDS.1&gt; E &lt;DP_UUIDS.2&gt;</code> </p> </td> 
   <td colname="col2"> <p> <code>dpuuid1 E dpuuid2</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>usuários:[&lt;USER_LIST:{user|&lt;user.dpUuids.1&gt; AND &lt;user.dpUuids.2&gt;}; separator=", "&gt;]</code> </p> </td> 
   <td colname="col2"> <p> <code>usuários:[dpuuid1 E dpuuid2]</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>test_known_string=loremlipsum&amp;segid=&lt;TRAITALIAS_LIST; separator=","&gt;&amp;test_dpuuid_1000=&lt;DP_UIDS.1000&gt;</code> </p> </td> 
   <td colname="col2"> <p> <code>test_known_string=loremlipsum&amp;segid=trait_1,trait_2&amp;test_dpuuid_1000=dpuuid_1000</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>test_dpuuids=&lt;DP_UUIDS.(DPID)&gt;</code> </p> </td> 
   <td colname="col2"> <p> <code>test_dpuuids=dpuuid2</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>"&lt;PID_ALIAS&gt;|&lt;DP_UUID&gt;|&lt;TRAITALIAS_LIST; separator=","&gt;|&lt;REMOVED_TRAITALIAS_LIST; separator=","&gt;</code> </p> </td> 
   <td colname="col2"> <p> <code>pid_alias|dp_uid|trait_1,trait_2|trait_3,trait_4</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 
     <code>
       {"Usuários": [&lt;USER_LIST:{user|&lt;OPEN_BRACKET&gt; "AAM_UID": "&lt;user.aamUuid&gt;", "DataPartner_UUID": "&lt;user.dpUuid&gt;", "Segmentos": [&lt;user.segment:{seg|&lt;OPEN_BRACKET&gt;"Segmento": .traitAlias&gt;"&lt;CLOSE_BRACKET&gt;}; separator=","&gt;] "Removed_Segments": [&lt;user.removeSegments:{rseg|&lt;OPEN_BRACKET&gt;"Segmento": "&lt;rseg.traitAlias&gt;"&lt;CLOSE_BRACKET&gt;}; separator=","&gt;] &lt;CLOSE BRACKET&gt;}; separador=","&gt;]} </code> </p> </td> 
   <td colname="col2"> <p> 
     <code>
       { "Usuários":[ { "AAM_UUID":"uuid1", "DataPartner_UID":"dpuuid1", "Segmentos":[ { "Segmento":"alias1" }, { "Segmento":"alias2" } ], "Removed_Segments":[ { "Segmento":"alias3" }, { "Segmento": alias4" } ] } ] </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 
     <code>
       {"Usuários": [&lt;USER_LIST:{user|&lt;OPEN_BRACKET&gt; "AAM_UID": "&lt;user.aamUuid&gt;", "DataPartner_UUID": "&lt;user.dpUuid&gt;", "Segmentos": [&lt;user.segment:{seg|&lt;OPEN_BRACKET&gt;"Segmento": .traitAlias&gt;","Status": "&lt;seg.status&gt;"&lt;CLOSE_BRACKET&gt;}; separator=","&gt;] &lt;CLOSE_BRACKET&gt;}; separator=","&gt;]} </code> </p> </td> 
   <td colname="col2"> <p> 
     <code>
       { "Usuários":[ { "AAM_UUID":"uuid1", "DataPartner_UID":"dpuuid1", "Segmentos":[ { "Segmento":"alias1" "Status":"1" }, { "Segmento":"alias2" "Status":"0" } ] } ] </code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>&lt;PID_ALIAS&gt;|&lt;DP_UUID&gt;|&lt;SEGMENTOS:{seg|&lt;seg.traitAlias&gt;}; separator=\",\"&gt;|&lt;REMOVED_SEGMENTS:{seg|&lt;seg.traitAlias&gt;}; separador=\",\"&gt;</code> </p> </td> 
   <td colname="col2"> <p> <code>pid_alias|dp_uid|trait_1,trait_2|trait_3,trait_4</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>&lt;if(user.segment &amp;&amp; user.removeSegments)&gt;&lt;COMMA&gt;&lt;endif&gt;</code> </p> </td> 
   <td colname="col2"> <p>Imprime uma vírgula se os <code>segmentos</code> dos campos e <code>removeSegments</code> não estiverem vazios. Esse condicional pode ser usado para solicitações POST ao concatenar listas para segmentos e segmentos removidos. </p> </td> 
  </tr> 
 </tbody> 
</table>
