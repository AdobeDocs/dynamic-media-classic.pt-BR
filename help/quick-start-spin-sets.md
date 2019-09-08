---
title: '" Início rápido: Conjuntos de rotação "'
seo-title: '" Início rápido: Conjuntos de rotação "'
description: 'null'
seo-description: Uma introdução e início rápido ao Spin Set para ajudá-lo a começar a usar rapidamente.
uuid: d 0 af 9 db 6-cb 6 f -48 f 0-89 f 6-f 3 ab 2 da 0659 f
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/spin_ sets
discoiquuid: 282 b 8 e 83-b 20 f -43 f 7-b 9 f 8-6 eebd 5 b 1 c 5 a 7
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Início rápido: Conjuntos de rotação{#quick-start-spin-sets}

Um Conjunto de rotação simula o ato real de girar um objeto para examiná-lo. Os Conjuntos de rotação possibilitam a exibição de itens de qualquer ângulo, obtendo os detalhes visuais principais de qualquer ângulo. Um Conjunto de rotação simula uma experiência de visualização de 360 graus. O Dynamic Media Classic oferece Conjuntos de rotação unidimensionais nos quais os visualizadores podem girar um item e bidões bidimensionais nos quais os visualizadores podem girar e virar o item. Além disso, os usuários podem aplicar zoom e deslocar o zoom de qualquer uma das exibições com alguns cliques do mouse simples. Dessa forma, os usuários podem examinar um item mais detalhadamente de um ponto de vista específico.

![Imagens para um conjunto de rotação.](/help/assets/spin_set.png)

Conjuntos de rotação também aceitam Mapas de imagem. Um Mapa de imagem é uma região em uma imagem no Conjunto de rotação que exibe um painel de rolagem com texto. Quando o usuário clica em um Mapa de imagem, uma ação de algum tipo é acionada. Por exemplo, uma página da Web é aberta para que o usuário saiba mais sobre um produto. Para chamar a atenção para o uso de um mapa de imagem em um Conjunto de rotação, um contorno aparece em torno do próprio Mapa de imagem quando o usuário move o ponteiro do mouse sobre ele.

Consulte [Criar mapas de imagem](creating-image-maps.md).

**Início rápido**

Esse Início rápido define o início rápido com técnicas de rotação de rotação no Dynamic Media Classic. Siga as etapas de 1 a 7. Ao final de cada etapa, é uma referência cruzada para um cabeçalho de tópico, onde você pode encontrar mais informações, se necessário.

**1. Como criar e carregar as imagens**

No mínimo, você precisa de capturas de 8-12 de um item para um Rotação de rotação unidimensional e 16-24 para um Conjunto de rotação bidimensional. As capturas devem ser realizadas em intervalos regulares para dar a impressão de que o item está girando e sendo girado. Por exemplo, se um Rotação de rotação unidimensional incluir 12 capturas, gire o item 30 graus (360/12) para cada captura.

Selecione o botão Carregar na barra Navegação global para carregar imagens de rotação do computador ou rede para o Sistema de publicação Scene 7.

Consulte [Diretrizes para tirar imagens de Conjunto de rotação](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

**2. Criar um conjunto de rotação**

Para criar um Conjunto de rotação, clique no botão Build e escolha Conjuntos de rotação. Na caixa de diálogo Tamanho do conjunto de rotação, escolha quantas linhas e células quiser e clique em OK. Em seguida, arraste imagens para a grade na tela Conjunto de rotação.

Consulte [Criar um conjunto de rotação](creating-spin-set.md#creating-a-spin-set).

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

**3. Edição de um conjunto de rotação**

Para editar um Conjunto de rotação, selecione o botão Editar rolagem. A tela de Rotação de rotação é aberta. Adicione, remova e altere a posição das imagens. É possível alterar a posição das linhas em conjuntos de rotação bidimensionais.

Consulte [Editando um conjunto de rotação](creating-spin-set.md#editing-a-spin-set).

**4. Configuração de predefinições do visualizador de rotação**

Os administradores podem criar predefinições do Visualizador de rotação. Essas predefinições determinam a aparência do Visualizador de rotação. Para configurar uma nova Predefinição do visualizador de rotação, selecione o botão Configuração na barra Navegação global. Na tela Configuração, exiba opções de Configuração de aplicativo e selecione Predefinições do visualizador.

Na tela Predefinições do visualizador, selecione o menu Adicionar e escolha Visualizador de rotação de rotação na caixa de diálogo Adicionar predefinição do visualizador. Em seguida, escolha opções na tela Configurar visualizador.

Consulte [Configuração de predefinições do visualizador de rotação](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

**5. Visualização de um conjunto de rotação**

Selecione seu Conjunto de rotação no Painel Procurar e clique no botão Visualizar sobreposições. Na tela Visualizar, mantenha o botão do mouse pressionado e arraste o ponteiro esquerdo ou direito para visualmente «girar» o item.

Consulte [Visualizar um conjunto de rotação](previewing-spin-set.md#previewing-a-spin-set).

**6. Publicar um conjunto de rotação**

A publicação de um Conjunto de rotação a coloca nos servidores do Dynamic Media Classic para que ela possa ser fornecida dinamicamente em seu site ou aplicativo. Ela também ativa a sequência de caracteres de URL que chama o Conjunto de rotação dos servidores de Imagem de Dynamic Media para o seu site ou aplicativo.

Para publicar um Conjunto de rotação, marque-o para publicar, selecionando **o ícone Marcar para publicar** ao lado de seu nome no Painel Procurar. Clique **em Publicar** na barra de navegação global para iniciar uma publicação. Na tela Publicar, clique **em Iniciar publicação**.

Consulte [Publicação de um conjunto de rotação](publishing-spin-set.md#publishing-a-spin-set).

**7. Vincular um conjunto de rotação a uma página da Web**

O Dynamic Media Classic cria sequências de caracteres de chamada de URL para Conjuntos de rotação e as ativa depois de publicá-las. Você pode copiar esses urls da tela Visualizar.

Selecione o Conjunto de rotação e clique **em Visualizar**. A tela Visualizar é aberta. Selecione uma Predefinição do visualizador de rotação. Em seguida, clique **em Copiar URL**.

Consulte [Vincular um conjunto de rotação a uma página da Web](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
