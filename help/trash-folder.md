---
title: Gerenciar a pasta Lixeira
seo-title: Gerenciar a pasta Lixeira
description: 'null'
seo-description: Saiba como gerenciar a pasta Lixeira.
uuid: 3992 a 5 b 8-1919-4924-b 07 d -7 fb 25565 effd
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/managing_ assets
discoiquuid: 553 c 95 fc -0 a 41-4 f 06-af 50-a 62 bc 1438149
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Gerenciar a pasta Lixeira{#managing-the-trash-folder}

Os itens excluídos do Sistema de publicação Scene 7 são movidos para a pasta Lixeira. Eles permanecem por sete dias nesta pasta até serem restaurados ou excluídos permanentemente. É possível examinar itens excluídos selecionando o ícone de Lixeira localizado na parte inferior da Biblioteca de ativos e exibindo itens na pasta Lixeira.

Todos os usuários podem restaurar itens na pasta Lixeira para as pastas a partir das quais foram excluídas. Todos os usuários também podem esvaziar a pasta Lixeira de todo seu conteúdo.

A exclusão de itens da pasta Lixeira exclui permanentemente itens do Sistema de publicação Scene 7; itens excluídos da pasta Lixeira não podem mais ser restaurados. Para obter informações sobre como configurar notificações para administradores de empresas quando os ativos estiverem prestes a ser excluídos automaticamente da Lixeira, consulte [Configurações gerais do aplicativo](application-setup.md#general_settings).

>[!NOTE]
>
>Os ativos que foram movidos para a pasta Lixeira ainda estão registrados no Sistema de publicação Scene 7. Se você tentar carregar um arquivo com o mesmo nome de um arquivo excluído na pasta Lixeira, o Dynamic Media Classic trata o ativo que deseja carregar como um ativo duplicado. Dessa forma, um número é anexado ao seu nome.

## Sobre a pasta Lixeira {#about-the-trash-folder}

A exclusão de um item em uma pasta coloca o item na pasta Lixeira. O seguinte acontece ao excluir um item e movê-lo para a pasta Lixeira:

* Embora o item tenha sido removido das pastas do Sistema de Publicação do Scene 7, a ID não pode ser atribuída a outro ativo enquanto permanece na pasta Lixeira. Se você tentar carregar um ativo com o mesmo nome de um arquivo na pasta Lixeira, o Dynamic Media Classic anexa um numeral ao nome do ativo.
* O item não pode ser publicado. Mesmo se o item foi marcado para publicação quando o excluiu, ele não é publicado.
* O item permanece na pasta Lixeira até ser restaurado, sete dias passaram ou alguém escolhe o comando Vazia o traço. Após sete dias, uma operação de limpeza automática exclui permanentemente o item.

## Restaurar ativos da pasta Lixeira {#restoring-assets-from-the-trash-folder}

Não é necessário para a pessoa que excluiu um ativo para restaurá-lo; qualquer pessoa pode restaurar ativos da pasta Lixeira. Os ativos restaurados são colocados nas pastas a partir das quais foram excluídos. Se essas pastas não existirem mais, o Sistema de publicação Scene 7 os recriará, e os ativos restaurados serão colocados nas pastas recriadas.

Siga estas etapas para restaurar ativos da pasta Lixeira para as pastas a partir das quais foram excluídas:

1. Clique no ícone Lixeira para abrir a pasta Lixeira.
1. Selecione o ativo ou os ativos que deseja restaurar.
1. Escolha Arquivo &gt; Restaurar da lixeira.

## Exclusão permanente de ativos na pasta Lixeira {#permanently-deleting-assets-in-the-trash-folder}

Quando você exclui ativos na pasta Lixeira, os ativos são excluídos permanentemente. Os ativos são excluídos automaticamente da pasta Lixeira após sete dias.

Para excluir ativos da pasta Lixeira, selecione o ícone Lixeira para abrir a pasta Lixeira. Em seguida, exclua ativos individuais ou exclua todos os ativos na pasta:

**Excluir ativos individuais** Selecione os ativos que deseja excluir permanentemente e clique em Arquivo &gt; Vazio da lixeira.

**Excluir todos os ativos** Clique em Arquivo &gt; Lixo vazio.

>[!MORELIKETHIS]
>
>* [Excluir ativos](moving-renaming-deleting-assets.md#delete_assets)

