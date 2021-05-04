---
title: Gerenciamento da pasta Lixeira
description: Saiba como gerenciar a pasta Lixeira.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Gerenciamento de ativos
role: Business Practitioner
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Gerenciando a pasta Lixeira{#managing-the-trash-folder}

Os itens que você excluir do Dynamic Media Classic são movidos para a pasta Lixeira. Os excluídos permanecem nessa pasta por sete dias até serem restaurados ou excluídos permanentemente. Você pode examinar os itens excluídos clicando no ícone **[!UICONTROL Trash]** na parte inferior da Biblioteca de ativos e visualizando os itens na página da pasta Lixeira.

Todos os usuários podem restaurar itens na pasta Lixeira para as pastas das quais foram excluídos. Todos os usuários também podem esvaziar a pasta Lixeira de todo o seu conteúdo.

A exclusão de itens da pasta Lixeira exclui permanentemente os itens do Dynamic Media Classic; os itens excluídos da pasta Lixeira não podem mais ser restaurados. Para obter informações sobre como configurar notificações para administradores de empresas quando os ativos estiverem prestes a ser excluídos automaticamente da Lixeira, consulte [Configurações gerais do aplicativo](application-setup.md#general_settings).

>[!NOTE]
>
>Os ativos que foram movidos para a pasta Lixeira ainda são registrados no Dynamic Media Classic. Se você tentar carregar um arquivo que tenha o mesmo nome de um arquivo excluído na pasta Lixeira, o Dynamic Media Classic tratará o ativo que você deseja fazer upload como um ativo duplicado. Dessa forma, um número é anexado ao seu nome.

## Sobre a pasta Lixeira {#about-the-trash-folder}

Excluir um item em uma pasta coloca o item na pasta Lixeira. O seguinte acontece quando você exclui um item e o move para a pasta Lixeira:

* Embora o item tenha sido removido das pastas do Dynamic Media Classic, a ID não poderá ser atribuída a outro ativo enquanto ele permanecer na pasta Lixeira. Se você tentar fazer upload de um ativo com o mesmo nome de um arquivo na pasta Lixeira, o Dynamic Media Classic anexará um numérico ao nome do ativo.
* O item não pode ser publicado. Mesmo se o item tiver sido marcado para publicação ao excluí-lo, ele não será publicado.
* O item permanece na pasta Lixeira até ser restaurado, sete dias se passam ou alguém escolhe o comando **[!UICONTROL Empty the Trash]**. Após sete dias, uma operação automática de limpeza exclui permanentemente o item.

## Restauração de ativos da pasta Lixeira {#restoring-assets-from-the-trash-folder}

Não é necessário que a pessoa que excluiu um ativo o restaure; qualquer pessoa pode restaurar ativos da pasta Lixeira. Os ativos restaurados são colocados nas pastas das quais foram excluídos. Se essas pastas não existirem mais, o Dynamic Media Classic as recriará e os ativos restaurados serão colocados nas pastas recriadas.

Para restaurar ativos da pasta Lixeira para as pastas das quais foram excluídos, faça o seguinte:

1. Na parte inferior do painel Biblioteca de ativos, clique no ícone **[!UICONTROL Trash]** para abrir a pasta Lixeira.
1. Selecione o ativo ou os ativos que deseja restaurar.
1. Clique em **[!UICONTROL File]** > **[!UICONTROL Restore from trash]**.

## Excluindo permanentemente ativos na pasta Lixeira {#permanently-deleting-assets-in-the-trash-folder}

Ao excluir ativos na pasta Lixeira, os ativos são excluídos permanentemente. Os ativos são excluídos automaticamente da pasta Lixeira após sete dias.

Para excluir permanentemente os ativos da pasta Lixeira, clique no ícone **[!UICONTROL Trash]**. Na página da pasta Lixeira, siga um destes procedimentos:

* **Exclusão de ativos individuais**  - Selecione os ativos que deseja excluir permanentemente e clique em  **[!UICONTROL File]** >  **[!UICONTROL Empty From Trash]**.

* **Exclusão de todos os ativos**  - Clique em  **[!UICONTROL File]** >  **[!UICONTROL Empty trash]**.

>[!MORELIKETHIS]
>
>* [Excluir ativos](moving-renaming-deleting-assets.md#delete_assets)

