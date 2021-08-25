---
title: Criar mapas de imagem do catálogo eletrônico
description: Saiba como criar mapas de imagem do catálogo eletrônico no Dynamic Media Classic.
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
feature: Dynamic Media Classic,Visualizadores,Catálogo eletrônico
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
source-git-commit: 7be3f63bfadeafa71eeb2567f982f579ccb85975
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 0%

---

# Criar mapas de imagem do catálogo eletrônico{#creating-ecatalog-image-maps}

Um Mapa de imagem é uma região em uma página de Catálogo eletrônico que você pode passar com o mouse ou selecionar para acionar ações de vários tipos. Ao mover o ponteiro sobre um Mapa de imagem, por exemplo, você vê uma descrição de texto sobreposto de um item. Ao selecionar um Mapa de imagem, outra ação é iniciada. Por exemplo, você pode abrir uma página da Web para que os visualizadores possam saber mais sobre um item ou comprá-lo, ou iniciar um vídeo para ver um item em uso.

## Desenhar mapas de imagem do catálogo eletrônico {#drawing-ecatalog-image-maps}

Para eCatalogs, você desenha mapas de imagem na guia Mapear páginas da tela eCatalog. Esta tela consiste na área Mapa de imagem onde as páginas de Catálogo eletrônico são exibidas e, à direita, na lista Mapa de imagem. À medida que você cria mapas de imagem, seus nomes são inseridos na Lista de mapas de imagem.

1. Selecione o botão **[!UICONTROL Edit]** de sobreposição do Catálogo eletrônico.
1. Selecione **[!UICONTROL Map Pages]**.
1. À esquerda da tela Mapear páginas, selecione a página desejada.
1. Na área do Mapa de imagem, desenhe um Mapa de imagem retangular ou polígono (de vários lados):

   * **Mapa retangular**  - Selecione a ferramenta Mapa de imagem do retângulo e arraste na página para criar o retângulo.

   * **Mapa poligonal**  - Selecione a ferramenta Mapa de imagem de polígono e selecione quantas vezes forem necessárias ao redor do perímetro da imagem. À medida que você seleciona, o Dynamic Media Classic desenha as bordas do Mapa de imagem.

      Depois de desenhar um Mapa de imagem, o Dynamic Media Classic atribui a ele um nome na lista Mapa de imagem. Para formar o nome, o Dynamic Media Classic anexa um número sequencial ao nome da página eCatalog na qual você está trabalhando.

1. (Opcional) Na lista Mapa de imagem, na coluna [!UICONTROL Name], você pode inserir um novo nome para o Mapa de imagem. Não inclua espaços em branco no nome inserido.
1. Você pode fazer com que os visualizadores abram uma nova página da Web ao selecionar o Mapa de imagem. No painel de lista Mapa de imagem, insira o URL da página da Web na coluna URL.

   Para facilitar a inserção de URLs (modelos Href), selecione **[!UICONTROL Edit]** e insira um modelo.

Consulte [Use um modelo para inserir JavaScript e URLs](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Opcional) Na lista suspensa Exibir , selecione **[!UICONTROL Rollover Text]** e insira o texto que deseja que os usuários vejam na tela quando moverem seus ponteiros sobre o Mapa de imagem.
1. (Opcional) Na lista suspensa Exibir , selecione **[!UICONTROL Other Actions]** e insira um atributo para acionar uma ação de desfoque ou foco quando os usuários moverem seus ponteiros sobre um Mapa de imagem.

   Consulte [Definir outras ações para Mapas de imagem](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Selecione **[!UICONTROL Save]**.
1. (Opcional) Selecione **[!UICONTROL Preview]** para exibir o eCatalog com a predefinição padrão do Visualizador do eCatalog.

Para excluir um Mapa de imagem, selecione seu nome na lista Mapa de imagem e selecione **[!UICONTROL Delete]**. Para desativar temporariamente um Mapa de imagem em uma página sem excluir o Mapa de imagem, desmarque a opção Ativado do Mapa de imagem no painel Lista de mapa de imagem .

## Incorporar mídia avançada a um eCatalog {#embedding-rich-media-in-an-ecatalog}

Você pode usar a opção Mídia avançada do Catálogo eletrônico para adicionar vídeos no formato MP4 ou conjuntos de rotação aos Mapas de imagem que você adicionou a um Catálogo eletrônico. Quando um usuário seleciona a área Mapa de imagem no eCatalog, o conjunto de rotação ou vídeo associado é exibido. Essa funcionalidade é especialmente útil se você quiser que os clientes vejam um item em uso ou vejam um item de diferentes ângulos e perspectivas.

Opcionalmente, também é possível exibir o texto da dica de ferramenta quando os clientes movem os ponteiros sobre o Mapa de imagem para que saibam o que estão selecionando.

**Para incorporar mídia avançada em um eCatalog:**

1. Desenhar um mapa de imagem do catálogo eletrônico.

   Consulte [Desenhar mapas de imagem do catálogo eletrônico](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Na lista suspensa Exibir , selecione **[!UICONTROL Rich Media]**.
1. No painel Adicionar ativos à esquerda, navegue até uma pasta que contém o conjunto de rotação ou o ativo de vídeo (formato MP4) que você deseja incorporar.
1. Arraste o ativo para o Mapa de imagem.
1. (Opcional) No painel da lista Mapa de imagem, no cabeçalho da coluna **[!UICONTROL Tool Tip]**, digite o texto que deseja que os visualizadores vejam na tela ao mover o ponteiro sobre o Mapa de imagem.
1. Selecione **[!UICONTROL Save]**.

## Edição de mapas de imagem do catálogo eletrônico {#editing-ecatalog-image-maps}

A partir da guia Mapear páginas da tela Catálogo eletrônico, use estas técnicas para editar os Mapas de imagem do catálogo eletrônico:

* **Ajustar a posição**  - Selecione a ferramenta Deslocar e mova o ponteiro para perto, mas não sobre a borda do mapa. Quando o ponteiro mostrar uma seta de quatro pontas, arraste o mapa de imagem inteiro até um novo local.

   Consulte [Ajuste a posição, a forma e o tamanho dos mapas de imagem](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Alterar a forma e o tamanho**  - Para redimensionar um Mapa de imagem retangular, selecione a ferramenta Deslocar. Em seguida, mova o ponteiro sobre uma linha de borda ou um canto e, ao visualizar o ícone de seta de duas pontas, arraste. Para redimensionar um Mapa de imagem polígono, arraste uma alça de seleção quadrada. Para criar uma alça de seleção, selecione a borda do Mapa de imagem e arraste.

   Consulte [Ajuste a posição, a forma e o tamanho dos mapas de imagem](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Exclusão de mapas de imagem**  - Selecione a ferramenta Deslocar, selecione o Mapa de imagem para selecioná-lo e selecione  **[!UICONTROL Delete]**.

   Para remover todos os mapas de imagem de um eCatalog, selecione a guia **[!UICONTROL Order Pages]** e selecione **[!UICONTROL Clear Maps]**.

* **Manuseio de mapas de imagem sobrepostos**  - Arraste para alterar a ordem dos mapas de imagem na lista do mapa de imagem.

   Consulte [Manipular mapas de imagem sobrepostos](creating-image-maps.md#handling_overlapping_image_maps).

* **Copiando mapas de imagem para outras páginas**  - Selecione  **[!UICONTROL Copy Maps To]** (verifique se você está na guia Mapear páginas). Na tela Selecionar imagens , selecione a página ou páginas em que deseja copiar os Mapas de imagem e selecione **[!UICONTROL Select]**.

   Consulte [Copiar mapas de imagem para outras imagens](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Além de copiar mapas de imagem para páginas diferentes em um eCatalog, você pode copiar todos os mapas de imagem em um eCatalog para um eCatalog diferente. Consulte [Copiar mapas de imagem entre eCatalogs](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Revisar e importar dados do Mapa de imagem {#reviewing-and-importing-image-map-data}

A tela Resumo do mapa fornece metadados sobre seu eCatalog. Também é possível importar em lote dados do Mapa de imagem para seu eCatalog, começando na tela Resumo do mapa. A importação de dados do Mapa de imagem dessa forma facilita a inserção de URLs do Mapa de imagem e o texto de sobreposição.

Para ver a tela Mapear resumo , na guia Mapear páginas da tela Catálogo eletrônico, selecione **[!UICONTROL Summary]**.

### Revisar resumo de dados do Mapa de imagem {#review-image-map-data-summary}

1. Na tela Mapear páginas , selecione **[!UICONTROL Summary]**.

   A tela Resumo do mapa exibe quantos mapas de imagem, URLs, descrições de texto de sobreposição e outras ações estão em seu eCatalog.

1. Se houver erros de chave de substituição, selecione o erro na coluna **[!UICONTROL Rollover_Key Error]** para ver o que deve ser alterado na planilha e corrigir o erro. Você pode selecionar e copiar o texto desta mensagem e colá-lo em sua planilha.
1. Selecione **[!UICONTROL Preview]** para poder examinar uma página no Visualizador de Catálogo Eletrônico; selecione o X para fechar a tela Resumo e retornar à tela Mapear páginas ou selecione **[!UICONTROL Close]** para retornar a Navegar.

### Importar dados do mapa de imagem {#import-image-map-data}

Em vez de inserir dados do Mapa de imagem em cada página, você pode importar os dados de todo o seu eCatalog para a tela do Resumo do mapa. Você importa os dados do Mapa de imagem no formulário de um arquivo delimitado por tabulação ou XML DTD. Os campos no arquivo devem estar na ordem mostrada na tela Mapear resumo : Nome, Rótulos de sumário, Mapas, URLs, Texto de sobreposição, Outras ações e Strings de pesquisa. Importar dados do mapa de imagem salva o trabalho de inserir os dados na Lista de mapa de imagem à medida que você cria cada mapa de imagem.

>[!NOTE]
>
>Antes de importar os dados do Mapa de imagem, é necessário que você já tenha criado os Mapas de imagem.

A partir da tela Resumo do mapa, siga estas etapas para importar os dados do Mapa de imagem para os Mapas de imagem que você criou:

1. Selecione **[!UICONTROL Import Map Data]**.
1. Na caixa de diálogo Importar metadados, selecione **[!UICONTROL Browse]** e selecione o arquivo DTD delimitado por tabulação ou XML.
1. No campo Nome do trabalho , digite um nome para o arquivo (tenha cuidado para manter sua extensão).
1. Selecione **[!UICONTROL Upload]**.

## Copiar mapas de imagem entre catálogos eletrônicos {#copying-image-maps-between-ecatalogs}

Você pode copiar todos os mapas de imagem em um eCatalog para um eCatalog diferente. Copiar mapas de imagem dessa forma é um método conveniente de copiar mapas de imagem entre traduções de idioma estrangeiro do mesmo eCatalog. Para que a cópia seja bem-sucedida, o Dynamic Media Classic recomenda copiar entre eCatalogs com o mesmo número de páginas e as mesmas imagens.

>[!NOTE]
>
>Se o eCatalog para o qual você copia mapas de imagem já contiver mapas de imagem, esses mapas serão excluídos quando a cópia for feita.

Para copiar todos os mapas de imagem em um eCatalog para outro eCatalog, faça o seguinte:

1. Selecione o eCatalog com os mapas de imagem que deseja copiar e selecione o botão **[!UICONTROL Edit]** de sobreposição do eCatalog.
1. Na guia Páginas da ordem , selecione **[!UICONTROL Copy Maps]**.
1. Na caixa de diálogo Selecionar ativo, selecione o eCatalog onde deseja copiar os mapas de imagem e selecione **[!UICONTROL Select]**.

O Dynamic Media Classic exibe uma mensagem de aviso se o eCatalog de destino (o eCatalog para o qual você copia mapas de imagem) tiver um número diferente de páginas ou imagens que tenham um tamanho diferente. Selecione **[!UICONTROL Continue]** para copiar os Mapas de imagem apesar do aviso.
