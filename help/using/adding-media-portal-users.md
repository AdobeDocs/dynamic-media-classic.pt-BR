---
title: Adicionar e gerenciar usuários do Portal de mídia
description: Saiba como adicionar e gerenciar usuários do Portal de mídia no Adobe Dynamic Media Classic.
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
topic: Administration
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 0%

---

# Adicionar e gerenciar usuários do Portal de mídia{#adding-and-managing-media-portal-users}

Como administrador, você pode adicionar e gerenciar usuários, decidir se eles podem alterar senhas, editar informações do usuário e fazer upload de listas de usuários. Essas tarefas são realizadas na tela Administração do usuário. Para acessar essa tela, navegue até **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.

>[!NOTE]
>
>Antes de adicionar usuários, configure grupos para administrá-los. O Media Portal não permite adicionar um usuário sem atribuir o usuário a um ou mais grupos. Para obter mais informações, consulte [Criar e gerenciar grupos do Portal de mídia](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Administração de senhas do Portal de mídia {#handling-media-portal-passwords}

Os usuários do Portal de mídia, os colaboradores e os usuários-colaboradores recebem uma mensagem de email de boas-vindas com uma senha ao se inscreverem. Os administradores podem decidir se os usuários do Portal de mídia podem alterar essa senha.

1. Navegue até **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL General Settings]**.
1. Na página Configurações gerais, marque ou desmarque **[!UICONTROL Allow Media Portal user to change Password]**.
1. Selecionar **[!UICONTROL Save]**.

>[!NOTE]
>
>Os usuários do Portal de mídia que têm permissão para alterar senhas podem fazer isso selecionando **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** e alterar senhas na tela Configuração Pessoal.

## Adicionar um usuário do Portal de mídia {#adding-a-media-portal-user}

1. Navegue até **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Na página Administração do usuário, selecione **Adicionar**.
1. Na caixa de diálogo Adicionar usuário, no painel Informações do usuário, digite o Nome, Sobrenome e Endereço de email do usuário e selecione **[!UICONTROL Next]**.
1. No painel Empresa/Função, na lista suspensa Empresas, selecione uma empresa ou empresas para o usuário.
1. Na lista Função, selecione uma função Portal de mídia e, em seguida, selecione **[!UICONTROL Next]**.

   Consulte [Funções de usuário do Portal de mídia](media-portal-user-roles.md#media_portal_user_roles).

1. No painel Grupos de acesso, selecione um ou mais grupos.

   Consulte [Criar e gerenciar grupos do Portal de mídia](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Opcional) Selecione **[!UICONTROL Email Settings]** para escolher configurações de email diferentes das configurações padrão.

   Consulte [Configure a mensagem de e-mail de boas-vindas para os usuários do Portal de mídia](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Selecionar **[!UICONTROL Add User]**.

Depois de adicionar um usuário, o Media Portal envia ao usuário uma mensagem de email de boas-vindas. A mensagem inclui uma senha temporária e o URL do Portal de mídia.

## Carregar uma lista de usuários do Portal de mídia {#uploading-a-media-portal-user-list}

Se você tiver vários usuários para adicionar, é possível fazer upload de uma lista de usuários. Os usuários são adicionados automaticamente à conta selecionada no momento.

Crie a lista de usuários como um arquivo CSV (valores separados por vírgula) contendo as informações do usuário. Depois que a lista é carregada, os usuários na lista são adicionados automaticamente à conta com suas atribuições de grupo especificadas. Um email de boas-vindas é enviado para cada novo usuário, incluindo um link para o Portal de mídia e uma senha temporária.

### Criar o arquivo CSV {#creating-the-csv-file}

Crie um arquivo CSV (filename.csv) que esteja em conformidade com o formato e os campos a seguir. A primeira linha do arquivo deve conter os cabeçalhos de coluna listados nesta tabela; é possível ordenar essas colunas conforme desejado. Todas as colunas são obrigatórias.

| Nome da coluna | Descrição |
|--- |--- |
| Nome | O nome. |
| Sobrenome | O sobrenome. |
| E-mail | Um endereço de email válido. |
| Senha | Uma string de senha que diferencia maiúsculas e minúsculas. |
| Função do usuário | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorUser |
| Grupos | Lista de uma ou mais atribuições de grupo de contas para cada usuário, separadas por vírgulas. Você especifica o grupo prefixando o nome da conta, separado por uma barra (/). Por exemplo, PortalCo/IT, onde PortalCo é a conta e IT é o grupo dentro da conta PortalCo. |

O exemplo de planilha a seguir demonstra como criar o layout de um arquivo CSV:

| Nome | Sobrenome | E-mail | Senha | Função do usuário | Grupos |
|--- |--- |--- |--- |--- |--- |
| Pradaria | Kat | `prairiek@company.com` | bem-vindo | MediaPortalAdmin | PortalCo/IT, PortalCo/Admin |
| Rick | Brough | `rickb@myco.com` | bem-vindo | MediaPortalUser | PortalCo/MarketingGroup, PortalCo/test |

### Fazer upload do arquivo CSV {#uploading-the-csv-file}

1. Abra a tela Configuração de administração de usuário.
1. Selecionar **[!UICONTROL Upload User List]**.
1. Na caixa de diálogo Selecionar arquivo para upload, selecione o arquivo CSV e, em seguida, **[!UICONTROL Open]**.

Cada usuário na lista é adicionado automaticamente aos grupos especificados. Uma mensagem de e-mail de boas-vindas é enviada para cada um.

>[!NOTE]
>
>Se o arquivo CSV não tiver sido formatado corretamente, a seguinte mensagem de erro será exibida: &quot;Ocorreu um erro ao processar o arquivo CSV carregado. Verifique se há dados válidos no conteúdo do arquivo.&quot; Além disso, se o CSV contiver um usuário IP ou IPS existente, o usuário não será adicionado à Lista de usuários.

## Gerar uma lista selecionável de usuários do Portal de mídia {#generating-a-selectable-list-of-media-portal-users}

Você pode exibir os nomes e endereços de email dos usuários do Portal de mídia em uma janela pop-up. Essa lista é útil se você deseja recortar e colar nomes de usuário e endereços para uso fora do Portal de mídia.

1. Navegue até **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. No **[!UICONTROL By User Role]** escolha o nome de uma função de usuário do Portal de mídia e selecione **[!UICONTROL Refresh]** para exibir os nomes de uma classe de usuário do Media Portal.
1. Selecionar **[!UICONTROL Popup List]**. Copie e cole esta lista.

## Configure a mensagem de e-mail de boas-vindas para os usuários do Portal de mídia {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Você pode enviar um email de boas-vindas ao adicionar novos usuários, colaboradores e usuários-colaboradores do Portal de mídia. Você pode configurar essa mensagem de email ou instruir o Adobe Dynamic Media Classic a não enviá-la.

1. Navegue até **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Na tela User Administration Setup, selecione **[!UICONTROL Email Settings]**.
1. Na caixa de diálogo Configurações de email, especifique qualquer uma das seguintes configurações:

   * **[!UICONTROL Send Email]** - Desmarque essa opção se não quiser informar novos usuários por e-mail que você os inscreveu.

   * **[!UICONTROL Default Password]** - Insira uma senha temporária para novos usuários ou deixe o campo vazio para que o Adobe Dynamic Media Classic gere senhas aleatórias. Os usuários são solicitados a alterar as senhas na primeira vez que entrarem.

   * **[!UICONTROL Replacement URL]** - Insira um URL diferente do padrão se os usuários acessarem o Adobe Dynamic Media Classic por meio de um URL diferente.

## Outras tarefas de gerenciamento de usuários {#other-user-management-tasks}

Começando pela tela Configuração de administração de usuário, você também pode executar estas tarefas:

* **[!UICONTROL Filter and sort the user list]** - Filtrar a lista de usuários do Portal de mídia para localizar usuários.

* **[!UICONTROL Delete users]** - Remover um usuário da lista.

* **[!UICONTROL Activate and deactivate users]** - Suspender um usuário de acessar pastas.

* **[!UICONTROL Edit user information]** - Insira informações atualizadas sobre um usuário.

* **[!UICONTROL Create user-defined fields]** : crie campos de metadados personalizados definidos pelo usuário para que eles possam ajudar você a organizar ativos na Adobe Dynamic Media Classic. Os campos também podem ser ativados ou desativados, conforme necessário.

Consulte [Campos definidos pelo usuário](application-setup.md#user_defined_fields).
