---
title: Mover, renomear e excluir ativos
seo-title: Mover, renomear e excluir ativos
description: nulo
seo-description: Saiba mais sobre como mover, renomear e excluir ativos.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---


# Mover, renomear e excluir ativos{#moving-renaming-and-deleting-assets}

É possível mover, renomear e excluir ativos do Painel de navegação. Além disso, você pode excluir vários ativos simultaneamente com um arquivo de texto.

## Mover ativos {#move-assets}

Você pode mover ativos para diferentes pastas no Painel de navegação.

1. Selecione o ativo ou os ativos no Painel de navegação e execute um dos procedimentos a seguir:

   * Exiba a pasta para a qual deseja mover os ativos na Biblioteca de ativos e arraste os ativos para a pasta.
   * Escolha Arquivo > Mover, selecione uma pasta na janela Mover ativos e selecione Mover.

## Renomear ativos {#rename-assets}

Para renomear um ativo:

1. Selecione o ativo no Painel de navegação e execute um dos procedimentos a seguir:

   * Selecione o nome, digite um novo nome e pressione Enter ou clique fora do nome.
   * Escolha Arquivo > Renomear. O nome do ativo é realçado. Digite um novo nome e pressione Enter.

Certifique-se de não inserir o nome de um ativo existente do Dynamic Media Classic.

## Excluir ativos {#delete-assets}

Você pode excluir ativos selecionados no Painel de navegação, bem como excluir pastas inteiras. Os ativos e pastas excluídos são movidos para a pasta Lixeira, onde permanecem por sete dias antes de serem excluídos permanentemente.

Quando você exclui um ativo, todos os ativos derivados dele também são excluídos. Por exemplo, excluir uma imagem para a qual você criou públicos alvos de zoom exclui os públicos alvos de zoom junto com a imagem.

>[!NOTE]
>
>Públicos alvos de zoom, atributos de imagem e entradas de histórico são excluídos permanentemente ao excluir os ativos dos quais eles derivam. Eles não são movidos junto com o ativo para a pasta Lixeira; eles não podem ser restaurados do lixo.

1. Execute um dos procedimentos a seguir:

   * Para excluir um ou mais ativos, selecione os ativos no Painel de navegação e pressione Excluir ou escolha Arquivo > Excluir.
   * Para excluir uma pasta, selecione-a na Biblioteca de ativos e clique em **Remover pasta**.

      A exclusão de uma pasta exclui a pasta, todos os ativos da pasta e todos os ativos das subpastas.

>[!NOTE]
>
>O Dynamic Media Classic recomenda substituir os arquivos de ativos em vez de excluí-los se seu motivo para excluir um arquivo de ativo for substituí-lo por outro com o mesmo nome.

## Excluir vários ativos com um arquivo de texto {#delete-multiple-assets-with-a-text-file}

Para excluir vários ativos ao mesmo tempo em toda a Biblioteca de ativos, é possível lista dos ativos que deseja excluir em um arquivo de texto e enviar a lista para o Dynamic Media Classic.

Crie a lista de IDs do Dynamic Media Classic e salve-a como um arquivo de texto (.txt). Cada Dynamic Media Classic ID deve estar em sua própria linha (seguida de uma devolução em disco).

Depois de criar a lista, siga estas etapas para usá-la para excluir ativos:

1. Escolha Arquivo > Excluir Lista de ativo.
1. Na caixa de diálogo Excluir lista de ativo, procure ou digite o caminho para o arquivo de texto com a lista de ativos que deseja excluir.
1. Clique no botão Excluir.

Quando você exclui ativos com um arquivo de texto, se qualquer ID do Dynamic Media Classic não estiver na lista, uma mensagem é exibida informando que o Dynamic Media Classic é &quot;Não é possível validar essas entradas na lista:&quot; junto com a lista de entradas. Entretanto, o Dynamic Media Classic não gerará um erro na tela Job.

>[!MORELIKETHIS]
>
>* [Seleção de ativos no painel Procurar](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Preparação de ativos e pastas para upload](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restaurar ativos da pasta Lixeira](trash-folder.md#restoring_assets_from_the_trash_folder)

