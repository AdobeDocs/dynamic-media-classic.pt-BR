---
title: "Início rápido: conjuntos de rotação"
description: Uma introdução e um conjunto de início rápido para rotação para ajudar você a começar a usar o Adobe Dynamic Media Classic rapidamente.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
topic: Content Management
level: Beginner
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Início rápido: conjuntos de rotação{#quick-start-spin-sets}

Um Conjunto de rotação simula o ato do mundo real de virar um objeto para examiná-lo. Os Conjuntos de rotação permitem a visualização de itens de qualquer ângulo, obtendo os principais detalhes visuais de qualquer ângulo. Um Conjunto de rotação simula uma experiência de visualização de 360 graus. O Adobe Dynamic Media Classic oferece Conjuntos de rotação unidimensionais nos quais os visualizadores podem girar um item e Conjuntos de rotação bidimensionais nos quais os visualizadores podem girar e virar o item. Além disso, os usuários podem aplicar o zoom de forma &quot;livre&quot; e deslocar qualquer uma das visualizações com apenas alguns cliques do mouse. Dessa forma, os usuários podem examinar um item mais detalhadamente de um ponto de vista específico.

![Imagens para um grupo de rotação.](/help/using/assets/spin_set.png)

Os conjuntos de rotação também aceitam mapas de imagem. Um Mapa de imagem é uma região em uma imagem no Conjunto de rotação que exibe um painel de sobreposição com texto. Quando o usuário seleciona um Mapa de imagem, uma ação de algum tipo é acionada. Por exemplo, uma página da Web é iniciada para que o usuário possa saber mais sobre um produto. Para apontar um mapa de imagem em um Conjunto de rotação, um contorno é exibido ao redor do próprio Mapa de imagem quando o usuário move o ponteiro do mouse sobre ele.

Consulte [Criar mapas de imagem](creating-image-maps.md).

Consulte [Conjuntos de imagem e rotação: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) vídeo de treinamento.

Ao criar um Conjunto de rotação, o Adobe recomenda a seguinte prática recomendada e impõe os seguintes limites:

| Tipo de limite do grupo de rotação | Prática recomendada | Limite imposto |
| --- | --- | --- |
| Número máximo de linhas/colunas por conjunto 2D | 12 a 18 imagens por conjunto | 1000 |

Consulte também [Limitações do Dynamic Media](/help/using/limitations.md).

Este Início rápido dos conjuntos de rotação foi projetado para colocar suas operações em funcionamento rapidamente com técnicas de Conjunto de rotação no Adobe Dynamic Media Classic. Siga as etapas de 1 a 7. Ao final de cada etapa, é possível selecionar um link de tópico para saber mais.

## 1. Criar e carregar as imagens

No mínimo, você precisa de 8 a 12 imagens de um item para um Conjunto de rotação unidimensional e 16 a 24 para um Conjunto de rotação bidimensional. As fotos devem ser tiradas em intervalos regulares para dar a impressão de que o item está girando e sendo virado. Por exemplo, se um Conjunto de rotação unidimensional incluir 12 disparos, gire o item 30° (360/12) para cada disparo.

Na barra Navegação global, selecione **[!UICONTROL Upload]** para fazer upload de imagens giratórias do seu computador ou rede para o Adobe Dynamic Media Classic.

Consulte [Diretrizes para fotografar imagens do grupo de rotação](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

## 2. Criar um grupo de rotação

Para criar um Conjunto de rotação, na barra de Navegação global, acesse **[!UICONTROL Build]** > **[!UICONTROL Spin Sets]**. Na caixa de diálogo Tamanho do conjunto de rotação, escolha quantas linhas e células você deseja e selecione **[!UICONTROL OK]**. Em seguida, arraste as imagens para a grade na página Conjunto de rotação.

Consulte [Criar um grupo de rotação](creating-spin-set.md#creating-a-spin-set).

## 3. Editar um grupo de rotação

Para editar um Conjunto de rotação, na barra de navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**. Selecione um conjunto de rotação e selecione **[!UICONTROL Edit]**. Adicionar, remover e alterar a posição das imagens. É possível alterar a posição das linhas em conjuntos de rotação bidimensionais.

Consulte [Editar um grupo de rotação](creating-spin-set.md#editing-a-spin-set).

## 4. Configurar as predefinições do visualizador de conjunto de rotação

Os administradores podem criar Predefinições do visualizador de conjunto de rotação. Essas predefinições determinam a aparência do Visualizador de conjunto de rotação. Para configurar uma nova Predefinição do visualizador de conjunto de rotação, na barra Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.

Na página Predefinições do visualizador, selecione **[!UICONTROL Add]** e selecione **[!UICONTROL Spin Set Viewer]** na lista suspensa e selecione **[!UICONTROL Add]**. Escolha as opções no `Configure Viewer` e selecione **[!UICONTROL Save]**.

Consulte [Configurar predefinições do visualizador de conjunto de rotação](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5. Visualizar um grupo de rotação

Selecione o Conjunto de rotação no Painel de navegação e selecione **[!UICONTROL Preview]**. Na página Visualização, mantenha pressionado o botão do mouse e arraste o ponteiro para a esquerda ou direita para &quot;girar&quot; visualmente o item.

Consulte [Visualizar um conjunto de rotação](previewing-spin-set.md#previewing-a-spin-set).

## 6. Publicar um grupo de rotação

A publicação de um conjunto de rotação o coloca em servidores Adobe Dynamic Media Classic para que ele possa ser entregue dinamicamente ao seu site ou aplicativo. Ele também ativa a cadeia de caracteres do URL que chama o Conjunto de rotação dos servidores de imagem da Dynamic Media para o site ou aplicativo.

Para publicar um Conjunto de rotação, marque-o para publicação selecionando o **[!UICONTROL Mark for Publish]** ícone ao lado de seu nome no Painel de navegação. Na barra Navegação global, selecione **[!UICONTROL Publish]** para iniciar uma publicação. Na página Publicação, selecione **[!UICONTROL Submit Publish]**.

Consulte [Publicar um grupo de rotação](publishing-spin-set.md#publishing-a-spin-set).

## 7. Vincular um conjunto de rotação a uma página da Web

O Adobe Dynamic Media Classic cria cadeias de caracteres de texto explicativo de URL para conjuntos de rotação e os ativa após a publicação. Você pode copiar esses URLs da página Pré-visualização.

Selecione o Conjunto de rotação e selecione **[!UICONTROL Preview]**. Selecione uma predefinição do visualizador de conjunto de rotação. Em seguida, selecione **[!UICONTROL Copy URL]**.

Consulte [Vincular um grupo de rotação a uma página da Web](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
