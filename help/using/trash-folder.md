---
title: Gerenciar a pasta Lixeira
description: Saiba como gerenciar a pasta Lixeira.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Gerenciar a pasta Lixeira{#managing-the-trash-folder}

Os itens excluídos do Adobe Dynamic Media Classic são movidos para a pasta Lixeira. Esses itens excluídos permanecem nessa pasta por sete dias até que sejam restaurados ou excluídos permanentemente. Você pode examinar os itens excluídos ao selecionar o ícone **[!UICONTROL Trash]** na parte inferior da Biblioteca de ativos e exibir os itens na página da pasta Lixeira.

Todos os usuários podem restaurar itens na pasta Lixeira para as pastas das quais foram excluídos. Todos os usuários também podem esvaziar a pasta Lixeira de todo o seu conteúdo.

A exclusão de itens da pasta Lixeira exclui permanentemente itens da Adobe Dynamic Media Classic; os itens excluídos da pasta Lixeira não podem mais ser restaurados. Para obter informações sobre como configurar notificações para administradores de empresas quando os ativos estiverem prestes a serem excluídos automaticamente da Lixeira, consulte [Configurações Gerais do Aplicativo](application-setup.md#general_settings).

>[!NOTE]
>
>Os Assets que foram movidos para a pasta Lixeira ainda estão registrados no Adobe Dynamic Media Classic. Por exemplo, suponha que você tente carregar um arquivo que tenha o mesmo nome de um arquivo excluído na pasta Lixeira. O Adobe Dynamic Media Classic trata o ativo que você deseja fazer upload como um ativo duplicado. Nesse caso, um número é anexado ao seu nome.

## Sobre a pasta Lixeira {#about-the-trash-folder}

A exclusão de um item em uma pasta coloca o item na pasta Lixeira. O seguinte acontece quando você exclui um item e o move para a pasta Lixeira:

* Embora o item seja removido da pasta do Adobe Dynamic Media Classic, a respectiva ID não pode ser atribuída a outro ativo enquanto ele permanecer na pasta Lixeira. Se você tentar fazer upload de um ativo com o mesmo nome de um arquivo na pasta Lixeira, o Adobe Dynamic Media Classic anexa um numeral ao nome do ativo.
* Não é possível publicar o item. Mesmo que o item tenha sido marcado para publicação quando você o excluiu, ele não será publicado.
* O item permanece na pasta Lixeira até ser restaurado, passar sete dias ou alguém escolher o comando **[!UICONTROL Empty the Trash]**. Após sete dias, uma operação de limpeza automática exclui permanentemente o item.

## Restaurar ativos da pasta Lixeira {#restoring-assets-from-the-trash-folder}

Não é necessário que a pessoa que excluiu um ativo o restaure; qualquer pessoa pode restaurar os ativos da pasta Lixeira. Os Assets restaurados são colocados nas pastas de onde foram excluídos. Se essas pastas não existirem mais, o Adobe Dynamic Media Classic as recriará e os ativos restaurados serão colocados nas pastas recriadas.

Para restaurar ativos da pasta Lixeira para as pastas das quais eles foram excluídos, faça o seguinte:

1. Na parte inferior do painel Biblioteca de ativos, selecione o ícone **[!UICONTROL Trash]** para abrir a pasta Lixeira.
1. Selecione o ativo ou os ativos que deseja restaurar.
1. Vá para **[!UICONTROL File]** > **[!UICONTROL Restore from trash]**.

## Excluir ativos permanentemente na pasta Lixeira {#permanently-deleting-assets-in-the-trash-folder}

Ao excluir ativos na pasta Lixeira, os ativos são excluídos permanentemente. As Assets são excluídas automaticamente da pasta Lixeira após sete dias.

Você pode excluir permanentemente os ativos da pasta Lixeira ao selecionar o ícone **[!UICONTROL Trash]**. Na página da pasta Lixeira, siga um destes procedimentos:

* **Excluindo ativos individuais**: você pode excluir ativos permanentemente. Selecione os ativos desejados e clique em **[!UICONTROL File]** > **[!UICONTROL Empty From Trash]**.

* **Excluindo todos os ativos**: Vá para **[!UICONTROL File]** > **[!UICONTROL Empty trash]**.

>[!MORELIKETHIS]
>
>* [Excluir ativos](moving-renaming-deleting-assets.md#delete_assets)
