---
title: Vincular visualizadores Zoom às suas páginas da Web
description: Saiba como vincular visualizadores de zoom às suas páginas da Web no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
topic: Administration, Content Management, Development
level: Intermediate
autotag-review: '2026-05-13T20:03:57.696Z'
TQID: 'https://experienceleague.adobe.com/Urf0qGJqj7tCCGDfNwprZnxf6YfDgavWb44pThwds0I'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 634
ht-degree: 0%

---

# Vincular visualizadores Zoom às suas páginas da Web{#linking-zoom-viewers-to-your-web-pages}

Seus sites e aplicativos acessam o conteúdo do Servidor de imagens do Dynamic Media por meio de cadeias de caracteres de URL ou código incorporado. Esse acesso inclui imagens primárias e Destinos de zoom associados. Também inclui Predefinições do visualizador de zoom. Essas cadeias de caracteres de URL são ativadas durante o processo de publicação. Para colocar essas cadeias de caracteres de URL ou o código incorporado nas páginas da Web e nos aplicativos, copie-as do Adobe Dynamic Media Classic.

>[!NOTE]
>
>O URL não estará ativo até que você publique o ativo.

## Copiar um URL do visualizador de zoom {#copying-a-zoom-viewer-url}

1. no painel Biblioteca de ativos à esquerda, navegue até a pasta de ativos que contém o visualizador de zoom cujo URL você deseja copiar.
1. Acima do painel Navegar por ativos, no lado direito da barra de ferramentas, siga um destes procedimentos:

   * Selecione **[!UICONTROL Grid View]** ou **[!UICONTROL List View]**. No painel Navegação de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. No painel URLs e Código de Inserção à direita, selecione **[!UICONTROL Copy URL]** à direita do visualizador desejado.
   * Selecione **[!UICONTROL Grid View]**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

   * Selecione **[!UICONTROL List View]**. No painel Navegar por ativos, selecione um único ativo e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

   * Selecione **[!UICONTROL Grid View]**, **[!UICONTROL List View]** ou **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

## Adicionar URLs do visualizador Zoom à sua página da Web {#adding-zoom-viewer-urls-to-your-web-page}

Normalmente, os visitantes ampliam imagens em um site selecionando primeiro um ícone Zoom (geralmente o ícone mostra a imagem de uma lupa). Selecionar esse ícone inicia uma página da Web dinâmica (ASP ou JSP) que exibe a imagem em uma janela pop-up. A janela pop-up é onde os visitantes realmente dão zoom na imagem.

Para obter mais detalhes e exemplos de código, consulte o [Visualizador de zoom básico incorporado do HTML5](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2) no Guia de referência de visualizadores do Adobe.

## Copiar a cópia incorporada de um visualizador de zoom {#copying-the-embed-copy-of-a-zoom-viewer}

O uso do recurso de código incorporado permite revisar o código do visualizador do visualizador de zoom selecionado. Você também pode copiar o código para a área de transferência para poder colá-lo em suas páginas da Web para implantação do visualizador. A edição do código não é permitida na caixa de diálogo Incorporar código.

**Para copiar o código inserido de um visualizador de zoom:**

1. no painel Biblioteca de ativos à esquerda, navegue até a pasta de ativos que contém o visualizador de zoom cujo Código incorporado você deseja copiar.
1. Acima do painel Navegar por ativos, no lado direito da barra de ferramentas, siga um destes procedimentos:

   * Selecione **[!UICONTROL Grid View]**. No painel Navegação de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. No painel URLs e Código de Inserção à direita, selecione **[!UICONTROL Embed Code]** à direita do visualizador desejado.
   * Selecione **[!UICONTROL Grid View]**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

   * Selecione **[!UICONTROL List View]**. No painel Navegar por ativos, selecione um único ativo e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

   * Selecione **[!UICONTROL Grid View]**, **[!UICONTROL List View]** ou **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

1. Na caixa de diálogo Incorporar código, selecione **[!UICONTROL Copy to Clipboard]**.

   A edição do código não é permitida na caixa de diálogo Incorporar código.

1. Selecione **[!UICONTROL Close]**.
