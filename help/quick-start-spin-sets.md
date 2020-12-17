---
title: '"Start rápido: Conjuntos de rotação"'
seo-title: '"Start rápido: Conjuntos de rotação"'
description: nulo
seo-description: Uma introdução e um Start rápido para o Conjunto de rotação para ajudá-lo a começar a funcionar rapidamente.
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---


# Start rápido: Conjuntos de rotação{#quick-start-spin-sets}

Um Conjunto de rotação simula o ato real de girar um objeto para examiná-lo. Os Conjuntos de rotação possibilitam a visualização de itens de qualquer ângulo, obtendo os detalhes visuais principais de qualquer ângulo. Um conjunto de rotação simula uma experiência de visualização de 360 graus. Conjuntos de rotação unidimensionais do Dynamic Media Classic oferta nos quais os visualizadores podem girar um item, e Conjuntos de rotação bidimensionais nos quais os visualizadores podem girar e girar o item. Além disso, os usuários podem aplicar zoom e deslocar qualquer uma das visualizações com apenas alguns cliques do mouse. Dessa forma, os usuários podem examinar um item mais detalhadamente de um ponto de vista específico.

![Imagens para um conjunto de rotação.](/help/assets/spin_set.png)

Os Conjuntos de rotação também aceitam os Mapas de imagem. Um Mapa de imagem é uma região em uma imagem dentro do Conjunto de rotação que exibe um painel de rolagem com texto. Quando o usuário clica em um Mapa de imagem, uma ação de algum tipo é acionada. Por exemplo, uma página da Web é aberta para que o usuário possa saber mais sobre um produto. Para chamar a atenção para o uso de um mapa de imagem em um Conjunto de rotação, um contorno é exibido ao redor do próprio Mapa de imagem quando o usuário move o ponteiro do mouse sobre ele.

Consulte [Criação de mapas de imagem](creating-image-maps.md).

**Start rápido**

Este Start rápido de Conjuntos de rotação foi projetado para começar a funcionar rapidamente com as técnicas de Conjunto de rotação no Dynamic Media Classic. Siga as etapas de 1 a 7. No final de cada etapa há uma referência cruzada para um cabeçalho de tópico no qual você pode encontrar mais informações se precisar.

**1. Criação e upload das imagens**

No mínimo, você precisa de 8 a 12 fotos de um item para um Conjunto de rotação unidimensional e 16 a 24 para um Conjunto de rotação bidimensional. As fotos devem ser tiradas a intervalos regulares para dar a impressão de que o item está girando e sendo virado. Por exemplo, se um Conjunto de rotação unidimensional incluir 12 fotos, gire o item 30 graus (360/12) para cada tomada.

Selecione o botão Carregar na barra Navegação global para carregar imagens de rotação do computador ou da rede para o Dynamic Media Classic.

Consulte [Diretrizes para fotografar imagens do Spin Set](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

**2. Criação de um conjunto de rotação**

Para criar um Conjunto de rotação, clique no botão Criar e escolha Conjuntos de rotação. Na caixa de diálogo Tamanho do conjunto de rotação, escolha quantas linhas e células deseja e clique em OK. Em seguida, arraste as imagens para a grade na tela Conjunto de rotação.

Consulte [Criação de um conjunto de rotação](creating-spin-set.md#creating-a-spin-set).

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

**3. Editar um conjunto de rotação**

Para editar um Conjunto de rotação, selecione o botão Editar sobreposição. A tela Conjunto de rotação é aberta. Adicione, remova e altere a posição das imagens. É possível alterar a posição das linhas em conjuntos de rotação bidimensionais.

Consulte [Editando um conjunto de rotação](creating-spin-set.md#editing-a-spin-set).

**4. Configuração das predefinições do visualizador Spin Set**

Os administradores podem criar predefinições do visualizador do Spin Set. Essas predefinições determinam a aparência do visualizador de conjunto de rotação. Para configurar uma nova predefinição do visualizador de conjunto de rotação, selecione o botão Configuração na barra Navegação global. Na tela Configuração, exiba as opções de Configuração do aplicativo e selecione Predefinições do visualizador.

Na tela Predefinições do visualizador, selecione o menu Adicionar e escolha Visualizador do conjunto de rotação na caixa de diálogo Adicionar predefinição do visualizador. Em seguida, escolha as opções na tela Configurar visualizador.

Consulte [Configurando predefinições do visualizador do Spin Set](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

**5. Pré-visualização de um Conjunto de rotação**

Selecione seu Conjunto de rotação no Painel de navegação e clique em seu botão de Pré-visualização de rolagem. Na tela de Pré-visualização, mantenha pressionado o botão do mouse e arraste o ponteiro para a esquerda ou para a direita para &quot;girar&quot; visualmente o item.

Consulte [Pré-visualização de um Conjunto de rotação](previewing-spin-set.md#previewing-a-spin-set).

**6. Publicar um conjunto de rotação**

A publicação de um conjunto de rotação o coloca em servidores Dynamic Media Classic para que possa ser entregue dinamicamente ao seu site ou aplicativo. Ela também ativa a string de URL que chama o Conjunto de rotação dos servidores de imagem Dynamic Media para o site ou aplicativo.

Para publicar um Conjunto de rotação, marque-o para publicação selecionando o ícone **Marcar para publicação** ao lado de seu nome no Painel de navegação. Clique em **Publicar** na barra Navegação global para iniciar uma publicação. Na tela Publicar, clique em **Publicar Start**.

Consulte [Publicar um conjunto de rotação](publishing-spin-set.md#publishing-a-spin-set).

**7. Vincular um conjunto de rotação a uma página da Web**

O Dynamic Media Classic cria sequências de chamada de URL para Conjuntos de rotação e as ativa depois que você as publica. Você pode copiar esses URLs da tela de Pré-visualização.

Selecione o Conjunto de rotação e clique em **Pré-visualização**. A tela Pré-visualização é aberta. Selecione uma predefinição do visualizador de conjunto de rotação. Em seguida, clique em **Copiar URL**.

Consulte [Vincular um conjunto de rotação a uma página da Web](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
