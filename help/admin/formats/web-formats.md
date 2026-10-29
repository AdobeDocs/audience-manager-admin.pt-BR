---
description: Lista as macros que você pode usar para criar arquivos de dados HTTP. HTTP envia dados em um formato JSON.
seo-description: Lists the macros you can use to create HTTP data files. HTTP sends data in a JSON format.
seo-title: HTTP Format Macros
title: Macros de formato HTTP
uuid: 91021f60-75d0-4b1d-86ca-91c9dadafac1
exl-id: 80ed24ac-1b84-4c1b-966f-039b587ea899
TQID: https://experienceleague.adobe.com/5j4Tq2P-dNGLa-yLSm8EY8xQWg7MBR9ggzdUi0oBMBQ
product_v2:
  - id: df80eeb1-8d72-467e-b0df-9d51c7d3a0a1
    internal-label: Audience Manager
source-git-commit: d2bed13a6ac7d38ae79b65d492b6de0ca6b6d488
workflow-type: tm+mt
source-wordcount: 394
ht-degree: 2%

---

# Macros de formato HTTP {#http-format-macros}

Lista as macros que você pode usar para criar arquivos de dados do [!DNL HTTP]. [!DNL HTTP] envia dados em um formato [!DNL JSON].

Consulte os [Exemplos de Macro de Formato HTTP](../formats/web-format-examples.md) para obter uma lista e exemplos de algumas combinações de macro usadas com frequência.

<table id="table_72A72EA63C3643FB84B47A76CD2CC1CA"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Macro </th> 
   <th colname="col2" class="entry"> Tipo de método </th> 
   <th colname="col3" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>AAM_UUID</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p> ID </span> do Audience Manager <span class="keyword">. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DP_UUID</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>ID de usuário exclusiva do parceiro de dados. Essa macro retorna a ID atribuída a um usuário se a ID dele já tiver sido sincronizada com uma ID de dispositivo do <span class="keyword"> Audience Manager </span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DPID</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>ID do provedor de dados. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>ECID</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>ID do provedor de dados. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>GENERATION_TIME</code> </p> </td> 
   <td colname="col2"> <p> <code>GET, POST</code> </p> </td> 
   <td colname="col3"> <p>Carimbo de data e hora Unix UTC. Um carimbo de data/hora interno representa a hora em que a AAM foi notificada para publicar o destino </span> do S2S <span class="wintitle"> para nossos parceiros. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>IP</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>O endereço IP do usuário. </p> </td> 
  </tr>
    <tr> 
   <td colname="col1"> <p> <code>MCID</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Experience Cloud ID. (MCID significa Marketing Cloud, que é o nome herdado do Experience Cloud) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>NUM_REMOVED_SEGMENTS</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>O número (inteiro) de segmentos aos quais um usuário não pertence mais. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>NUM_SEGMENTS</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>O número de segmentos aos quais um usuário pertence. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>ORDER_ID</code> </p> </td> 
   <td colname="col2"> <p> <code>GET, POST</code> </p> </td> 
   <td colname="col3"> <p>ID do pedido ou destino. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>PID_ALIAS</code> </p> </td> 
   <td colname="col2"> <p> <code>GET, POST</code> </p> </td> 
   <td colname="col3"> <p>Um alias para a ID do parceiro. Também conhecida como ID de conta estrangeira. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>RANDOM</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Gera um número aleatório. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>REGION_ID_LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>A região </a> do Audience Manager DCS <a href="https://experienceleague.adobe.com/docs/audience-manager/user-guide/api-and-sdk-code/dcs/dcs-api-reference/dcs-regions.html?lang=pt-BR"> de onde a atividade se originou.</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>REMOVED_SEGMENT_LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Retorna uma lista de IDs de segmento, se houver, para as quais um usuário não está mais qualificado. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>REMOVED_SEGMENTS</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Uma lista de segmentos para os quais um usuário não está mais qualificado. Também é possível retornar campos de segmento específicos que incluem: </p> <p> 
     <ul id="ul_29B83093A7624A908F0C06F2A248981A"> 
      <li id="li_57A60A54F5D44E38ACB4E2648095F246"> <code>traitAlias</code> </li> 
      <li id="li_4079F646493F40DBA0CE75D662A69454"> <code>legacySegmentId (formerly segmentId)</code> </li> 
      <li id="li_D3509A2D379E4C1FB3BC1B5E7D45A916"> <code>newSegmentId</code> </li> 
      <li id="li_EA901C20EEEB4CFAA39A5E0E822D2394"> <code>status</code> </li> 
      <li id="li_6310E21F88CC4691980DD3C9D551409F"> <code>dateTime</code> </li> 
     </ul> </p> <p>Especifique esses campos em uma matriz, como mostrado neste exemplo: </p> <p> <code>[&lt;REMOVED_SEGMENTS:{seg|&lt;OPEN_BRACKET&gt;"Mapping":&lt;seg.traitAlias&gt;,"Status:"&lt;seg.status&gt;, "Time":&lt;seg.dateTime&gt;,"LegacySegmentId":&lt;seg.LegacySegmentId&gt;, "NewSegmentId":&lt;seg.NewSegmentId&gt;&lt;CLOSE_BRACKET&gt;}; "separator=","&gt;]</code> </p> <p>Consulte também <a href="../formats/web-format-examples.md#reference_98828E32B0964FF9AAC7C5400E88BA31"> Exemplos de macro de formato HTTP </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>REMOVED_TIME_LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> Uma lista de últimas realizações para segmentos para os quais o usuário não está mais qualificado. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>REMOVED_TRAITALIAS_LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Uma lista de nomes com alias de segmentos para os quais um usuário não está mais qualificado. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SEGMENT_LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Retorna uma lista de IDs de segmento. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SEGMENTS</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Uma lista de segmentos para os quais um usuário se qualifica. Também é possível retornar campos de segmento específicos que incluem: </p> <p> 
     <ul id="ul_9209683A8E0A4B8081E5EFA4602F743F"> 
      <li id="li_D796526C1C9E45BEA891D619539888C4"> <code>traitAlias</code> </li> 
      <li id="li_BF12E010E1AD432C84605B9817F209DD"> <code>legacySegmentId (formerly segmentId)</code> </li> 
      <li id="li_4A81E3B715254549B9EADB983A2FC32B"> <code>newSegmentId</code> </li> 
      <li id="li_1F01A60829DF4C87879D94299E1D589C"> <code>status</code> </li> 
      <li id="li_E52F10CD5A04487D81A4B1750B0DC4E3"> <code>dateTime</code> </li> 
     </ul> </p> <p>Especifique esses campos em uma matriz, como mostrado neste exemplo: </p> <p> <code>[&lt;SEGMENTS:{seg|&lt;OPEN_BRACKET&gt;"Mapping":&lt;seg.traitAlias&gt;,"Status:"&lt;seg.status&gt;, "Time":&lt;seg.dateTime&gt;,"LegacySegmentId":&lt;seg.LegacySegmentId&gt;, "NewSegmentId":&lt;seg.NewSegmentId&gt;&lt;CLOSE_BRACKET&gt;}; "separator=","&gt;]</code> </p> <p>Consulte também <a href="../formats/web-format-examples.md#reference_98828E32B0964FF9AAC7C5400E88BA31"> Exemplos de macro de formato HTTP </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TIME_LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Uma lista de últimas realizações. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TIMESTAMP</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Carimbo de data e hora Unix, UTC. Representa a última realização do segmento. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TRAITALIAS_LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Uma lista de nomes com alias para um segmento específico. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>USER_AGENT</code> </p> </td> 
   <td colname="col2"> <p> <code>GET</code> </p> </td> 
   <td colname="col3"> <p>Agente do usuário da solicitação inicial. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>USER_LIST</code> </p> </td> 
   <td colname="col2"> <p> <code>POST</code> </p> </td> 
   <td colname="col3"> <p>Uma lista de <span class="keyword"> IDs de usuário do Audience Manager </span>. Você também pode retornar campos específicos que incluem o seguinte: </p> 
    <ul id="ul_B6857D809FDC46749B7E745BD8C45F8E"> 
     <li id="li_F31CD82D16ED41FD82518141D90B5B35"> <code>user.aamUuid</code> </li> 
     <li id="li_623FA758C84D4A2D9B25C7FBE90F62B7"> <code>user.dpUuid</code> </li> 
     <li id="li_976B941908EB494EB476B5FB68B8972D"> <code>user.segments</code> </li> 
     <li id="li_D7E129833D1E4D59A554FFCE353924EE"> <code>user.removedSegments</code> </li> 
     <li id="li_8B3DD69D3FE3493492FC9F162812FCD5"> <code>user.userAgent</code> </li> 
     <li id="li_8C7EA05585A64141876DF169C31322FE"> <code>user.ip</code> </li> 
     <li id="li_678076A31A7743C480F718C9E7A07E99"> <code>user.dpuuids</code> </li> 
     <li id="li_B598A5AED28C4304972E51DBD4E480D8"> <code>user.timestamp</code> </li> 
     <li id="li_8424D540282F449CA5AF6B3CC343DDCB"> <code>user.random</code> </li>
     <li><code>user.regionIds</code></li> 
    </ul> <p>Especifique esses campos conforme mostrado neste exemplo: </p> <p> 
     <codeblock>
       "AAM_UUID": "&lt;user.aamUuid&gt;" 
"DataPartner_UUID": "&lt;user.dpUuid&gt;" 
     </codeblock> </p> <p>Consulte também <a href="../formats/web-format-examples.md#reference_98828E32B0964FF9AAC7C5400E88BA31"> Exemplos de macro de formato HTTP </a> para obter um exemplo completo. </p> </td> 
  </tr>
 </tbody>
</table>
