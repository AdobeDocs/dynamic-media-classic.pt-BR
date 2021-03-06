---
title: Vincular um conjunto de rotação a uma página da Web
description: Saiba como vincular um Conjunto de rotação a uma página da Web no Adobe Dynamic Media Classic.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 1%

---

# Vincular um conjunto de rotação a uma página da Web{#linking-a-spin-set-to-a-web-page}

Os sites e aplicativos da Web acessam o conteúdo do Dynamic Media Image Server, incluindo Conjuntos de rotação, por meio de cadeias de caracteres de URL ou código incorporado. Essas cadeias de caracteres do URL são ativadas durante o processo de publicação. Para colocar a string do URL ou o código incorporado do Conjunto de rotação nas páginas e aplicativos da Web, você a copia do Adobe Dynamic Media Classic.

>[!NOTE]
>
>O URL não fica ativo até que você publique o ativo.

## Copiar um URL de conjunto de rotação {#copying-a-spin-set-url}

1. No painel Navegação de ativos , na lista suspensa Mostrar , selecione **[!UICONTROL Spin Set]**.
1. no painel Biblioteca de ativos , no lado esquerdo, navegue até a pasta de ativos que contém o Conjunto de rotação cujo código incorporado você deseja copiar.
1. Acima do painel Navegação de ativos , no lado direito da barra de ferramentas, execute um dos seguintes procedimentos:

   * Selecione **[!UICONTROL Grid View]**. No painel Navegação de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. No painel URLs e Código incorporado à direita, selecione **[!UICONTROL Copy URL]** à direita do visualizador desejado.
   * Selecione **[!UICONTROL Grid View]**. No painel Navegação de ativos, selecione um único ativo e, em seguida, abaixo da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Na página Lista de visualizadores , na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

   * Selecione **[!UICONTROL List View]**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Na página Lista de visualizadores , na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

   * Selecione **[!UICONTROL Grid View]**, **[!UICONTROL List View]** ou **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Na página Lista de visualizadores , na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

## Adicionar URLs do conjunto de rotação à sua página da Web {#adding-spin-set-urls-to-your-web-page}

Os Conjuntos de rotação são implantados como todos os visualizadores de zoom, por meio de uma página dinâmica (ASP ou JSP) que exibe o Conjunto de rotação em uma janela de zoom. A chamada de URL para a plataforma Adobe Dynamic Media Classic segue o mesmo protocolo no visualizador de zoom. No entanto, o nome da Predefinição do visualizador depende da Predefinição que seu administrador definiu como a Predefinição padrão do visualizador de conjunto de rotação. Por exemplo, o seguinte exemplo de sintaxe de URL não ativo inclui um nome de predefinição chamado `viewer.jsp` e o parâmetro SKU agora é o nome do Conjunto de rotação:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

Neste exemplo de sintaxe de URL (o link não está ativo), observe um número SKU ( `sku=backpack_spin`). A string depois de `sku=` é o nome do Conjunto de rotação ( `backpack spin`).

## Copiar o código incorporado de um visualizador de Conjunto de rotação {#copying-the-embed-code-of-a-spin-set-viewer}

Usar o recurso Incorporar código permite que você revise o código do visualizador para o Conjunto de rotação selecionado. Você também pode copiar o código para a área de transferência, de modo que possa colá-lo em suas páginas da Web para a implantação do visualizador. A edição do código não é permitida na caixa de diálogo Incorporar código.

**Para copiar o código incorporado de um visualizador de Conjunto de rotação:**

1. No painel Navegação de ativos , na lista suspensa Mostrar , selecione **[!UICONTROL Spin Set]**.
1. no painel Biblioteca de ativos , no lado esquerdo, navegue até a pasta de ativos que contém o Conjunto de rotação cujo código incorporado você deseja copiar.
1. Acima do painel Navegação de ativos , no lado direito da barra de ferramentas, execute um dos seguintes procedimentos:

   * Selecione **[!UICONTROL Grid View]**. No painel Navegação de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. No painel URLs e Código incorporado à direita, selecione **[!UICONTROL Embed Code]** à direita do visualizador desejado.
   * Selecione **[!UICONTROL Grid View]**. No painel Navegação de ativos, selecione um único ativo e, em seguida, abaixo da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Na página Lista de visualizadores , na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

   * Selecione **[!UICONTROL List View]**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Na página Lista de visualizadores , na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

   * Selecione **[!UICONTROL Grid View]**, **[!UICONTROL List View]** ou **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Na página Lista de visualizadores , na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

1. Na caixa de diálogo Incorporar código, selecione **[!UICONTROL Copy to Clipboard]**.

   A edição do código não é permitida na caixa de diálogo Incorporar código .

1. Selecione **[!UICONTROL Close]**.
