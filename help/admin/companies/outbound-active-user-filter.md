---
description: Siga estas instruções para gerar um arquivo de sincronização completo que inclua apenas usuários ativos recentemente. Talvez você queira filtrar por usuários ativos para enviar dados relevantes para um sistema de direcionamento no site ou limitar o tamanho dos arquivos enviados para um DSP. Não é possível usar esse filtro com sincronização incremental.
seo-description: Follow these instructions to generate a full synchronization file that includes recently active users only. You may want to filter for active users to push relevant data to an on-site targeting system or to limit the size of the files sent to a DSP. You cannot use this filter with incremental synchronization.
seo-title: Filter Outbound Data by Active Users Only
title: Filtrar dados de saída somente por usuários ativos
uuid: a2b4a385-eee3-458c-b978-09509cacb397
exl-id: d501cfd1-64dd-448e-92c5-180c0081d3e5
source-git-commit: f5d74995f0664cf63e68b46f1f3c608f34df0e80
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Filtrar dados de saída somente por usuários ativos {#filter-outbound-data-by-active-users-only}

Siga estas instruções para gerar um arquivo de sincronização completo que inclua apenas usuários ativos recentemente. Talvez você queira filtrar por usuários ativos para enviar dados relevantes para um sistema de direcionamento no site ou limitar o tamanho dos arquivos enviados para um DSP. Não é possível usar esse filtro com sincronização incremental.

>[!NOTE]
>
>Um visitante não precisa ser visto em um site de cliente selecionado ou em seu tráfego de anúncio para se qualificar como &quot;ativo&quot;. Elas podem ser vistas por qualquer cliente ou parceiro do [!DNL Audience Manager] como &quot;ativas&quot;.

Para filtrar somente por usuários ativos:

1. Clique em **[!UICONTROL Companies]**.
1. Selecione a empresa com a qual deseja trabalhar e clique em **[!UICONTROL Destinations]**.
1. Na seção [!UICONTROL Batch Data], defina as seguintes opções:

   * **[!UICONTROL Sync Type]**: Selecione **[!UICONTROL Customer]** ou **[!UICONTROL Platform]**.
   * **[!UICONTROL Sync Type Lookback Period]**: esse intervalo de tempo define o intervalo do arquivo de dados. As opções incluem **[!UICONTROL 24 hours]**, **[!UICONTROL 7 days]**, **[!UICONTROL 30 days]**.
   * **[!UICONTROL Incremental Sync Scheduled Run]**: Selecione **[!UICONTROL Never]**. Lembre-se de que esse filtro se aplica somente aos arquivos de sincronização completa.
   * **[!UICONTROL Full Sync Scheduled Run]**: Isso determina com que frequência você deseja receber esse arquivo. As opções incluem **[!UICONTROL 24 hours]**, **[!UICONTROL 7 days]**, **[!UICONTROL 30 days]** ou **[!UICONTROL Never]** (para desabilitar).

1. Clique em **[!UICONTROL Save]**.
