---
title: Mover, renomear e excluir ativos
description: Saiba como mover, renomear e excluir ativos no Adobe Dynamic Media Classic.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 741e31e64125a2dfe3f801480837ffbaf81767aa
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# Mover, renomear e excluir ativos{#moving-renaming-and-deleting-assets}

Você pode mover, renomear e excluir ativos no Painel de navegação. Além disso, é possível excluir muitos ativos simultaneamente com um arquivo de texto.

## Mover ativos {#move-assets}

Você pode mover ativos para pastas diferentes no Painel de navegação.

**Para mover ativos:**

1. Selecione o ativo ou os ativos no Painel de navegação e siga um destes procedimentos:

   * Exiba a pasta para a qual deseja mover os ativos na Biblioteca de ativos e arraste os ativos para a pasta.
   * Ir para **[!UICONTROL File]** > **[!UICONTROL Move]**, selecione uma pasta na janela Mover ativos e selecione **[!UICONTROL Move]**.

## Renomear ativos {#rename-assets}

1. Selecione o ativo no Painel de navegação e siga um destes procedimentos:

   * Selecione o nome, digite um novo nome e pressione **[!UICONTROL Enter]** ou selecione fora do nome.
   * Ir para **[!UICONTROL File]** > **[!UICONTROL Rename]**. O nome do ativo é realçado. Digite um novo nome e pressione **[!UICONTROL Enter]**. Certifique-se de não inserir o nome de um ativo existente do Adobe Dynamic Media Classic.

## Excluir ativos {#delete-assets}

Você pode excluir ativos selecionados no Painel de navegação e excluir pastas inteiras. Os ativos e as pastas excluídos são movidos para a pasta Lixeira, onde permanecem por sete dias antes de serem excluídos permanentemente.

Ao excluir um ativo, todos os ativos derivados dele também são excluídos. Por exemplo, a exclusão de uma imagem para a qual você criou destinos de zoom exclui os destinos de zoom junto com a imagem.

Os destinos de zoom, os atributos de imagem e as entradas do histórico são excluídos permanentemente quando você exclui os ativos dos quais eles derivam. Eles não são movidos juntamente com o ativo para a pasta Lixeira; eles não podem ser restaurados da Lixeira.

>[!IMPORTANT]
>
>A exclusão em massa é uma operação intensiva. Certifique-se de executar as exclusões em massa sequencialmente, e não como operações de exclusão intensa e simultânea. A Adobe recomenda que você limite as operações de exclusão para 5.000 exclusões de ativos ou menos por hora. Qualquer número maior que 5000 por hora pode causar limitação de taxa.

**Para excluir ativos:**

1. Siga um destes procedimentos:

   * Para excluir um ou mais ativos, selecione-os no Painel Procurar e pressione **[!UICONTROL Delete]** ou vá para **[!UICONTROL File]** > **[!UICONTROL Delete]**.
   * Para excluir uma pasta, selecione-a na Biblioteca de ativos e selecione **[!UICONTROL Remove Folder]**.

      A exclusão de uma pasta exclui a pasta, todos os ativos na pasta e todos os ativos em suas subpastas.

A Adobe Dynamic Media Classic recomenda substituir os arquivos de ativos em vez de excluí-los se o motivo para excluir um arquivo de ativos for substituí-lo por outro com o mesmo nome.

## Excluir vários ativos com um arquivo de texto {#delete-multiple-assets-with-a-text-file}

Para excluir vários ativos de uma só vez na Biblioteca de ativos, você pode listar os ativos que deseja excluir em um arquivo de texto e enviar a lista para o Adobe Dynamic Media Classic.

Crie a lista de Adobe Dynamic Media Classic IDs e salve-a como um arquivo de texto (.txt). Cada Adobe Dynamic Media Classic ID deve estar em sua própria linha (seguida por um retorno permanente).

Depois de criar a lista, siga estas etapas para usá-la para excluir ativos:

1. Ir para **[!UICONTROL File]** > **[!UICONTROL Delete Asset List]**.
1. Na caixa de diálogo Excluir ativo, navegue ou digite o caminho para o arquivo de texto com a lista de ativos que deseja excluir.
1. Selecionar **[!UICONTROL Delete]**.

Ao excluir ativos com um arquivo de texto, se qualquer ID do Adobe Dynamic Media Classic não estiver na lista, a mensagem &quot;Não é possível validar essas entradas na lista:&quot; será exibida. A lista de entradas também é exibida. No entanto, o Adobe Dynamic Media Classic não gera um erro na página Job.

>[!MORELIKETHIS]
>
>* [Selecionar ativos no painel Procurar](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Preparar seus ativos e pastas para upload](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restaurar ativos da pasta Lixeira](trash-folder.md#restoring_assets_from_the_trash_folder)

