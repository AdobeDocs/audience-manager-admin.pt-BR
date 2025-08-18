---
description: É possível que alguns clientes não queiram fornecer acesso ao Amazon Simple Storage Service (Amazon S3) ou chaves secretas ao Adobe para autorizar o upload de dados de destino para seus buckets.
seo-description: Some customers may not want to provide their Amazon Simple Storage Service (Amazon S3) access or secret keys to Adobe to authorize destination data upload to their buckets.
seo-title: How To  Authorize Cross-Account Amazon S3 Bucket Access for Batch Destinations
title: Como autorizar acesso ao bucket do Amazon S3 entre contas para destinos em lote
uuid: da2bcbda-a765-437a-bfe9-4355383a4730
exl-id: f3b97c31-714f-4841-884b-bc507267a932
source-git-commit: f5d74995f0664cf63e68b46f1f3c608f34df0e80
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---

# Como autorizar acesso ao bucket do Amazon S3 entre contas para destinos em lote{#authorize-cross-account-bucket-batch}

É possível que alguns clientes não queiram fornecer acesso ao [!DNL Amazon S3] ou chaves secretas ao Adobe para autorizar o upload de dados de destino para seus buckets.

Uma alternativa que podemos oferecer aos nossos clientes é o [!UICONTROL Cross-Account Bucket Permissions] em [!DNL Amazon S3]. Este processo está descrito na [documentação do AWS](https://docs.aws.amazon.com/AmazonS3/latest/dev/example-walkthroughs-managing-access-example2.html). Para ativar essa alternativa no Audience Manager, siga as etapas abaixo:

1. Vá para **[!UICONTROL Servers]** e selecione **[!UICONTROL Create Server]**.
1. Selecione **[!UICONTROL S3]** na máscara suspensa **[!UICONTROL Protocol/Credentials]**.
1. Marque a opção **[!UICONTROL Use Internal Adobe Key]**.
1. Use a conta e o nome do bucket do seu cliente no [!DNL Amazon S3].
1. Certifique-se de que o cliente liste a conta [!DNL Amazon S3] do `975822914085` no seu bucket [!DNL S3].

>[!NOTE]
>
>Nosso editor de saída garante que o nível de permissão `bucket-owner-full-control` esteja definido nos dados carregados, para que o cliente possa ser o proprietário desses dados.
