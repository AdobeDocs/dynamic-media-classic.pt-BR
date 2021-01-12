---
title: Adicionar e gerenciar usuários do Media Portal
seo-title: Adicionar e gerenciar usuários do Media Portal
description: nulo
seo-description: Saiba como adicionar e gerenciar usuários do Media Portal
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
translation-type: tm+mt
source-git-commit: 3a8283196c9c99a5709cf4995c426da7e4f6c83b
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---


# Adicionar e gerenciar usuários do Portal de mídia{#adding-and-managing-media-portal-users}

Como administrador, você pode adicionar e gerenciar usuários, decidir se eles podem alterar senhas, editar informações do usuário e carregar listas do usuário. Essas tarefas são realizadas na tela Administração do usuário. Para acessar essa tela, clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.

>[!NOTE]
>
>Antes de adicionar usuários, configure grupos para administrá-los. O Portal de mídia não permite que você adicione um usuário sem atribuí-lo a um ou mais grupos. Para obter mais informações, consulte [Criar e gerenciar grupos do Portal de Mídia](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Tratamento de senhas do Portal de mídia {#handling-media-portal-passwords}

Usuários, contribuidores e contribuidores do Portal de mídia recebem uma mensagem de email de boas-vindas com uma senha quando você os inscreve. Os administradores podem decidir se os usuários do Media Portal podem alterar essa senha.

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL General Settings]**.
1. Na página Configurações gerais, selecione ou desmarque **[!UICONTROL Allow Media Portal user to change Password]**.
1. Clique em **[!UICONTROL Save]**.

>[!NOTE]
>
>Os usuários do Portal de mídia que têm permissão para alterar senhas podem fazê-lo clicando em **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** e alterando as senhas na tela Configuração pessoal.

## Adicionando um usuário do Portal de mídia {#adding-a-media-portal-user}

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administation]**.
1. Na página Administração do usuário, clique em **Adicionar**.
1. Na caixa de diálogo Adicionar usuário, no painel Informações do usuário, digite o nome, o sobrenome e o endereço de email do usuário e clique em **[!UICONTROL Next]**.
1. No painel Empresa/Função, na lista suspensa Empresas, selecione uma empresa ou empresas para o usuário.
1. Na lista Função, selecione uma função do Portal de mídia e clique em **[!UICONTROL Next]**.

   Consulte [Funções de usuário do Media Portal](media-portal-user-roles.md#media_portal_user_roles).

1. No painel Grupos de acesso, selecione um ou mais grupos.

   Consulte [Criar e gerenciar grupos do Portal de Mídia](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Opcional) Clique em **[!UICONTROL Email Settings]** para escolher configurações de email diferentes das configurações padrão.

   Consulte [Configure a mensagem de email de boas-vindas para usuários do Portal de mídia](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Clique em **[!UICONTROL Add User]**.

Depois de adicionar um usuário, o Media Portal envia ao usuário uma mensagem de email de boas-vindas. A mensagem inclui uma senha temporária e o URL do Portal de mídia.

## Carregando uma lista de usuário do Portal de mídia {#uploading-a-media-portal-user-list}

Se você tiver vários usuários para adicionar, será possível carregar uma lista do usuário. Os usuários são adicionados automaticamente à conta selecionada no momento.

Crie a lista do usuário como um arquivo CSV (valores separados por vírgulas) contendo as informações do usuário. Depois que a lista é carregada, os usuários na lista são adicionados automaticamente à conta com suas atribuições de grupo especificadas. Um email de boas-vindas é enviado a cada novo usuário, incluindo um link para o Portal de mídia e uma senha temporária.

### Criação do arquivo CSV {#creating-the-csv-file}

Crie um arquivo CSV (filename.csv) que esteja em conformidade com o formato e os campos a seguir. A primeira linha do ficheiro deve conter os cabeçalhos de coluna listados nesta tabela; é possível ordenar essas colunas conforme desejado. Todas as colunas são obrigatórias.

| Nome da coluna | Descrição |
|--- |--- |
| Nome | O nome. |
| Sobrenome | O sobrenome. |
| Email | Um endereço de email válido. |
| Senha | Uma string de senha que diferencia maiúsculas e minúsculas. |
| Função do usuário | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorUsuário |
| Grupos | Lista de uma ou mais atribuições de grupos de contas para cada usuário, separadas por vírgulas. Você especifica o grupo prefixando o nome da conta, separado por uma barra (/). Por exemplo, PortalCo/IT, onde PortalCo é a conta e TI é o grupo na conta PortalCo. |

A planilha de amostra a seguir demonstra como dispor um arquivo CSV:

| Nome | Sobrenome | Email | Senha | Função do usuário | Grupos |
|--- |--- |--- |--- |--- |--- |
| Peter | Peterson | `petep@company.com` | welcome | MediaPortalAdmin | PortalCo/IT,PortalCo/Admin |
| Kevin | Marcas | `kevinm@myco.com` | welcome | MediaPortalUser | PortalCo/MktgGroup, PortalCo/test |


### Carregando o arquivo CSV {#uploading-the-csv-file}

1. Abra a tela Configuração da administração do usuário.
1. Clique em **[!UICONTROL Upload User List]**.
1. Na caixa de diálogo Selecionar arquivo para carregar, selecione o arquivo CSV e clique em **[!UICONTROL Open]**.

Cada usuário na lista é automaticamente adicionado aos grupos especificados. Uma mensagem de email de boas-vindas é enviada a cada um deles.

>[!NOTE]
>
>Se o arquivo CSV não tiver sido formatado corretamente, a seguinte mensagem de erro será exibida: &quot;Erro ao processar o arquivo CSV carregado. Verifique se há dados válidos no conteúdo do arquivo.&quot; Além disso, se o CSV contiver um IP existente ou um usuário IPS, o usuário não será adicionado à Lista Usuário.

## Gerando uma lista selecionável de usuários do Portal de mídia {#generating-a-selectable-list-of-media-portal-users}

Você pode exibir os nomes e endereços de email dos usuários do Media Portal em uma janela pop-up. Essa lista é útil se você deseja recortar e colar nomes de usuários e endereços para uso fora do Media Portal.

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Na lista suspensa **[!UICONTROL By User Role]**, escolha o nome de uma função de usuário do Portal de mídia e clique em **[!UICONTROL Refresh]** para exibir os nomes de uma classe de usuário do Portal de mídia.
1. Clique em **[!UICONTROL Popup List]** para abrir a janela pop-up. Você pode copiar e colar esta lista.

## Configuração da mensagem de email de boas-vindas para usuários do Media Portal {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Você pode enviar um e-mail de boas-vindas ao adicionar novos usuários do Portal de mídia, contribuidores e contribuidores-usuários. Você pode configurar esta mensagem de email ou informar o Dynamic Media Classic para não enviá-la.

1. Escolha **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Na tela Configuração da administração do usuário, clique em **[!UICONTROL Email Settings]**.
1. Na caixa de diálogo Configurações de e-mail, especifique qualquer uma das seguintes configurações:

   **[!UICONTROL Send Email]** Desmarque essa opção se não quiser informar novos usuários por email que você os inscreveu.

   **[!UICONTROL Default Password]** Digite uma senha temporária para novos usuários ou deixe o campo vazio para que o Dynamic Media Classic gere senhas aleatórias. Os usuários devem alterar as senhas na primeira vez que fizerem logon.

   **[!UICONTROL Replacement URL]** Insira um URL diferente do padrão se os usuários acessarem o Dynamic Media Classic por meio de um URL diferente.

## Outras tarefas de gerenciamento de usuários {#other-user-management-tasks}

A partir da tela Configuração da administração do usuário, você também pode fazer estas tarefas:

**[!UICONTROL Filter and sort the user list]** Filtre a lista de usuários do Portal de mídia para localizar usuários. Consulte Filtrar e classificar a lista do usuário.

**[!UICONTROL Delete users]** Exclua um usuário da lista. Consulte Excluir um usuário.

**[!UICONTROL Activate and deactivate users]** Suspenda o acesso de um usuário às pastas. Consulte Ativar e desativar usuários.

**[!UICONTROL Edit user information]** Insira informações atualizadas sobre um usuário. Consulte Editar informações do usuário.

**[!UICONTROL Create user-defined fields]** Crie campos de metadados personalizados e definidos pelo usuário para ajudar a organizar ativos no Dynamic Media Classic. Os campos também podem ser ativados ou desativados, conforme necessário.

Consulte [Campos Definidos pelo Usuário](application-setup.md#user_defined_fields).
