---
title: Gerenciamento da pasta Lixeira
description: Saiba como gerenciar a pasta Lixeira.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---


# Gerenciando a pasta Lixeira{#managing-the-trash-folder}

Os itens que você excluir do Dynamic Media Classic são movidos para a pasta Lixeira. Eles permanecem por sete dias nessa pasta até serem restaurados ou excluídos permanentemente. Você pode examinar os itens excluídos selecionando o ícone Lixeira localizado na parte inferior da Biblioteca de ativos e visualizando os itens na pasta Lixeira.

Todos os usuários podem restaurar itens na pasta Lixeira para as pastas das quais foram excluídos. Todos os usuários também podem esvaziar a pasta Lixeira de todo o seu conteúdo.

A exclusão de itens da pasta Lixeira exclui permanentemente os itens do Dynamic Media Classic; os itens excluídos da pasta Lixeira não podem mais ser restaurados. Para obter informações sobre como configurar notificações para administradores de empresas quando os ativos estiverem prestes a ser excluídos automaticamente da Lixeira, consulte [Configurações gerais do aplicativo](application-setup.md#general_settings).

>[!NOTE]
>
>Os ativos que foram movidos para a pasta Lixeira ainda são registrados no Dynamic Media Classic. Se você tentar carregar um arquivo que tenha o mesmo nome de um arquivo excluído na pasta Lixeira, o Dynamic Media Classic tratará o ativo que você deseja fazer upload como um ativo duplicado. Dessa forma, um número é anexado ao seu nome.

## Sobre a pasta Lixeira {#about-the-trash-folder}

Excluir um item em uma pasta coloca o item na pasta Lixeira. O seguinte acontece quando você exclui um item e o move para a pasta Lixeira:

* Embora o item tenha sido removido das pastas do Dynamic Media Classic, a ID não poderá ser atribuída a outro ativo enquanto ele permanecer na pasta Lixeira. Se você tentar fazer upload de um ativo com o mesmo nome de um arquivo na pasta Lixeira, o Dynamic Media Classic anexará um numérico ao nome do ativo.
* O item não pode ser publicado. Mesmo se o item tiver sido marcado para publicação ao excluí-lo, ele não será publicado.
* O item permanece na pasta Lixeira até ser restaurado, sete dias se passam ou alguém escolhe o comando Vazio da Lixeira. Após sete dias, uma operação automática de limpeza exclui permanentemente o item.

## Restauração de ativos da pasta Lixeira {#restoring-assets-from-the-trash-folder}

Não é necessário que a pessoa que excluiu um ativo o restaure; qualquer pessoa pode restaurar ativos da pasta Lixeira. Os ativos restaurados são colocados nas pastas das quais foram excluídos. Se essas pastas não existirem mais, o Dynamic Media Classic as recriará e os ativos restaurados serão colocados nas pastas recriadas.

Siga estas etapas para restaurar ativos da pasta Lixeira para as pastas das quais foram excluídos:

1. Clique no ícone Lixeira para abrir a pasta Lixeira.
1. Selecione o ativo ou os ativos que deseja restaurar.
1. Escolha Arquivo > Restaurar da lixeira.

## Excluindo permanentemente ativos na pasta Lixeira {#permanently-deleting-assets-in-the-trash-folder}

Ao excluir ativos na pasta Lixeira, os ativos são excluídos permanentemente. Os ativos são excluídos automaticamente da pasta Lixeira após sete dias.

Para excluir permanentemente os ativos da pasta Lixeira, selecione o ícone Lixeira para abrir a pasta Lixeira. Em seguida, exclua ativos individuais ou exclua todos os ativos na pasta:

* **Exclusão de** ativos individuaisSelecione os ativos que deseja excluir permanentemente e clique em  **[!UICONTROL File > Empty From Trash]**.

* **Excluindo todos os** ativosClique  **[!UICONTROL File > Empty Trash]**.

>[!MORELIKETHIS]
>
>* [Excluir ativos](moving-renaming-deleting-assets.md#delete_assets)

