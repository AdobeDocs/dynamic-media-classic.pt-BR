---
title: Gerenciamento da pasta Lixeira
seo-title: Gerenciamento da pasta Lixeira
description: nulo
seo-description: Saiba como gerenciar a pasta Lixeira.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: referência
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/category/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Gerenciamento da pasta Lixeira{#managing-the-trash-folder}

Os itens que você excluir do Scene7 Publishing System serão movidos para a pasta Lixeira. Eles permanecem por sete dias nesta pasta até que sejam restaurados ou excluídos permanentemente. Você pode examinar itens excluídos selecionando o ícone Lixeira localizado na parte inferior da Biblioteca de ativos e exibindo itens na pasta Lixeira.

Todos os usuários podem restaurar itens na pasta Lixeira para as pastas das quais foram excluídos. Todos os usuários também podem esvaziar a pasta Lixeira de todo o seu conteúdo.

A exclusão de itens da pasta Lixeira exclui permanentemente os itens do Scene7 Publishing System; os itens excluídos da pasta Lixeira não podem mais ser restaurados. Para obter informações sobre como configurar notificações para administradores de empresas quando os ativos estiverem prestes a serem excluídos automaticamente do Lixeira, consulte Configurações [gerais do](application-setup.md#general_settings)aplicativo.

>[!NOTE]
>
>Os ativos que foram movidos para a pasta Lixeira ainda estão registrados no Scene7 Publishing System. Se você tentar carregar um arquivo que tenha o mesmo nome que um arquivo excluído na pasta Lixeira, o Dynamic Media Classic trata o ativo que você deseja carregar como um ativo duplicado. Assim, um número é anexado ao seu nome.

## Sobre a pasta Lixeira {#about-the-trash-folder}

A exclusão de um item em uma pasta coloca o item na pasta Lixeira. O seguinte acontece quando você exclui um item e o move para a pasta Lixeira:

* Embora o item tenha sido removido de suas pastas do Scene7 Publishing System, sua ID não pode ser atribuída a outro ativo enquanto permanece na pasta Lixeira. Se você tentar carregar um ativo com o mesmo nome de um arquivo na pasta Lixeira, o Dynamic Media Classic anexará um número ao nome do ativo.
* O item não pode ser publicado. Mesmo que o item tenha sido marcado para publicação ao excluí-lo, ele não será publicado.
* O item permanece na pasta Lixeira até que seja restaurado, sete dias depois, ou alguém escolhe o comando Vazio The Trash. Após sete dias, uma operação automática de limpeza exclui permanentemente o item.

## Restaurar ativos da pasta Lixeira {#restoring-assets-from-the-trash-folder}

Não é necessário que a pessoa que excluiu um ativo o restaure; qualquer pessoa pode restaurar ativos da pasta Lixeira. Os ativos restaurados são colocados nas pastas das quais foram excluídos. Se essas pastas não existirem mais, o Scene7 Publishing System as recriará e os ativos restaurados serão colocados nas pastas recriadas.

Siga estas etapas para restaurar ativos da pasta Lixeira para as pastas das quais foram excluídos:

1. Clique no ícone Lixeira para abrir a pasta Lixeira.
1. Selecione o ativo ou os ativos que deseja restaurar.
1. Escolha Arquivo &gt; Restaurar do lixo.

## Excluindo permanentemente ativos na pasta Lixeira {#permanently-deleting-assets-in-the-trash-folder}

Quando você exclui ativos na pasta Lixeira, os ativos são permanentemente excluídos. Os ativos são automaticamente excluídos da pasta Lixeira após sete dias.

Para excluir permanentemente os ativos da pasta Lixeira, selecione o ícone Lixeira para abrir a pasta Lixeira. Em seguida, exclua ativos individuais ou exclua todos os ativos na pasta:

* **Excluindo ativos** individuais Selecione os ativos que deseja excluir permanentemente e clique em **[!UICONTROL File > Empty From Trash]**.

* **Excluindo todos os ativos** Clique em **[!UICONTROL File > Empty Trash]**.

>[!MORELIKETHIS]
>
>* [Excluir ativos](moving-renaming-deleting-assets.md#delete_assets)

