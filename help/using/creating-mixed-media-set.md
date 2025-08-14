---
title: Criar um conjunto de mix de mídia
description: Saiba como criar um Conjunto de mídias mistas no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Criar um conjunto de mix de mídia{#creating-a-mixed-media-set}

Crie um Conjunto de mídias mistas quando quiser combinar vários tipos de visualizadores em uma apresentação. Verifique se os arquivos, os Conjuntos de imagens, os Conjuntos de amostras e os Conjuntos de rotação estão prontos para publicação antes de adicioná-los ao Conjunto de mídia mista.

![Conjunto de mix de mídia](/help/using/assets/mm_mixed_media_set.png)

## Criar um conjunto de mix de mídia {#create-a-mixed-media-set}

Ao criar um conjunto, a opção **Publicar após salvar** afeta o conjunto e os membros do conjunto das seguintes maneiras:

| A opção &quot;Publicar após salvar&quot; foi selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um Conjunto de Mídias Mistas:**

1. Vá para **[!UICONTROL Build]** > **[!UICONTROL Mixed Media Sets]**.
1. Arraste os vídeos, Conjuntos de imagens, Conjuntos de rotação e amostras da Biblioteca de ativos para a tela Conjunto de mídias mistas.

   >[!NOTE]
   >
   >Um Conjunto de mídias mistas não oferece suporte a ativos com nomes de arquivo que contenham qualquer um dos seguintes caracteres: `( ) { }`.

1. Siga um destes procedimentos:

   * Para adicionar uma trilha sonora, arraste um arquivo de áudio da Biblioteca de ativos para a caixa Trilha sonora. A trilha sonora é reproduzida enquanto as imagens são exibidas. Ele para quando um vídeo é reproduzido.
   * Para alterar a ordem dos conjuntos, arraste-os para novos locais na tela Conjunto de mídias mistas. A ordem dos conjuntos na tela determina a ordem da esquerda para a direita na qual os usuários veem os conjuntos no Visualizador de conjunto de mídias mistas.
   * (Opcional) Para adicionar uma miniatura personalizada para representar um vídeo no Visualizador, arraste um arquivo de imagem da Biblioteca de ativos para a caixa de espaço reservado Miniatura.

1. Próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after a save]** está selecionado (padrão).
1. Selecione **[!UICONTROL Save]**.
1. Selecione uma pasta para armazenar o Conjunto de mídias mistas e digite um nome para o conjunto.
1. Selecione **[!UICONTROL Save]**.

   Para ver a aparência do Conjunto de imagens combinado em um Visualizador de Conjunto de imagens, selecione **[!UICONTROL Preview]**.

## Editar um conjunto de mix de mídia {#edit-a-mixed-media-set}

É possível editar um Conjunto de mídias mistas. Se você quiser editar um conjunto em um Conjunto de mídias mistas, abra esse conjunto separadamente, edite-o e salve-o. As edições são exibidas no Conjunto de mídias mistas.

Se você editar um conjunto publicado ou não, a opção **[!UICONTROL Publish after a save]** afetará o conjunto e os membros do conjunto das seguintes maneiras:

| Conjunto já publicado? | **[!UICONTROL Publish after a save]** opção selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existentes mantêm seu estado publicado. Qualquer novo membro do conjunto adicionado durante sua edição manterá seu estado publicado ou não. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existentes e os novos membros do conjunto adicionados durante a edição mantêm seus estados publicado ou não. |

Consulte também [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um Conjunto de Mídias Mistas:**

1. Selecione o botão de sobreposição **[!UICONTROL Edit]** do Conjunto de mídias mistas.
1. Siga um destes procedimentos:

   * Para remover itens, selecione-os e selecione **[!UICONTROL Delete]**.
   * Para reordenar itens, arraste-os para novos locais.

1. Quando terminar de editar o conjunto, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after a save]** está selecionado (padrão).
1. Selecione **[!UICONTROL Save]** ou **[!UICONTROL Save As]**.

## Excluir um conjunto de mix de mídia

Quando você exclui um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Consulte também [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um conjunto de mídia mista:**

1. Na Exibição em grade, Exibição em lista ou Exibição de detalhes, selecione um ou mais Conjuntos de mídias mistas.
1. Na Barra de Navegação Global, vá para **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
