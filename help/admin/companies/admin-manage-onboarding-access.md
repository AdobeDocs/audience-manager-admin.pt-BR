---
description: Para evitar a integração acidental de arquivos e dados em fontes de dados de destino pertencentes a outros parceiros ou clientes, a Audience Manager adicionou um requisito de mapeamento entre a ID do parceiro (PID) e as fontes de dados de propriedade de outros parceiros.
title: Gerenciar o acesso de integração para dados de terceiros
exl-id: 03bec978-dd31-41cc-a3aa-d67fbb98963c
source-git-commit: cc04863272005964cfbf1bb2319cc0dd86863680
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Gerenciar o acesso de integração para dados secundários {#manage-onboarding-access-for-second-party-data}

>[!IMPORTANT]
>
> O público-alvo desta página são funcionários internos da Adobe. Se você for um cliente da Audience Manager e solicitar um mapeamento de fonte de dados de terceiros conforme descrito nesta página, entre em contato com o Atendimento ao cliente ou com o Gerente técnico de conta.
> &#x200B;> Observe que não é necessário solicitar um mapeamento para os relacionamentos de compartilhamento de dados existentes. O mapeamento também não é necessário ao integrar dados em fontes de dados de destino que pertencem ao seu PID.

Para evitar a integração acidental de arquivos e dados em fontes de dados de destino pertencentes a outros parceiros, a Audience Manager adicionou um requisito de mapeamento entre a ID do parceiro (PID) e as fontes de dados (DPID) de propriedade de outros parceiros. Leia mais sobre PID e DPID no [índice de Audience Manager IDs](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/ids-in-aam.html).

Para fins de compartilhamento de dados de terceiros, se um parceiro ou cliente da Audience Manager quiser assimilar arquivos em uma fonte de dados de destino que não seja sua, será necessário solicitar um mapeamento entre a ID do parceiro (PID) e essa fonte de dados específica (DPID). Se o mapeamento estiver ausente, os arquivos não serão processados pelo trabalho de dados de entrada e os dados não serão integrados no Audience Manager.

Para criar esse mapeamento, envie um tíquete Jira à equipe de engenharia do Audience Manager. Veja um exemplo de tíquete Jira [aqui](https://jira.corp.adobe.com/browse/AAM-60353). Não é necessário solicitar que os mapeamentos sejam criados para quaisquer relações de compartilhamento de dados existentes.
