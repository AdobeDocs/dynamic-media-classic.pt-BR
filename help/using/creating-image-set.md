---
title: Criar um conjunto de imagens
description: Saiba como criar um Conjunto de imagens no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
topic: Content Management
level: Intermediate
source-git-commit: edd893482cbafd9674a44cf9878b8ee3079d98f7
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Criar um conjunto de imagens{#creating-an-image-set}

Para criar um Conjunto de imagens com várias visualizações, você precisa de imagens que mostrem um item de diferentes pontos de vista ou mostrem diferentes aspectos do mesmo item. O objetivo é apresentar aos visualizadores imagens de um item para que eles tenham uma ideia sólida de como um item se parece ou faz.

## Criar um conjunto de imagens {#create}

Ao criar um conjunto, a variável **[!UICONTROL Publish after save]** opção afeta os membros set e set das seguintes maneiras:

| **[!UICONTROL `Publish after save`]** opção selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos mantêm seu estado publicado ou não publicado. |

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

Ao criar um Conjunto de imagens, o Adobe recomenda as seguintes práticas recomendadas e impõe os seguintes limites:

| Tipo de limite | Prática recomendada | Limite imposto |
| --- | --- | --- |
| Número de ativos duplicados por conjunto | Sem duplicatas | 20‡ |
| Número máximo de imagens por conjunto | De 5 a 10 imagens por conjunto | 1000 |

‡ A prática recomendada é não ter ativos duplicados em um conjunto. O limite é de 20 duplicatas para um único ativo. Se, no conjunto, você adicionar outra duplicata para esse ativo, a solicitação retornará um erro ou ignorará a duplicata.

Consulte também [Limitações do Dynamic Media](/help/using/limitations.md).

**Para criar um conjunto de imagens:**

1. Siga um destes procedimentos:

   * **Selecione as imagens primeiro** - No Painel de navegação, selecione as imagens que deseja para o seu Conjunto de imagens, vá para **[!UICONTROL Build]** > **[!UICONTROL Image Sets]**.

   * **Comece na tela Conjunto de imagens** - Vá para **[!UICONTROL Build]** > **[!UICONTROL Image Sets]**. A tela Conjunto de imagens é aberta. Selecione uma pasta na Biblioteca de ativos e arraste as imagens desejadas para o Conjunto de imagens na tela Conjunto de imagens.

1. Para alterar a ordem das imagens, arraste as imagens para novos locais.
1. Próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]**, selecione uma pasta para armazenar o Conjunto de imagens, digite um nome para o conjunto e selecione **[!UICONTROL Save]**.
1. Para ver o conjunto de imagens no Visualizador do conjunto de imagens, selecione **[!UICONTROL Preview]** na tela Conjunto de imagens. Você pode selecionar miniaturas de amostras no Visualizador de conjunto de imagens para ver como elas se comportam.

## Editar um conjunto de imagens {#editing-an-image-set}

Se você editar um conjunto publicado ou não, a variável **[!UICONTROL Publish after save]** opção afeta os membros set e set das seguintes maneiras:

| Conjunto já publicado? | **[!UICONTROL `Publish after save`]** opção selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- | --- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existentes mantêm seu estado publicado. Qualquer novo membro do conjunto adicionado durante sua edição manterá seu estado publicado ou não. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existentes e os novos membros do conjunto adicionados durante a edição mantêm seus estados publicado ou não. |

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um conjunto de imagens:**

1. Na Exibição de grade, navegue até um ImageSet e, abaixo da imagem, selecione **[!UICONTROL Edit]**.
1. Siga um destes procedimentos:

   * Para adicionar uma imagem (publicada ou não), arraste-a de uma pasta em Adicionar ativos para a **[!UICONTROL Views]** página.
   * Para remover uma imagem, selecione-a e **[!UICONTROL Delete]** na barra de ferramentas.
   * Para reordenar imagens, arraste uma imagem para uma nova posição.

1. Quando terminar de editar o conjunto, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]**, selecione uma pasta de armazenamento para o conjunto, digite um nome para o conjunto e selecione **[!UICONTROL Save]**.

## Excluir um conjunto de imagens

Quando você exclui um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um conjunto de imagens:**

1. Na Exibição em Grade, Exibição em Lista ou Exibição de Detalhes, selecione um Conjunto de Imagens ou mais.
1. Na Barra de navegação global, acesse **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
