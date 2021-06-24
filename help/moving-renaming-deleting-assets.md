---
title: Mover, renomear e excluir ativos
description: Saiba mais sobre como mover, renomear e excluir ativos.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Gerenciamento de ativos
role: Business Practitioner
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Mover, renomear e excluir ativos{#moving-renaming-and-deleting-assets}

Você pode mover, renomear e excluir ativos do Painel de navegação. Além disso, é possível excluir muitos ativos simultaneamente com um arquivo de texto.

## Mover ativos {#move-assets}

Você pode mover ativos para pastas diferentes no Painel de navegação.

1. Selecione o ativo ou os ativos no Painel de navegação e siga um destes procedimentos:

   * Exiba a pasta para a qual deseja mover os ativos na Biblioteca de ativos e arraste os ativos para a pasta.
   * Clique em **[!UICONTROL File]** > **[!UICONTROL Move]**, selecione uma pasta na janela Mover ativos e selecione **[!UICONTROL Move]**.

## Renomear ativos {#rename-assets}

1. Selecione o ativo no Painel de navegação e siga um destes procedimentos:

   * Selecione o nome, digite um novo nome e pressione **[!UICONTROL Enter]** ou clique fora do nome.
   * Clique em **[!UICONTROL File]** > **[!UICONTROL Rename]**. O nome do ativo é realçado. Insira um novo nome e pressione **[!UICONTROL Enter]**.

Certifique-se de não inserir o nome de um ativo existente do Dynamic Media Classic.

## Excluir ativos {#delete-assets}

É possível excluir ativos selecionados no Painel de navegação e excluir pastas inteiras. Os ativos e pastas excluídos são movidos para a pasta Lixeira, onde permanecem por sete dias antes de serem excluídos permanentemente.

Ao excluir um ativo, todos os ativos derivados dele também são excluídos. Por exemplo, excluir uma imagem para a qual você criou destinos de zoom exclui os destinos de zoom junto com a imagem.

>[!NOTE]
>
>Destinos de zoom, atributos de imagem e entradas de histórico são excluídos permanentemente quando você exclui os ativos dos quais derivam. Eles não são movidos junto com o ativo para a pasta Lixeira; eles não podem ser restaurados a partir da lixeira.

1. Siga um destes procedimentos:

   * Para excluir um ou mais ativos, selecione os ativos no Painel de navegação e pressione **[!UICONTROL Delete]** ou clique em **[!UICONTROL File]** > **[!UICONTROL Delete]**.
   * Para excluir uma pasta, selecione-a na Biblioteca de ativos e clique em **[!UICONTROL Remove Folder]**.

      A exclusão de uma pasta exclui a pasta, todos os ativos na pasta e todos os ativos em suas subpastas.

>[!NOTE]
>
>O Dynamic Media Classic recomenda a substituição de arquivos de ativos em vez de excluí-los se o motivo para excluir um arquivo de ativos for substituí-lo por outro pelo mesmo nome.

## Excluir vários ativos com um arquivo de texto {#delete-multiple-assets-with-a-text-file}

Para excluir muitos ativos de uma só vez na Biblioteca de ativos, é possível listar os ativos que deseja excluir em um arquivo de texto e enviar a lista para o Dynamic Media Classic.

Crie a lista de Dynamic Media Classic IDs e salve-a como um arquivo de texto (.txt). Cada ID do Dynamic Media Classic deve estar em sua própria linha (seguida de um retorno permanente).

Após criar a lista, siga estas etapas para usá-la para excluir ativos:

1. Clique em **[!UICONTROL File]** > **[!UICONTROL Delete Asset List]**.
1. Na caixa de diálogo Excluir ativo, procure ou digite o caminho para o arquivo de texto com a lista de ativos que deseja excluir.
1. Clique em **[!UICONTROL Delete]**.

Ao excluir ativos com um arquivo de texto, se qualquer ID do Dynamic Media Classic não estiver na lista, a mensagem &quot;Não é possível validar essas entradas na lista:&quot; é exibida e a lista de entradas. No entanto, o Dynamic Media Classic não gera um erro na página Job.

>[!MORELIKETHIS]
>
>* [Seleção de ativos no painel Procurar](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
* [Preparação de ativos e pastas para upload](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
* [Restauração de ativos da pasta Lixeira](trash-folder.md#restoring_assets_from_the_trash_folder)

