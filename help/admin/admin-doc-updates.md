---
description: Todas as atualizações (adições, exclusões e correções) no Guia do Administrador do Audience Manager, por data.
seo-description: All updates (additions, deletions, and corrections) to the Audience Manager Admin Guide, by date.
seo-title: Documentation Updates
title: Atualizações de documentação
uuid: 1c02dff5-8e3f-42bf-a50c-03b75e121ac7
exl-id: 8221b4df-99c2-47d3-a2ea-186a701a2b20
TQID: https://experienceleague.adobe.com/QQHJ9VBxkF-pMFYIvgny6JJRS38Q-3nXD1kSzWdGJxQ
product_v2:
  - id: df80eeb1-8d72-467e-b0df-9d51c7d3a0a1
feature_v2:
  - id: baaa0dd2-d27e-4921-aae3-7888623a5fa5
  - id: c814092e-2730-45e8-a12d-e084529f52cb
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: d2bed13a6ac7d38ae79b65d492b6de0ca6b6d488
workflow-type: tm+mt
source-wordcount: 644
ht-degree: 88%

---

# Atualizações de documentação {#documentation-updates}

Todas as atualizações (adições, exclusões e correções) no Guia do Administrador do Audience Manager, por data.

Para obter informações sobre lançamentos de recursos, melhorias e correções de erros, consulte as [Notas de versão da Experience Cloud](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=en). Para [!DNL Audience Manager] alterações na documentação, consulte [Atualizações na Documentação](https://experienceleague.adobe.com/docs/audience-manager/user-guide/documentation-updates/docs-2019.html?lang=en).

## Atualizações de documentação do AAM 2019 {#aam-2019-docs-updates}

| Tópico | Descrição |
|--- |--- |
| Macros de formato HTTP | Adicionamos uma nova macro, `REGION_ID_LIST`, e três novos campos, `sda`, `sda` e `sda` à macro `USER_LIST`. |
| Macros de formato HTTP | Adicionamos duas novas macros: `ECID` e `MCID`. |

## Atualizações de documentação do AAM 2018 {#aam-2018-docs-updates}

<!-- c_doc_updates.xml -->

<table id="table_AECF59E131F84E7791A5A421BFB203FA"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Tópico </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p><a href="admin-servers/create-ftp-server.md#task_BF1DD0E5ECA64AEC87EACABFCAEA2C6D"> Criar ou editar um servidor FTP</a> </p> </td> 
   <td colname="col2"> <p>Adicionamos mais informações sobre autenticação de chave SSH para servidores SFTP (etapa 5). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="admin-destination-troubleshooting.md#set-up-destinations-export"> Como configurar seus destinos para exportar IDs da Experience Cloud...</a> </p> </td> 
   <td colname="col2"> <p>Esta página mostra como configurar destinos para exportar dados com o tipo de ID que você deseja em Arquivos de dados de saída. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="admin-servers/admin-authorize-s3-cross-bucket.md#task_20B12994C5484A9D8CC40DF6F456CBE7"> Como autorizar acesso ao bucket do Amazon S3 entre contas para destinos em lote</a> </p> </td> 
   <td colname="col2"> <p>É possível usar permissões de acesso ao bucket do Amazon S3 entre contas para a entrega de arquivos de dados de saída, caso não queira compartilhar chaves de acesso ou secretas do Amazon S3. Este documento mostra como configurar essa alternativa na interface do Administrador do Audience Manager. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Atualizações de documentação do AAM 2017 {#aam-2017-docs-updates}

<table id="table_81D2DA9293A9417085C630D00A7C96E1"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Tópico </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"><a href="formats/web-formats.md#reference_C392124A5F3F42E49F8AADDBA601ADFE"> Macros de formato HTTP</a> </td> 
   <td colname="col2">Substituição da macro <code>segmentId</code> por <code>legacySegmentId</code> e adição da macro <code>newSegmentId</code>. </td> 
  </tr> 
  <tr> 
   <td colname="col1"><a href="companies/admin-company-limits.md#task_3004C10CB9A9430A8D25E25BB830B5D6"> Gerenciar limites da empresa</a> </td> 
   <td colname="col2"> Adição do número máximo de pastas de características e da profundidade máxima da estrutura de características à documentação sobre limites. </td> 
  </tr> 
  <tr> 
   <td colname="col1"><a href="formats/enable-outbound-seq.md#concept_526744C9433F40BF8269E18245B2F0BD"> Ativar transferências de arquivos de sequência do Hadoop para saída</a> </td> 
   <td colname="col2"> Saiba como permitir que os clientes enviem arquivos SEQ de saída para a própria instância do Hadoop. </td> 
  </tr> 
  <tr> 
   <td colname="col1"><a href="companies/admin-manage-containers.md#task_61DB5CEECC5049DD8D059C642AC3F967"> Gerenciar containers</a> </td> 
   <td colname="col2"> Adição de uma breve instrução sobre como criar containers. </td> 
  </tr> 
  <tr> 
   <td colname="col1"><a href="companies/admin-manage-company-destinations.md#create-edit-company-destinations"> Criar ou editar destinos da empresa</a> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_527E0E75C03846B0AB39EEE544904BE2"> 
      <li id="li_FC276B34158D44E3A5450C6C8BAF3184">Adição de instruções sobre como equilibrar o uso de sincronizações completas e incrementais. </li> 
      <li id="li_3975DA78DE9E441D8F8CB80F752DD7B7">A viabilização do <span class="keyword"> Adobe Media Otimizer</span> como destino do <span class="keyword"> Audience Manager</span> é feito no próprio <span class="keyword"> Adobe Media Otimizer</span>. </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="companies/admin-manage-company-destinations.md#manage-company-destinations"> Gerenciar destinos da empresa</a> </p> </td> 
   <td colname="col2"> <p>Pequenas revisões. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="companies/admin-amo-sync.md#concept_2B5537233DAA4860B3503B344F937D83"> Sincronização de ID com o Media Otimizer</a> </p> </td> 
   <td colname="col2"> <p>Nova documentação que descreve a caixa de seleção de sincronização AMO em cada container de empresa. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="companies/admin-device-graph-options.md#concept_563615F1018340C683E0EE075F8F639D"> Opções de gráfico de dispositivo para empresas</a> </p> </td> 
   <td colname="col2"> <p>Nova documentação que descreve como configurar opções de gráfico de dispositivo. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="admin-oauth2/aam-admin-api-requirements.md#concept_A7FAC9443CF34974A873E6B787616421"> Requisitos da API e recomendações</a> </p> </td> 
   <td colname="col2"> <p>Nova documentação que descreve alguns requisitos e recomendações a serem observados e comunicados aos clientes. Essa documentação é duplicada com o mesmo título nos documentos públicos, incluindo alterações para se adaptar a um público diferente de leitores. Consulte <a href="https://experienceleague.adobe.com/docs/audience-manager/user-guide/api-and-sdk-code/rest-apis/aam-api-getting-started.html?lang=en#api-requirements-recommendations" format="https" scope="external"> Requisitos da API e recomendações</a> nos documentos públicos. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Atualizações de documentação do AAM 2016 {#aam-2016-docs-updates}

<table id="table_E9D9810EA8244B58A4F27D56CFE521FD"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Tópico </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"><a href="admin-servers/create-ftp-server.md#task_BF1DD0E5ECA64AEC87EACABFCAEA2C6D"> Criar ou editar um servidor FTP</a> </td> 
   <td colname="col2">Adição do IP de FTP de saída <b>52.44.29.204</b>. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="companies/admin-manage-company-destinations.md#manage-company-destinations"> Gerenciar destinos da empresa</a> </p> </td> 
   <td colname="col2"> <p>Pequenas revisões. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="admin-servers/create-http-server.md#task_5BF59581868E4144B965D644D36BEACD"> Criar ou editar um servidor HTTP</a> </p> </td> 
   <td colname="col2"> <p>Adição da <b>Assinatura HTTP</b> ao assistente Criar configuração de servidor. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="admin-beta-environment.md#concept_4AA12E66F49A452C8BA4E91AA28060AA"> Ambiente beta</a> </p> </td> 
   <td colname="col2"> <p>URLs e nomes de host atualizados no ambiente beta. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="companies/outbound-active-user-filter.md#task_F5CF8BDDA5DB4D23837B59CADF7A623B"> Filtrar dados de saída somente por usuários ativos</a> </p> </td> 
   <td colname="col2"> <p>Instruções para gerar um arquivo de sincronização completo que inclua apenas usuários ativos. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="formats/web-formats.md#reference_C392124A5F3F42E49F8AADDBA601ADFE"> Macros de formato HTTP</a> </p> </td> 
   <td colname="col2" morerows="1"> <p>Nova documentação que lista macros HTTP e exemplos comuns. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="formats/web-format-examples.md#reference_98828E32B0964FF9AAC7C5400E88BA31"> Exemplos de macro de formato HTTP</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Atualizações de documentação do AAM 2015 {#aam-2015-docs-updates}

<table id="table_90F524BAAED44A45A1F6BF8BBA9F26F9"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Data e tópico </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Dezembro de 2015 </p> <p><a href="formats/formats.md#concept_66AA2E78A25C4973B3230D5F75B192A2"> Formatos</a> </p> </td> 
   <td colname="col2"> <p>Revisão da seção de macro e adição de exemplos. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Atualizações de documentação do AAM 2014 {#aam-2014-docs-updates}

<table id="table_FA9962E19248418BA73D5A794A378C9D"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Data e tópico </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>12 de novembro de 2014 </p> <p> <a href="formats/formats.md#concept_66AA2E78A25C4973B3230D5F75B192A2"> Formatos</a> </p> </td> 
   <td colname="col2"> <p>Adição de informações sobre a macro &lt;MCID&gt;. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>23 de outubro de 2014 </p> <p><a href="formats/admin-create-format.md#task_1A51FC9189DB439FB218D91F3875FD67"> Criar ou editar um formato</a> </p> </td> 
   <td colname="col2"> <p>Adição de informações sobre a opção <span class="wintitle"> Recebimento de .info</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>23 de outubro de 2014 </p> <p><a href="formats/formats.md#concept_66AA2E78A25C4973B3230D5F75B192A2"> Formatos</a> </p> </td> 
   <td colname="col2"> <p>Nova página. Observe que esta página está em construção e será atualizada nos próximos dias. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>22 de outubro de 2014 </p> <p><a href="admin-destination-troubleshooting.md#"> Solução de problemas de configuração de destino</a> </p> </td> 
   <td colname="col2"> <p>Novo tópico. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>21 de outubro de 2014 </p> <p><a href="companies/admin-manage-company-destinations.md#manage-company-destinations"> Gerenciar destinos da empresa</a> </p> </td> 
   <td colname="col2"> <p>Reformulação de todo o tópico. Adição de mais informações e configurações. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>25 de setembro de 2014 </p> <p><a href="companies/admin-manage-company-profiles.md"> Criar uma empresa</a> </p> </td> 
   <td colname="col2"> <p>Adição de mais informações às seções <span class="wintitle"> Ciclo de vida</span> e <span class="wintitle"> Tipos de conta</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>25 de setembro de 2014 </p> <p><a href="companies/admin-manage-company-profiles.md#edit-company-profile"> Editar um perfil de empresa</a> </p> </td> 
   <td colname="col2"> <p>Adição de mais informações às seções <span class="wintitle"> Ciclo de vida</span> e <span class="wintitle"> Tipos de conta</span>. </p> </td> 
  </tr> 
 </tbody> 
</table>
