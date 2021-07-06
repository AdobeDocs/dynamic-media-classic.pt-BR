---
title: '"Início rápido: Conjuntos de rotação"'
description: Uma introdução e o Início rápido para o Conjunto de rotação para ajudá-lo a ativar e executar rapidamente.
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Visualizadores,Conjuntos de rotação
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

# Início rápido: Conjuntos de rotação{#quick-start-spin-sets}

Um Conjunto de rotação simula o ato real de girar um objeto para examiná-lo. Os Conjuntos de rotação permitem visualizar itens de qualquer ângulo, obtendo os detalhes visuais principais de qualquer ângulo. Um Conjunto de rotação simula uma experiência de visualização de 360 graus. O Dynamic Media Classic oferece Conjuntos de rotação unidimensionais em que os visualizadores podem girar um item, e Conjuntos de rotação bidimensionais em que os visualizadores podem girar e virar o item. Além disso, os usuários podem &quot;formar livremente&quot; o zoom e deslocar qualquer uma das exibições com apenas alguns cliques do mouse. Dessa forma, os usuários podem examinar um item mais detalhadamente de um ponto de vista específico.

![Imagens para um conjunto de rotação.](/help/assets/spin_set.png)

Os Conjuntos de rotação também aceitam os Mapas de imagem. Um Mapa de imagem é uma região em uma imagem dentro do Conjunto de rotação que exibe um painel de rolagem com texto. Quando o usuário clica em um Mapa de imagem, uma ação de algum tipo é acionada. Por exemplo, uma página da Web é iniciada para que o usuário possa saber mais sobre um produto. Para apontar um mapa de imagem em um Conjunto de rotação, um contorno aparece ao redor do próprio Mapa de imagem quando o usuário move seu ponteiro do mouse sobre ele.

Consulte [Criação de mapas de imagem](creating-image-maps.md).

O Início rápido dos conjuntos de rotação foi projetado para entrar em operação rapidamente com as técnicas do conjunto de rotação no Dynamic Media Classic. Siga as etapas de 1 a 7. Ao final de cada etapa, você pode clicar em um link de tópico para saber mais.

## 1. Criação e upload das imagens

No mínimo, você precisa de 8 a 12 capturas de um item para um Conjunto de rotação unidimensional e 16 a 24 para um Conjunto de rotação bidimensional. As fotos devem ser tiradas regularmente para dar a impressão de que o item está girando e sendo virado. Por exemplo, se um Conjunto de rotação unidimensional incluir 12 capturas, gire o item 30° (360/12) para cada disparo.

Na barra Navegação global, clique em **[!UICONTROL Upload]** para carregar imagens de rotação do seu computador ou rede para o Dynamic Media Classic.

Consulte [Diretrizes para fotografar imagens do Conjunto de rotação](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

## 2. Criação de um conjunto de rotação

Para criar um Conjunto de rotação, na barra Navegação global, clique em **[!UICONTROL Build]** > **[!UICONTROL Spin Sets]**. Na caixa de diálogo Tamanho do conjunto de rotação, escolha quantas linhas e células você deseja e clique em **[!UICONTROL OK]**. Em seguida, arraste as imagens para a grade na página Conjunto de rotação .

Consulte [Criação de um Conjunto de rotação](creating-spin-set.md#creating-a-spin-set).

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>See <a href="#UnresolvedLink-sc7_spinsets_sp.xml#WS98ca2e6790647c06-245331fc135ab744793-8000">Including Image Maps in Spin Sets</a> to add clickable, hotspot regions, known as Image Maps, to images in a Spin Set. </p>

 -->

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>See also <a href="#UnresolvedLink-sc7_spinsets_sp.xml#WS98ca2e6790647c06229f600f135ab7cc461-8000">Managing InfoPanel content</a>.</p>

 -->

## 3. Editar um conjunto de rotação

Para editar um Conjunto de rotação, na barra Navegação global, clique em **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**. Selecione um conjunto de rotação e clique em **[!UICONTROL Edit]**. Adicione, remova e altere a posição das imagens. É possível alterar a posição das linhas em conjuntos de rotação bidimensionais.

Consulte [Editar um Conjunto de rotação](creating-spin-set.md#editing-a-spin-set).

## 4. Configuração das predefinições do visualizador do conjunto de rotação

Os administradores podem criar Predefinições do visualizador de conjunto de rotação. Essas predefinições determinam a aparência do Visualizador de conjunto de rotação. Para configurar uma nova Predefinição do Visualizador do Conjunto de rotação, na barra Navegação global, clique em **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.

Na página Predefinições do visualizador , clique em **[!UICONTROL Add]**, selecione **[!UICONTROL Spin Set Viewer]** na lista suspensa e clique em **[!UICONTROL Add]**. Escolha as opções na página Configurar visualizador e clique em **[!UICONTROL Save]**.

Consulte [Configuração das predefinições do visualizador do conjunto de rotação](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5. Visualização de um conjunto de rotação

Selecione seu Conjunto de rotação no painel Procurar e clique em **[!UICONTROL Preview]**. Na página Visualização, mantenha pressionado o botão do mouse e arraste o ponteiro para a esquerda ou direita para &quot;girar&quot; visualmente o item.

Consulte [Pré-visualização de um Conjunto de rotação](previewing-spin-set.md#previewing-a-spin-set).

## 6. Publicar um conjunto de rotação

A publicação de um Conjunto de rotação o coloca em servidores Dynamic Media Classic, de modo que possa ser entregue dinamicamente ao seu site ou aplicativo. Ela também ativa a cadeia de caracteres do URL que chama o Conjunto de rotação dos servidores de imagem da Dynamic Media para o site ou aplicativo.

Para publicar um Conjunto de rotação, marque-o para publicação selecionando o ícone **[!UICONTROL Mark for Publish]** ao lado de seu nome no Painel de navegação. Na barra Navegação global, clique em **[!UICONTROL Publish]** para iniciar uma publicação. Na tela Publicar , clique em **[!UICONTROL Submit Publish]**.

Consulte [Publicar um conjunto de rotação](publishing-spin-set.md#publishing-a-spin-set).

## 7. Vincular um conjunto de rotação a uma página da Web

O Dynamic Media Classic cria sequências de chamada de URL para Conjuntos de rotação e as ativa após você publicá-las. Você pode copiar esses URLs da página Visualizar.

Selecione o Conjunto de rotação e clique em **[!UICONTROL Preview]**. Selecione uma predefinição do visualizador de conjunto de rotação. Em seguida, clique em **[!UICONTROL Copy URL]**.

Consulte [Vincular um conjunto de rotação a uma página da Web](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
