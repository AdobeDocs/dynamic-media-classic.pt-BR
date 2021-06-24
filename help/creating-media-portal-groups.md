---
title: Criar e gerenciar grupos do Media Portal
description: Saiba como criar e gerenciar grupos do Media Portal.
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
feature: Dynamic Media Classic,Colaboração,Gerenciamento de ativos
role: Administrator,Business Practitioner
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Criar e gerenciar grupos do Media Portal{#creating-and-managing-media-portal-groups}

** Os grupos foram projetados para ajudar a administrar usuários do Media Portal. Para acessar um ativo, o usuário deve ser membro de pelo menos um grupo que tenha permissão para acessá-lo. Ao adicionar um usuário, você o atribui a um ou mais grupos. Ao fazer isso, você concede ao usuário acesso às pastas às quais o grupo foi atribuído. Você também pode escolher as Predefinições de imagem disponíveis para um grupo.

## Uso de grupos para restringir o acesso a pastas, ativos e predefinições de imagens {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Para conceder permissão de acesso em diferentes níveis, crie grupos. Para cada grupo, você atribui permissões de leitura, gravação e exclusão a pastas e ativos diferentes em pastas. Além disso, você decide quais Predefinições de imagem estão disponíveis para o grupo. Em seguida, você atribui usuários a grupos. Um usuário pode ser membro de mais de um grupo. O conceito de grupo oferece a flexibilidade de atribuir acesso a conjuntos limitados do conteúdo total.

Se você não conceder especificamente permissão de grupo a um ativo ou pasta, esse ativo ou pasta herdará as permissões atribuídas à pasta pai (a pasta acima dela na hierarquia de pastas). Conceda permissões a uma pasta pai se quiser garantir que todas as suas pastas filho herdem as mesmas permissões.

>[!NOTE]
>
>Os usuários podem pertencer a mais de um grupo. Quando um usuário pertence a dois grupos com permissões de acesso diferentes para uma pasta, o usuário recebe o maior acesso.

## Adicionar um grupo {#adding-a-group}

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Clique em **[!UICONTROL Add]**.
1. Na caixa de diálogo Adicionar grupo , digite um nome para o grupo na caixa Nome do grupo e clique em **[!UICONTROL Add Group]**.
1. Se desejar, você pode selecionar as caixas ao lado dos nomes dos usuários para adicionar usuários ao novo grupo.
1. Se desejar especificar permissões de acesso agora, clique na guia **[!UICONTROL Asset Access Permissions]** e especifique as opções desejadas.

   Consulte [Estabelecer permissões de acesso a ativos para um grupo](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Se desejar escolher quais Predefinições de imagem estão disponíveis para o grupo, clique na guia **[!UICONTROL Image Preset Access Permissions]** e selecione Predefinições de imagem que o grupo pode usar.

   Consulte [Escolher permissões de acesso à Predefinição de Imagem para um grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Clique em **[!UICONTROL Close]**.

## Estabelecimento de permissões de acesso a ativos para um grupo {#establishing-asset-access-permissions-for-a-group}

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Na página da lista Grupos, execute um dos seguintes procedimentos:

   * Para adicionar um grupo e especificar permissões, clique em **[!UICONTROL Add]**. Na caixa de diálogo Adicionar grupo , digite um nome para o grupo, clique em **[!UICONTROL Add Group]** e adicione usuários ao grupo.
   * Para editar as permissões de um grupo, selecione o grupo e clique em **[!UICONTROL Edit]**.

1. Na caixa de diálogo Adicionar grupo ou Editar grupo, clique na guia **[!UICONTROL Asset Access Permissions]**. O lado direito da guia oferece caixas para estabelecer permissões de leitura, gravação e exclusão para pastas e ativos. Você pode expandir e recolher pastas e subpastas no painel esquerdo.
1. Para atribuir direitos a pastas ou ativos individuais, selecione a pasta no painel esquerdo. O conteúdo da pasta é exibido no painel direito. Em seguida, atribua direitos ao grupo selecionando as caixas dos arquivos ou pastas correspondentes no painel direito.

   Esta tabela mapeia diferentes tarefas para ler, gravar e excluir permissões.

   | Tarefa | Ler | Gravar | Excluir |
   |--- |--- |--- |--- |
   | Procurar pastas e arquivos | X |  |  |
   | Editar arquivos (recortar, ajustar, ajustar) |  | X |  |
   | Alterar nomes de arquivo |  | X |  |
   | Mover arquivos para pastas diferentes |  | X |  |
   | Renomear arquivos |  | X |  |
   | Excluir arquivos |  |  | X |

1. Clique em **[!UICONTROL Close]**.

>[!NOTE]
>
>Os direitos de acesso são estabelecidos ao selecionar uma caixa. Ao atribuir direitos a uma pasta, suas subpastas e todos os arquivos dentro dela receberão os mesmos direitos que a pasta pai. No entanto, é possível especificar direitos diferentes para subpastas e arquivos de ativos individuais.

## Como escolher permissões de acesso à Predefinição de imagem para um grupo {#choosing-image-preset-access-permissions-for-a-group}

Escolha permissões de acesso à Predefinição de imagem para um grupo se desejar especificar quais Predefinições de imagem estão disponíveis para os membros do grupo ao exportar ativos com o Media Portal.

Consulte também [Especificar opções de exportação disponíveis para usuários do Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Na página da lista Grupos, execute um dos seguintes procedimentos:

   * Para adicionar um grupo e especificar quais Predefinições de imagem estão disponíveis para ele, clique em **[!UICONTROL Add]**. Na caixa de diálogo Adicionar grupo , digite um nome para o grupo, clique em **[!UICONTROL Add Group]** e adicione usuários ao grupo.
   * Para editar as opções de Predefinição de imagem de um grupo, selecione o grupo e clique em **[!UICONTROL Edit]**.

1. Na caixa de diálogo Adicionar grupo ou Editar grupo, clique na guia **[!UICONTROL Image Preset Access Permissions]**.
1. Para especificar quais predefinições estão disponíveis para os usuários do Media Portal ao exportar ativos, selecione ou desmarque Predefinições de imagem.
1. Clique em **[!UICONTROL Close]**.

## Editar e excluir grupos {#edit-and-delete-groups}

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Na página Lista de grupos , selecione um grupo e edite-o ou exclua-o.

   **Editar um grupo**  - Clique em  **[!UICONTROL Edit]** e escolha opções na caixa de diálogo Editar grupo.

   **Excluindo um grupo**  - Clique em  **[!UICONTROL Delete]**.
