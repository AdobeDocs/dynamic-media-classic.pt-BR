---
title: Criar um conjunto de amostras
description: Saiba como criar um conjunto de amostras no Adobe Dynamic Media Classic.
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Criar um conjunto de amostras{#creating-a-swatch-set}

Um Conjunto de amostras oferece aos usuários a oportunidade de visualizar um item em uma cor, padrão ou fim diferente. Para criar um Conjunto de amostras com amostras de cores, é necessário ter uma imagem para cada cor, padrão ou término diferente que você deseja apresentar aos usuários. Você também precisa de uma amostra de cor, padrão ou fim para cada cor, padrão ou fim.

Por exemplo, suponha que você queira apresentar imagens de tampas com diferentes listas de cores; as listas são vermelha, verde e azul. Neste caso, você precisa de três doses do mesmo boné. Você precisa de uma foto com um vermelho, uma com verde e outra com uma nota azul. Você também precisa de uma amostra de cor vermelha, verde e azul. As amostras de cores servem como miniaturas que os usuários selecionam no Visualizador de conjuntos de amostras para ver a tampa de faturamento vermelho, verde ou azul.

## Criar um conjunto de amostras {#create}

Ao criar um conjunto, a variável **Publicar após salvar** opção afeta os membros set e set das seguintes maneiras:

| **[!UICONTROL Publish after save]** opção selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- |
| Sim | Publicado | publicado |
| Não | Não publicado | Os membros definidos mantêm seu estado publicado ou não publicado. |

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um Conjunto de amostras:**

1. Siga um destes procedimentos:

   * **Selecione as imagens primeiro** - No Painel Procurar, selecione as imagens e vá para **[!UICONTROL Build]** > **[!UICONTROL Swatch Sets]**.

   * **Iniciar na tela Conjunto de amostras** - Vá para **[!UICONTROL Build]** > **[!UICONTROL Swatch Sets]**. Selecione uma pasta na Biblioteca de ativos e arraste as imagens para a seção Exibições da página Conjunto de amostras.

1. Arraste as cores, os padrões ou os acabamentos da amostra para a caixa de espaço reservado Amostras na página Conjunto de amostras.

   Verifique se a amostra de cor, padrão ou fim arrastada para cada espaço reservado representa a cor, o padrão ou o fim da imagem adjacente.

1. Para alterar a ordem das imagens no Conjunto de amostras, arraste as imagens para novos locais.
1. Próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]**, selecione uma pasta para armazenar o Conjunto de amostras de cores, digite um nome para o conjunto e selecione **[!UICONTROL Submit]**.
1. Para ver o conjunto de amostras no Visualizador de conjuntos de amostras, selecione **[!UICONTROL Preview]** na tela Conjunto de amostras. Você pode selecionar miniaturas de amostras no Visualizador de conjuntos de amostras para ver como elas se comportam.

## Editar um conjunto de amostras {#editing-a-swatch-set}

Se você editar um conjunto publicado ou não, a variável **[!UICONTROL Publish after save]** opção afeta os membros set e set das seguintes maneiras:

| Conjunto já publicado? | **[!UICONTROL Publish after]** opção salvar selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existentes mantêm seu estado publicado. Qualquer novo membro do conjunto adicionado durante sua edição manterá seu estado publicado ou não. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existentes e os novos membros do conjunto adicionados durante a edição mantêm seus estados publicado ou não. |

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um Conjunto de amostras:**

1. Na Exibição de grade, navegue até um SwatchSet e, abaixo da imagem, selecione **[!UICONTROL Edit]**.
1. Siga um destes procedimentos:

   * Para adicionar uma imagem (publicada ou não), arraste-a de uma pasta em Adicionar ativos para o do Conjunto de amostras **[!UICONTROL Views]** página.
   * Para remover uma imagem, selecione-a e **[!UICONTROL Delete]** na barra de ferramentas.
   * Para reordenar imagens, arraste uma imagem para uma nova posição.

1. Quando terminar de editar o conjunto, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]**, selecione uma pasta de armazenamento, digite um nome para o conjunto e selecione **[!UICONTROL Save]**.

## Excluir um conjunto de amostras {#deleting-a-swatch-set}

Quando você exclui um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um conjunto de amostras:**

1. Na Exibição em Grade, em Lista ou em Detalhes, selecione um Conjunto de Amostras ou mais.
1. Na Barra de navegação global, acesse **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
