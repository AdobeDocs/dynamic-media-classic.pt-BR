---
title: Configuração de administração
description: Aprenda a configurar a área de administração do Adobe Systems Mídia dinâmica Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
topic: Administration
level: Intermediate
source-git-commit: dd799969ff9fd2638537254ae928a598eec627a3
workflow-type: tm+mt
source-wordcount: '1871'
ht-degree: 0%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Configuração de administração{#administration-setup}

As telas de Configuração de administração são para administrar Adobe Systems usuários Mídia dinâmica Classic. Use essas telas para permitir que os usuários trabalhem em Adobe Systems Mídia dinâmica Classic e se comuniquem email com outros usuários.

1. Para acessar as opções de Instalação Administrativa, vá para **Instalação** > **Instalação Pessoal** > **Instalação Administrativa**.

## Administração de usuários {#user-administration}

Todos os usuários do Adobe Dynamic Media Classic recebem uma função que determina seus privilégios e direitos de acesso aos recursos no Adobe Dynamic Media Classic. Os administradores determinam as diferentes funções e responsabilidades das empresas às quais estão atribuídos.

Normalmente, Adobe Systems Mídia dinâmica Classic configura o primeiro conjunto de empresas e atribui um Administrador da Empresa. Em seguida, o Administrador da empresa configura e administra Adobe Systems Mídia dinâmica usuários clássicos.

Adobe Systems Mídia dinâmica Classic é compatível com várias funções usuário. Essas funções podem acessar empresas configuradas para o Adobe Dynamic Media Classic:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Usuário do Adobe Dynamic Media Classic** Pode acessar empresas às quais foi atribuído; não pode executar nenhuma tarefa administrativa.

**Administrador da Empresa Adobe Dynamic Media Classic** Pode exibir e administrar apenas suas próprias empresas. Um Administrador da empresa também pode executar todas as funções administrativas, incluindo adicionar administradores e usuários. Um Administrador de empresa pode adicionar um usuário às contas de administrador da empresa do DMC. (Esta é a função de usuário padrão.)

Após adicionar um usuário, o Adobe Dynamic Media Classic envia a ele uma mensagem de e-mail de boas-vindas. A mensagem inclui uma senha e o URL do Adobe Dynamic Media Classic.

### Adicionar um usuário ou administrador {#adding-a-user-or-administrator}

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Selecione **[!UICONTROL Add]**.
1. Digite o nome e o endereço de email do usuário ou administrador que deseja adicionar e selecione **[!UICONTROL Next]**.

   >[!NOTE]
   >
   >O apóstrofo (`'`) não é permitido em endereços de email.

1. Para atribuir uma função ao usuário, escolha uma opção Função.

   Consulte [funções e privilégios de usuário do Adobe Dynamic Media Classic](administration-setup.md#user_administration).

1. Para adicionar um usuário a uma empresa, selecione o nome de uma empresa.
1. Se quiser adicionar o usuário a um grupo (se estiver adicionando um usuário ou colaborador do Portal de mídia), selecione **[!UICONTROL Next]** e adicione o usuário.
1. Selecione **[!UICONTROL Save]** para concluir a configuração do usuário.

   Depois de salvar, um prompt pergunta se você deseja adicionar um usuário a outra empresa. Selecione **[!UICONTROL Add]** se deseja adicionar o usuário a uma empresa.

   Todos os novos usuários recebem uma senha gerada aleatoriamente; os usuários são solicitados a alterar as senhas na primeira vez que fazem logon no aplicativo de desktop do Adobe Dynamic Media Classic.

   Um email de boas-vindas é enviado a novos usuários depois que você os adiciona. O email fornece uma senha temporária e explica como fazer logon no Adobe Dynamic Media Classic.

   Se o usuário não receber o email de boas-vindas, solicite que ele acesse a página de entrada da Adobe Dynamic Media Classic (https://s7sps1.scene7.com) e selecione **[!UICONTROL Forgot My Password]**. A senha é redefinida e um novo email é enviado. Se o usuário não receber o email e ele não estiver na pasta Lixo Eletrônico, entre em contato com o Suporte Técnico.

   Ao adicionar novos usuários ao Portal de Mídia, você também pode ir para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL User Administration]**, selecionar **[!UICONTROL Upload User List]** e selecionar um arquivo .csv que contenha no máximo 500 usuários.

### Excluir um usuário {#delet-a-user}

Você pode excluir usuários do Adobe Dynamic Media Classic tornando-os inválidos. Usuários inválidos são removidos do sistema e de todas as contas.

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Selecione um usuário na lista e, em seguida, selecione **[!UICONTROL Edit]**.
1. Desmarque Válido.
1. Selecione **[!UICONTROL Save]**.

### Ativar ou desativar usuários {#activating-or-deactivating-users}

Os usuários que foram desativados não têm mais permissão para inserir a conta listada na parte superior do menu Selecionar contas para acesso.

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Na lista de usuários, selecione ou desmarque a opção **[!UICONTROL Active]** ao lado do nome do usuário.

### Editar usuário informações {#editing-user-information}

As informações do usuário que você pode editar dependem da sua função como administrador e da função atribuída do usuário cujas informações você deseja editar. As opções esmaecidas (indisponíveis) não são editáveis.

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Selecione um usuário na lista e, em seguida, selecione **[!UICONTROL Edit]**.
1. Selecione a entrada na tabela que mostra a empresa para a qual você está tentando modificar permissões ou acesso e selecione **[!UICONTROL Manage Company]**.
1. Selecione a função de usuário.
1. Se quiser alterar a associação de grupo do usuário (se estiver editando ou adicionando um usuário ou colaborador do Portal de Mídia), selecione **[!UICONTROL Next]** e edite a associação de grupo.
1. Selecione **[!UICONTROL Save]**.

### Filtrar e classificar a lista de usuários {#filtering-and-sorting-the-user-list}

É possível filtrar e classificar a lista de usuários para localizar os usuários. Todos os usuários em todas as contas que você administra aparecem na lista Usuários, independentemente da conta selecionada no menu Selecionar conta para acesso.

Você pode usar as seguintes técnicas de filtragem de lista de usuários:

* **Filtrar por grupo**: selecione o menu **[!UICONTROL By Group]** e escolha uma opção para restringir a lista a usuários em um grupo.

* **Filtrar por função de usuário**: selecione o menu **[!UICONTROL By User Role]** e escolha uma opção para restringir a lista a usuários ou administradores de tipos diferentes.

* **Filtrar por nome de campo**: Selecione **[!UICONTROL Enable Filter By Field]**. Em seguida, selecione o menu **[!UICONTROL By Field Name]**, escolha uma coluna para filtrar a lista, selecione o menu Caractere de Filtro e escolha uma letra. A lista é filtrada em uma das colunas pela letra escolhida. Para ver a lista completa, desmarque a opção **[!UICONTROL Enable Filter By Field]**.

* **Filtrar inválido usuários**: Desmarcar **[!UICONTROL Include Invalid]**. Os resultados pesquisa exibem apenas os usuários que estão no sistema. Usuários inválidos foram excluídos do sistema e das contas que você administra.

* **Classificar por cabeçalho** de coluna: selecione um cabeçalho para classificar todos os usuários pelo status, em ordem alfabética, pelo nome, sobrenome ou email. Ou classifique por usuário função ou por status válido/inválido.

Se você tiver muitos usuários, poderá limitar o tamanho da lista selecionando o menu Tamanho Máximo da Lista e escolhendo um número.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to an Adobe Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to an Adobe Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Adobe Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Select **Manage Organizations**.
1. Select **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Select **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Adobe Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, select **Solutions** > **Experience Manager**. Under the Adobe Dynamic Media Classic card, select **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace "N" in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Largura de banda e armazenamento {#bandwidth-storage}

Os administradores da Adobe Dynamic Media Classic podem gerar largura de banda, armazenamento e outros tipos de relatórios para as empresas que administram. Esses relatórios estão disponíveis na página Largura de banda e armazenamento.

Para abrir esta página, vá para **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**. Expanda **[!UICONTROL Administration Setup]** e selecione **[!UICONTROL Bandwidth & Storage]**.

### Tipos de relatórios {#types-of-reports}

A tabela a seguir descreve os relatórios que podem ser gerados pela Largura de banda &amp;página de armazenamento:

| Relatório | Informações | Uso |
| --- | --- | --- |
| Largura de banda | | **IMPORTANTE**: a guia Largura de Banda não é mais suportada. Embora ainda apareça na interface, os dados de largura de banda não estão disponíveis e todos os valores são exibidos como `0`. |
| Armazenamento | Utilização do armazenamento | Rastreie a quantidade de dados carregados pela empresa. |
| Conteúdo da imagem | Exibe o total de ocorrências e o volume de entrega de imagens dividido por tipo de solicitação e subtipo. | Rastreie o número de solicitações e o volume para diferentes tipos de imagem, incluindo métricas de ativos que não são de vídeo. |
| Domínio | O número de solicitações de URL por domínio | Rastreie o uso da imagem com base no domínio da solicitação de imagem de uma empresa específica. (A Adobe Dynamic Media Classic pode fornecer mais de um domínio por conta. Para obter mais informações, entre em contato com o suporte técnico.) |
| Transmissão de vídeo | Uso da largura de banda para streaming de vídeo | Rastreie o uso de streaming de vídeo por empresa em intervalos de datas específicos para determinar os padrões de tráfego. |
| Conteúdo de vídeo | Tempo de reprodução de vídeos diferentes | Determine quais são os vídeos mais e menos visualizados. |

O relatório Conteúdo da imagem fornece informações sobre solicitações dos seguintes tipos de imagem:

* **Solicitação de imagem**: solicitações de imagens.

* **Solicitação de miniatura**: solicitações de imagens de amostra ou alternativas em visualizadores.

* **Solicitação de máscara**: solicitações para imagens que retornam máscaras de escala de cinza.

* **Solicitação de Bloco do Visualizador**: solicitações de imagem carregadas por um visualizador.

* **Solicitação de Objeto VNT**: solicitações de renderização de imagem que retornam uma imagem com objetos especificados nas vinhetas solicitadas.

* **Solicitação de Informações de VNT**: solicitações de renderização de imagem que retornam informações sobre as vinhetas solicitadas.

>[!NOTE]
>
>O relatório de transmissão de vídeo se aplica somente à transmissão de vídeos. Ele não rastreia a visualização de vídeos progressivos.

### Gerar um relatório {#generating-a-report}

Para gerar um relatório de largura de banda, armazenamento, conteúdo de imagem, domínio, fluxo contínuo de vídeo ou conteúdo de vídeo:

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Expanda Configuração da Administração e selecione **[!UICONTROL Bandwidth & Storage]**.
1. Selecione uma guia: **[!UICONTROL Bandwidth]**, **[!UICONTROL Storage]**, **[!UICONTROL Image Content]**, **[!UICONTROL Domain]**, **[!UICONTROL Video Streaming]** ou **[!UICONTROL Video Content]**.

   Consulte [Tipos de relatórios](administration-setup.md#types_of_reports).

### Visualizar dados de maneiras diferentes {#viewing-data-in-different-ways}

Depois de gerar um relatório na página Largura de banda e armazenamento, você pode escolher opções para visualizar informações. Você pode escolher como as informações são apresentadas, exibir as informações em um gráfico ou grade de dados e especificar um período para capturar as informações. Na Visualização de dados, também é possível classificar informações e reorganizar colunas.

* **Exibir dados em um gráfico ou grade de dados**: Selecione **[!UICONTROL Chart View]** para ver os dados em um gráfico; selecione **[!UICONTROL Data View]** para ver os dados em uma grade de dados.

* **Escolha um tipo de apresentação de relatório**: no menu Tipo de Relatório, selecione **[!UICONTROL Summary]**, **[!UICONTROL Daily]** ou **[!UICONTROL Monthly]** para organizar os dados em forma de resumo, por dia ou por mês. Nem todos os relatórios fornecem essa opção.

* **Especificar um período**: escolha opções para definir um período para o relatório e selecione **[!UICONTROL Update]** depois de definir um período:

* **Período predefinido**: no menu Relatório predefinido, escolha uma opção. Por exemplo, escolha Último mês para capturar dados do mês anterior.

* **Período personalizado**: no menu Relatório predefinido, selecione **[!UICONTROL Custom]**. Em seguida, escolha uma data no menu **[!UICONTROL Start Month]** (ou **[!UICONTROL Start Date]**) e uma data no menu # de Meses (ou # ou Dias). Para relatórios de conteúdo de domínio e vídeo, é possível escolher uma data de início e término específica para capturar informações de relatório.

* **Classificar dados (somente visualização de dados)**: Classificar informações em uma coluna. Selecione o cabeçalho da coluna. Selecione novamente para classificar em ordem decrescente.

* **Reorganizar colunas (Somente para exibição de dados)**: para mover uma coluna para um local diferente na grade de dados, arraste seu cabeçalho.

### Exportar e imprimir relatórios {#exporting-and-printing-reports}

Depois de gerar um relatório, é possível exportar seus dados para uso em planilhas e outros aplicativos. Também é possível imprimir relatórios.

* **Exportar dados** de relatório: em Visualização de dados, classifique e organize os dados conforme necessário. Em seguida, abra o **[!UICONTROL Export]** menu e escolha um formato: **[!UICONTROL Tab Delimited]**, **[!UICONTROL Comma Separated]** ou **[!UICONTROL HTML Formatted]**. Os dados são copiados para o Área de transferência no formato escolhido. Agora é possível colar os dados em uma planilha ou aplicativo.

* **Imprimir um relatório**: selecione **[!UICONTROL Print]**, escolha as opções desejadas na caixa de diálogo Imprimir e selecione **[!UICONTROL OK]**.

## Erros de imagem {#image-errors}

Os administradores do Adobe Dynamic Media Classic podem gerar relatórios de erro de imagem. Um relatório de Erro de imagem fornece uma lista dos 20 erros de imagem mais frequentes, nas últimas 24 horas, para a empresa à qual você está conectado no momento. Para gerar um relatório de Erro de imagem, faça o seguinte:

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Expanda a configuração de administração e selecione **[!UICONTROL Image Errors]**.
1. (Opcional) Siga um destes procedimentos:

   * Para classificar os erros pelas informações do cabeçalho, selecione um cabeçalho. Por padrão, os erros são classificados por número de ocorrências, do mais alto para o mais baixo.
   * Mova o cursor sobre o campo Response para ver uma mensagem de erro específica.
   * Para ver o link para a imagem ou a página da Web do referenciador, mova o cursor sobre o campo URL ou sobre o campo Referenciador.
   * Para copiar o link para a imagem real, selecione **[!UICONTROL URL Copy URL]**. Você pode colar esse link em uma janela do navegador para ir para a imagem e investigar o erro.
   * Para copiar o link para a página da Web de referência, selecione **[!UICONTROL Referrer Copy URL]**.

Os erros exibidos são para a empresa na qual você está conectado no momento. Cada erro inclui as seguintes informações:

* **ID da Imagem**: ID da imagem incorreta.

* **Hora**: o intervalo de tempo da primeira vez que o erro foi relatado até a última vez que o erro foi relatado, nas últimas 24 horas.

* **Contagem**: o número de erros relatados na imagem.

* **Resposta**: a mensagem de erro específica. Os erros são 4xx ou 5xx.

* **URLs**: lista a URL para a imagem no Adobe Dynamic Media Classic.

* **Referenciador**: especifica a URL do site de onde a solicitação inicial veio. O referenciador pode ser qualquer site da Web que tenha um link para a imagem.

As colunas URL e Referenciador têm URL de cópia associado a elas para simplificar os testes.
