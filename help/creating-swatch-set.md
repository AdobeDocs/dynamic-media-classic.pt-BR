---
title: Criação de um conjunto de amostras
description: Saiba como criar um conjunto de amostras.
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Visualizadores
role: Business Practitioner
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Criando um Conjunto de Amostras{#creating-a-swatch-set}

Um Conjunto de amostras oferece aos usuários a oportunidade de visualizar um item em uma cor, padrão ou conclusão diferente. Para criar um Conjunto de amostras com amostras de cores, você precisa de uma imagem para cada cor, padrão ou acabamento diferente que deseja apresentar aos usuários. Você também precisa de uma cor, padrão ou amostra de finalização para cada cor, padrão ou finalização.

Por exemplo, suponha que você deseja apresentar imagens de maiúsculas com diferentes notas coloridas; as notas são vermelhas, verdes e azuis. Neste caso, você precisa de três tiros do mesmo boné. Você precisa de um tiro com um vermelho, um com um verde e um com uma nota azul. Você também precisa de uma amostra de cor vermelha, verde e azul. As amostras de cores servem como miniaturas que os usuários clicam no Visualizador de Conjunto de Amostras para ver a tampa vermelha, verde ou azul.

## Criação de um conjunto de amostras {#create}

Ao criar um conjunto, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:
|**[!UICONTROL Publish after save]** opção selecionada antes de salvar?|Estado do conjunto após salvar|Estado do conjunto de membros após salvar|
|— |— |— |
|Sim|Publicado|Publicado|
|Não|Não publicado|Definir membros mantêm o estado publicado ou não publicado.|

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um Conjunto de amostras:**

1. Siga um destes procedimentos:

   * **Selecione as imagens primeiro**  - No painel Procurar, selecione as imagens e clique em  **[!UICONTROL Build]** >  **[!UICONTROL Swatch Sets]**.

   * **Comece na tela**  Conjunto de amostras - Clique em  **[!UICONTROL Build]** >  **[!UICONTROL Swatch Sets]**. Selecione uma pasta na Biblioteca de ativos e arraste as imagens até a seção Exibições da página Conjunto de amostras.

1. Arraste cores, padrões ou finalizações da amostra para a caixa de espaço reservado Amostras na página Conjunto de amostras.

   Certifique-se de que a cor, o padrão ou a amostra de conclusão que você arrastar para cada espaço reservado representa a cor, o padrão ou o término da imagem adjacente.

1. Para alterar a ordem das imagens no Conjunto de amostras, arraste as imagens para novos locais.
1. Próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionado (padrão).
1. Clique em **[!UICONTROL Save]**, selecione uma pasta para armazenar o Conjunto de Amostras de cores, insira um nome para o conjunto e clique em **[!UICONTROL Submit]**.
1. Para ver seu Conjunto de amostras no Visualizador de conjunto de amostras, clique em **[!UICONTROL Preview]** na tela Conjunto de amostras. Você pode clicar em miniaturas de amostra no Visualizador do conjunto de amostras para ver como elas se comportam.

## Editar um conjunto de amostras {#editing-a-swatch-set}

Independentemente de você editar um conjunto publicado ou não, a opção **[!UICONTROL Publish after save]** afeta o conjunto e define os membros das seguintes maneiras:

| Definir já publicado? | **[!UICONTROL Publish after]** salvar opção selecionada antes de salvar a edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado. Qualquer novo conjunto de membros adicionado durante a edição manterá o estado publicado ou não. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto adicionados durante a edição mantêm o estado publicado ou não. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um conjunto de amostras:**

1. Na exibição de Grade, navegue até um SwatchSet e, em seguida, abaixo da imagem, clique em **[!UICONTROL Edit]**.
1. Siga um destes procedimentos:

   * Para adicionar uma imagem (publicada ou não publicada), arraste-a de uma pasta em Adicionar ativos para a página do Conjunto de amostras **[!UICONTROL Views]**.
   * Para remover uma imagem, selecione-a e clique em **[!UICONTROL Delete]** na barra de ferramentas.
   * Para reorganizar imagens, arraste uma imagem para uma nova posição.

1. Quando terminar de editar o conjunto, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionado (padrão).
1. Clique em **[!UICONTROL Save]**, selecione uma pasta de armazenamento, insira um nome para o conjunto e clique em **[!UICONTROL Save]**.

## Excluindo um Conjunto de Amostras {#deleting-a-swatch-set}

Ao excluir um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) desse conjunto não são afetados; em vez disso, cada um mantém seu estado publicado ou não publicado.

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um conjunto de amostras:**

1. Na Exibição de Grade, Exibição de Lista ou Exibição de Detalhes, selecione um ou mais Conjuntos de Amostras.
1. Na Barra de Navegação Global, clique em **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
