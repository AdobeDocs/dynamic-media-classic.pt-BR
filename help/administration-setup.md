---
title: Configuração da administração
description: Saiba como configurar a área de administração do Dynamic Media Classic.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1814'
ht-degree: 0%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Configuração da administração{#administration-setup}

As telas de Configuração de administração são para administrar usuários do Dynamic Media Classic. Use essas telas para permitir que os usuários trabalhem no Dynamic Media Classic e se comuniquem por email com os usuários.

1. Para acessar as opções de Configuração de administração, clique em **Configuração** > **Configuração Pessoal** > **Configuração de Administração**.

## Administração do usuário {#user-administration}

Todos os usuários do Dynamic Media Classic recebem uma função que determina seus privilégios e direitos de acesso aos recursos no Dynamic Media Classic. Os administradores determinam as diferentes funções e responsabilidades para as empresas às quais estão atribuídos.

Normalmente, o Dynamic Media Classic configura o primeiro conjunto de empresas e atribui um administrador de empresa. Em seguida, o administrador da empresa configura e administra os usuários do Dynamic Media Classic.

O Dynamic Media Classic é compatível com várias funções de usuário. Essas funções podem acessar empresas configuradas para o Dynamic Media Classic:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic** UserCan acesse empresas às quais foram atribuídas; Não possam desempenhar quaisquer funções administrativas.

**Adobe Dynamic Media Classic Company** AdminPode visualizar e administrar somente suas próprias empresas. Um Administrador da empresa também pode executar todas as funções de administração, incluindo a adição de administradores e usuários. Um Administrador da empresa pode adicionar um usuário às contas de administrador da empresa DMC. (Essa é a função de usuário padrão.)

Após adicionar um usuário, o Dynamic Media Classic envia uma mensagem de email de boas-vindas ao usuário. A mensagem inclui uma senha e o URL do Dynamic Media Classic.

### Adicionar um usuário ou administrador {#adding-a-user-or-administrator}

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Clique em **[!UICONTROL Add]**.
1. Insira o nome e o endereço de email do usuário ou administrador que deseja adicionar e clique em **[!UICONTROL Next]**.

   >[!NOTE]
   >
   >O caractere apóstrofo (`‘`) não é permitido em endereços de email.

1. Para atribuir uma função ao usuário, escolha uma opção Função .

   Consulte [Funções e privilégios de usuário do Dynamic Media Classic](administration-setup.md#user_administration).

1. Para adicionar um usuário a uma empresa, selecione um nome de empresa.
1. Se quiser adicionar o usuário a um grupo (se estiver adicionando um usuário ou colaborador do Media Portal), clique em **[!UICONTROL Next]** e adicione o usuário.
1. Clique em **[!UICONTROL Save]** para concluir a configuração do usuário.

   Depois de salvar, um prompt pergunta se você deseja adicionar um usuário a outra empresa. Clique em **[!UICONTROL Add]** se desejar adicionar o usuário a uma empresa.

   Todos os novos usuários recebem uma senha gerada aleatoriamente; os usuários devem alterar as senhas na primeira vez que fizerem logon no aplicativo de desktop do Dynamic Media Classic.

   Um email de boas-vindas é enviado aos novos usuários depois que você os adiciona. O email fornece uma senha temporária e explica como fazer logon no Dynamic Media Classic.

   Se o usuário não receber o email de boas-vindas, faça com que ele acesse a página de logon do Dynamic Media Classic (https://s7sps1.scene7.com) e clique em Esqueceu minha senha. A senha é redefinida e um novo email é enviado. Se o usuário não receber o email e ele não estiver na pasta de lixo eletrônico, entre em contato com o Suporte Técnico.

   Ao adicionar novos usuários do Media Portal, você também pode ir para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL User Administration]**, clicar em **[!UICONTROL Upload User List]** e selecionar um arquivo .csv que não contenha mais de 500 usuários.

### Excluir um usuário {#deleting-a-user}

Você pode excluir usuários do Dynamic Media Classic tornando-os inválidos. Usuários inválidos são removidos do sistema e de todas as contas.

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Selecione um usuário na lista e clique em **[!UICONTROL Edit]**.
1. Desmarque Válido.
1. Clique em **[!UICONTROL Save]**.

### Ativar ou desativar usuários {#activating-or-deactivating-users}

Os usuários que foram desativados não têm mais permissão para entrar na conta listada na parte superior do menu Selecionar contas para acessar .

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Na lista de usuários, selecione ou desmarque a opção **[!UICONTROL Active]** ao lado do nome do usuário.

### Editar informações do usuário {#editing-user-information}

As informações do usuário que você pode editar dependem de sua função como administrador e da função atribuída ao usuário cujas informações você deseja editar. As opções que estão esmaecidas (indisponíveis) não são editáveis.

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Selecione o usuário e clique em **[!UICONTROL Edit]**.
1. Selecione a entrada na tabela que mostra a empresa para a qual você está tentando modificar permissões ou acesso e clique em **[!UICONTROL Manage Company]**.
1. Selecione a função de usuário.
1. Se quiser alterar a associação de grupo do usuário (se estiver editando ou adicionando um usuário ou colaborador do Media Portal), clique em **[!UICONTROL Next]** e edite a associação de grupo.
1. Clique em **[!UICONTROL Save]**.

### Filtragem e classificação da lista de usuários {#filtering-and-sorting-the-user-list}

Você pode filtrar e classificar a lista de usuários para localizar os usuários. Todos os usuários em todas as contas que você administra aparecem na lista Usuários, independentemente da conta selecionada no menu Selecionar Conta para Acesso.

Você pode usar as seguintes técnicas de filtragem da lista de usuários:

* **Filtrar por grupo**  - Selecione o  **[!UICONTROL By Group]** menu e escolha uma opção para restringir a lista aos usuários em um grupo.

* **Filtrar por função de usuário**  - Selecione o  **[!UICONTROL By User Role]** menu e escolha uma opção para restringir a lista a usuários ou administradores de tipos diferentes.

* **Filtrar por nome**  de campo - Selecione  **[!UICONTROL Enable Filter By Field]**. Em seguida, selecione o menu **[!UICONTROL By Field Name]**, escolha uma coluna para filtrar a lista, selecione o menu Filtrar caractere e escolha uma letra. A lista é filtrada em uma das colunas pela letra escolhida. Para ver a lista completa, desmarque a opção **[!UICONTROL Enable Filter By Field]**.

* **Filtrar usuários**  inválidos - Desmarcar  **[!UICONTROL Include Invalid]**. Os resultados da pesquisa exibem somente os usuários que estão no sistema. Usuários inválidos foram excluídos do sistema e das contas que você administra.

* **Classificar por cabeçalho de coluna**  - Clique em um cabeçalho para classificar todos os usuários por seu status, alfabeticamente por nome, sobrenome ou email, por função de usuário ou por status válido/inválido.

Se você tiver muitos usuários, poderá limitar o tamanho da lista selecionando o menu Tamanho máximo da lista e escolhendo um número.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to a Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to a Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Click **Manage Organizations**.
1. Click **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Click **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, click **Solutions** > **Experience Manager**. Under the Dynamic Media Classic card, click **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Largura de banda e armazenamento {#bandwidth-storage}

Os administradores do Dynamic Media Classic podem gerar largura de banda, armazenamento e outros tipos de relatórios para as empresas que administram. Esses relatórios estão disponíveis na página Largura de banda e armazenamento .

Para abrir esta página, clique em **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**. Expanda **[!UICONTROL Administration Setup]** e clique em **[!UICONTROL Bandwidth & Storage]**.

### Tipos de relatórios {#types-of-reports}

A tabela a seguir descreve os relatórios que podem ser gerados a partir da página Largura de banda e Armazenamento:

| Relatório | Informações | Use |
|:--- |:--- |:--- |
| Largura de banda | Largura de banda usada por empresa | Rastreie o uso da largura de banda por empresa em intervalos de datas específicos para determinar os padrões de tráfego. |
| Armazenamento | Uso do armazenamento | Rastreie a quantidade de dados carregados pela empresa. |
| Conteúdo da imagem | O número de solicitações de imagem por tipo | Rastreie o número de solicitações e o volume para diferentes tipos de imagens. |
| Domínio | O número de solicitações de URL por domínio | Rastreie o uso da imagem com base no domínio da solicitação de imagem de uma empresa específica. (O Dynamic Media Classic pode fornecer mais de um domínio por conta. Para obter mais informações, entre em contato com o Suporte Técnico.) |
| Streaming de vídeo | Uso de largura de banda para streaming de vídeo | Rastreie o uso de vídeo de streaming por empresa em intervalos de datas específicos para determinar os padrões de tráfego. |
| Conteúdo de vídeo | Tempo de reprodução de diferentes vídeos | Determine quais são os vídeos mais visualizados e menos visualizados. |

O relatório Conteúdo da imagem fornece informações sobre solicitações para os seguintes tipos de imagem:

* **Solicitação de imagem**  - Solicitações de imagens.

* **Solicitação de miniatura**  - Solicitações de amostra ou imagens alternativas em visualizadores.

* **Solicitação de máscara**  - Solicitações para imagens retornando máscaras de escala de cinza.

* **Solicitação de mosaico do visualizador**  - Solicitações de imagem carregadas por um visualizador.

* **Solicitação de objeto Vnt**  - Solicitações de renderização de imagem que retornam uma imagem com objetos especificados nas vinhetas solicitadas.

* **Solicitação de informações de Vnt**  - Solicitação de renderização de imagem que retorna informações sobre as vinhetas solicitadas.

>[!NOTE]
>
>O relatório de transmissão de vídeo se aplica somente a vídeos de transmissão. Ele não rastreia a visualização de vídeos progressivos.

### Gerar um relatório {#generating-a-report}

Para gerar uma largura de banda, armazenamento, conteúdo de imagem, domínio, streaming de vídeo ou relatório de conteúdo de vídeo:

1. Escolha **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Expanda Configuração da Administração e clique em **[!UICONTROL Bandwidth & Storage]**.
1. Clique em uma guia : **[!UICONTROL Bandwidth]**, **[!UICONTROL Storage]**, **[!UICONTROL Image Content]**, **[!UICONTROL Domain]**, **[!UICONTROL Video Streaming]** ou **[!UICONTROL Video Content]**.

   Consulte [Tipos de relatórios](administration-setup.md#types_of_reports).

### Visualização de dados de maneiras diferentes {#viewing-data-in-different-ways}

Após gerar um relatório na página Largura de banda e armazenamento , é possível escolher as opções para exibir as informações. Você pode escolher como as informações são apresentadas, exibir informações em um gráfico ou grade de dados e especificar um período de tempo para capturar informações. Na Exibição de dados, também é possível classificar as informações e reorganizar as colunas.

* **Exibição de dados em um gráfico ou grade de dados**  - Clique em  **[!UICONTROL Chart View]** para exibir os dados em um gráfico; clique em  **[!UICONTROL Data View]** para exibir dados em uma grade de dados.

* **Escolha de um tipo de apresentação de relatório**  - No menu Tipo de relatório, clique em  **[!UICONTROL Summary]**,  **[!UICONTROL Daily]** ou  **[!UICONTROL Monthly]** para organizar os dados em forma de resumo, por dia ou por mês. Nem todos os relatórios fornecem essa opção.

* **Especificação de um período**  de tempo - Escolha as opções para definir um período de tempo para seu relatório e, em seguida, clique em  **[!UICONTROL Update]** após definir um período de tempo:

* **Período de tempo predefinido**  - No menu Relatório predefinido, escolha uma opção. Por exemplo, escolha Último mês para capturar dados do mês anterior.

* **Período de tempo personalizado**  - No menu Relatório predefinido, clique em  **[!UICONTROL Custom]**. Em seguida, escolha uma data no menu **[!UICONTROL Start Month]** (ou **[!UICONTROL Start Date]**) e uma data no menu # of Months (ou # ou Days) . Para os Relatórios de conteúdo de domínio e vídeo, é possível escolher uma data de início e de término específica para capturar as informações do relatório.

* **Classificação de dados (somente Exibição de dados)**  - Para classificar as informações em uma coluna, clique no cabeçalho da coluna. Clique novamente para classificar em ordem decrescente.

* **Reorganização de colunas (somente exibição de dados)**  - Para mover uma coluna para um local diferente na grade de dados, arraste o cabeçalho.

### Exportação e impressão de relatórios {#exporting-and-printing-reports}

Após gerar um relatório, é possível exportar seus dados para uso em planilhas e outros aplicativos. Também é possível imprimir relatórios.

* **Exportar dados de relatório**  - Na Exibição de dados, classifique e organize os dados conforme necessário. Em seguida, abra o menu **[!UICONTROL Export]** e escolha um formato: **[!UICONTROL Tab Delimited]**, **[!UICONTROL Comma Separated]** ou **[!UICONTROL HTML Formatted]**. Os dados são copiados para a Área de Transferência no formato escolhido. Agora é possível colar os dados em uma planilha ou aplicativo.

* **Impressão de um relatório**  - Clique em  **[!UICONTROL Print]**, escolha as opções desejadas na caixa de diálogo Imprimir e clique em  **[!UICONTROL OK]**.

## Erros de imagem {#image-errors}

Os administradores do Dynamic Media Classic podem gerar relatórios de erro de imagem. Um relatório de Erro de imagem fornece uma lista dos 20 erros de imagem mais frequentes, nas últimas 24 horas, para a empresa na qual você está conectado no momento. Para gerar um relatório de Erro de imagem, faça o seguinte:

1. Clique em **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Expanda Configuração da Administração e clique em **[!UICONTROL Image Errors]**.
1. (Opcional) Siga um destes procedimentos:

   * Para classificar erros pelas informações do cabeçalho, clique em um cabeçalho. Por padrão, os erros são classificados por número de ocorrências, do mais alto ao mais baixo.
   * Mova o cursor sobre o campo Response de um erro para ver a mensagem de erro específica.
   * Para ver o link para a imagem ou página da Web do referenciador, mova o cursor sobre o campo URL ou o campo Referenciador .
   * Para copiar o link para a imagem real, clique em **[!UICONTROL URL Copy URL]**. Você pode colar esse link em uma janela do navegador para ir para a imagem e investigar o erro.
   * Para copiar o link para a página da Web do referenciador, clique em **[!UICONTROL Referrer Copy URL]**.

Os erros exibidos são para a empresa na qual você está conectado no momento. Cada erro inclui as seguintes informações:

* **ID da imagem**  - ID da imagem ofensiva.

* **Hora**  - o intervalo de tempo da primeira vez em que o erro foi relatado na última vez em que o erro foi relatado, nas últimas 24 horas.

* **Count**  - O número de erros relatados na imagem.

* **Resposta**  - A mensagem de erro específica. Os erros são 4xx ou 5xx.

* **URLs**  - Lista o URL para a imagem no Dynamic Media Classic.

* **Referenciador**  - Especifica o URL do site de onde a solicitação inicial veio. O referenciador pode ser qualquer site da Web que tenha um link para a imagem.

As colunas URL e Referenciador têm Copiar URL associado a elas para simplificar o teste.
