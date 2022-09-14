---
title: "Início rápido: Conjuntos de imagens"
description: Uma introdução e o Início rápido para conjuntos de imagens para ajudar você a ativar e executar rapidamente com as técnicas do Conjunto de imagens no Adobe Dynamic Media Classic.
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Início rápido: Conjuntos de imagens{#quick-start-image-sets}

Os Conjuntos de imagens da Adobe Dynamic Media Classic fornecem aos usuários uma experiência de visualização integrada. No Visualizador dinâmico de conjunto de imagens, os usuários podem ver diferentes visualizações de um item clicando em uma imagem em miniatura. Conjuntos de imagens permite apresentar exibições alternativas de alta resolução de um item.

O Visualizador de conjunto de imagens oferece ferramentas de zoom para examinar as imagens de perto. Se desejar, você pode tornar os destinos de zoom guiados e os Mapas de imagem parte do seu Conjunto de imagens. Os conjuntos de imagens proporcionam uma experiência de visualização mais concertada e íntima.

Consulte [Conjuntos de imagem e rotação: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) vídeo de treinamento.

Ao criar um Conjunto de imagens, o Adobe recomenda as seguintes práticas recomendadas e aplica os seguintes limites:

| Tipo de limite | Prática recomendada | Limite imposto |
| --- | --- | --- |
| Número de ativos duplicados por conjunto | Sem duplicatas | 20º |
| Número máximo de imagens por conjunto | 5 a 10 imagens por conjunto | 1000 |

Consulte também [Limitações do Dynamic Media](/help/limitations.md).

O Início rápido dos conjuntos de imagens a seguir foi projetado para ajudar você a trabalhar rapidamente com as técnicas do Conjunto de imagens no Adobe Dynamic Media Classic.

## 1. Carregue suas imagens primárias para várias exibições e amostras

Comece carregando as imagens dos seus Conjuntos de imagens. Como os usuários podem ampliar imagens no Visualizador do conjunto de imagens, certifique-se de contabilizar essa capacidade ao escolher imagens. Certifique-se de que as imagens tenham pelo menos 2000 pixels no tamanho maior. O Adobe Dynamic Media Classic oferece suporte a vários formatos de arquivo de imagem, mas as imagens TIFF, PNG e EPS sem perdas são recomendadas.

Na barra Navegação global, selecione **[!UICONTROL Upload]** para carregar arquivos do seu computador para uma pasta no Adobe Dynamic Media Classic.

Consulte [Preparar ativos do Conjunto de imagens para upload](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) e [Fazer upload de seus arquivos](uploading-files.md#uploading-your-files).

## 2. Criar um conjunto de imagens

Em Conjuntos de imagens, os usuários selecionam imagens em miniatura no Visualizador de conjunto de imagens para ver uma imagem de um lado ou ângulo diferente.

Para criar um Conjunto de imagens, na barra Navegação global, selecione **[!UICONTROL Build]** e escolha **[!UICONTROL Image Sets]**. Na janela Conjunto de imagens, arraste suas imagens para a página para compor seu Conjunto de imagens. Organize, adicione e exclua imagens conforme necessário.

Consulte [Criar um conjunto de imagens](creating-image-set.md#creating-an-image-set).

Consulte também [Incluir metas de zoom e mapas de imagem em conjuntos de imagens](/help/including-zoom-targets-image-maps-image-sets.md)

## 3. Prepare as predefinições do visualizador do conjunto de imagens, conforme necessário

Os administradores podem criar ou modificar as Predefinições do visualizador de conjunto de imagens. O Adobe Dynamic Media Classic vem com as Predefinições do visualizador padrão para cada tipo de mídia avançada. Usar o Visualizador de Zoom: **[!UICONTROL Custom]** > **[!UICONTROL Images]** ou **[!UICONTROL Image Sets]**/**[!UICONTROL Multiple Views]** predefinições para visualizar seus Conjuntos de imagens.

Adicione ou edite Predefinições do visualizador na tela Configuração do aplicativo .

Consulte [Criar e editar predefinições do visualizador](application-setup.md#adding-and-editing-viewer-presets).

## 4. Visualizar um conjunto de imagens

Selecione o Conjunto de imagens no painel Procurar e selecione **[!UICONTROL Preview]**. Na página Visualização , selecione os ícones de miniatura para examinar seu Conjunto de imagens no Visualizador selecionado. Você pode escolher visualizadores diferentes no menu Predefinições.

Consulte [Visualizar um ativo](previewing-asset.md#previewing-an-asset).

## 5. Publicar um conjunto de imagens

A publicação de um Conjunto de imagens o coloca em servidores da Adobe Dynamic Media Classic e ativa a string do URL.

>[!NOTE]
>
>Esta etapa não é necessária se você selecionou **[!UICONTROL Publish after save]** (padrão) no momento em que você criou e salvou o Conjunto de imagens.

Selecionar **[!UICONTROL Mark for Publish]** à esquerda de seu nome no Painel de navegação. Em seguida, selecione **[!UICONTROL Publish]**. Na página Publicar , selecione **[!UICONTROL Submit Publish]**.

Consulte [Publicar arquivos](publishing-files.md#publishing-files).

## 6. Vincular um conjunto de imagens ao seu site

O Adobe Dynamic Media Classic cria chamadas de URL para conjuntos de imagens e as ativa após a publicação. Você pode copiar esses URLs da tela de Visualização.

Selecione o Conjunto de imagens e selecione **[!UICONTROL Preview]**. Em seguida, selecione uma Predefinição do visualizador de conjunto de imagens e selecione **[!UICONTROL Copy URL]**.

Consulte [Vincular um conjunto de imagens a uma página da Web](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
