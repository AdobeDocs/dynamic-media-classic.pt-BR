---
title: Vincular um conjunto de rotação a uma página da Web
seo-title: Vincular um conjunto de rotação a uma página da Web
description: nulo
seo-description: Saiba como vincular um Conjunto de rotação a uma página da Web.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 2%

---


# Vincular um conjunto de rotação a uma página da Web{#linking-a-spin-set-to-a-web-page}

Os sites e aplicativos da Web acessam o conteúdo do Dynamic Media Image Server, incluindo Conjuntos de rotação, por meio de sequências de caracteres de URL ou código incorporado. Essas sequências de caracteres de URL são ativadas durante o processo de publicação. Para colocar a string de URL ou o código incorporado para seu Conjunto de rotação em suas páginas da Web e aplicativos, copie-o do Dynamic Media Classic.

>[!NOTE]
>
>O URL não estará ativo até que você publique o ativo.

## Copiando um URL de conjunto de rotação {#copying-a-spin-set-url}

1. No painel Navegação de ativos, na lista suspensa Mostrar, clique em **Conjunto de rotação**.
1. no painel Biblioteca de ativos, à esquerda, navegue até a pasta de ativos que contém o Conjunto de rotação cujo código incorporado você deseja copiar.
1. Acima do painel Navegação de ativos, no lado direito da barra de ferramentas, execute um dos procedimentos a seguir:

   * Clique em **Visualização de grade**. No painel Navegação de ativos, clique com o duplo em um único ativo para abri-lo na Visualização Detalhe. No painel URLs e Código incorporado à direita, clique em **Copiar URL** à direita do visualizador desejado.
   * Clique em **Visualização de grade**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem em miniatura, clique em **Pré-visualização** > **Lista do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique em **Copiar URL**.

   * Clique em **Visualização de Lista**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, clique em **Pré-visualização** > **Lista do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique em **Copiar URL**.

   * Clique em **Visualização de grade**, **Visualização de Lista** ou **Visualização de detalhes**. Na mesma barra de ferramentas, clique em **Pré-visualização** > **Lista do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique em **Copiar URL**.

## Adicionar URLs de conjunto de rotação à sua página da Web {#adding-spin-set-urls-to-your-web-page}

Os Conjuntos de rotação são implantados como todos os visualizadores de zoom, por meio de uma página dinâmica (ASP ou JSP) que exibe o Conjunto de rotação em uma janela de zoom. A chamada de URL para a plataforma Dynamic Media Classic segue o mesmo protocolo no visualizador de zoom. Entretanto, o nome da predefinição do visualizador depende da predefinição definida definida pelo administrador como a predefinição padrão do visualizador de conjuntos de rotação. Por exemplo, o seguinte exemplo de sintaxe de URL não ativa inclui um nome predefinido chamado `viewer.jsp` e o parâmetro SKU agora é o nome do Conjunto de rotação:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

Neste exemplo de sintaxe de URL (o link não está ativo), observe um número SKU ( `sku=backpack_spin`). A string depois de `sku=` é o nome do Conjunto de rotação ( `backpack spin`).

## Copiando o código incorporado de um visualizador do Spin Set {#copying-the-embed-code-of-a-spin-set-viewer}

Usar o recurso Incorporar código permite que você revise o código do visualizador para o conjunto de rotação selecionado. Você também pode copiar o código para a área de transferência para colá-lo em suas páginas da Web para a implantação do visualizador. A edição do código não é permitida na caixa de diálogo Incorporar código.

**Para copiar o código incorporado de um visualizador de Conjunto de rotação**

1. No painel Navegação de ativos, na lista suspensa Mostrar, clique em **Conjunto de rotação**.
1. no painel Biblioteca de ativos, à esquerda, navegue até a pasta de ativos que contém o Conjunto de rotação cujo código incorporado você deseja copiar.
1. Acima do painel Navegação de ativos, no lado direito da barra de ferramentas, execute um dos procedimentos a seguir:

   * Clique em **Visualização de grade**. No painel Navegação de ativos, clique com o duplo em um único ativo para abri-lo na Visualização Detalhe. No painel URLs e Código incorporado à direita, clique em **Código incorporado** à direita do visualizador desejado.
   * Clique em **Visualização de grade**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem em miniatura, clique em **Pré-visualização** > **Lista do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique em **Código incorporado**.

   * Clique em **Visualização de Lista**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, clique em **Pré-visualização** > **Lista do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique em **Código incorporado**.

   * Clique em **Visualização de grade**, **Visualização de Lista** ou **Visualização de detalhes**. Na mesma barra de ferramentas, clique em **Pré-visualização** > **Lista do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique em **Código incorporado**.

1. Na caixa de diálogo Incorporar código, clique em **Copiar para a área de transferência**.

   A edição do código não é permitida na caixa de diálogo Incorporar código.

1. Clique em Fechar.

