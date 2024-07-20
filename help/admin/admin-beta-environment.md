---
description: O ambiente beta é usado para testar implementações de Audience Manager. As alterações feitas na versão beta não afetam os dados de produção. O ambiente beta do Audience Manager é uma versão independente e em menor escala do ambiente de produção. Todos os dados que você deseja testar devem ser inseridos e coletados neste ambiente.
seo-description: The beta environment is for testing Audience Manager implementations. Changes made in beta do not affect production data. The Audience Manager beta environment is a smaller-scale, standalone version of the production environment. All the data that you want to test must be entered and collected in this environment.
seo-title: Beta Environment
solution: Audience Manager
title: Ambiente do Beta
uuid: 6a253f4e-96e7-4395-a783-a8eb213b7daf
exl-id: 78d5a1ff-c016-4366-ba34-9814a0d92067
source-git-commit: 79415eba732c2a6d50f04124774664f788ccc78c
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 2%

---

# Ambiente do Beta {#beta-environment}

O ambiente beta é usado para testar implementações de Audience Manager. As alterações feitas na versão beta não afetam os dados de produção. O ambiente beta do Audience Manager é uma versão independente e em menor escala do ambiente de produção. Todos os dados que você deseja testar devem ser inseridos e coletados neste ambiente.

## Visão geral {#overview}

<!-- beta_environment_admin.xml -->

| Serviço | URL/Nome do host | Etapas para provisionar |
|--- |--- |--- |
| S3 | | Consulte [Provisionar buckets do Amazon S3](admin-beta-environment.md#provision-s3-buckets). |
| DCS | https&amp;colon;//dcs-beta.demdex.net/... | Não são necessários passos extras da nossa parte. Consulte [Acessar o DCS no Ambiente Beta](admin-beta-environment.md#access-dcs-beta-environment). |
| Interface do usuário | https&amp;colon;//bank-beta.demdex.com | Os dados são copiados do ambiente de produção para o ambiente beta mensalmente. As credenciais de produção são válidas para o beta. |
| API | https&amp;colon;//api-beta.demdex.com/... | Os dados são copiados do ambiente de produção para o ambiente beta mensalmente. As credenciais de produção são válidas para o beta. |

## Provisionamento de buckets do Amazon S3 {#provision-s3-buckets}

>[!NOTE]
>
>Estamos deixando de usar o [!DNL FTP/SFTP]. Além disso, observe que as transferências de dados de saída não funcionam para o ambiente beta.

Para provisionar [!DNL S3] buckets para dados de entrada:

1. Use o recurso [**Ajuda de TechOps para Solicitação do SKMS**](https://skms.adobe.com/).
1. Vá para **[!UICONTROL Request TechOps Help]** no painel de navegação esquerdo.
1. Em **[!UICONTROL Request Search]**, digite Audience Manager no campo de pesquisa.
1. Role para baixo nos resultados da pesquisa e clique em **Audience Manager - Configuração de conta de entrada/saída S3**.
1. Preencha os campos na janela de provisionamento e especifique **Ambiente de sandbox** no campo **[!UICONTROL Environment]**.

>[!NOTE]
>
>Desincentivamos o uso do [!DNL FTP/SFTP] e incentivamos o uso do [!UICONTROL Amazon S3]. Os motivos pelos quais incentivamos o uso do [!UICONTROL Amazon S3] estão listados no [Amazon S3:About](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/amazon-s3.html).

## Acessar o DCS no ambiente Beta {#access-dcs-beta-environment}

Para acessar o [!UICONTROL DCS] no ambiente beta:

1. Fazer uma chamada [!UICONTROL DCS], usando o [!DNL curl] [comando](https://curl.haxx.se/docs/manpage.html). [!DNL Curl] é uma ferramenta para transferir dados de ou para um servidor, usando um dos vários protocolos com suporte.

   Por exemplo: `curl -v https://dcs-beta.demdex.net/event`

1. Verifique se sua solicitação foi atendida pelo beta [!UICONTROL DCS] procurando por &quot;[!DNL sandbox]&quot; no cabeçalho de resposta [!UICONTROL DCS].

   Por exemplo:

   ```
   curl -v http://dcs-beta.demdex.net/?event
   [...]
   < DCS: va6-sandbox-dcs-3.sandbox.demdex.com <release_number>
   [...]
   ```

<!--
1. Determine the load balancer's endpoint IP addresses.

   Run the `dig` [command](https://en.wikipedia.org/wiki/Dig_(command)) to determine the IP address of the nearest load balancer. The `dig` command queries the Domain Name System and returns the name and IP addresses of the Audience Manager [!UICONTROL Data Collection Servers (DCS)].

   ```
   dig dcs-beta.demdex.net
   ...
   dcs-sandbox-1754093861.us-east-1.elb.amazonaws.com. 60 IN A 52.87.15.51
   dcs-sandbox-1754093861.us-east-1.elb.amazonaws.com. 60 IN A 50.16.150.8
   dcs-sandbox-1754093861.us-east-1.elb.amazonaws.com. 60 IN A 52.2.228.100
   ```

1. Using one of the addresses in the above table, add a static DNS entry in the [!DNL `/etc/hosts`] file.

   On Windows, modify [!DNL `c:\WINDOWS\system32\drivers\etc\hosts`].

   For example:

[!DNL `52.87.15.51 samplepartner.demdex.net`]

   >[!NOTE]
   >
   >The addresses change occasionally, so you must keep your [!DNL /etc/hosts] file up to date.

   Additionally, if you need to set up ID synchronization, you must add a similar entry for [!DNL dpm.demdex.net.]

[!DNL `52.87.15.51 dpm.demdex.net`] [!DNL]. 

1. Make a [!UICONTROL DCS] call, using the `curl` [command](https://curl.haxx.se/docs/manpage.html). Curl is a tool to transfer data from or to a server, using one of many supported protocols.

   For example:

[!DNL `https://<domain>/event?product=camera`] 

1. Verify that your request was served by the beta [!UICONTROL DCS] by looking for "sandbox" in the [!UICONTROL DCS] response header.

   For example:

   ```
   curl -v https://dcs-beta.demdex.net/?event
   [...]
   < DCS: va6-sandbox-dcs-3.sandbox.demdex.com <release_number>
   [...]
   ```
-->
