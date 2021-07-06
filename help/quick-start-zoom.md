---
title: '"Início rápido: Zoom"'
description: Uma introdução e o Início rápido para o Zoom para ajudá-lo a ativar e executar rapidamente.
uuid: 31eda632-3469-4f90-885b-e90c6a2e5e75
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 559c986d-313d-46df-a5ff-0b49316ad3a7
feature: Dynamic Media Classic,Visualizadores,Zoom
role: User
exl-id: eae35207-000c-4ced-b9ab-714c2384a9e7
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Início rápido: Zoom{#quick-start-zoom}

O zoom permite que você visualize interativamente detalhes de alta resolução em imagens. Por exemplo, você pode ver as cores, opções, ângulos e detalhes de uma imagem em um visualizador dinâmico, totalmente configurável e integrado. Esse visualizador pode ser incorporado em uma página da Web ou aparecer em uma janela pop-up. Você pode auditar imagens de perto e deslocar imagens em altas resoluções para examiná-las de perto. O zoom oferece aos clientes uma experiência de visualização envolvente, informativa e interativa.

O Dynamic Media Classic também oferece zoom guiado — um meio para destacar os recursos importantes em uma imagem. Por exemplo, para concentrar a atenção dos visualizadores em um logotipo, você pode criar um direcionamento de zoom para o logotipo. Quando os visualizadores clicam nesse direcionamento de zoom, eles fazem zoom no logotipo.

Todas as imagens de zoom são criadas e servidas a partir de imagens principais únicas, gráficos e atributos orientados por banco de dados. O zoom do Dynamic Media Classic reduz bastante o tempo e o custo de produção e entrega de imagens. Você pode usar Visualizadores de zoom para ampliar e diminuir o zoom das imagens. O Visualizador de Zoom tem botões que você pode clicar para aplicar zoom e deslocar; também é possível deslocar ao arrastar na tela. Usando Predefinições de Visualizador de Zoom, é possível configurar o Visualizador de Zoom no qual você aplica zoom às imagens.

Este Início rápido de Zoom foi projetado para se ativar e executar rapidamente com as técnicas de Zoom no Dynamic Media Classic. Siga as etapas de 1 a 6. Após cada etapa é uma referência cruzada a um cabeçalho de tópico, onde você pode encontrar mais informações.

## 1. Upload de imagens de zoom

Comece carregando suas imagens de zoom no Dynamic Media Classic. Para obter o zoom ideal, o Dynamic Media Classic recomenda que as imagens tenham pelo menos 2000 pixels no tamanho mais longo.

Na barra Navegação global, clique em **[!UICONTROL Upload]** para carregar imagens do seu computador ou rede para uma pasta no Dynamic Media Classic. Consulte [Upload de imagens de zoom](uploading-zoom-images.md#uploading_zoom_images).

## 2. Criação de destinos de zoom para zoom guiado

Os direcionamentos de zoom apresentam uma maneira de destacar partes específicas de uma imagem. Por exemplo, você pode direcionar a atenção para as partes de uma imagem que a tornam exclusiva ou distinta. Na janela Visualizador de zoom, os destinos de zoom são exibidos na forma de imagens em miniatura ao lado da imagem. Selecionar uma dessas miniaturas de direcionamento de zoom automaticamente amplia para uma parte da imagem especificada.

Para criar um direcionamento de zoom, clique em **[!UICONTROL Edit]** e escolha Metas de zoom ou abra uma imagem no Painel de navegação na exibição Detalhes e clique em **[!UICONTROL Zoom Targets]**. Em seguida, use as ferramentas de Zoom na página Editor de direcionamento de zoom para isolar parte da imagem como destino. Consulte [Criação de destinos de zoom para o Zoom Guiado](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).

## 3. Configuração das predefinições do visualizador de zoom

As Predefinições do visualizador de zoom determinam o estilo e o comportamento dos visualizadores de zoom. É possível configurar as Predefinições do visualizador de zoom se você for um administrador; O Dynamic Media Classic também vem com as predefinições padrão do visualizador de zoom.

Para criar uma Predefinição de Visualizador de Zoom, na barra Navegação Global, clique em **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**. Na página Predefinições do visualizador , clique em **[!UICONTROL Add]**, escolha uma plataforma e um Visualizador de zoom e clique em **[!UICONTROL Add]**. Em seguida, escolha as opções na página Configurar visualizador .

O Dynamic Media Classic oferece **[!UICONTROL Zoom Viewer Preset]** opções que permitem selecionar o estilo do botão e a aparência geral do visualizador. Também é possível personalizar as configurações de zoom do site. Consulte [Configuração das predefinições do visualizador de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## 4. Visualização de imagens com o Visualizador de Zoom

Você pode visualizar imagens em um Visualizador de zoom para ver qual é a experiência de zoom quando as imagens são ampliadas.

Para explorar diferentes predefinições do visualizador de zoom e como elas apresentam a experiência de zoom, selecione uma imagem no painel Procurar e clique em **[!UICONTROL Preview]**. Clique em **[!UICONTROL Presets]** > **[!UICONTROL Zoom]** e selecione uma predefinição com os menus de Zoom.

Os botões de zoom são exibidos. Você pode ver a aparência das imagens de zoom em seu site. Clique nos botões Zoom (e direcionamentos de zoom) para testar as configurações da Predefinição do Visualizador de Zoom que você escolher. Consulte [Visualização de imagens com visualizadores de zoom diferentes](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

## 5. Publicação de imagens de zoom

A publicação de imagens de zoom as coloca em Servidores de imagem da Dynamic Media para que possam ser entregues ao seu site e aplicativo. Como parte do processo de publicação, o Dynamic Media Classic ativa cadeias de caracteres de URL. Essas sequências de caracteres do URL chamam imagens de zoom dos Servidores de Imagem Dynamic Media para seu site ou aplicativo.

Na barra Navegação global, clique em **[!UICONTROL Publish]**. Na caixa de diálogo Publicar , clique em **[!UICONTROL Submit Publish]**. Consulte [Publicação de imagens de zoom](publishing-zoom-images.md#publishing_zoom_images).

## 6. Vincular visualizadores de zoom à sua página da Web

O Dynamic Media Classic cria as cadeias de caracteres de chamada de URL necessárias para ampliar imagens e as ativa ao publicar imagens nos Dynamic Media Image Servers. Você pode copiar essas cadeias de caracteres de URL da página **[!UICONTROL Preview]**. Após copiar as cadeias de caracteres do URL, elas ficam disponíveis nos sites e aplicativos da Web. Consulte [Vincular visualizadores de zoom à sua página da Web](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages).
