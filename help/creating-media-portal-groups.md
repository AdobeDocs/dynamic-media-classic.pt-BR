---
title: Criação e gerenciamento de grupos do Portal de mídia
seo-title: Criação e gerenciamento de grupos do Portal de mídia
description: nulo
seo-description: Saiba como criar e gerenciar grupos do Portal de mídia.
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---


# Criação e gerenciamento de grupos do Portal de mídia{#creating-and-managing-media-portal-groups}

*Os grupos* são projetados para ajudá-lo a administrar usuários do Portal de mídia. Para acessar um ativo, um usuário deve ser membro de pelo menos um grupo que tenha permissão para acessar esse ativo. Quando você adiciona um usuário, você o atribui a um ou mais grupos. Ao fazer isso, você concede ao usuário acesso às pastas às quais o grupo foi atribuído. Você também pode escolher quais predefinições de imagens estão disponíveis para um grupo.

## Uso de grupos para restringir o acesso a pastas, ativos e predefinições de imagens {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Para conceder permissão de acesso em diferentes níveis, crie grupos. Para cada grupo, você atribui permissões de leitura, gravação e exclusão a pastas e ativos diferentes em pastas. Além disso, você decide quais predefinições de imagens estão disponíveis para o grupo. Em seguida, você atribui usuários a grupos. Um usuário pode ser membro de mais de um grupo. O conceito de grupo oferece a flexibilidade de atribuir acesso a conjuntos limitados do conteúdo total.

Se você não conceder especificamente uma permissão de grupo a um ativo ou pasta, esse ativo ou pasta herdará as permissões atribuídas à pasta pai (a pasta acima dele na hierarquia de pastas). Conceda permissões a uma pasta pai se desejar garantir que todas as pastas filhas herdem as mesmas permissões.

>[!NOTE]
>
>Os usuários podem pertencer a mais de um grupo. Quando um usuário pertence a dois grupos com permissões de acesso diferentes para uma pasta, o usuário recebe o maior acesso.

## Adicionar um grupo {#adding-a-group}

1. Clique em **Configuração** > Configuração **do** Media Portal > **Grupos**.
1. Clique em **Adicionar**.
1. Na caixa de diálogo Adicionar grupo, digite um nome para o grupo na caixa Nome do grupo e clique em **Adicionar grupo**.
1. Se desejar, você pode selecionar as caixas ao lado dos nomes dos usuários para adicionar usuários ao novo grupo.
1. Se desejar especificar permissões de acesso no momento, clique na guia Permissões **de acesso a** ativos e especifique as opções desejadas.

   Consulte [Estabelecer permissões de acesso a ativos para um grupo](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Se desejar escolher quais predefinições de imagens estão disponíveis para o grupo, clique na guia Permissões **de acesso à predefinição de** imagem e selecione Predefinições de imagem que o grupo pode usar.

   Consulte [Escolher permissões de acesso à predefinição de imagem para um grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Clique em **Fechar**.

## Estabelecendo permissões de acesso a ativos para um grupo {#establishing-asset-access-permissions-for-a-group}

1. Clique em **Configuração** > Configuração **do** Media Portal > **Grupos**.
1. Na página lista Grupos, execute um dos procedimentos a seguir:

   * Para adicionar um grupo e especificar permissões, clique em **Adicionar**. Na caixa de diálogo Adicionar grupo, digite um nome para o grupo, clique em **Adicionar grupo** e adicione usuários ao grupo.
   * Para editar as permissões de um grupo, selecione-o e clique em **Editar**.

1. Na caixa de diálogo Adicionar grupo ou Editar grupo, clique na guia Permissões **de acesso a** ativos. O lado direito da guia oferta as caixas para estabelecer permissões de leitura, gravação e exclusão para pastas e ativos. Você pode expandir e recolher pastas e subpastas no painel esquerdo.
1. Para atribuir direitos a pastas ou ativos individuais, selecione a pasta no painel esquerdo. O conteúdo da pasta é exibido no painel direito. Em seguida, atribua direitos ao grupo selecionando as caixas para os arquivos ou pastas correspondentes no painel direito.

   Esta tabela mapeia tarefas diferentes para ler, gravar e excluir permissões.

   | Tarefa | Leitura | Gravar | Excluir |
   |--- |--- |--- |--- |
   | Procurar pastas e arquivos | X |  |  |
   | Editar arquivos (cortar, aumentar a nitidez, ajustar) |  | X |  |
   | Alterar nomes de arquivo |  | X |  |
   | Mover arquivos para pastas diferentes |  | X |  |
   | Renomear arquivos |  | X |  |
   | Excluir arquivos |  |  | X |

1. Clique em **Fechar**.

>[!NOTE]
>
>Os direitos de acesso são estabelecidos quando você seleciona uma caixa. Quando você atribui direitos a uma pasta, suas subpastas e todos os arquivos dentro dela recebem os mesmos direitos que a pasta pai. No entanto, você pode especificar direitos diferentes para subpastas individuais e arquivos de ativos.

## Escolhendo permissões de acesso à Predefinição de imagem para um grupo {#choosing-image-preset-access-permissions-for-a-group}

Escolha permissões de acesso à predefinição de imagem para um grupo se desejar especificar quais predefinições de imagem estão disponíveis para os membros do grupo ao exportar ativos com o Portal de mídia.

Consulte também [Especificação de opções de exportação disponíveis para usuários](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)do Portal de mídia.

1. Clique em **Configuração** > Configuração **do** Media Portal > **Grupos**.
1. Na página lista Grupos, execute um dos procedimentos a seguir:

   * Para adicionar um grupo e especificar quais predefinições de imagens estão disponíveis para ele, clique em **Adicionar**. Na caixa de diálogo Adicionar grupo, digite um nome para o grupo, clique em **Adicionar grupo** e adicione usuários ao grupo.
   * Para editar as opções de Predefinição de imagem de um grupo, selecione o grupo e clique em **Editar**.

1. Na caixa de diálogo Adicionar grupo ou Editar grupo, clique na guia Permissões **de acesso à predefinição de** imagem.
1. Selecione ou desmarque Predefinições de imagem para especificar quais predefinições estão disponíveis para os usuários do Portal de mídia quando eles exportam ativos.
1. Clique em **Fechar**.

## Editar e excluir grupos {#edit-and-delete-groups}

1. Clique em **Configuração** > Configuração **do** Media Portal > **Grupos**.
1. Na página Lista do grupo, selecione um grupo e edite-o ou exclua-o.

   **Edição de um grupo** Clique em Editar e escolha opções na caixa de diálogo Editar grupo.

   **Excluindo um grupo** Clique em Excluir.

