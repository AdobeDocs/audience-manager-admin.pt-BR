---
description: Aspectos que você deve incentivar seus clientes a estarem cientes quando estiverem trabalhando com as APIs do Audience Manager.
seo-description: Things you should encourage your clients to be aware of when they're working with the Audience Manager APIs.
seo-title: API Requirements and Recommendations
title: Requisitos da API e Recommendations
uuid: eba9cf92-f0c8-4394-8532-0de9a2e7b103
exl-id: 24f90732-31a6-436d-862b-e6871d279c7a
source-git-commit: c7c5da62b32f6a56152e1c09a965facfc601cade
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Requisitos da API e Recommendations {#api-requirements-and-recommendations}

Aspectos que você deve incentivar seus clientes a saber ao trabalhar com o Audience Manager [!DNL API]s.

## Requisitos {#requirements}

Observe o seguinte ao trabalhar com o código [!DNL Audience Manager] [!DNL API]:

* **Parâmetros de solicitação:** Todos os parâmetros de solicitação são necessários, a menos que especificado de outra forma.
* **[!DNL JSON]tipo de conteúdo:** Especifique `content-type: application/json` *e* `accept: application/json` no seu código.

* **Solicitações e respostas:** envia solicitações como um objeto [!DNL JSON] formatado corretamente. [!DNL Audience Manager] responde com [!DNL JSON] dados formatados. As respostas do servidor podem conter dados solicitados, um código de status ou ambos.

* **Acesso:** O consultor do [!DNL Audience Manager] fornecerá a você uma ID de cliente e uma chave que permitem fazer solicitações do [!DNL API].

* **Documentação e exemplos de código:** O texto em *itálico* representa uma variável que você fornece ou transmite ao criar ou receber dados [!DNL API]. Substitua o texto *em itálico* pelo seu próprio código, parâmetros ou outras informações necessárias.

## Recommendations: criar um usuário da API genérica {#recommendations}

Recomendamos criar uma conta de usuário técnica separada para trabalhar com o Audience Manager [!DNL API]s. Essa é uma conta genérica que não está vinculada a um usuário específico na organização do cliente ou associada a ele. Este tipo de conta de usuário do [!DNL API] ajuda em duas coisas:

* Identifique qual serviço está chamando o [!DNL API] (por exemplo, chamadas de um aplicativo cliente que usa nosso [!DNL API]s ou de fazer alterações em massa).
* Forneça acesso ininterrupto ao [!DNL API]s. Uma conta vinculada a um funcionário específico pode ser excluída ao sair da empresa. Isso impedirá que seus clientes trabalhem com o código [!DNL API] disponível. Uma conta genérica que não esteja vinculada a um funcionário específico ajuda a evitar esse problema.

Como exemplo ou caso de uso para esse tipo de conta, considere que seus clientes desejam alterar muitos segmentos ao mesmo tempo com as [Ferramentas de gerenciamento em massa](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/bulk-management-tools/bulk-management-intro.html?lang=pt-BR). Para fazer isso, eles precisam de acesso de [!DNL API]. Em vez de adicionar permissões a um usuário específico, crie uma conta de usuário [!DNL API] não específica que tenha as credenciais, a chave e o segredo apropriados para fazer chamadas [!DNL API]. Isso também é útil se os clientes desenvolverem seus próprios aplicativos que usam o [!DNL Audience Manager] [!DNL API]s.
