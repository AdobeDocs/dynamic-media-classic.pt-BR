---
title: Visão geral da plataforma Adobe Dynamic Media Classic
seo-title: Visão geral da plataforma Adobe Dynamic Media Classic
description: nulo
seo-description: Uma visão geral da plataforma e do processo de fluxo de trabalho do Dynamic Media Classic.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: referência
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/category/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Visão geral da plataforma Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

O Dynamic Media Classic é um ambiente integrado de gerenciamento de mídia avançada, publicação e serviço. A mídia avançada pode ser fornecida para todos os canais de marketing e venda, incluindo Web, material impresso, campanhas por email, portais da Web, desktops e dispositivos.

## Processo de fluxo de trabalho {#workflow-process}

As principais etapas do fluxo de trabalho do Dynamic Media Classic são:

* **Carregue e gerencie seus ativos** Carregue seus ativos de mídia na SPS. Você pode organizar, navegar e procurar ativos no sistema. Você também pode aplicar metadados a ativos. Se você instalar o aplicativo Adobe Scene7 Publishing System para desktop, poderá carregar arquivos e pastas arrastando-os da área de trabalho para uma pasta de upload.

* **Criar mídia avançada** Crie configurações diferentes de seus ativos, como catálogos, conjuntos de imagens, conjuntos de rotação, conjuntos de amostras, conjuntos de mídia mista, modelos básicos e modelos FXG. Para obter mais informações, consulte Sobre rich media.

* **Publique e administre** Publique ativos na rede do Dynamic Media Classic Saas, além de monitorar o status dos ativos quando eles são publicados, administrar direitos de usuário e manter a segurança.

* **Fornecer** mídia da rede SaaS do Dynamic Media Classic para páginas da Web, aplicativos e dispositivos móveis; a mídia é otimizada para desempenho e é fornecida com o armazenamento em cache CDN. O Dynamic Media Classic fornece um URL para cada ativo. Depois de publicar o ativo, o URL se torna ativo.

![O processo de fluxo de trabalho do Dynamic Media Classic](/help/assets/gs_workflow.png)

## Imagens mestre únicas e chamadas de URL únicas {#single-master-images-and-single-url-calls}

O Dynamic Media Classic é fundamentalmente diferente de outros sistemas porque você pode usar o Dynamic Media Classic para fornecer mídia dinamicamente de ativos mestre individuais e chamadas de URL.

As strings de URL geradas com o Dynamic Media Classic incluem instruções que informam ao servidor como exibir o ativo quando ele é entregue. Por exemplo, a mesma imagem mestre pode ser entregue em tamanhos, formatos, pesos, cores e exibições de zoom diferentes. Como parte da criação e publicação de ativos de mídia com o Dynamic Media Classic, você configura visualmente os efeitos. Ao fazer isso, você cria as chamadas de URL que informam corretamente o servidor sobre como apresentar seu ativo mestre aos aplicativos.

![O Dynamic Media Classic pode fornecer a mesma imagem mestre para diferentes mídias em diferentes tamanhos e formatos.](/help/assets/gs_dynamic_publishing.png)

## Armazenamento de conteúdo em cache {#content-caching}

As imagens geradas dinamicamente pelo Dynamic Media Classic são compatíveis com cache; na maioria dos casos, são imagens JPEG com chamadas de URL exclusivas que as identificam. As imagens são fornecidas na CDN (Content Delivery Network, rede de entrega de conteúdo), um sistema de servidores que são conectados em rede na Internet para fornecer conteúdo mais rápido. As imagens são distribuídas de servidores localizados globalmente e, em seguida, de computadores. Ao implementar um mecanismo de cache usando qualquer fornecedor de CDN, basta alterar o nome do servidor para apontar para o Servidor de Imagem de Mídia Dinâmica habilitado para CDN. Todas as edições do Dynamic Media Classic incluem cache CDN empacotado.
