---
title: Gerenciar a pasta Lixeira
description: Saiba como gerenciar a pasta Lixeira.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Gerenciar a pasta Lixeira{#managing-the-trash-folder}

Os itens que você excluir do Adobe Dynamic Media Classic são movidos para a pasta Lixeira. Os excluídos permanecem nessa pasta por sete dias até serem restaurados ou excluídos permanentemente. Você pode examinar os itens excluídos clicando no botão **[!UICONTROL Trash]** na parte inferior da Biblioteca de ativos e na exibição de itens na página da pasta Lixeira.

Todos os usuários podem restaurar itens na pasta Lixeira para as pastas das quais foram excluídos. Todos os usuários também podem esvaziar a pasta Lixeira de todo o seu conteúdo.

A exclusão de itens da pasta Lixeira exclui permanentemente os itens do Adobe Dynamic Media Classic; os itens excluídos da pasta Lixeira não podem mais ser restaurados. Para obter informações sobre como configurar notificações para administradores de empresas quando os ativos estiverem prestes a ser excluídos automaticamente da Lixeira, consulte [Configurações gerais do aplicativo](application-setup.md#general_settings).

>[!NOTE]
>
>Os ativos que foram movidos para a pasta Lixeira ainda são registrados no Adobe Dynamic Media Classic. Se você tentar fazer upload de um arquivo com o mesmo nome de um arquivo excluído na pasta Lixeira, a Adobe Dynamic Media Classic tratará o ativo que deseja fazer upload como um ativo duplicado. Dessa forma, um número é anexado ao seu nome.

## Sobre a pasta Lixeira {#about-the-trash-folder}

Excluir um item em uma pasta coloca o item na pasta Lixeira. O seguinte acontece quando você exclui um item e o move para a pasta Lixeira:

* Embora o item tenha sido removido de suas pastas do Adobe Dynamic Media Classic, sua ID não poderá ser atribuída a outro ativo enquanto ele permanecer na pasta Lixeira. Se você tentar fazer upload de um ativo com o mesmo nome de um arquivo na pasta Lixeira, o Adobe Dynamic Media Classic anexará um numérico ao nome do ativo.
* O item não pode ser publicado. Mesmo se o item tiver sido marcado para publicação ao excluí-lo, ele não será publicado.
* O item permanece na pasta Lixeira até ser restaurado, sete dias se passaram ou alguém escolhe o **[!UICONTROL Empty the Trash]** comando. Após sete dias, uma operação automática de limpeza exclui permanentemente o item.

## Restaurar ativos da pasta Lixeira {#restoring-assets-from-the-trash-folder}

Não é necessário que a pessoa que excluiu um ativo o restaure; qualquer pessoa pode restaurar ativos da pasta Lixeira. Os ativos restaurados são colocados nas pastas das quais foram excluídos. Se essas pastas não existirem mais, a Adobe Dynamic Media Classic as recriará e os ativos restaurados serão colocados nas pastas recriadas.

Para restaurar ativos da pasta Lixeira para as pastas das quais foram excluídos, faça o seguinte:

1. Na parte inferior do painel Biblioteca de ativos , selecione o **[!UICONTROL Trash]** para abrir a pasta Lixeira.
1. Selecione o ativo ou os ativos que deseja restaurar.
1. Ir para **[!UICONTROL File]** > **[!UICONTROL Restore from trash]**.

## Exclusão permanente de ativos na pasta Lixeira {#permanently-deleting-assets-in-the-trash-folder}

Ao excluir ativos na pasta Lixeira, os ativos são excluídos permanentemente. Os ativos são excluídos automaticamente da pasta Lixeira após sete dias.

Para excluir permanentemente os ativos da pasta Lixeira, selecione o **[!UICONTROL Trash]** ícone . Na página da pasta Lixeira, siga um destes procedimentos:

* **Exclusão de ativos individuais** - Selecione os ativos que deseja excluir permanentemente e vá para **[!UICONTROL File]** > **[!UICONTROL Empty From Trash]**.

* **Excluir todos os ativos** - Ir para **[!UICONTROL File]** > **[!UICONTROL Empty trash]**.

>[!MORELIKETHIS]
>
>* [Excluir ativos](moving-renaming-deleting-assets.md#delete_assets)

