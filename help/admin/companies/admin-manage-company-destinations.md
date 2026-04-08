---
description: Criar, editar e excluir destinos do Audience Manager.
seo-description: Create, edit, and delete Audience Manager destinations.
seo-title: Manage Company Destinations
title: Gerenciar destinos da empresa
uuid: d9a6bfb1-7629-44e0-b7d7-ece44f65ea2b
exl-id: a2e73613-07cd-4ab8-8c6e-be451ed50bfc
TQID: https://experienceleague.adobe.com/-MWpMACN0bFPIRAWejD0-VV5nG8BGAukmV1QXxXal-E
product_v2:
  - id: df80eeb1-8d72-467e-b0df-9d51c7d3a0a1
feature_v2:
  - id: c814092e-2730-45e8-a12d-e084529f52cb
source-git-commit: d2bed13a6ac7d38ae79b65d492b6de0ca6b6d488
workflow-type: tm+mt
source-wordcount: 1101
ht-degree: 0%

---

# Gerenciar destinos da empresa {#manage-company-destinations}

Criar, editar e excluir destinos do Audience Manager.

<!-- t_company_destinations.xml -->

Para obter informações detalhadas, consulte [Destinos](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/destinations/destinations.html) no *Guia do Usuário do Audience Manager*.

## Criar ou editar destinos da empresa {#create-edit-company-destinations}

Percorra as seções para obter instruções passo a passo sobre como criar novos destinos do [!DNL Audience Manager] ou editar destinos existentes.

<!-- create-edit-company-destinations.xml -->

Visite a [página de integração do parceiro Experience Cloud](https://wiki.corp.adobe.com/x/mPIMPw) antes de configurar destinos. A página contém as informações específicas que você precisa preencher para cada integração de parceiro do [!DNL Audience Manager].

Se o seu cliente quiser usar [!DNL Adobe Media Optimizer] como um destino em [!DNL Audience Manager] , você precisará configurar isso em [!DNL Adobe Media Optimizer].

## Navegue até a guia Destinos {#navigate-destinations}

1. Clique em **[!UICONTROL Companies]**, localize e clique na empresa desejada para exibir sua página [!UICONTROL Profile]. Você pode usar a caixa [!UICONTROL Search] ou os controles de paginação na parte inferior da lista para encontrar a empresa desejada. Você pode classificar cada coluna em ordem crescente ou decrescente clicando no cabeçalho da coluna desejada.
1. Clique na guia **[!UICONTROL Destinations]**.
1. Para criar um novo destino, clique em **[!UICONTROL Add Destination]**. Para editar um destino existente, clique no nome do destino na coluna **[!UICONTROL Name]**.

## Configurações básicas {#basic-settings}

Preencha os campos na janela **[!UICONTROL Basic Settings]**.

* **[!UICONTROL Name]:** (Obrigatório) Especifique o nome deste destino.
* **[!UICONTROL Description]:** Especifique as informações descritivas sobre este destino.
* **[!UICONTROL Type]:** (obrigatório) Selecione o tipo de destino desejado:
   * **[!UICONTROL Bulk ID]**: sincronizar IDs entre plataformas diferentes.
   * **[!UICONTROL Bulk Trait]**: envia informações de características em massa para plataformas diferentes.
   * **[!UICONTROL Bulk Segment]**: Enviar informações de segmento em massa para plataformas diferentes.
   * **[!UICONTROL S2S]**: use destinos de servidor para servidor para enviar dados em lote e em tempo real para plataformas diferentes.
* **[!UICONTROL Auto-Fill Destination Mapping]:** (somente [!UICONTROL S2S]) Selecione uma opção:
   * **[!UICONTROL Segment ID]:** Se você selecionar essa configuração, o mapeamento do valor de destino será preenchido com a ID do Segmento [!DNL Audience Manager].
   * **[!UICONTROL Integration Code Value]:** Se você selecionar essa configuração, o mapeamento do valor de destino será preenchido com o código de integração do segmento [!DNL Audience Manager].
* **[!UICONTROL User ID Key]:** (Obrigatório) Selecione a chave de ID de usuário desejada para este destino na lista suspensa.

Essa ID é usada como a ID da fonte de dados mestre. Isso determina as IDs de usuário a serem ultrapassadas no arquivo.

>[!NOTE]
>
>Para o tipo de destino [!UICONTROL Bulk ID], você não pode usar o [!DNL Audience Manager] [!UICONTROL User ID] ou a ID de [!DNL Adobe Experience Cloud].

Se a sua ID de fonte de dados ( [!UICONTROL DPID]) não for exibida na lista suspensa, você deverá marcar a caixa de seleção **[!UICONTROL Outbound]** no nível de fonte de dados na [página Configurações do Data Source](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/data-sources/manage-datasources.html).

* **[!UICONTROL Target Data Source]:** (obrigatório) Selecione a fonte de dados desejada para este destino na lista suspensa. Essa configuração permite rotular os dados enviados, o que permite a assimilação em sistemas separados do lado do cliente.
* **[!UICONTROL Foreign Account ID]:** Especifique a ID de conta externa para este destino. Este é o valor de identificação no sistema do recipient para esses dados limitados.
* **[!UICONTROL Outbound Sample Rate Denominator]:** Quando a quantidade total de dados retornados for desconhecida, use esta configuração para retornar apenas uma quantidade de dados de exemplo, em vez da quantidade total. Ajuste o número aqui para representar uma fração dos dados (por exemplo, um valor de &quot;100&quot; retorna 1/100 da quantidade regular de dados, um valor de &quot;10&quot; retorna 1/10 da quantidade regular de dados). O padrão é &#39;1&#39;, que retorna todos os dados.

## Dados em tempo real (para destinos S2S) {#realtime-s2s}

Se você estiver criando um destino [!UICONTROL S2S], preencha os campos abaixo:

**[!UICONTROL Servers]**: Selecione o servidor `HTTP` desejado para este destino.
**[!UICONTROL Format]**: Selecione o formato desejado para este destino na lista suspensa: [!UICONTROL HTTP only].

>[!NOTE]
>
>Somente para [!DNL S2S], você pode habilitar ou desabilitar os destinos [!UICONTROL Realtime] ou [!UICONTROL Batch] usando os controles deslizantes Desligado/Ligado na tela. Não é possível desativar as duas opções.

## Dados em lote {#batch-data}

Para destinos [!UICONTROL Bulk ID], [!UICONTROL Bulk Trait] ou [!UICONTROL Bulk Segment], preencha os campos abaixo:

* **[!UICONTROL Protocol]**: (Obrigatório) Selecione o protocolo desejado para este destino na lista suspensa:
   * **[!UICONTROL FTP]**
   * **[!UICONTROL HTTP]**
   * **[!UICONTROL S3]**
* **[!UICONTROL Servers]**: (Obrigatório) Selecione o servidor desejado para este destino na lista suspensa.
* **[!UICONTROL Format]**: (Obrigatório) Selecione o formato desejado para este destino na lista suspensa: [!DNL HTTP] ou tipo de arquivo, dependendo do protocolo escolhido acima.
* **[!UICONTROL Sync Type]**: (Obrigatório) Selecione o tipo de sincronização desejado para este destino. Isso indica o nível de atividades de usuário que os clientes desejariam incluir nas ordens de saída. Selecione **[!UICONTROL Customer]** se os clientes só estiverem interessados em analisar as qualificações de segmento a partir de suas propriedades. Selecione **[!UICONTROL Platform]** se eles quiserem incluir qualificações de segmento de atividades externas em todos os [!DNL Audience Manager] clientes.
* **[!UICONTROL Customer]**: o arquivo contém usuários ativos que têm pelo menos uma realização de característica apenas nas propriedades do cliente (associadas ao [!UICONTROL PID] do cliente) para o período selecionado. Seus clientes devem usar essa opção para enviar suas qualificações de segmento *em tempo real* para destinos.
* **[!UICONTROL Platform]**: o arquivo contém usuários ativos que têm pelo menos uma interação em tempo real, seja ela de sincronização de ID ou de realização de características, em qualquer lugar nas propriedades de todos os clientes [!DNL Audience Manager] (associadas a todos os PIDs de clientes) do período selecionado. Seus clientes devem usar essa opção para enviar suas *totais* qualificações de segmento para destinos.
* **[!UICONTROL Lifetime]**: o arquivo contém usuários ativos vistos em qualquer lugar em todas as propriedades de clientes do [!DNL Audience Manager] desde a criação do destino.
* **[!UICONTROL Sync Type Lookback Period]**: Se você selecionar [!UICONTROL Customer] ou [!UICONTROL Platform], selecione um período. Os arquivos contêm usuários ativos para o período selecionado.
Em seguida, selecione o tipo de pedido. Isso indica a frequência e o escopo de cada integração de saída com parceiros. Selecione entre pedidos incrementais e completos.
* **[!UICONTROL Incremental Scheduled Run]**: a cada execução, [!DNL Audience Manager] somente sairá dos novos usuários qualificados desde a ordem de saída anterior. Selecione o período desejado para que o [!DNL Audience Manager] execute processos de sincronização incremental. Por exemplo, você pode selecionar a cada 24 horas, a cada sete dias, a cada 30 dias ou nunca.

<!--
I removed {importance="high"} from note for Exp League rendering. -Bob
-->

>[!NOTE]
>
>A primeira ordem incremental é equivalente a uma ordem completa porque nenhum usuário anterior foi enviado ao destino.

* **[!UICONTROL Full Sync Scheduled Run]**: a cada execução, [!DNL Audience Manager] sairá de todos os usuários ativos desde que o destino foi configurado pela primeira vez. Selecione o agendamento desejado que você deseja que [!DNL Audience Manager] use para executar processos de sincronização completa. Por exemplo, você pode selecionar a cada 24 horas, a cada sete dias, a cada 30 dias ou nunca.

<!--
I removed {importance="high"} from note for Exp League rendering. -Bob
-->

>[!NOTE]
>
>Recomendamos usar sincronizações incrementais com mais frequência do que sincronizações completas. As sincronizações incrementais só enviam arquivos que contêm novas realizações de características ou sincronizações de ID. Sincronizações completas enviam todos os arquivos, independentemente de incluírem ou não novas realizações ou sincronizações de ID. Use a configuração do [!UICONTROL Full Sync Scheduled Run] somente quando os clientes precisarem de uma cópia completa de todos os usuários para reduzir o volume de dados de saída.

## Configurar fontes de dados {#configure-data-sources}

Para destinos [!UICONTROL Bulk ID], [!UICONTROL Bulk Trait] ou [!UICONTROL Bulk Segment], preencha os campos abaixo. Essas configurações permitem enviar todos os dados (características, segmentos ou IDs, com base no tipo selecionado) associados às fontes de dados.

* **[!UICONTROL All Unrestricted First Party Data]**: selecione para usar todas as fontes de dados primárias. Se você selecionar esta opção, as opções [!UICONTROL Available Data Sources] serão desabilitadas.
* **[!UICONTROL Available Data Sources]**: Use as setas para mover fontes de dados entre as caixas **[!UICONTROL Available Data Sources]** e **[!UICONTROL In File Data Sources]**.

## Salvar e finalizar {#save-and-finalize}

O botão **[!UICONTROL Save]** é ativado após o preenchimento de todos os campos obrigatórios. Clique em **[!UICONTROL Save]** para finalizar o processo de criação de destino.

## Excluir destinos da empresa {#delete-company-destinations}

<!-- delete-company-destinations.xml -->

Para excluir um destino:

1. Clique em **[!UICONTROL Companies]**, localize e clique na empresa desejada e, em seguida, clique na guia **[!UICONTROL Destinations]**.
1. Clique em ![](assets/icon_delete.png) na coluna **[!UICONTROL Actions]** do destino desejado.
1. Clique em **[!UICONTROL OK]** para confirmar a exclusão.

>[!NOTE]
>
>Não é possível excluir um destino se ele tiver segmentos mapeados a ele.
