---
title: Criar mapas de imagem de eCatalog
description: Saiba como criar mapas de imagem de eCatalog no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
topic: Integrations, Development
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '1449'
ht-degree: 0%

---

# Criar mapas de imagem de eCatalog{#creating-ecatalog-image-maps}

Um Mapa de imagem é uma região em uma página de eCatalog que você pode rolar com o mouse ou selecionar para acionar ações de vários tipos. Ao mover o ponteiro sobre um Mapa de imagem, por exemplo, você verá uma descrição de texto de sobreposição de um item. Quando você seleciona um Mapa de imagem, outra ação é iniciada. Por exemplo, você pode abrir uma página da Web para que os visualizadores possam saber mais sobre um item ou comprá-lo, ou iniciar um vídeo para ver um item em uso.

## Desenhar mapas de imagem do eCatalog {#drawing-ecatalog-image-maps}

Para eCatalogs, você desenha Mapas de imagem na guia Páginas de mapa da tela eCatalog. Essa tela consiste na área do Mapa de imagem onde as páginas do eCatalog são exibidas e, à direita, na lista Mapa de imagem. À medida que você cria Mapas de imagem, seus nomes são inseridos na Lista de Mapas de imagem.

1. Selecione a sobreposição do eCatalog **[!UICONTROL Edit]** botão.
1. Selecionar **[!UICONTROL Map Pages]**.
1. À esquerda da tela Mapear páginas, selecione a página desejada.
1. Na área do Mapa de imagem, desenhe um Mapa de imagem retangular ou poligonal (em vários lados):

   * **Mapa retangular** - Selecione a ferramenta Mapa de imagem de retângulo e arraste na página para criar o retângulo.

   * **Mapa poligonal** - Selecione a ferramenta Mapa de imagem de polígono e, em seguida, selecione quantas vezes forem necessárias em torno do perímetro da imagem. À medida que você seleciona, o Adobe Dynamic Media Classic desenha as bordas do Mapa de imagem.

     Depois de desenhar um Mapa de imagem, o Adobe Dynamic Media Classic atribui a ele um nome na lista Mapa de imagem. Para formar o nome, o Adobe Dynamic Media Classic anexa um número sequencial ao nome da página do eCatalog na qual você está trabalhando.

1. (Opcional) Na lista Mapa de imagem, na guia [!UICONTROL Name] é possível inserir um novo nome para o Mapa de imagem. Não inclua espaços em branco no nome digitado.
1. Os visualizadores podem abrir uma nova página da Web ao selecionar o Mapa de imagem. No painel Image Map list, digite o URL da página da Web na coluna URL.

   Para facilitar a inserção de URLs (modelos Href), selecione **[!UICONTROL Edit]** e insira um template.

Consulte [Use um modelo para inserir JavaScript e URLs](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Opcional) Na lista suspensa Mostrar, selecione **[!UICONTROL Rollover Text]** e, em seguida, insira o texto que você deseja que os usuários vejam na tela quando moverem seus ponteiros sobre o Mapa de imagem.
1. (Opcional) Na lista suspensa Mostrar, selecione **[!UICONTROL Other Actions]** e insira um atributo para acionar uma ação de desfoque ou foco quando os usuários moverem seus ponteiros sobre um Mapa de imagem.

   Consulte [Definir outras ações para Mapas de imagem](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Selecionar **[!UICONTROL Save]**.
1. (Opcional) Selecione **[!UICONTROL Preview]** para exibir o eCatalog com a predefinição padrão do eCatalog Viewer.

Para excluir um Mapa de imagem, selecione seu nome na lista Mapa de imagem e selecione **[!UICONTROL Delete]**. Para desativar temporariamente um Mapa de imagem em uma página sem excluir o Mapa de imagem, desmarque a opção Ativado do Mapa de imagem no painel Lista do Mapa de imagem.

## Incorporar mídia avançada em um eCatalog {#embedding-rich-media-in-an-ecatalog}

Você pode usar a opção de mídia avançada do eCatalog para adicionar vídeos em formato MP4 ou conjuntos de rotação a Mapas de imagem adicionados a um eCatalog. Quando um usuário seleciona a área Mapa de imagem no eCatalog, o conjunto de rotação ou vídeo associado é exibido. Essa funcionalidade é especialmente útil se você quiser que os clientes vejam um item em uso ou vejam um item de diferentes ângulos e perspectivas.

Opcionalmente, também é possível exibir o texto da dica de ferramenta quando os clientes movem os ponteiros sobre o Mapa de imagem para que eles saibam o que estão selecionando.

**Para incorporar mídia avançada em um eCatalog:**

1. Desenhe um Mapa de imagem de eCatalog.

   Consulte [Desenhar mapas de imagem do eCatalog](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Na lista suspensa Mostrar, selecione **[!UICONTROL Rich Media]**.
1. No painel Adicionar ativos à esquerda, navegue até uma pasta que contenha o conjunto de rotação ou ativo de vídeo (formato MP4) que deseja incorporar.
1. Arraste o ativo para o Mapa de imagem.
1. (Opcional) No painel Lista de mapas de imagem, na guia **[!UICONTROL Tool Tip]** cabeçalho de coluna, digite o texto que você deseja que os visualizadores vejam na tela quando movem o ponteiro sobre o Mapa de imagem.
1. Selecionar **[!UICONTROL Save]**.

## Edição de Mapas de Imagem de eCatalog {#editing-ecatalog-image-maps}

Começando pela guia Mapear páginas da tela do eCatalog, use essas técnicas para editar os mapas de imagem do eCatalog:

* **Ajustar a posição** - Selecione a ferramenta Deslocar e mova o ponteiro próximo, mas não acima, da borda do mapa. Quando o ponteiro mostrar uma seta de quatro pontas, arraste o mapa de imagem inteiro para um novo local.

  Consulte [Ajustar a posição, a forma e o tamanho dos Mapas de imagem](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Alterar forma e tamanho** - Para redimensionar um Mapa de Imagem retangular, selecione a ferramenta Deslocar. Em seguida, mova o ponteiro sobre uma linha de borda ou um canto e, ao visualizar o ícone de seta de duas pontas, arraste. Para redimensionar um Mapa de Imagem poligonal, arraste uma alça de seleção quadrada. Para criar uma alça de seleção, selecione a borda do Mapa de imagem e arraste.

  Consulte [Ajustar a posição, a forma e o tamanho dos Mapas de imagem](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Exclusão de Mapas de Imagem** - Selecione a ferramenta Panorâmica, selecione o Mapa de imagem para selecioná-lo e, em seguida, selecione **[!UICONTROL Delete]**.

  Para remover todos os Mapas de imagens de um eCatalog, selecione o **[!UICONTROL Order Pages]** e selecione **[!UICONTROL Clear Maps]**.

* **Lidar com mapas de imagem sobrepostos** - Arraste para alterar a ordem dos Mapas de imagem na lista Mapa de imagem.

  Consulte [Manipular mapas de imagem sobrepostos](creating-image-maps.md#handling_overlapping_image_maps).

* **Como copiar mapas de imagem para outras páginas** - Selecionar **[!UICONTROL Copy Maps To]** (verifique se você está na guia Mapear páginas ). Na tela Selecionar imagens, selecione as páginas nas quais deseja copiar os Mapas de imagens e selecione **[!UICONTROL Select]**.

  Consulte [Copiar Mapas de Imagens para outras imagens](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Além de copiar Mapas de imagens para páginas diferentes em um eCatalog, você pode copiar todos os Mapas de imagens em um eCatalog para um eCatalog diferente. Consulte [Copiar Mapas de Imagem entre eCatalogs](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Revisar e importar dados do Mapa de imagem {#reviewing-and-importing-image-map-data}

A tela Resumo do mapa fornece metadados sobre seu eCatalog. Você também pode importar dados de Mapa de imagem em lote para o seu eCatalog, iniciando na tela Resumo de mapa. A importação de dados do Mapa de imagem dessa maneira facilita a inserção de URLs do Mapa de imagem e a sobreposição de texto.

Para ver a tela Resumo do mapa, na guia Páginas do mapa da tela eCatalog, selecione **[!UICONTROL Summary]**.

### Revisar resumo de dados do Mapa de imagem {#review-image-map-data-summary}

1. Na tela Mapear Páginas, selecione **[!UICONTROL Summary]**.

   A tela Resumo do mapa exibe quantos Mapas de imagem, URLs, descrições de texto de rolagem e outras ações estão no eCatalog.

1. Se houver erros de chave de rollover, selecione o erro no campo **[!UICONTROL Rollover_Key Error]** para ver o que deve ser alterado na planilha para corrigir o erro. Você pode selecionar e copiar o texto desta mensagem e colá-lo em sua planilha.
1. Selecionar **[!UICONTROL Preview]** para que você possa examinar uma página no eCatalog Viewer; selecione o X para fechar a tela Summary e retornar à tela Map Pages (Mapear páginas) ou selecione **[!UICONTROL Close]** para retornar a Procurar.

### Importar dados do Mapa de imagem {#import-image-map-data}

Em vez de inserir dados do Mapa de imagem em cada página, você pode importar os dados do eCatalog inteiro para a tela Resumo de mapa. Importe os dados do Mapa de imagem no formato de um arquivo delimitado por tabulação ou DTD XML. Os campos no arquivo devem estar na ordem mostrada na tela Resumo do Mapa: Nome, Rótulos do índice, Mapas, URLs, Texto de rolagem, Outras ações e Strings de pesquisa. A importação de dados do Mapa de imagem evita a dificuldade de inserir os dados na Lista de Mapas de imagem à medida que você cria cada Mapa de imagem.

>[!NOTE]
>
>Antes de importar os dados do Mapa de imagem, é necessário que você já tenha criado os Mapas de imagem.

A partir da tela Resumo do mapa, siga estas etapas para importar dados do Mapa de imagem para os Mapas de imagem que você criou:

1. Selecionar **[!UICONTROL Import Map Data]**.
1. Na caixa de diálogo Importar metadados, selecione **[!UICONTROL Browse]** e selecione o arquivo DTD XML ou delimitado por tabulação.
1. No campo Nome da tarefa, digite um nome para o arquivo (tenha cuidado para manter a extensão).
1. Selecionar **[!UICONTROL Upload]**.

## Copiar Mapas de Imagem entre eCatalogs {#copying-image-maps-between-ecatalogs}

É possível copiar todos os Mapas de imagens em um eCatalog para um eCatalog diferente. Copiar mapas de imagem dessa maneira é um método conveniente de copiar mapas de imagem entre traduções em idiomas estrangeiros do mesmo eCatalog. Para que a cópia seja bem-sucedida, a Adobe Dynamic Media Classic recomenda copiar entre eCatalogs com o mesmo número de páginas e as mesmas imagens.

>[!NOTE]
>
>Se o eCatalog para o qual você copiar Mapas de imagem já contiver Mapas de imagem, esses Mapas de imagem serão excluídos quando a cópia for feita.

Para copiar todos os Mapas de imagens de um eCatalog para outro eCatalog, faça o seguinte:

1. Selecione o eCatalog com os Mapas de imagem que deseja copiar e selecione a sobreposição do eCatalog **[!UICONTROL Edit]** botão.
1. Na guia Ordenar páginas, selecione **[!UICONTROL Copy Maps]**.
1. Na caixa de diálogo Selecionar ativo, selecione o eCatalog no qual deseja copiar os Mapas de imagem e selecione **[!UICONTROL Select]**.

O Adobe Dynamic Media Classic exibirá uma mensagem de aviso se o eCatalog de destino (o eCatalog para o qual você copia Mapas de imagem) tiver um número diferente de páginas ou imagens de tamanho diferente. Selecionar **[!UICONTROL Continue]** para copiar os Mapas de imagem apesar do aviso.
