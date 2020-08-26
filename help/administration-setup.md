---
title: Configuração da administração
seo-title: Configuração da administração
description: nulo
seo-description: Saiba como configurar a área de administração do Dynamic Media Classic.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
translation-type: tm+mt
source-git-commit: 1ee586fab6a4e10a946848fd079438ade38490d9
workflow-type: tm+mt
source-wordcount: '1945'
ht-degree: 0%

---


<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Configuração da administração{#administration-setup}

As telas de Configuração de administração são para administrar usuários do Dynamic Media Classic. Use essas telas para permitir que os usuários trabalhem no Dynamic Media Classic e se comuniquem por email com os usuários.

1. Para acessar as opções de Configuração da administração, clique em **Configuração** > Configuração **pessoal** > Configuração **da** administração.

## Administração do usuário {#user-administration}

Todos os usuários do Dynamic Media Classic recebem uma função que determina seus privilégios e direitos de acesso aos recursos no Dynamic Media Classic. Os administradores determinam as diferentes funções e responsabilidades para as empresas às quais estão atribuídos.

Normalmente, o Dynamic Media Classic configura o primeiro conjunto de empresa e atribui um administrador de empresa. O administrador da empresa então configura e administra os usuários do Dynamic Media Classic.

O Dynamic Media Classic suporta várias funções de usuário. Essas funções podem acessar empresas configuradas para o Dynamic Media Classic:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Usuário** do Adobe Dynamic Media Classic pode acessar empresas às quais foram atribuídas; não possa desempenhar quaisquer funções administrativas.

**O administrador** da Empresa Adobe Dynamic Media Classic pode visualização e administrar somente suas próprias empresas. Um administrador de Empresa também pode executar todas as funções administrativas, incluindo a adição de administradores e usuários. Um administrador da Empresa pode adicionar um usuário às contas de administrador da empresa do DMC. (Essa função é a função padrão do usuário.)

Depois de adicionar um usuário, o Dynamic Media Classic envia ao usuário uma mensagem de email de boas-vindas. A mensagem inclui uma senha e o URL do Dynamic Media Classic.

### Adicionar um usuário ou administrador {#adding-a-user-or-administrator}

1. Clique em Configuração > Configuração do aplicativo > Configuração da administração > Administração do usuário.
1. Clique em Adicionar.
1. Digite o nome e o endereço de email do usuário ou administrador que deseja adicionar e clique em Avançar.

   >[!NOTE]
   >
   >O caractere apóstrofo (&#39;) não é permitido em endereços de email.

1. Escolha uma opção Função para atribuir uma função ao usuário.

   Consulte Funções e privilégios [de usuário do](administration-setup.md#user_administration)Dynamic Media Classic.

1. Selecione um nome de empresa para adicionar um usuário a uma empresa.
1. Se desejar adicionar o usuário a um grupo (se estiver adicionando um usuário ou contribuidor do Portal de mídia), clique em Avançar e adicione o usuário.
1. Clique em Salvar para concluir a configuração do usuário.

   Depois de salvar, um prompt perguntará se você deseja adicionar um usuário a outra empresa. Clique em Adicionar se desejar adicionar o usuário a uma empresa.

   Todos os novos usuários recebem uma senha gerada aleatoriamente; os usuários devem alterar as senhas na primeira vez que fizerem logon no Dynamic Media Classic.

   Os novos usuários recebem um email de boas-vindas após adicioná-los. O e-mail fornece uma senha temporária e explica como fazer logon no Scene 7 Publishing System.

   Se o usuário não receber o email de boas-vindas, vá para a página de logon do Dynamic Media Classic (https://s7sps1.scene7.com) e clique em Esqueci minha senha. A senha é redefinida e um novo email é enviado. Se o usuário não receber o email e ele não estiver na pasta Lixo eletrônico, entre em contato com o Suporte Técnico.

   Ao adicionar novos usuários do Media Portal, você também pode ir até Configuração > Configuração do aplicativo > Administração do usuário, clicar em Carregar Lista do usuário e selecionar um arquivo .csv que contenha no máximo 500 usuários.

### Excluindo um usuário {#deleting-a-user}

Você pode excluir usuários do Dynamic Media Classic tornando-os inválidos. Usuários inválidos são removidos do sistema e de todas as contas.

1. Clique em **Configuração** > Configuração **** do aplicativo > Configuração **** administrativa > Administração **** do usuário.
1. Selecione um usuário na lista e clique em **Editar**.
1. Desmarque Válido.
1. Clique em **Salvar**.

### Ativar ou desativar usuários {#activating-or-deactivating-users}

Os usuários que foram desativados não têm mais permissão para entrar na conta listada na parte superior do menu Selecionar contas para acessar.

1. Clique em **Configuração** > Configuração **** do aplicativo > Configuração **** administrativa > Administração **** do usuário.
1. Na lista do usuário, selecione ou desmarque a opção Ativa ao lado do nome do usuário.

### Editar informações do usuário {#editing-user-information}

As informações de usuário que você pode editar dependem de sua função de administrador e da função atribuída ao usuário cujas informações você deseja editar. As opções que estão esmaecidas (indisponíveis) não são editáveis.

1. Vá até **Configuração** > Configuração **do aplicativo**> Configuração **** administrativa > Administração **** do usuário.
1. Selecione o usuário e clique em **Editar**.
1. Selecione a entrada na tabela que mostra a empresa para a qual você está tentando modificar permissões ou acesso e clique no link Gerenciar Empresa.
1. Selecione a função do usuário.
1. Se desejar alterar a associação de grupo do usuário (se você estiver editando ou adicionando um usuário ou contribuidor do Portal de mídia), clique em Avançar e edite a associação de grupo.
1. Clique em **Salvar**.

### Filtragem e classificação da lista do usuário {#filtering-and-sorting-the-user-list}

Você pode filtrar e classificar a lista do usuário para localizar usuários. Todos os usuários em todas as contas que você administra são exibidos na lista Usuários, independentemente da conta selecionada no menu Selecionar conta para acesso.

Você pode usar as seguintes técnicas de filtragem de lista do usuário:

**Filtrar por grupo** Selecione o menu Por grupo e escolha uma opção para restringir a lista aos usuários em um grupo.

**Filtrar por função** de usuário Selecione o menu Por função de usuário e escolha uma opção para restringir a lista a usuários ou administradores de tipos diferentes.

**Filtrar por nome** de campo Selecione a opção Ativar filtro por campo. Em seguida, selecione o menu Por nome de campo, escolha uma coluna para filtrar a lista, selecione o menu Filtrar caractere e escolha uma letra. A lista é filtrada em uma das colunas pela letra escolhida. Desmarque a opção Ativar filtro por campo para ver a lista completa.

**Filtrar usuários** inválidos Desmarque a opção Incluir inválidos. Os resultados da pesquisa exibem somente os usuários que estão no sistema. Usuários inválidos foram excluídos do sistema e das contas que você administra.

**Classificar por cabeçalho** de coluna Clique em um cabeçalho para classificar todos os usuários por status, em ordem alfabética por nome, sobrenome ou email, por função de usuário ou por status válido/inválido.

Se você tiver muitos usuários, poderá limitar o tamanho da lista selecionando o menu Tamanho máximo da Lista e escolhendo um número.

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

    * To launch Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, click **Solutions** &gt; **Experience Manager**. Under the Dynamic Media Classic card, click **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Largura de banda e Armazenamento {#bandwidth-storage}

Os administradores do Dynamic Media Classic podem gerar largura de banda, armazenamento e outros tipos de relatórios para as empresas que administram. Esses relatórios estão disponíveis na tela Largura de banda e Armazenamento.

Para abrir essa tela, clique em Configuração > Configuração pessoal. Expanda Instalação da administração e clique em Largura de banda e Armazenamento.

### Tipos de relatórios {#types-of-reports}

A tabela a seguir descreve os relatórios que podem ser gerados na tela Largura de banda e Armazenamento:

| Relatório | Informações | Use |
|:--- |:--- |:--- |
| Largura de banda | Uso da largura de banda por empresa | Rastreie o uso da largura de banda por empresa em intervalos de datas específicos para determinar os padrões de tráfego. |
| Armazenamento | uso do armazenamento | Rastreie a quantidade de dados carregada pela empresa. |
| Conteúdo da imagem | O número de solicitações de imagem por tipo | Rastreie o número de solicitações e o volume de diferentes tipos de imagem. |
| Domínio | O número de solicitações de URL por domínio | Rastrear o uso da imagem com base no domínio da solicitação de imagem para uma empresa específica. (O Dynamic Media Classic pode fornecer mais de um domínio por conta. Para obter mais informações, entre em contato com o Suporte Técnico.) |
| Streaming de vídeo | Uso de largura de banda para transmissão de vídeo | Rastreie o uso de vídeo de fluxo contínuo por empresa em intervalos de datas específicos para determinar os padrões de tráfego. |
| Conteúdo do vídeo | Tempo de reprodução de vídeos diferentes | Determine quais são os vídeos mais exibidos e menos exibidos. |


O relatório de Conteúdo de imagem fornece informações sobre solicitações para os seguintes tipos de imagem:

**Solicitações** de imagem para imagens.

**Solicitações** de miniatura para imagens de amostra ou alternativas em visualizadores.

**Solicitação** de máscara para imagens que retornam máscaras em escala de cinza.

**Solicitações de Imagem de solicitação** de mosaico do visualizador carregadas por um visualizador.

**Solicitação** de imagem de objeto Vnt que retornam uma imagem com objetos especificados nas vinhetas solicitadas.

**Solicitação** de Imagem de Solicitação de Informações de Vnt que retornam informações sobre as vinhetas solicitadas.

>[!NOTE]
>
>O relatório de transmissão de vídeo se aplica somente aos vídeos de transmissão. Ele não rastreia a visualização de vídeos progressivos.

### Gerando um relatório {#generating-a-report}

Para gerar uma largura de banda, armazenamento, conteúdo de imagem, domínio, streaming de vídeo ou relatório de conteúdo de vídeo:

1. Escolha Configuração > Configuração pessoal.
1. Expanda Instalação da administração e clique em Largura de banda e Armazenamento.
1. Clique em uma guia: Largura de banda, Armazenamento, Conteúdo de imagem, Domínio, Streaming de vídeo ou Conteúdo de vídeo.

   Consulte [Tipos de relatórios](administration-setup.md#types_of_reports).

### Exibição de dados de diferentes maneiras {#viewing-data-in-different-ways}

Depois de gerar um relatório na página Largura de banda e Armazenamento, você pode escolher opções para exibir informações. Você pode escolher como as informações são apresentadas, as informações de visualização em um gráfico ou grade de dados e especificar um período de tempo para capturar as informações. Na visualização de dados, também é possível classificar informações e reorganizar colunas.

**Exibição de dados em um gráfico ou grade** de dados Clique na opção Visualização do gráfico para visualização de dados em um gráfico; clique na opção Visualização de dados para visualização de dados em uma grade de dados.

**Escolhendo um tipo** de apresentação de relatório No menu Tipo de relatório, escolha Resumo, Diário ou Mensal para organizar os dados no formulário de resumo, por dia ou por mês. Nem todos os relatórios fornecem essa opção.

**Especificação de um período** Escolha opções para definir um período de tempo para o relatório e clique em Atualizar depois de definir um período de tempo:

**Período** de tempo predefinido No menu Relatório predefinido, escolha uma opção. Por exemplo, escolha Último mês para capturar dados do mês anterior.

**Período** de tempo personalizado No menu Relatório predefinido, escolha Personalizado. Em seguida, escolha uma data no menu Mês do Start (ou Data do Start) e uma data no menu # de Meses (ou # ou Dias). Para Relatórios de conteúdo de domínio e vídeo, você pode escolher um start específico e uma data de término para capturar informações do relatório.

**Classificação de dados (somente visualização de dados)** Para classificar informações em uma coluna, clique no cabeçalho da coluna. Clique novamente para classificar em ordem decrescente.

**Reorganização de colunas (somente visualização de dados)** Para mover uma coluna para um local diferente na grade de dados, arraste o cabeçalho.

### Exportar e imprimir relatórios {#exporting-and-printing-reports}

Depois de gerar um relatório, você pode exportar seus dados para uso em planilhas e outros aplicativos. Também é possível imprimir relatórios.

**Exportar dados** do relatório Na visualização de dados, classifique e organize os dados conforme necessário. Em seguida, abra o menu Exportar e escolha um formato: Delimitado por tabulação, Separado por vírgula ou Formatado por HTML. Os dados são copiados para a Área de transferência no formato escolhido. Agora é possível colar os dados em uma planilha ou aplicativo.

**Imprimindo um relatório** Clique em Imprimir, escolha as opções desejadas na caixa de diálogo Imprimir e clique em OK.

## Erros de imagem {#image-errors}

Os administradores do Dynamic Media Classic podem gerar relatórios de erro de imagem. Um relatório de Erro de imagem fornece uma lista dos 20 erros de imagem mais frequentes, nas últimas 24 horas, para a empresa à qual você está conectado no momento. Siga estas etapas para gerar um relatório de Erro de imagem:

1. Clique em Configuração > Configuração pessoal.
1. Expanda a Configuração de administração e clique em Erros de imagem.
1. (Opcional) Execute um dos procedimentos a seguir:

   * Clique em um cabeçalho para classificar erros pelas informações do cabeçalho. Por padrão, os erros são classificados por número de ocorrências, de mais alto a mais baixo.
   * Mova o cursor sobre o campo Resposta para ver uma mensagem de erro específica.
   * Mova o cursor sobre o campo URL ou o campo Quem indicou para ver o link para a página da Web da imagem ou quem indicou.
   * Clique em URL Copiar URL para copiar o link para a imagem real. Você pode colar esse link em uma janela do navegador para ir até a imagem e investigar o erro.
   * Clique em URL de cópia de Quem indicou para copiar o link para a página da quem indicou.

Os erros exibidos são para a empresa na qual você está conectado no momento. Cada erro inclui as seguintes informações:

**ID** da imagem para a imagem que está causando a ofensa.

**Hora** O intervalo de tempo da primeira vez que o erro foi relatado para a última vez que o erro foi relatado, nas últimas 24 horas.

**Contagem** O número de erros reportados na imagem.

**Resposta** A mensagem de erro específica. Os erros são 4xx ou 5xx.

**URLs** Lista o URL para a imagem no Scene 7.

**Quem indicou** Especifica o URL do site de onde a solicitação inicial veio. A quem indicou pode ser qualquer site que tenha um link para a imagem.

As colunas URL e Quem indicou têm o URL Copiar associado a elas para simplificar os testes.
