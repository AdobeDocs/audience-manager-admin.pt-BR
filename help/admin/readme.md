---
source-git-commit: b76aa4a35a5216aabd60d07352a7c4bd2b3e6e32
workflow-type: tm+mt
translation-type: tm+mt
source-wordcount: '329'
ht-degree: 2%

---
# Instruções

**Observação: Esta página (ou qualquer página readme.md) não será publicada na documentação voltada para o cliente**

## TOC

+ `TOC.md` na raiz do guia do usuário, é fornecida a organização dos tópicos contidos no guia para esta solução.
+ Cada guia do usuário terá seu próprio `TOC.md` exclusivo, no qual você pode ordenar todas as páginas/tópicos conforme necessário.
+ A primeira página de todos os guias de usuário é `overview.md`.

## Guia do usuário

+ A introdução ao guia do usuário é chamada de `overview.md`
+ Cada tópico no guia do usuário tem seu próprio diretório distinto.
   + Se houver um tópico no guia chamado *Implementação*, o diretório correspondente será `/implementation`
+ Todos os ativos de imagem são armazenados em `/assets` na raiz do guia do usuário.
   + Todas as imagens no diretório `/assets` serão localizadas.
   + Quaisquer imagens no diretório `/no-localize` não serão localizadas (há uma surpresa!). Isso pode ser usado para garantir que, em versões de loc, ativos específicos não sejam reproduzidos desnecessariamente.

## Metadados do nível do guia do usuário

+ Metadados que descrevem o guia do usuário são armazenados em `TOC.md`. Isso inclui:
   + product - nome do produto/capacidade.
   + nuvem - nuvem à qual este produto pertence.
   + audiência - audiência ou arquétipo para o qual o guia é direcionado.
   + guia do usuário - nome do guia do usuário.

## Metadados de nível de página

+ Os metadados necessários para descrever um documento são armazenados como parte de cada página individual. Isso inclui:
   + título - título da página.
   + descrição - descrição da página.
   + seo-title - seo título alternativo.
   + segunda descrição - título alternativo para fins de SEO.
   + título curto - (campo opcional).
   + index - yes / no - a página será indexada pela plataforma de pesquisa do Adobe.
   + traduzir - sim / não - esta página será localizada.
   + versão - usada principalmente para AEM e Campanha, para indicar a versão do produto.
   + private-feature-pack - usado principalmente para AEM.
   + beta - este produto está em beta?
   + redirecionamento - pode ser usado para criar uma referência para uma nova página, caso seja necessário.
   + doc-type: referência (padrão) / solução de problemas / desenvolvedor / tutorial / kb / whitepaper.

## Mais Informações

Para obter mais instruções de publicação, guias de estilo, amostras e outros recursos, visite o [Collaborative Documentation Repo](https://git.corp.adobe.com/AdobeDocs/collaborative-doc-instructions)
