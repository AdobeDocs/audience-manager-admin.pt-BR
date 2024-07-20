---
description: Por padrão, todas as empresas sincronizam dados com o Adobe Media Optimizer (AMO). Na interface do Administrador, cada contêiner de empresa tem uma fonte de dados que gerencia esse processo. Essa fonte de dados é o Adobe AMO (ID 411). Clique em uma linha de contêiner (na guia Contêineres ) de uma empresa selecionada para desativar esta sincronização padrão ou para adicionar e remover outras fontes de dados ao processo de sincronização AMO.
seo-description: By default, all companies sync data with Adobe Media Optimizer (AMO). In the Admin UI, each company container has a data source that manages this process. This data source is Adobe AMO (ID 411). Click a container row (under the Containers tab) for a selected company to disable this default sync or to add and remove other data sources to the AMO sync process.
seo-title: ID Syncing with Media Optimizer
title: Sincronização de ID com o Media Otimizer
uuid: b741dfa7-2947-4288-b214-79eccf18d53a
exl-id: ebd978ef-3825-4a96-94bd-5cdae269cf7c
source-git-commit: f5d74995f0664cf63e68b46f1f3c608f34df0e80
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 2%

---

# Sincronização de ID com o Media Otimizer {#id-syncing-with-media-optimizer}

Por padrão, todas as empresas sincronizam dados com [!DNL Adobe Media Optimizer] ([!DNL AMO]). No [!UICONTROL Admin UI], cada container de empresa tem uma fonte de dados que gerencia esse processo. Esta fonte de dados é [!UICONTROL Adobe AMO] ([!UICONTROL ID] 411). Clique em uma linha de contêiner (na guia [!UICONTROL Containers]) de uma empresa selecionada para desabilitar esta sincronização padrão ou para adicionar e remover outras fontes de dados ao processo de sincronização [!DNL AMO].

![](assets/id-sync.png)

## Status da sincronização de ID {#id-sync-status}

A tabela a seguir descreve o status de sincronização de uma fonte de dados.

| Status | Descrição |
|------ | -------- |
| Desligado | Remova todas as fontes de dados de [!UICONTROL Selected Data Sources] desse contêiner para desabilitar sincronizações de ID com [!DNL AMO] |
| Ativado (independentemente da versão do serviço de ID) | Uma fonte de dados é sincronizada com [!DNL AMO] independentemente da versão do serviço de ID quando: <ul><li>A fonte de dados aparece na lista [!UICONTROL Selected Data Sources].</li><li>A caixa de seleção *de [!DNL AMO] não está* marcada.</li></ul> |
| Ativado (independentemente da versão do serviço de ID) | Uma fonte de dados será sincronizada com [!DNL AMO] com o serviço de ID versão 2.0 (ou posterior) quando: <ul><li>A fonte de dados aparece na lista [!UICONTROL Selected Data Sources].</li><li>A caixa de seleção *is* de [!DNL AMO] está marcada.</li></ul> |

>[!MORELIKETHIS]
>
>* [Gerenciar containers](../companies/admin-manage-containers.md#task_61DB5CEECC5049DD8D059C642AC3F967)
