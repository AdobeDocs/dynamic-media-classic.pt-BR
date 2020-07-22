---
title: Visão geral da plataforma Adobe Dynamic Media Classic
seo-title: Visão geral da plataforma Adobe Dynamic Media Classic
description: nulo
seo-description: Uma visão geral da plataforma Dynamic Media Classic e do processo de fluxo de trabalho.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---


# Visão geral da plataforma Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

O Dynamic Media Classic é um ambiente integrado e avançado de gerenciamento de mídia, publicação e serviço. A mídia avançada pode ser fornecida a todos os canais de marketing e venda, incluindo a Web, material impresso, campanhas de e-mail, portais da Web, desktops e dispositivos.

## Processo de fluxo de trabalho {#workflow-process}

As principais etapas do fluxo de trabalho do Dynamic Media Classic são:

* **Carregue e gerencie seus ativos** Carregue seus ativos de mídia no Dynamic Media Classic. Você pode organizar, navegar e procurar ativos no sistema. Você também pode aplicar metadados a ativos.

* **Criar mídia avançada** Crie configurações diferentes de seus ativos, como eCatalogs, Conjuntos de imagens, Conjuntos de rotação, Conjuntos de amostras, Conjuntos de mídia mista, Modelos básicos e Modelos FXG. Para obter mais informações, consulte Sobre rich media.

* **Publique e administre** Publique ativos na rede do Dynamic Media Classic Saas, além de monitorar o status dos ativos quando eles são publicados, administrar direitos de usuário e manter a segurança.

* **Fornecer** mídia da rede Dynamic Media Classic SaaS para páginas da Web, aplicativos e dispositivos móveis; a mídia é otimizada para desempenho e é fornecida com o armazenamento em cache CDN. O Dynamic Media Classic fornece um URL para cada ativo. Depois de publicar o ativo, o URL torna-se ativo.

![O processo de fluxo de trabalho do Dynamic Media Classic](/help/assets/gs_workflow.png)

## Imagens principais únicas e chamadas de URL únicas {#single-master-images-and-single-url-calls}

O Dynamic Media Classic é fundamentalmente diferente de outros sistemas porque você pode usar o Dynamic Media Classic para fornecer mídia dinamicamente de ativos principais únicos e chamadas de URL.

As sequências de caracteres de URL geradas com o Dynamic Media Classic incluem instruções que informam ao servidor como exibir o ativo quando ele é entregue. Por exemplo, a mesma imagem principal pode ser entregue em tamanhos, formatos, pesos, cores e visualizações de zoom diferentes. Como parte da criação e publicação de ativos de mídia com o Dynamic Media Classic, você configura visualmente os efeitos. Ao fazer isso, você cria as chamadas de URL que informam corretamente o servidor sobre como apresentar seu ativo principal aos aplicativos.

![O Dynamic Media Classic pode fornecer a mesma imagem principal para diferentes mídias em diferentes tamanhos e formatos.](/help/assets/gs_dynamic_publishing.png)

## Armazenamento de conteúdo em cache {#content-caching}

As imagens geradas dinamicamente pelo Dynamic Media Classic são compatíveis com cache; na maioria dos casos, são imagens JPEG com chamadas de URL exclusivas que as identificam. As imagens são fornecidas na rede de delivery de conteúdo (CDN), um sistema de servidores que são conectados em rede na Internet para fornecer conteúdo mais rápido. As imagens são distribuídas de servidores localizados globalmente e, em seguida, de computadores. Ao implementar um mecanismo de cache usando qualquer fornecedor de CDN, basta alterar o nome do servidor para apontar para o Dynamic Media Image Server habilitado para CDN. Todas as edições do Dynamic Media Classic incluem armazenamento em cache CDN empacotado.
