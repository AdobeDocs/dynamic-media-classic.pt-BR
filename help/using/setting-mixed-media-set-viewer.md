---
title: Configurar uma predefinição do visualizador de conjunto de mídia mista
description: Saiba como configurar uma Predefinição do visualizador de conjunto de mídia mista no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: d41b30e7-994a-43f3-8698-7dbfc36305ae
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Configurar uma predefinição do visualizador de conjunto de mídia mista{#setting-up-a-mixed-media-set-viewer-preset}

As Predefinições do visualizador de conjunto de mídia mista determinam o estilo, o comportamento e a aparência do visualizador principal. Ao configurar uma predefinição, especifique quais outros visualizadores você deseja exibir dentro do Visualizador de mídia mista. Por exemplo, se você incluiu um Conjunto de imagens no Conjunto de mídias mistas, especifique uma Predefinição do visualizador de Conjunto de imagens para o visualizador de Conjunto de mídias mistas.

Você pode optar por incluir todos ou alguns recursos da comunidade no Visualizador de conjunto de mídia mista. O recurso Incorporar adiciona um link ao visualizador que permite aos usuários copiar o código necessário para exibir o visualizador em uma página externa (como um blog, site ou site de rede social). O recurso Link fornece o URL para o visualizador, para que os usuários possam vincular-se de volta a esse visualizador. O recurso Visita fornece um link para o site da Web especificado.

1. Na barra de Navegação Global, vá para **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Na página Predefinições do visualizador, siga um destes procedimentos:

   * Para criar uma predefinição, selecione **[!UICONTROL Add]**. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma. Depois clique em **[!UICONTROL Mixed Media Set Viewer]** > **[!UICONTROL Add]**.
   * Para editar uma Predefinição do visualizador de conjunto de mídia mista, selecione-a e, em seguida, **[!UICONTROL Edit]**.

1. Na página Visualizador de configuração, digite um nome na caixa Nome da predefinição da Predefinição do visualizador de conjunto de mídia mista.
1. Especifique **[!UICONTROL Tabs]** ou **[!UICONTROL No Tabs]**. Tabulações separam itens por tipo, como vídeos, amostras e Conjuntos de rotação. Quando você não especificar nenhuma guia, todos os itens aparecerão em uma linha na janela Visualizar.
1. Na caixa **[!UICONTROL Name]**, digite um nome para o visualizador que deseja adicionar.

   Por exemplo, se você estiver adicionando um Conjunto de amostras ao seu Conjunto de mídias mistas, digite `Swatch Set A`.

1. No menu Visualizador, selecione o tipo de ativo que deseja exibir, como Conjuntos de amostras.
1. No menu Predefinição, selecione uma predefinição para o tipo de ativo escolhido.

   Por exemplo, se você estiver adicionando um Conjunto de Amostras, selecione **[!UICONTROL SwatchSet1-Colors]**.

1. Selecione **[!UICONTROL Add]**.

   A nova predefinição do visualizador é exibida na lista.

1. Repita as etapas 6: 9 para todas as predefinições do visualizador que você deseja adicionar.
1. Para editar a lista predefinida, siga um destes procedimentos:

   * Para excluir uma predefinição da lista, selecione-a e, em seguida, selecione **[!UICONTROL Delete]**.
   * Para reordenar predefinições na lista, selecione uma predefinição e a seta azul **[!UICONTROL Up]** ou **[!UICONTROL Down]**.

1. Para adicionar recursos da comunidade (Incorporar, Link, Visita) ao visualizador, especifique opções para qualquer um dos seguintes itens:

   * **Email**: selecione **[!UICONTROL On]** para habilitar um botão Email no visualizador. Quando os usuários selecionam o botão Email ao visualizar o conjunto, um email contendo o link para o conjunto é aberto.

   * **Incorporado**: Selecione **[!UICONTROL Live]**. Na caixa Rótulo do botão Incorporar, digite o nome que deseja exibir no visualizador do botão Incorporar. Se desejar, selecione **[!UICONTROL Browse]** para localizar e selecionar uma capa personalizada para o botão.

   * **Link**: Selecione **[!UICONTROL Live]**. Na caixa Rótulo do botão de link, digite o nome que deseja exibir no visualizador do botão Link. Se desejar, selecione **[!UICONTROL Browse]** para localizar e selecionar uma capa personalizada para o botão.

   * **Visita**: Selecione **[!UICONTROL Live]**. Na caixa Rótulo do botão de visita, digite o nome que deseja exibir no visualizador do botão de visita. Na caixa URL da visita, digite o URL do site que você deseja abrir quando o link for selecionado.

1. Especifique outras opções, conforme desejado. Para ver uma descrição de uma opção, selecione o ícone Dica de informações ao lado da opção.

   A página Visualizar exibe o visualizador à medida que você atualiza e altera as configurações.

1. Selecione **[!UICONTROL Save]**.

>[!MORELIKETHIS]
>
>* [Criar e editar Predefinições do Visualizador](application-setup.md#adding_and_editing_viewer_presets)
