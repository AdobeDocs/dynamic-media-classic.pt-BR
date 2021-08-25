---
title: Criar um conjunto de imagens
description: Saiba como criar um conjunto de imagens no Dynamic Media Classic.
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
source-git-commit: 976f739e5233ae9da24b06cffa729353a7d03c46
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Criar um conjunto de imagens{#creating-an-image-set}

Para criar um Conjunto de imagens com várias exibições, você precisa de imagens que mostrem um item de diferentes pontos de vista ou que mostrem diferentes aspectos do mesmo item. O objetivo é apresentar aos visualizadores imagens de um item para que eles tenham uma ideia sólida de como um item se parece ou faz.

## Criar um conjunto de imagens {#create}

Ao criar um conjunto, a opção **[!UICONTROL Publish after save]** afeta o conjunto e os membros do conjunto das seguintes maneiras:

| **[!UICONTROL Publish after save]** opção selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
| --- | --- | --- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros do conjunto mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um conjunto de imagens:**

1. Siga um destes procedimentos:

   * **Selecione as imagens primeiro**  - No painel Procurar, selecione as imagens que deseja para seu Conjunto de imagens, vá para  **[!UICONTROL Build]** >  **[!UICONTROL Image Sets]**.

   * **Comece a partir da tela**  Conjunto de imagens - Vá para  **[!UICONTROL Build]** >  **[!UICONTROL Image Sets]**. A tela Conjunto de imagens é aberta. Selecione uma pasta na Biblioteca de ativos e arraste as imagens desejadas para seu Conjunto de imagens para a tela Conjunto de imagens.

1. Para alterar a ordem das imagens, arraste as imagens para novos locais.
1. Próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionado (padrão).
1. Selecione **[!UICONTROL Save]**, selecione uma pasta para armazenar o Conjunto de Imagens, insira um nome para o conjunto e selecione **[!UICONTROL Save]**.
1. Para ver seu Conjunto de imagens no Visualizador de conjunto de imagens, selecione **[!UICONTROL Preview]** na tela Conjunto de imagens. Você pode selecionar miniaturas de amostra no Visualizador do conjunto de imagens para ver como elas se comportam.

## Editar um conjunto de imagens {#editing-an-image-set}

Independentemente de você editar um conjunto publicado ou não, a opção **[!UICONTROL Publish after save]** afeta o conjunto e define os membros das seguintes maneiras:

| Definir já publicado? | **[!UICONTROL Publish after save]** opção selecionada antes de salvar a edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
| --- | --- | --- | --- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado. Qualquer novo conjunto de membros adicionado durante a edição manterá o estado publicado ou não. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto adicionados durante a edição mantêm o estado publicado ou não. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um conjunto de imagens:**

1. Na exibição de Grade, navegue até um ImageSet e, em seguida, abaixo da imagem, selecione **[!UICONTROL Edit]**.
1. Siga um destes procedimentos:

   * Para adicionar uma imagem (publicada ou não publicada), arraste-a de uma pasta em Adicionar ativos para a página **[!UICONTROL Views]** do conjunto de imagens.
   * Para remover uma imagem, selecione-a e, em seguida, selecione **[!UICONTROL Delete]** na barra de ferramentas.
   * Para reorganizar imagens, arraste uma imagem para uma nova posição.

1. Quando terminar de editar o conjunto, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionado (padrão).
1. Selecione **[!UICONTROL Save]**, selecione uma pasta de armazenamento para o seu conjunto, insira um nome para o conjunto e selecione **[!UICONTROL Save]**.

## Excluir um conjunto de imagens {#deleting-an-image-set}

Ao excluir um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) desse conjunto não são afetados; em vez disso, cada um mantém seu estado publicado ou não publicado.

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um conjunto de imagens:**

1. Na Exibição de Grade, Exibição de Lista ou Exibição de Detalhes, selecione um Conjunto de Imagens ou mais.
1. Na Barra de Navegação Global, vá para **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
