---
title: Mover, renomear e excluir ativos
seo-title: Mover, renomear e excluir ativos
description: 'null'
seo-description: Saiba mais sobre como mover, renomear e excluir ativos.
uuid: deff 6521-0 ad 0-4 db 9-b 4 e 0-e 3211 ff 97740
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/managing_ assets
discoiquuid: 1 c 9 e 29 f 0-3083-4 d 22-a 439-2 a 01 faf 59683
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Mover, renomear e excluir ativos{#moving-renaming-and-deleting-assets}

Você pode mover, renomear e excluir ativos do Painel Procurar. Além disso, você pode excluir muitos ativos simultaneamente com um arquivo de texto.

## Mover ativos {#move-assets}

Você pode mover ativos para pastas diferentes no Painel Procurar.

1. Selecione o ativo ou os ativos no Painel Procurar e execute um dos procedimentos a seguir:

   * Exiba a pasta para a qual deseja mover os ativos na Biblioteca de ativos e arraste os ativos para a pasta.
   * Escolha Arquivo &gt; Mover, selecione uma pasta na janela Mover ativos e selecione Mover.

## Renomear ativos {#rename-assets}

Para renomear um ativo:

1. Selecione o ativo no Painel Procurar e execute um dos procedimentos a seguir:

   * Selecione o nome, digite um novo nome e pressione Enter ou clique fora do nome.
   * Escolha Arquivo &gt; Renomear. O nome do ativo é destacado. Digite um novo nome e pressione Enter.

Certifique-se de não inserir o nome de um ativo existente do Scene 7 Publishing System.

## Excluir ativos {#delete-assets}

Você pode excluir os ativos selecionados no Painel Procurar, bem como excluir pastas inteiras. Os ativos e pastas excluídos são movidos para a pasta Lixeira, onde permanecem por sete dias antes de serem excluídos permanentemente.

Ao excluir um ativo, todos os ativos derivados também são excluídos. Por exemplo, excluir uma imagem para a qual você criou metas de zoom exclui os destinos de zoom junto com a imagem.

>[!NOTE]
>
>Os direcionamentos de zoom, os atributos de imagem e as entradas do histórico são excluídos permanentemente quando os ativos são excluídos. Eles não são movidos junto com o ativo para a pasta Lixeira; não podem ser restauradas a partir da Lixeira.

1. Execute um dos procedimentos a seguir:

   * Para excluir um ou mais ativos, selecione os ativos no Painel Procurar e pressione Excluir ou escolha Arquivo &gt; Excluir.
   * Para excluir uma pasta, selecione a pasta na Biblioteca de ativos e clique **em Remover pasta**.

      Excluir uma pasta exclui a pasta, todos os ativos na pasta, bem como todos os ativos em suas subpastas.

>[!NOTE]
>
>O Dynamic Media Classic recomenda substituir arquivos de ativos em vez de excluí-los se o motivo para excluir um arquivo de ativo for substituí-lo por outro nome.

## Excluir vários ativos com um arquivo de texto {#delete-multiple-assets-with-a-text-file}

Para excluir muitos ativos de uma vez na Biblioteca de ativos, você pode listar os ativos que deseja excluir em um arquivo de texto e enviar a lista para o Dynamic Media Classic.

Crie a lista de IDs do sistema de publicação Scene 7 e salve-a como um arquivo de texto (.txt). Cada ID do sistema de publicação Scene 7 deve estar em sua própria linha (seguido por um retorno rígido).

Depois de criar a lista, siga estas etapas para usá-la para excluir ativos:

1. Escolha Arquivo &gt; Excluir lista de ativos.
1. Na caixa de diálogo Excluir ativos, procure ou digite o caminho para o arquivo de texto com a lista de ativos que deseja excluir.
1. Clique no botão Excluir.

Quando você exclui ativos com um arquivo de texto, se qualquer ID do sistema de publicação Scene 7 não estiver na lista, será exibida uma mensagem informando que o Dynamic Media Classic é «Não é possível validar essas entradas na lista: » junto com a lista de entradas. No entanto, o Dynamic Media Classic não gerará um erro na tela Trabalho.

>[!MORELIKETHIS]
>
>* [Seleção de ativos no Painel Procurar](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Preparação de ativos e pastas para upload](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restaurar ativos da pasta Lixeira](trash-folder.md#restoring_assets_from_the_trash_folder)

