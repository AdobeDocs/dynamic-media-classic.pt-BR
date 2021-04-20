---
title: Adicionar e gerenciar usuários do Media Portal
description: Saiba como adicionar e gerenciar usuários do Media Portal
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Administrator,Business Practitioner
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
translation-type: tm+mt
source-git-commit: 31ac96e6fd11c47284d58540f5ec0135f0e6223b
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# Adicionar e gerenciar usuários do Media Portal{#adding-and-managing-media-portal-users}

Como administrador, você pode adicionar e gerenciar usuários, decidir se eles podem alterar senhas, editar informações do usuário e fazer upload de listas de usuários. Essas tarefas são realizadas na tela Administração do usuário . Para acessar essa tela, clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.

>[!NOTE]
>
>Antes de adicionar usuários, configure grupos para administrá-los. O Media Portal não permite adicionar um usuário sem atribuí-lo a um ou mais grupos. Para obter mais informações, consulte [Criação e gerenciamento de grupos do Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Lidar com senhas do Media Portal {#handling-media-portal-passwords}

Usuários do Media Portal, colaboradores e colaboradores-usuários recebem uma mensagem de email de boas-vindas com uma senha ao se inscrever. Os administradores podem decidir se os usuários do Media Portal podem alterar essa senha.

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL General Settings]**.
1. Na página Configurações gerais , selecione ou desmarque **[!UICONTROL Allow Media Portal user to change Password]**.
1. Clique em **[!UICONTROL Save]**.

>[!NOTE]
>
>Os usuários do Media Portal que têm permissão para alterar senhas podem fazer isso clicando em **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** e alterando senhas na tela Configuração Pessoal.

## Adicionar um usuário do Media Portal {#adding-a-media-portal-user}

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Na página Administração de Usuário, clique em **Adicionar**.
1. Na caixa de diálogo Adicionar usuário , no painel Informações do usuário , digite o Nome, Sobrenome e Endereço de email do usuário e clique em **[!UICONTROL Next]**.
1. No painel Empresa/função , na lista suspensa Empresas , selecione uma empresa ou empresas para o usuário.
1. Na lista Função, selecione uma função do Media Portal e clique em **[!UICONTROL Next]**.

   Consulte [Funções de usuário do Media Portal](media-portal-user-roles.md#media_portal_user_roles).

1. No painel Grupos de acesso , selecione um ou mais grupos.

   Consulte [Criar e gerenciar grupos do Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Opcional) Clique em **[!UICONTROL Email Settings]** para escolher configurações de email diferentes das configurações padrão.

   Consulte [Configurar a mensagem de email de boas-vindas para usuários do Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Clique em **[!UICONTROL Add User]**.

Após adicionar um usuário, o Media Portal envia uma mensagem de email de boas-vindas ao usuário. A mensagem inclui uma senha temporária e o URL do Media Portal.

## Fazer upload de uma lista de usuários do Media Portal {#uploading-a-media-portal-user-list}

Se você tiver vários usuários para adicionar, é possível fazer upload de uma lista de usuários. Os usuários são adicionados automaticamente à conta selecionada no momento.

Crie a lista de usuários como um arquivo CSV (valores separados por vírgulas) contendo as informações do usuário. Após a lista ser carregada, os usuários na lista são adicionados automaticamente à conta com suas atribuições de grupo especificadas. Um email de boas-vindas é enviado a cada novo usuário, incluindo um link para o Media Portal e uma senha temporária.

### Criação do arquivo CSV {#creating-the-csv-file}

Crie um arquivo CSV (filename.csv) que esteja em conformidade com o formato e os campos a seguir. A primeira linha do ficheiro deve conter os cabeçalhos de coluna enumerados nesta tabela; é possível ordenar essas colunas conforme desejado. Todas as colunas são obrigatórias.

| Nome da coluna | Descrição |
|--- |--- |
| Nome | O nome. |
| Sobrenome | O sobrenome. |
| Email | Um endereço de email válido. |
| Senha | Uma string de senha que diferencia maiúsculas e minúsculas. |
| Função do usuário | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorUser |
| Grupos | Lista de uma ou mais atribuições de grupo de contas para cada usuário, separadas por vírgulas. Você especifica o grupo com o prefixo do nome da conta, separado por barra (/). Por exemplo, PortalCo/IT, onde PortalCo é a conta e TI é o grupo na conta PortalCo. |

A planilha de amostra a seguir demonstra como elaborar o layout de um arquivo CSV:

| Nome | Sobrenome | Email | Senha | Função do usuário | Grupos |
|--- |--- |--- |--- |--- |--- |
| Prairie | Kat | `prairiek@company.com` | welcome | MediaPortalAdmin | PortalCo/IT,PortalCo/Admin |
| Rick | Básico | `rickb@myco.com` | welcome | MediaPortalUser | PortalCo/MktgGroup, PortalCo/test |


### Upload do arquivo CSV {#uploading-the-csv-file}

1. Abra a tela Configuração da administração do usuário .
1. Clique em **[!UICONTROL Upload User List]**.
1. Na caixa de diálogo Selecionar arquivo para upload , selecione o arquivo CSV e clique em **[!UICONTROL Open]**.

Cada usuário na lista é adicionado automaticamente aos grupos especificados. Uma mensagem de email de boas-vindas é enviada para cada mensagem.

>[!NOTE]
>
>Se o arquivo CSV não tiver sido formatado corretamente, a seguinte mensagem de erro será exibida: &quot;Erro ao processar o arquivo CSV carregado. Verifique se há dados válidos no conteúdo do arquivo.&quot; Além disso, se o CSV contiver um IP ou usuário IPS existente, o usuário não será adicionado à Lista de usuários.

## Gerar uma lista selecionável de usuários do Media Portal {#generating-a-selectable-list-of-media-portal-users}

Você pode exibir os nomes e endereços de email dos usuários do Media Portal em uma janela pop-up. Essa lista é útil se você deseja recortar e colar nomes de usuário e endereços para uso fora do Media Portal.

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Na lista suspensa **[!UICONTROL By User Role]**, escolha o nome de uma função de usuário do Media Portal e clique em **[!UICONTROL Refresh]** para exibir os nomes de uma classe de usuário do Media Portal.
1. Clique em **[!UICONTROL Popup List]** para abrir a janela pop-up. Copie e cole esta lista.

## Configuração da mensagem de email de boas-vindas para usuários do Media Portal {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Você pode enviar um email de boas-vindas quando adiciona novos usuários do Media Portal, colaboradores e usuários do contribuidor. Você pode configurar essa mensagem de email ou dizer ao Dynamic Media Classic para não enviá-la.

1. Escolha **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Na tela Configuração de administração do usuário, clique em **[!UICONTROL Email Settings]**.
1. Na caixa de diálogo Configurações de email , especifique qualquer uma das seguintes configurações:

   * **[!UICONTROL Send Email]** - Desmarque essa opção se não quiser informar novos usuários por e-mail que você os inscreveu.

   * **[!UICONTROL Default Password]** - Digite uma senha temporária para novos usuários ou deixe o campo vazio para que o Dynamic Media Classic gere senhas aleatórias. Os usuários são solicitados a alterar senhas na primeira vez que fizerem logon.

   * **[!UICONTROL Replacement URL]** - Digite um URL diferente do padrão se os usuários acessarem o Dynamic Media Classic por meio de um URL diferente.

## Outras tarefas de gerenciamento de usuários {#other-user-management-tasks}

A partir da tela de Configuração de administração do usuário, você também pode executar as seguintes tarefas:

* **[!UICONTROL Filter and sort the user list]** - Filtre a lista de usuários do Media Portal para localizar usuários.

* **[!UICONTROL Delete users]** - Remova um usuário da lista.

* **[!UICONTROL Activate and deactivate users]** - Suspender um usuário de acessar pastas.

* **[!UICONTROL Edit user information]** - Insira informações atualizadas sobre um usuário.

* **[!UICONTROL Create user-defined fields]** - Crie campos de metadados personalizados e definidos pelo usuário para ajudar a organizar ativos no Dynamic Media Classic. Os campos também podem ser ativados ou desativados, conforme necessário.

Consulte [Campos definidos pelo usuário](application-setup.md#user_defined_fields).
