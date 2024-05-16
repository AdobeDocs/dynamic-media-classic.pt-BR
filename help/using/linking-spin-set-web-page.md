---
title: Vincular um conjunto de rotação a uma página da Web
description: Saiba como vincular um Conjunto de rotação a uma página da Web no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 0%

---

# Vincular um conjunto de rotação a uma página da Web{#linking-a-spin-set-to-a-web-page}

Os sites e aplicativos acessam o conteúdo do Dynamic Media Image Server, incluindo Conjuntos de rotação, por meio de cadeias de caracteres de URL ou código incorporado. Essas cadeias de caracteres de URL são ativadas durante o processo de publicação. Para colocar a string de URL ou o código incorporado do seu conjunto de rotação nas páginas e aplicativos da Web, copie-o do Adobe Dynamic Media Classic.

>[!NOTE]
>
>O URL não estará ativo até que você publique o ativo.

## Copiar um URL do grupo de rotação {#copying-a-spin-set-url}

1. No painel Navegar por ativos, na lista suspensa Mostrar, selecione **[!UICONTROL Spin Set]**.
1. no painel Biblioteca de ativos à esquerda, navegue até a pasta de ativos que contém o conjunto de rotação cujo código de inserção você deseja copiar.
1. Acima do painel Navegar por ativos, no lado direito da barra de ferramentas, siga um destes procedimentos:

   * Selecionar **[!UICONTROL Grid View]**. No painel Navegação de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. No painel URLs e código incorporado à direita, selecione **[!UICONTROL Copy URL]** à direita do visualizador desejado.
   * Selecionar **[!UICONTROL Grid View]**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem em miniatura, acesse **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

   * Selecionar **[!UICONTROL List View]**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

   * Selecionar **[!UICONTROL Grid View]**, **[!UICONTROL List View]** ou **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

## Adicionar URLs do grupo de rotação à página da Web {#adding-spin-set-urls-to-your-web-page}

Os Conjuntos de rotação são implantados como todos os visualizadores de zoom, por meio de uma página dinâmica (ASP ou JSP) que exibe o Conjunto de rotação em uma janela de zoom. A chamada de URL para a plataforma Adobe Dynamic Media Classic segue o mesmo protocolo no visualizador de zoom. No entanto, o nome da Predefinição do visualizador depende da Predefinição que o administrador definiu como a Predefinição do visualizador do conjunto de rotação padrão. Por exemplo, o seguinte exemplo de sintaxe de URL inativa inclui um nome de Predefinição chamado `viewer.jsp` e o parâmetro SKU agora é o nome do conjunto de rotação:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

Neste exemplo de sintaxe de URL (o link não está ativo), observe um número SKU ( `sku=backpack_spin`). A string após `sku=` é o nome do grupo de rotação ( `backpack spin`).

## Copiar o código incorporado de um visualizador de conjunto de rotação {#copying-the-embed-code-of-a-spin-set-viewer}

Usar o recurso Incorporar código permite revisar o código do visualizador do conjunto de rotação selecionado. Você também pode copiar o código para a área de transferência para poder colá-lo em suas páginas da Web para implantação do visualizador. A edição do código não é permitida na caixa de diálogo Incorporar código.

**Para copiar o código incorporado de um visualizador de conjunto de rotação:**

1. No painel Navegar por ativos, na lista suspensa Mostrar, selecione **[!UICONTROL Spin Set]**.
1. no painel Biblioteca de ativos à esquerda, navegue até a pasta de ativos que contém o conjunto de rotação cujo código de inserção você deseja copiar.
1. Acima do painel Navegar por ativos, no lado direito da barra de ferramentas, siga um destes procedimentos:

   * Selecionar **[!UICONTROL Grid View]**. No painel Navegação de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. No painel URLs e código incorporado à direita, selecione **[!UICONTROL Embed Code]** à direita do visualizador desejado.
   * Selecionar **[!UICONTROL Grid View]**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem em miniatura, acesse **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

   * Selecionar **[!UICONTROL List View]**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

   * Selecionar **[!UICONTROL Grid View]**, **[!UICONTROL List View]** ou **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

1. Na caixa de diálogo Incorporar código, selecione **[!UICONTROL Copy to Clipboard]**.

   A edição do código não é permitida na caixa de diálogo Incorporar código.

1. Selecionar **[!UICONTROL Close]**.
