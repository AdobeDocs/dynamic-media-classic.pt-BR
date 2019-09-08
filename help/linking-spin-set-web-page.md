---
title: Vincular um conjunto de rotação a uma página da Web
seo-title: Vincular um conjunto de rotação a uma página da Web
description: 'null'
seo-description: Saiba como vincular um Spin Set a uma página da Web.
uuid: d 3 c 5773 e -60 c 4-4 e 8 b -9 c 48-e 1 e 3 eb 8028 d 0
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/spin_ sets
discoiquuid: 651 b 21 ef-e 322-4 e 6 d -8 e 37-45 ffd 56 f 7 a 58
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Vincular um conjunto de rotação a uma página da Web{#linking-a-spin-set-to-a-web-page}

Os sites e aplicativos acessam o conteúdo do Servidor de imagem do Dynamic Media, incluindo Conjuntos de rotação, por meio de sequências de caracteres de URL ou código incorporado. Essas strings de URL são ativadas durante o processo de publicação. Para colocar a sequência de URL ou o código incorporado para seu Conjunto de rotação em suas páginas e aplicativos da Web, copie-o do Sistema de publicação Scene 7.

>[!NOTE]
>
>O URL não estará ativo até que você publique o ativo.

## Copiando um URL de conjunto de rotação {#copying-a-spin-set-url}

1. No painel Procurar ativo, na lista suspensa Mostrar, clique em Conjunto **de rotação**.
1. no painel Biblioteca de ativos no lado esquerdo, navegue até a pasta de ativos que contém o Conjunto de rotação cujo código incorporado você deseja copiar.
1. Acima do painel Navegador de ativos, no lado direito da barra de ferramentas, execute um dos seguintes procedimentos:

   * Clique **em Exibição de grade**. No painel Navegador de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. Nos urls e no painel Incorporar código à direita, clique **em Copiar URL** à direita do visualizador desejado.
   * Clique **em Exibição de grade**. No painel Procurar ativo, selecione um único ativo e depois abaixo da imagem em miniatura, clique **em Visualizar** &gt; Lista **do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique **em Copiar URL**.

   * Clique **em Exibição de lista**. No painel Procurar ativo, selecione um único ativo e, à direita da imagem em miniatura, clique **em Visualizar** &gt; Lista **do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique **em Copiar URL**.

   * Clique **em Exibição de grade**, **Exibição de lista** ou Exibição **de detalhes**. Na mesma barra de ferramentas, clique **em Visualizar** &gt; Lista **de visualizadores**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique **em Copiar URL**.

## Adicionar urls de conjunto de rotação à sua página da Web {#adding-spin-set-urls-to-your-web-page}

Os Conjuntos de rotação são implantados como todos os visualizadores de zoom por meio de uma página dinâmica (ASP ou JSP) que exibe o Spin Set em uma janela de zoom. A chamada de URL para a plataforma do Dynamic Media Classic segue o mesmo protocolo no visualizador de zoom. No entanto, o nome Predefinido do visualizador depende da predefinição definida como a Predefinição padrão do Visualizador de rotação. Por exemplo, o exemplo de sintaxe de URL a seguir inclui um nome Predefinido chamado `viewer.jsp` e o parâmetro SKU agora é o nome do Conjunto de rotação:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

Neste exemplo de sintaxe de URL (o link não está ao vivo), observe um número de SKU ( `sku=backpack_spin`). A string depois `sku=` é o nome do Conjunto de rotação ( `backpack spin`).

## Copiando o código incorporado de um visualizador de Conjunto de rotação {#copying-the-embed-code-of-a-spin-set-viewer}

Usar o recurso Incorporar código permite analisar o código do visualizador para o Conjunto de rotação selecionado. Também é possível copiar o código para a área de transferência para que você possa colá-lo em suas páginas da Web para implantação do visualizador. A edição do código não é permitida na caixa de diálogo Incorporar código.

**Para copiar o código incorporado de um visualizador de Conjunto de rotação**

1. No painel Procurar ativo, na lista suspensa Mostrar, clique em Conjunto **de rotação**.
1. no painel Biblioteca de ativos no lado esquerdo, navegue até a pasta de ativos que contém o Conjunto de rotação cujo código incorporado você deseja copiar.
1. Acima do painel Navegador de ativos, no lado direito da barra de ferramentas, execute um dos seguintes procedimentos:

   * Clique **em Exibição de grade**. No painel Navegador de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. Nos urls e no painel Incorporar código à direita, clique em **Incorporar código** à direita do visualizador desejado.
   * Clique **em Exibição de grade**. No painel Procurar ativo, selecione um único ativo e depois abaixo da imagem em miniatura, clique **em Visualizar** &gt; Lista **do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique **em Incorporar código**.

   * Clique **em Exibição de lista**. No painel Procurar ativo, selecione um único ativo e, à direita da imagem em miniatura, clique **em Visualizar** &gt; Lista **do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique **em Incorporar código**.

   * Clique **em Exibição de grade**, **Exibição de lista** ou Exibição **de detalhes**. Na mesma barra de ferramentas, clique **em Visualizar** &gt; Lista **de visualizadores**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique **em Incorporar código**.

1. Na caixa de diálogo Incorporar código, clique **em Copiar para a área de transferência**.

   A edição do código não é permitida na caixa de diálogo Incorporar código.

1. Clique em Fechar.

