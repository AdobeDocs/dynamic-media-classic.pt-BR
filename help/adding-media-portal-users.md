---
title: Adicionar e gerenciar usuários do Media Portal
seo-title: Adicionar e gerenciar usuários do Media Portal
description: 'null'
seo-description: Saiba como adicionar e gerenciar usuários do Media Portal
uuid: 96 d 4103 c -6428-4 ce 1-b 9 e 4-231599304 f 27
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/media_ portal
discoiquuid: 5 e 933045-ce 1 a -41 b 9-ba 8 b -2151 c 396 b 7 a 2
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Adicionar e gerenciar usuários do Media Portal{#adding-and-managing-media-portal-users}

Como administrador, você pode adicionar e gerenciar usuários, decidir se eles podem mudar as senhas, editar informações do usuário e fazer upload das listas de usuários. Essas tarefas são realizadas na tela Administração do usuário. Para acessar esta tela, clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Configuração de administração** &gt; **Administração do usuário**.

>[!NOTE]
>
>Antes de adicionar usuários, configure grupos para administração. O Media Portal não permite que você adicione um usuário sem atribuir o usuário a um ou mais grupos. Para obter mais informações, consulte [Criar e gerenciar grupos do portal de mídia](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Manipulação de senhas do portal de mídia {#handling-media-portal-passwords}

Usuários, colaboradores e colaboradores do portal de mídia recebem uma mensagem de email de boas-vindas com uma senha ao assiná-los. Os administradores podem decidir se os usuários do portal de mídia podem alterar essa senha.

1. Clique **em Configuração** &gt; **Configuração do portal de mídia** &gt; **Configurações gerais**.
1. Na página Configurações gerais, selecione ou desmarque **Permitir que o usuário do portal de mídia altere a senha**.
1. Clique **em Salvar**.

>[!NOTE]
>
>Os usuários do Media Portal que têm permissão para alterar senhas podem fazê-lo clicando **em Configuração** &gt; **Configuração** pessoal e alterando senhas na tela Configuração pessoal.

## Adicionar um usuário do portal de mídia {#adding-a-media-portal-user}

1. Clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Configuração de administração** &gt; **Administrador do usuário**.
1. Na página Administração do usuário, clique **em Adicionar**.
1. Na caixa de diálogo Adicionar usuário, no painel Informações do usuário, digite o Nome, o Sobrenome e o endereço de e-mail do usuário e clique **em Avançar**.
1. No painel Empresa/Função, na lista suspensa Empresa, selecione uma empresa ou empresa para o usuário.
1. Na lista Função, selecione uma função do Portal de mídia e clique **em Avançar**.

   Consulte [Funções do usuário do Media Portal](media-portal-user-roles.md#media_portal_user_roles).

1. No painel de Grupos de acesso, selecione um ou mais grupos.

   Consulte [Criar e gerenciar grupos do Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Opcional) Clique **em Configurações de e-mail** para escolher configurações de email diferentes das configurações padrão.

   Consulte [Configurar a mensagem de email de boas-vindas para usuários](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)do Media Portal.

1. Clique **em Adicionar usuário**.

Depois de adicionar um usuário, o Media Portal envia ao usuário uma mensagem de email de boas-vindas. A mensagem inclui uma senha temporária e o URL do portal de mídia.

## Upload de uma lista de usuários do Media Portal {#uploading-a-media-portal-user-list}

Se você tiver vários usuários para adicionar, poderá carregar uma lista de usuários. Os usuários são adicionados automaticamente à conta selecionada no momento.

Crie a lista de usuários como um arquivo CSV (valores separados por vírgula) que contém as informações do usuário. Depois que a lista é carregada, os usuários na lista são automaticamente adicionados à conta com suas atribuições de grupo especificadas. Um email de boas-vindas é enviado para cada novo usuário, incluindo um link para o Media Portal e uma senha temporária.

### Criação do arquivo CSV {#creating-the-csv-file}

Crie um arquivo CSV (arquivo. csv) que esteja em conformidade com o formato e os campos a seguir. A primeira linha do arquivo deve conter os cabeçalhos de coluna listados nesta tabela; você pode ordenar essas colunas conforme desejado. Todas as colunas são necessárias.

| Nome da coluna | Descrição |
|--- |--- |
| Nome | O nome. |
| Sobrenome | O sobrenome. |
| Email | Um endereço de email válido. |
| Senha | Uma string de senha com distinção entre maiúsculas e minúsculas. |
| Função do usuário | Mediaportaladminmediaportalusermediaportalcontributormediaportalcontributoruser |
| Grupos | Lista de uma ou mais atribuições de grupo de contas para cada usuário, separadas por vírgulas. Você especifica o grupo prefixando o nome da conta, separados por barra (/). Por exemplo, portalco/IT, em que portalco é a conta e o IT é o grupo na conta portalco. |

A amostra de amostra a seguir demonstra como dispor um arquivo CSV:

| Nome | Sobrenome | Email | Senha | Função do usuário | Grupos |
|--- |--- |--- |--- |--- |--- |
| Peter | Peterson | `petep@company.com` | welcome | Mediaportaladmin | Portalco/IT, portalco/Admin |
| Kevin | Marcas | `kevinm@myco.com` | welcome | Mediaportaluser | Portalco/mktggroup, portalco/test |


### Fazer upload do arquivo CSV {#uploading-the-csv-file}

1. Abra a tela de Configuração de administração do usuário.
1. Clique em **Carregar lista de usuários**.
1. Na caixa de diálogo Selecionar arquivo para carregar, selecione o arquivo CSV e clique **em Abrir**.

Cada usuário na lista é automaticamente adicionado aos grupos especificados. Uma mensagem de email de boas-vindas é enviada para cada um.

>[!NOTE]
Se o arquivo CSV não tiver sido formatado corretamente, a seguinte mensagem de erro é exibida: «Erro ao processar o arquivo CSV carregado. Verifique o conteúdo do arquivo de dados válidos. » Além disso, se o CSV contiver um usuário IP ou IPS existente, o usuário não será adicionado à Lista de usuários.

## Geração de uma lista selecionável de usuários do Media Portal {#generating-a-selectable-list-of-media-portal-users}

É possível exibir os nomes e endereços de email dos usuários do Media Portal em uma janela pop-up. Essa lista é útil se você deseja cortar e colar nomes de usuário e endereços para uso fora do Media Portal.

1. Clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Configuração de administração** &gt; **Administração do usuário**.
1. Na lista **suspensa Função** de usuário, escolha o nome da função de usuário do Media Portal e clique **em Atualizar** para exibir os nomes de uma classe do usuário do Media Portal.
1. Clique **em Lista** de pop-up para abrir a janela pop-up. Você pode copiar e colar esta lista.

## Configuração da mensagem de email de boas-vindas para usuários do Media Portal {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Você pode enviar um email de boas-vindas ao adicionar novos usuários, colaboradores e colaboradores do Media Portal. Você pode configurar esse email ou informar o Dynamic Media Classic para não enviá-lo.

1. Escolha **Configuração** &gt; **Configuração do aplicativo** &gt; **Configuração de administração** &gt; **Administração do usuário**.
1. Na tela Configuração de administração do usuário, clique **em Configurações de e-mail**.
1. Na caixa de diálogo Configurações de email, especifique qualquer uma das seguintes configurações:

   **Envie e-mail** desmarque essa opção se não quiser informar os novos usuários por e-mail que os assinou.

   **Senha padrão** Insira uma senha temporária para novos usuários, ou deixe o campo vazio para que o Dynamic Media Classic gere senhas aleatórias. Os usuários serão solicitados a alterar as senhas na primeira vez que fizerem logon.

   **URL de substituição** Insira um URL diferente do padrão se os usuários acessarem o Dynamic Media Classic por meio de um URL diferente.

## Outras tarefas de gerenciamento de usuários {#other-user-management-tasks}

A partir da tela de Configuração de administração do usuário, você também pode executar estas tarefas:

**Filtre e classifique a lista de usuários** Filtrar a lista de usuários do Media Portal para localizar usuários. Consulte Filtrar e classificar a lista de usuários.

**Excluir usuários** Exclua um usuário da lista. Consulte Excluir um usuário.

**Ativar e desativar os usuários** Suspender um usuário de acessar pastas. Consulte Ativar e desativar usuários.

**Editar informações** de usuário Informações atualizadas sobre um usuário. Consulte Editar informações do usuário.

**Criar campos definidos pelo usuário** Crie campos de metadados definidos pelo usuário para ajudar a organizar ativos no Sistema de publicação Scene 7. Os campos também podem ser ativados ou desativados, conforme necessário.

Consulte [Campos definidos pelo usuário](application-setup.md#user_defined_fields).
