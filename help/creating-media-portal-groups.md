---
title: Criação e gerenciamento de grupos do Media Portal
seo-title: Criação e gerenciamento de grupos do Media Portal
description: 'null'
seo-description: Saiba como criar e gerenciar grupos do Media Portal.
uuid: 23 f 360 e 1-ddcb -491 b-ab 9 f -428 f 3 ac 9 c 316
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/media_ portal
discoiquuid: 91524 d 36-b 77 a -4 dc 4-acba-a 7 bd 85297 e 98
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# Criação e gerenciamento de grupos do Media Portal{#creating-and-managing-media-portal-groups}

*Os grupos* foram projetados para ajudar a administrar usuários do Media Portal. Para acessar um ativo, um usuário deve ser membro de pelo menos um grupo com permissão para acessar esse ativo. Quando você adiciona um usuário, atribui o usuário a um ou mais grupos. Assim, você concede ao usuário acesso a pastas para as quais o grupo foi atribuído. Você também pode escolher quais Predefinições de imagens estão disponíveis para um grupo.

## Uso de grupos para restringir o acesso a pastas, ativos e predefinições de imagens {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Para conceder permissão de acesso em níveis diferentes, você cria grupos. Para cada grupo, você atribui permissões de leitura, gravação e exclusão a diferentes pastas e ativos em pastas. Além disso, você decide quais Predefinições de imagens estão disponíveis para o grupo. Em seguida, você atribui usuários a grupos. Um usuário pode ser membro de mais de um grupo. O conceito de grupo proporciona a flexibilidade de atribuir acesso a conjuntos limitados do conteúdo total.

Se você não conceder especificamente permissão de um grupo para um ativo ou pasta, esse ativo ou pasta herdará as permissões atribuídas à sua pasta pai (a pasta acima na hierarquia de pastas). Conceda permissões para uma pasta pai se quiser garantir que todas as pastas secundárias herdem as mesmas permissões.

>[!NOTE]
>
>Os usuários podem pertencer a mais de um grupo. Quando um usuário pertencer a dois grupos com permissões de acesso diferentes a uma pasta, o usuário recebe o maior acesso.

## Adicionar um grupo {#adding-a-group}

1. Clique **em Configuração** &gt; **Configuração do portal de mídia** &gt; **Grupos**.
1. Clique **em Adicionar**.
1. Na caixa de diálogo Adicionar grupo, digite um nome para o grupo na caixa Nome do grupo e clique **em Adicionar grupo**.
1. Se desejar, você pode selecionar as caixas ao lado dos nomes dos usuários para adicionar usuários ao novo grupo.
1. Se desejar especificar permissões de acesso no momento, clique na **guia Permissões** de acesso ao ativo e especifique as opções desejadas.

   Consulte [Estabelecer permissões de acesso de ativos para um grupo](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Se quiser escolher quais Predefinições de imagens estão disponíveis para o grupo, clique na **guia Permissões de acesso** a imagens e selecione Predefinições de imagens que o grupo pode usar.

   Consulte [Escolher permissões de acesso predefinidas de imagens para um grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Clique **em Fechar**.

## Estabelecimento de permissões de acesso a ativos para um grupo {#establishing-asset-access-permissions-for-a-group}

1. Clique **em Configuração** &gt; **Configuração do portal de mídia** &gt; **Grupos**.
1. Na página da lista Grupos, execute um dos procedimentos a seguir:

   * Para adicionar um grupo e especificar permissões, clique **em Adicionar**. Na caixa de diálogo Adicionar grupo, digite um nome para o grupo, clique **em Adicionar grupo** e adicione usuários ao grupo.
   * Para editar as permissões de um grupo, selecione o grupo e clique **em Editar**.

1. Na caixa de diálogo Adicionar grupo ou Editar, clique na **guia Permissões** de acesso ao ativo. O lado direito das caixas de ofertas de guias para estabelecer as permissões de leitura, gravação e exclusão para pastas e ativos. É possível expandir e recolher pastas e subpastas no painel esquerdo.
1. Para atribuir direitos a pastas ou ativos individuais, selecione a pasta no painel esquerdo. O conteúdo da pasta é exibido no painel direito. Em seguida, atribua direitos para o grupo selecionando as caixas para os arquivos ou pastas correspondentes no painel direito.

   Esta tabela mapeia diferentes tarefas para ler, gravar e excluir permissões.

   | Tarefa | Leitura | Gravar | Excluir |
   |--- |--- |--- |--- |
   | Procurar pastas e arquivos | X |  |  |
   | Editar arquivos (cortar, ajustar nitidez, ajustar) |  | X |  |
   | Alterar nomes de arquivo |  | X |  |
   | Mover arquivos para pastas diferentes |  | X |  |
   | Renomear arquivos |  | X |  |
   | Excluir arquivos |  |  | X |

1. Clique **em Fechar**.

>[!NOTE]
>
>Os direitos de acesso são estabelecidos quando uma caixa é selecionada. Quando você atribui direitos a uma pasta, suas subpastas e todos os arquivos nele recebem os mesmos direitos que a pasta pai. No entanto, é possível especificar direitos diferentes para subpastas individuais e arquivos de ativos.

## Como escolher permissões de acesso a predefinição de imagem para um grupo {#choosing-image-preset-access-permissions-for-a-group}

Escolha as permissões de acesso a Predefinição de imagem para um grupo se desejar especificar quais Predefinições de imagens estão disponíveis para membros do grupo quando eles exportarem ativos com o Media Portal.

Consulte [também Especificação das opções de exportação disponíveis para usuários](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)do Media Portal.

1. Clique **em Configuração** &gt; **Configuração do portal de mídia** &gt; **Grupos**.
1. Na página da lista Grupos, execute um dos procedimentos a seguir:

   * Para adicionar um grupo e especificar quais Predefinições de imagens estão disponíveis, clique **em Adicionar**. Na caixa de diálogo Adicionar grupo, digite um nome para o grupo, clique **em Adicionar grupo** e adicione usuários ao grupo.
   * Para editar as opções de Predefinição de imagens de um grupo, selecione o grupo e clique **em Editar**.

1. Na caixa de diálogo Adicionar grupo ou Editar, clique na **guia Permissões de acesso** a imagens predefinidas.
1. Selecione ou cancela a seleção de Predefinições de imagens para especificar quais predefinições estão disponíveis para usuários do Media Portal quando eles exportam ativos.
1. Clique **em Fechar**.

## Editar e excluir grupos {#edit-and-delete-groups}

1. Clique **em Configuração** &gt; **Configuração do portal de mídia** &gt; **Grupos**.
1. Na página Lista de grupos, selecione um grupo e edite-o ou exclua-o.

   **Editando um grupo** Clique em Editar e escolha opções na caixa de diálogo Editar grupo.

   **Excluir um grupo** clicar em Excluir.

