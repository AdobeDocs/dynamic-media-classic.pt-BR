---
title: Criar um conjunto de amostras
description: Saiba como criar um Conjunto de amostras no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:44:21.987Z'
TQID: 'https://experienceleague.adobe.com/8nWsAO1rwDZnpj3GkUv7iUEqQR894oeoo81Vtr-uHcs'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 1343214cf19c9cfc6153e3f8b90c8ffc260de999
workflow-type: tm+mt
source-wordcount: 672
ht-degree: 0%

---

# Criar um conjunto de amostras{#creating-a-swatch-set}

Um Conjunto de amostras permite que os usuários visualizem um item em uma cor, padrão ou fim diferente. Para criar um Conjunto de amostras com amostras de cores, é necessário ter uma imagem para cada cor, padrão ou término diferente que você deseja apresentar aos usuários. Você também precisa de uma amostra de cor, padrão ou fim para cada cor, padrão ou fim.

Por exemplo, suponha que você queira apresentar imagens de tampas com diferentes listas de cores; as listas são vermelha, verde e azul. Neste caso, você precisa de três imagens do mesmo quepe. Você precisa de uma imagem para cada uma das notas vermelha, verde e azul. Você também precisa de amostras de cores vermelho, verde e azul. As amostras de cores servem como miniaturas que os usuários selecionam no Visualizador de conjuntos de amostras para ver a tampa de faturamento vermelho, verde ou azul.

## Criar um conjunto de amostras {#create}

Ao criar um conjunto, a opção **Publicar após salvar** afeta o conjunto e os membros do conjunto das seguintes maneiras:

| **[!UICONTROL Publish after a save]** opção selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- |
| Sim | Publicado | publicado |
| Não | Não publicado | Os membros definidos mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um Conjunto de Amostras:**

1. Siga um destes procedimentos:

   * **Selecione as imagens primeiro**: no painel Procurar, selecione as imagens e vá para **[!UICONTROL Build]** > **[!UICONTROL Swatch Sets]**.

   * **Comece na tela Conjunto de Amostras**: vá para **[!UICONTROL Build]** > **[!UICONTROL Swatch Sets]**. Selecione uma pasta na Biblioteca de ativos e arraste as imagens para a seção Exibições da página Conjunto de amostras.

1. Arraste as cores, os padrões ou os acabamentos da amostra para a caixa de espaço reservado Amostras na página Conjunto de amostras.

   Verifique se a amostra de cor, padrão ou fim arrastada para cada espaço reservado representa a cor, o padrão ou o fim da imagem adjacente.

1. Para alterar a ordem das imagens no Conjunto de amostras, arraste as imagens para novos locais.
1. Próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after a save]** está selecionado (padrão).
1. Selecione **[!UICONTROL Save]**, selecione uma pasta para armazenar o Conjunto de Amostras, digite um nome para o conjunto e selecione **[!UICONTROL Submit]**.
1. Para ver o Conjunto de Amostras no Visualizador de Conjunto de Amostras, selecione **[!UICONTROL Preview]** na tela Conjunto de Amostras. Você pode selecionar miniaturas de amostras no Visualizador de conjuntos de amostras para ver como elas funcionam.

## Editar um conjunto de amostras {#editing-a-swatch-set}

Se você editar um conjunto publicado ou não, a opção **[!UICONTROL Publish after a save]** afetará o conjunto e os membros do conjunto das seguintes maneiras:

| Conjunto já publicado? | **[!UICONTROL Publish after a save]** opção de salvar selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
|--- | --- | --- | --- |
| Sim | Sim | Publicado | Publicado. |
| Sim | Não | Publicado | Os membros do conjunto existentes mantêm seu estado publicado. Qualquer novo membro do conjunto adicionado durante sua edição manterá seu estado publicado ou não. |
| Não | Sim | Publicado | Publicado. |
| Não | Não | Não publicado | Os membros do conjunto existentes e os novos membros do conjunto adicionados durante a edição mantêm seus estados publicado ou não. |

Consulte também [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um Conjunto de Amostras:**

1. Na exibição de grade, navegue até um Conjunto de Amostras e, abaixo da imagem, selecione **[!UICONTROL Edit]**.
1. Execute uma das seguintes ações:

   * Para adicionar uma imagem (publicada ou não), arraste-a de uma pasta em Adicionar Assets para a página **[!UICONTROL Views]** do Conjunto de amostras.
   * Para remover uma imagem, selecione-a e, em seguida, selecione **[!UICONTROL Delete]** na barra de ferramentas.
   * Para reordenar imagens, arraste uma imagem para uma nova posição.

1. Quando terminar de editar o conjunto, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after a save]** está selecionado (padrão).
1. Selecione **[!UICONTROL Save]**, selecione uma pasta de armazenamento, insira um nome para o conjunto e selecione **[!UICONTROL Save]**.

## Excluir um conjunto de amostras

Ao excluir um conjunto, o próprio conjunto é movido para a pasta de itens excluídos. Os membros nesse conjunto não são afetados; eles mantêm seu estado existente, publicado ou não.

Consulte também [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um Conjunto de Amostras:**

1. Na Exibição em grade, Exibição em lista ou Exibição de detalhes, selecione um ou mais Conjuntos de amostras.
1. Na Barra de Navegação Global, vá para **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
