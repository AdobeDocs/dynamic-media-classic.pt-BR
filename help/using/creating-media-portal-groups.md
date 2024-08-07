---
title: Criar e gerenciar grupos do Portal de mídia
description: Saiba como criar e gerenciar grupos do Portal de mídia no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 0%

---

# Criar e gerenciar grupos do Portal de mídia{#creating-and-managing-media-portal-groups}

Os *Grupos* foram criados para ajudá-lo a administrar os usuários do Portal de Mídia. Para acessar um ativo, o usuário deve ser membro de pelo menos um grupo que tenha permissão para acessar esse ativo. Ao adicionar um usuário, você o atribui a um ou mais grupos. Ao fazer isso, você concede ao usuário acesso às pastas às quais o grupo foi atribuído. Você também pode escolher quais Predefinições de imagem estarão disponíveis para um grupo.

## Use grupos para restringir o acesso a pastas, ativos e Predefinições de imagem {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Para conceder permissão de acesso em diferentes níveis, crie grupos. Para cada grupo, você atribui permissões de leitura, gravação e exclusão a diferentes pastas e ativos em pastas. Além disso, você decide quais Predefinições de imagem estão disponíveis para o grupo. Em seguida, você atribui usuários a grupos. Um usuário pode ser membro de mais de um grupo. O conceito de grupo oferece a flexibilidade de atribuir acesso a conjuntos limitados do conteúdo total.

Se você não conceder especificamente uma permissão de grupo a um ativo ou pasta, esse ativo ou pasta herdará as permissões atribuídas à pasta principal (a pasta acima dela na hierarquia de pastas). Conceda permissões a uma pasta principal se desejar garantir que todas as pastas secundárias herdem as mesmas permissões.

>[!NOTE]
>
>Os usuários podem pertencer a mais de um grupo. Quando um usuário pertence a dois grupos com permissões de acesso diferentes para uma pasta, o usuário recebe o acesso mais alto.

## Adicionar um grupo {#adding-a-group}

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Selecione **[!UICONTROL Add]**.
1. Na caixa de diálogo Adicionar Grupo, digite um nome para o grupo na caixa Nome do Grupo e selecione **[!UICONTROL Add Group]**.
1. Se desejar, você pode selecionar as caixas ao lado dos nomes dos usuários para adicionar usuários ao novo grupo.
1. Se quiser especificar permissões de acesso agora, selecione a guia **[!UICONTROL Asset Access Permissions]** e especifique as opções desejadas.

   Consulte [Estabelecer permissões de acesso a ativos para um grupo](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Você pode escolher quais Predefinições de imagem estarão disponíveis para o grupo. Basta clicar na guia **[!UICONTROL Image Preset Access Permissions]** e selecionar Predefinições de imagem que o grupo pode usar.

   Consulte [Escolher permissões de acesso de Predefinição de imagem para um grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Selecione **[!UICONTROL Close]**.

## Estabelecer permissões de acesso a ativos para um grupo {#establishing-asset-access-permissions-for-a-group}

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Na página Lista de grupos, siga um destes procedimentos:

   * Para adicionar um grupo e especificar permissões, selecione **[!UICONTROL Add]**. Na caixa de diálogo Adicionar Grupo, digite um nome para o grupo, selecione **[!UICONTROL Add Group]** e adicione usuários ao grupo.
   * Para editar as permissões de um grupo, selecione o grupo e **[!UICONTROL Edit]**.

1. Na caixa de diálogo Adicionar grupo ou Editar grupo, selecione a guia **[!UICONTROL Asset Access Permissions]**. O lado direito da guia oferece caixas para estabelecer permissões de leitura, gravação e exclusão para pastas e ativos. Você pode expandir e recolher pastas e subpastas no painel esquerdo.
1. Para atribuir direitos a pastas ou ativos individuais, selecione a pasta no painel esquerdo. O conteúdo da pasta é exibido no painel direito. Em seguida, atribua direitos ao grupo selecionando as caixas dos arquivos correspondentes. Ou selecione as pastas no painel direito.

   Esta tabela mapeia diferentes tarefas para permissões de leitura, gravação e exclusão.

   | Tarefa | Ler | Gravar | Excluir |
   | --- | --- | --- | --- |
   | Procurar pastas e arquivos | X | | |
   | Editar arquivos (cortar, ajustar, nitidez) | | X | |
   | Alterar nomes de arquivo | | X | |
   | Mover arquivos para pastas diferentes | | X | |
   | Renomear arquivos | | X | |
   | Excluir arquivos | | | X |

1. Selecione **[!UICONTROL Close]**.

>[!NOTE]
>
>Os direitos de acesso são estabelecidos ao selecionar uma caixa. Quando você atribuiu direitos a uma pasta, suas subpastas e todos os arquivos dentro dela recebem os mesmos direitos que a pasta principal. No entanto, é possível especificar direitos diferentes para subpastas individuais e arquivos de ativos.

## Escolher permissões de acesso de Predefinição de imagem para um grupo

Escolha permissões de acesso de Predefinição de imagem para um grupo se desejar especificar quais Predefinições de imagem estão disponíveis para os membros do grupo quando eles exportam ativos com o Media Portal.

Consulte também [Especificar opções de exportação disponíveis para usuários do Portal de Mídia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**Para escolher permissões de acesso de Predefinição de Imagem para um grupo:**

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Na página Lista de grupos, siga um destes procedimentos:

   * Para adicionar um grupo e especificar quais Predefinições de Imagem estão disponíveis para ele, selecione **[!UICONTROL Add]**. Na caixa de diálogo Adicionar Grupo, digite um nome para o grupo, selecione **[!UICONTROL Add Group]** e adicione usuários ao grupo.
   * Para editar as opções de Predefinição de imagem de um grupo, selecione o grupo e **[!UICONTROL Edit]**.

1. Na caixa de diálogo Adicionar grupo ou Editar grupo, selecione a guia **[!UICONTROL Image Preset Access Permissions]**.
1. Para especificar quais predefinições estão disponíveis para os usuários do Media Portal ao exportar ativos, selecione ou desmarque Predefinições de imagem.
1. Selecione **[!UICONTROL Close]**.

## Editar e excluir grupos {#edit-and-delete-groups}

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Na página Lista de grupos, selecione um grupo e edite-o ou exclua-o.

   **Editar um grupo**: selecione **[!UICONTROL Edit]** e escolha as opções na caixa de diálogo Editar Grupo.

   **Excluir um grupo**: Selecione **[!UICONTROL Delete]**.
