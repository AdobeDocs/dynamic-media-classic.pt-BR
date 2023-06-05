---
title: Criar e gerenciar grupos do Portal de mídia
description: Saiba como criar e gerenciar grupos do Portal de mídia no Adobe Dynamic Media Classic.
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 0%

---

# Criar e gerenciar grupos do Portal de mídia{#creating-and-managing-media-portal-groups}

*Grupos* foram projetados para ajudar a administrar os usuários do Media Portal. Para acessar um ativo, o usuário deve ser membro de pelo menos um grupo que tenha permissão para acessar esse ativo. Ao adicionar um usuário, você o atribui a um ou mais grupos. Ao fazer isso, você concede ao usuário acesso às pastas às quais o grupo foi atribuído. Você também pode escolher quais Predefinições de imagem estarão disponíveis para um grupo.

## Use grupos para restringir o acesso a pastas, ativos e Predefinições de imagem {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Para conceder permissão de acesso em diferentes níveis, crie grupos. Para cada grupo, você atribui permissões de leitura, gravação e exclusão a diferentes pastas e ativos em pastas. Além disso, você decide quais Predefinições de imagem estão disponíveis para o grupo. Em seguida, você atribui usuários a grupos. Um usuário pode ser membro de mais de um grupo. O conceito de grupo oferece a flexibilidade de atribuir acesso a conjuntos limitados do conteúdo total.

Se você não conceder especificamente uma permissão de grupo a um ativo ou pasta, esse ativo ou pasta herdará as permissões atribuídas à pasta principal (a pasta acima dela na hierarquia de pastas). Conceda permissões a uma pasta principal se desejar garantir que todas as pastas secundárias herdem as mesmas permissões.

>[!NOTE]
>
>Os usuários podem pertencer a mais de um grupo. Quando um usuário pertence a dois grupos com permissões de acesso diferentes para uma pasta, o usuário recebe o acesso mais alto.

## Adicionar um grupo {#adding-a-group}

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Selecionar **[!UICONTROL Add]**.
1. Na caixa de diálogo Adicionar grupo, digite um nome para o grupo na caixa Nome do grupo e selecione **[!UICONTROL Add Group]**.
1. Se desejar, você pode selecionar as caixas ao lado dos nomes dos usuários para adicionar usuários ao novo grupo.
1. Se quiser especificar permissões de acesso agora, selecione o **[!UICONTROL Asset Access Permissions]** e especifique as opções desejadas.

   Consulte [Estabelecer permissões de acesso a ativos para um grupo](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Se quiser escolher quais Predefinições de imagem estarão disponíveis para o grupo, selecione a **[!UICONTROL Image Preset Access Permissions]** e selecione Predefinições de imagem que o grupo pode usar.

   Consulte [Escolher permissões de acesso de Predefinição de imagem para um grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Selecionar **[!UICONTROL Close]**.

## Estabelecer permissões de acesso a ativos para um grupo {#establishing-asset-access-permissions-for-a-group}

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Na página Lista de grupos, siga um destes procedimentos:

   * Para adicionar um grupo e especificar permissões, selecione **[!UICONTROL Add]**. Na caixa de diálogo Adicionar grupo, digite um nome para o grupo, selecione **[!UICONTROL Add Group]** e adicionar usuários ao grupo.
   * Para editar as permissões de um grupo, selecione o grupo e **[!UICONTROL Edit]**.

1. Na caixa de diálogo Adicionar grupo ou Editar grupo, selecione a **[!UICONTROL Asset Access Permissions]** guia. O lado direito da guia oferece caixas para estabelecer permissões de leitura, gravação e exclusão para pastas e ativos. Você pode expandir e recolher pastas e subpastas no painel esquerdo.
1. Para atribuir direitos a pastas ou ativos individuais, selecione a pasta no painel esquerdo. O conteúdo da pasta é exibido no painel direito. Em seguida, atribua direitos ao grupo selecionando as caixas dos arquivos ou pastas correspondentes no painel direito.

   Esta tabela mapeia diferentes tarefas para permissões de leitura, gravação e exclusão.

   | Tarefa | Ler | Gravar | Excluir |
   | --- | --- | --- | --- |
   | Procurar pastas e arquivos | X |  |  |
   | Editar arquivos (cortar, ajustar, nitidez) |  | X |  |
   | Alterar nomes de arquivo |  | X |  |
   | Mover arquivos para pastas diferentes |  | X |  |
   | Renomear arquivos |  | X |  |
   | Excluir arquivos |  |  | X |

1. Selecionar **[!UICONTROL Close]**.

>[!NOTE]
>
>Os direitos de acesso são estabelecidos ao selecionar uma caixa. Quando você atribui direitos a uma pasta, suas subpastas e todos os arquivos dentro dela recebem os mesmos direitos da pasta principal. No entanto, é possível especificar direitos diferentes para subpastas individuais e arquivos de ativos.

## Escolher permissões de acesso de Predefinição de imagem para um grupo {#choosing-image-preset-access-permissions-for-a-group}

Escolha permissões de acesso de Predefinição de imagem para um grupo se desejar especificar quais Predefinições de imagem estão disponíveis para os membros do grupo quando eles exportam ativos com o Media Portal.

Consulte também [Especifique as opções de exportação disponíveis para os usuários do Portal de mídia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**Para escolher permissões de acesso de Predefinição de imagem para um grupo:**

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Na página Lista de grupos, siga um destes procedimentos:

   * Para adicionar um grupo e especificar quais Predefinições de imagem estão disponíveis para ele, selecione **[!UICONTROL Add]**. Na caixa de diálogo Adicionar grupo, digite um nome para o grupo, selecione **[!UICONTROL Add Group]** e adicionar usuários ao grupo.
   * Para editar as opções de Predefinição de imagem de um grupo, selecione o grupo e **[!UICONTROL Edit]**.

1. Na caixa de diálogo Adicionar grupo ou Editar grupo, selecione a **[!UICONTROL Image Preset Access Permissions]** guia.
1. Para especificar quais predefinições estão disponíveis para os usuários do Media Portal ao exportar ativos, selecione ou desmarque Predefinições de imagem.
1. Selecionar **[!UICONTROL Close]**.

## Editar e excluir grupos {#edit-and-delete-groups}

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Na página Lista de grupos, selecione um grupo e edite-o ou exclua-o.

   **Editar um grupo** - Selecionar **[!UICONTROL Edit]** e escolha opções na caixa de diálogo Editar grupo.

   **Excluir um grupo** - Selecionar **[!UICONTROL Delete]**.
