---
title: '"Start rápido: Zoom"'
seo-title: '"Start rápido: Zoom"'
description: nulo
seo-description: Uma introdução e Start rápido para Zoom para ajudá-lo a começar a funcionar rapidamente.
uuid: 31eda632-3469-4f90-885b-e90c6a2e5e75
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 559c986d-313d-46df-a5ff-0b49316ad3a7
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---


# Start rápido: Zoom{#quick-start-zoom}

O zoom permite que você visualização interativamente detalhes de alta resolução em imagens. Por exemplo, você pode ver as cores, opções, ângulos e detalhes de uma imagem em um visualizador dinâmico, totalmente configurável e integrado. Esse visualizador pode ser incorporado em uma página da Web ou aparecer em uma janela pop-up. Você pode inspecionar imagens em locais próximos e deslocar imagens em altas resoluções para examiná-las de perto. O zoom oferece aos clientes uma experiência de visualização envolvente, informativa e interativa.

O Dynamic Media Classic também orientou o zoom do oferta — um meio de destacar os recursos importantes em uma imagem. Por exemplo, para focar a atenção dos visualizadores em um logotipo, é possível criar um público alvo de zoom para o logotipo. Quando os visualizadores clicam nesse público alvo de zoom, eles aumentam o zoom para o logotipo.

Todas as imagens de zoom são criadas e servidas a partir de imagens principais, gráficos e atributos orientados por banco de dados. O zoom do Dynamic Media Classic reduz muito o tempo e o custo de produção e entrega de imagens. Você pode usar Visualizadores de zoom para aumentar e diminuir o zoom das imagens. O Visualizador de zoom tem botões nos quais você pode clicar para aplicar zoom e deslocar; você também pode deslocar arrastando na tela. Usando as Predefinições do visualizador de zoom, é possível configurar o Visualizador de zoom no qual você aplica zoom nas imagens.

**Start rápido**

Este Start de zoom rápido foi projetado para começar a funcionar rapidamente com as técnicas de zoom do Dynamic Media Classic. Siga as etapas de 1 a 6. Depois de cada etapa é uma referência cruzada para um cabeçalho de tópico no qual você pode encontrar mais informações.

**1. Upload de imagens de zoom**

Start carregando suas imagens de zoom no Dynamic Media Classic. Para obter o zoom ideal, o Dynamic Media Classic recomenda que as imagens tenham pelo menos 2000 pixels na dimensão mais longa.

Selecione o botão Carregar na barra Navegação global para carregar imagens do computador ou da rede para uma pasta no Dynamic Media Classic. Consulte [Carregando imagens de zoom](uploading-zoom-images.md#uploading_zoom_images).

**2. Criação de públicos alvos de zoom para zoom guiado**

Públicos alvos de zoom apresentam uma maneira de realçar partes específicas de uma imagem. Por exemplo, você pode direcionar a atenção para as partes de uma imagem que a tornam única ou distinta. Na janela do Visualizador de zoom, públicos alvos de zoom são exibidos na forma de imagens em miniatura na lateral da imagem. A seleção de uma dessas miniaturas de público alvo de zoom aumenta automaticamente para uma parte da imagem especificada.

Para criar um público alvo de zoom, clique no botão Editar de sobreposição e escolha Zoom em Públicos alvos ou abra uma imagem no Painel Procurar em visualização de detalhes e clique em Zoom em Públicos alvos. Em seguida, use as ferramentas de Zoom na tela do Editor de Públicos alvos de Zoom para isolar parte da imagem como um público alvo. Consulte [Criação de públicos alvos de zoom para Zoom Guiado](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).

**3. Configuração das predefinições do visualizador de zoom**

As predefinições do visualizador de zoom determinam o estilo e o comportamento dos visualizadores de zoom. Você pode configurar as Predefinições do Visualizador de Zoom se for um administrador; O Dynamic Media Classic também é fornecido com as predefinições padrão de &quot;prática recomendada&quot; do visualizador de zoom.

Para criar uma Predefinição do Visualizador de zoom, clique no botão Configuração na barra de navegação global e escolha Predefinições do visualizador. Em seguida, clique no botão Adicionar na tela Predefinições do visualizador, escolha uma plataforma, escolha um Visualizador de zoom e clique em Adicionar. Em seguida, escolha as opções na tela Configurar visualizador.

Opções de predefinição do visualizador de zoom do Dynamic Media Classic oferta que permitem selecionar o estilo do botão e a aparência geral do visualizador. Você também pode personalizar as configurações de zoom para seu site. Consulte [Configuração das predefinições do visualizador de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

**4. Visualização de imagens com o Visualizador de zoom**

Você pode pré-visualização imagens em um Visualizador de zoom para ver qual é a experiência de zoom quando as imagens são ampliadas.

Para explorar diferentes predefinições do visualizador de zoom e como elas apresentam a experiência de zoom, selecione uma imagem no painel Procurar e clique no botão Pré-visualização. A tela Pré-visualização é aberta. Escolha Predefinições > Zoom e selecione uma predefinição com os menus Zoom.

Botões de zoom são exibidos. Você pode ver a aparência das imagens de zoom em seu site. Selecione os botões Zoom (e públicos alvos de zoom) para testar as configurações da Predefinição do visualizador de zoom escolhida. Consulte [Visualizar imagens com visualizadores de zoom diferentes](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

**5. Publicar imagens de zoom**

A publicação de imagens com zoom as coloca em servidores de imagem Dynamic Media para que possam ser entregues ao seu site e aplicativo. Como parte do processo de publicação, o Dynamic Media Classic ativa strings de URL. Essas sequências de caracteres de URL chamam imagens de zoom dos Servidores de imagem Dynamic Media para o site ou aplicativo.

Selecione o botão Publicar na barra Navegação global para iniciar uma publicação. Na tela Publicar, selecione o botão Publicar Start. Consulte [Publicar imagens de zoom](publishing-zoom-images.md#publishing_zoom_images).

**6. Vincular visualizadores de zoom à sua página da Web**

O Dynamic Media Classic cria as sequências de caracteres de chamada de URL necessárias para aplicar zoom em imagens e as ativa ao publicar imagens nos Dynamic Media Image Servers. É possível copiar essas sequências de caracteres de URL da tela de Pré-visualização. Após copiar as sequências de caracteres do URL, elas estarão disponíveis para seus sites e aplicativos. Consulte [Vincular visualizadores de zoom à sua página da Web](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages).
