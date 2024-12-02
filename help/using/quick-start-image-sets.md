---
title: 'Início rápido: conjuntos de imagens'
description: Uma introdução e o Início rápido para conjuntos de imagens para ajudar você a começar a usar rapidamente as técnicas do Conjunto de imagens no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Início rápido: conjuntos de imagens{#quick-start-image-sets}

Os Conjuntos de imagens do Adobe Dynamic Media Classic oferecem aos usuários uma experiência de visualização integrada. No Visualizador dinâmico do conjunto de imagens, os usuários podem ver diferentes exibições de um item selecionando uma imagem em miniatura. Os Conjuntos de imagens permitem apresentar visualizações alternativas de alta resolução de um item.

O Visualizador de conjunto de imagens oferece ferramentas de zoom para examinar as imagens com atenção. Se desejar, você poderá tornar Destinos de zoom e Mapas de imagem parte do Conjunto de imagens. Os conjuntos de imagens proporcionam uma experiência de visualização mais organizada e íntima.

Veja [Conjuntos de imagem e rotação: vídeo de treinamento Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS).

Ao criar um Conjunto de imagens, o Adobe recomenda as seguintes práticas recomendadas e impõe os seguintes limites:

| Tipo de limite | Prática recomendada | Limite imposto |
| --- | --- | --- |
| Número de ativos duplicados por conjunto | Sem duplicatas | 20‡ |
| Número máximo de imagens por conjunto | De 5 a 10 imagens por conjunto | 1000 |

‡ A prática recomendada é não ter ativos duplicados em um conjunto. O limite é de 20 duplicatas para um único ativo. Se você adicionar outra duplicata para esse ativo — dentro desse conjunto — a solicitação retornará um erro ou ignorará a duplicata.

Consulte também [limitações do Dynamic Media](/help/using/limitations.md).

O seguinte Início rápido dos conjuntos de imagens foi projetado para você começar a usar rapidamente as técnicas do Conjunto de imagens no Adobe Dynamic Media Classic.

## 1. Faça upload das imagens principais para várias exibições e amostras

Comece fazendo upload das imagens para os seus Conjuntos de imagens. Como os usuários podem ampliar imagens no Visualizador de conjunto de imagens, certifique-se de levar em conta essa capacidade ao escolher imagens. Verifique se as imagens têm pelo menos 2000 pixels no maior tamanho. O Adobe Dynamic Media Classic é compatível com muitos formatos de arquivo de imagem, mas são recomendados TIFF, PNG e imagens EPS sem perdas.

Na barra Navegação global, selecione **[!UICONTROL Upload]** para carregar arquivos do seu computador para uma pasta no Adobe Dynamic Media Classic.

Consulte [Preparar ativos do Conjunto de Imagens para carregamento](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) e [Carregar seus arquivos](uploading-files.md#uploading-your-files).

## 2. Criar um conjunto de imagens

Em Conjuntos de imagens, os usuários selecionam imagens em miniatura no Visualizador de conjuntos de imagens para ver uma imagem de um lado ou ângulo diferente.

Para criar um Conjunto de imagens, na barra de Navegação global, selecione **[!UICONTROL Build]** e escolha **[!UICONTROL Image Sets]**. Na janela Conjunto de imagens, arraste as imagens para a página para compor seu Conjunto de imagens. Organize, adicione e exclua imagens conforme necessário.

Consulte [Criar um conjunto de imagens](creating-image-set.md#creating-an-image-set).

Consulte também [Incluir destinos de zoom e mapas de imagem em conjuntos de imagens](/help/using/including-zoom-targets-image-maps-image-sets.md)

## 3. Prepare Predefinições do visualizador do Conjunto de imagens, conforme necessário

Os administradores podem criar ou modificar as Predefinições do visualizador de conjunto de imagens. O Adobe Dynamic Media Classic vem com Predefinições do visualizador padrão para cada tipo de mídia avançada. Use o Visualizador de Zoom: **[!UICONTROL Custom]** > **[!UICONTROL Images]** ou **[!UICONTROL Image Sets]**/**[!UICONTROL Multiple Views]** predefinições para exibir seus Conjuntos de Imagens.

Você pode adicionar ou editar as Predefinições do visualizador na tela Configuração do aplicativo.

Consulte [Criar e editar Predefinições do Visualizador](application-setup.md#adding-and-editing-viewer-presets).

## 4. Visualizar um conjunto de imagens

Selecione o Conjunto de imagens no painel Procurar e selecione **[!UICONTROL Preview]**. Na página Visualizar, selecione os ícones de miniatura para examinar seu Conjunto de imagens no Visualizador selecionado. É possível escolher Visualizadores diferentes no menu Predefinições.

Consulte [Visualizar um ativo](previewing-asset.md#previewing-an-asset).

## 5. Publish e conjunto de imagens

A publicação de um Conjunto de imagens o coloca nos servidores do Adobe Dynamic Media Classic e ativa a cadeia de caracteres do URL.

>[!NOTE]
>
>Esta etapa não será necessária se você tiver selecionado **[!UICONTROL Publish after a save]** (padrão) no momento em que criou e salvou o Conjunto de imagens.

Selecione o ícone **[!UICONTROL Mark for Publish]** à esquerda de seu nome no painel Procurar. Depois selecione **[!UICONTROL Publish]**. Na página Publicação, selecione **[!UICONTROL Submit Publish]**.

Consulte [arquivos Publish](publishing-files.md#publishing-files).

## 6. Vincule um conjunto de imagens ao seu site

O Adobe Dynamic Media Classic cria chamadas de URL para conjuntos de imagens e as ativa após a publicação. Você pode copiar esses URLs da tela Preview.

Selecione o Conjunto de Imagens e selecione **[!UICONTROL Preview]**. Agora, selecione uma Predefinição do visualizador do Conjunto de imagens e clique no botão **[!UICONTROL Copy URL]**.

Consulte [Vincular o Conjunto de Imagens a uma página da Web](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
