---
title: Configuração de administração
seo-title: Configuração de administração
description: 'null'
seo-description: Saiba como configurar a área de administração do Dynamic Media Classic.
uuid: 16 ba 9 alimentando b 5 c 6-4991-83 b 3-8 d 7 d 7129013 a
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 3 c 9 ee 4 ec-dd 37-498 d -98 d 6-1339 b 80177 ff
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Configuração de administração{#administration-setup}

As telas de Configuração de administração são para administrar usuários do Scene 7 Publishing System. Use essas telas para permitir que os usuários trabalhem no Sistema de publicação Scene 7 e se comuniquem por email com usuários.

1. Para acessar as opções de Configuração de administração, clique **em Configuração** &gt; **Configuração pessoal** &gt; **Configuração de administração**.

## Administração do usuário {#user-administration}

Todos os usuários do Dynamic Media Classic recebem uma função que determina seus privilégios e direitos de acesso aos recursos do Sistema de publicação Scene 7. Os administradores determinam as diferentes funções e responsabilidades das empresas às quais elas são atribuídas.

Normalmente, o Dynamic Media Classic configura o primeiro conjunto de empresas e atribui um administrador da empresa. O administrador da empresa então configura e administra usuários do Scene 7 Publishing System.

O Scene 7 Publishing System oferece suporte a três funções de usuário. As três funções podem acessar empresas configuradas para o Sistema de publicação Scene 7:

**O administrador do SPS** pode exibir e administrar todos os recursos no Sistema de publicação Scene 7, bem como configurar empresas e adicionar administradores e usuários.

**O Administrador da empresa** pode exibir e administrar somente suas próprias empresas. Um administrador da empresa também pode executar todas as funções de administração, incluindo a adição de administradores e usuários. Um administrador de empresa pode adicionar um usuário às contas de administrador da empresa do SPS. (Esta função é a função do usuário padrão.)

**Usuário** do SPS pode acessar empresas às quais elas foram atribuídas; não pode realizar quaisquer tarefas administrativas.

Depois de adicionar um usuário, o Scene 7 Publishing System envia ao usuário uma mensagem de email de boas-vindas. A mensagem inclui uma senha e o URL do sistema de publicação Scene 7.

### Adicionando um usuário ou administrador {#adding-a-user-or-administrator}

1. Clique em Configuração &gt; Configuração do aplicativo &gt; Configuração de administração &gt; Administração do usuário.
1. Clique em Adicionar.
1. Digite o nome e o endereço de e-mail do usuário ou administrador que você deseja adicionar e clique em Avançar.

   >[!NOTE]
   >
   >O caractere apóstrofo (') não é permitido em endereços de email.

1. Escolha uma opção de Função para atribuir uma função ao usuário.

   Consulte [Funções e privilégios do usuário do Dynamic Media Classic](administration-setup.md#user_administration).

1. Selecione um nome de empresa para adicionar um usuário a uma empresa.
1. Se você quiser adicionar o usuário a um grupo (se estiver adicionando um usuário ou colaborador do Media Portal), clique em Avançar e adicione o usuário.
1. Clique em Salvar para concluir a configuração do usuário.

   Depois de salvar, um prompt perguntará se você deseja adicionar um usuário a outra empresa. Clique em Adicionar se desejar adicionar o usuário a uma empresa.

   Todos os novos usuários recebem uma senha gerada aleatoriamente; os usuários devem alterar as senhas na primeira vez que fizerem logon no Sistema de publicação Scene 7.

   Os novos usuários recebem um email de boas-vindas depois de adicioná-los. O email fornece uma senha temporária e explica como fazer logon no Sistema de publicação Scene 7.

   Se o usuário não receber o email de boas-vindas, peça para que vá para a página de logon do SPS (https://s7sps1.scene7.com) e clique em Esqueci minha senha. A senha é redefinida e um novo email é enviado. Se o usuário não receber o e-mail e ele não estiver na pasta Junk, entre em contato com o Suporte técnico.

   Ao adicionar novos usuários do Media Portal, você também pode ir para Configuração &gt; Configuração do aplicativo &gt; Administração do usuário, em seguida, clicar em Carregar lista de usuários e selecionar um arquivo. csv contendo não mais do que 500 usuários.

### Excluir um usuário {#deleting-a-user}

Você pode excluir usuários do Sistema de publicação Scene 7 tornando-os inválidos. Os usuários inválidos são removidos do sistema e de todas as contas.

1. Clique **em Configuração** &gt; **Configuração do aplicativo** &gt; Configuração de administração **** &gt; **Administração do usuário**.
1. Selecione um usuário na lista e clique **em Editar**.
1. Desmarque Válido.
1. Clique **em Salvar**.

### Ativação ou desativação de usuários {#activating-or-deactivating-users}

Os usuários desativados não terão mais permissão para inserir a conta listada na parte superior do menu Selecionar contas para acesso.

1. Clique **em Configuração** &gt; **Configuração do aplicativo** &gt; Configuração de administração **** &gt; **Administração do usuário**.
1. Na lista de usuários, marque ou desmarque a opção Ativa ao lado do nome do usuário.

### Editar informações do usuário {#editing-user-information}

As informações de usuário que podem ser editadas dependem da sua função como administrador e da função atribuída do usuário cujas informações você deseja editar. As opções esmaecidas (indisponíveis) não são editáveis.

1. Vá para **Configuração** &gt; **Configuração do aplicativo**&gt; Configuração de administração **** &gt; **Administração do usuário**.
1. Selecione o usuário e clique **em Editar**.
1. Selecione a entrada na tabela que mostra a empresa que você está tentando modificar permissões ou acesso, em seguida, clique no link Gerenciar empresa.
1. Selecione a função do usuário.
1. Se você quiser alterar a associação de grupo do usuário (se estiver editando ou adicionando um usuário ou colaborador do Media Portal), clique em Avançar e edite a associação de grupo.
1. Clique **em Salvar**.

### Filtragem e classificação da lista de usuários {#filtering-and-sorting-the-user-list}

Você pode filtrar e classificar a lista de usuários para localizar usuários. Todos os usuários em todas as contas que você administra são exibidos na lista Usuários, independentemente da conta selecionada no menu Selecionar conta para acesso.

Você pode usar as seguintes técnicas de filtragem da lista de usuários:

**Filtrar por grupo** Selecione o menu Por grupo e escolha uma opção para restringir a lista aos usuários em um grupo.

**Filtrar por função** do usuário Selecione o menu Função por usuário e escolha uma opção para restringir a lista a usuários ou administradores de tipos diferentes.

**Filtrar por nome de campo** Selecione a opção Ativar filtro por campo. Em seguida, selecione o menu Por campo, escolha uma coluna para filtrar a lista e selecione o menu Filtro de filtro e escolha uma letra. A lista é filtrada em uma das colunas pela letra escolhida. Desmarque a opção Ativar filtro por campo para ver a lista completa.

**Filtrar usuários inválidos** desmarque a opção Incluir inválidos. Os resultados da pesquisa exibem apenas os usuários que estão no sistema. Usuários inválidos foram excluídos do sistema e das contas que você administra.

**Classificar por cabeçalho** da coluna Clique em um cabeçalho para classificar todos os usuários por seu status, alfabeticamente pelo nome, sobrenome ou email, por função do usuário ou por status válido/inválido.

Se você tiver muitos usuários, poderá limitar o tamanho da lista selecionando o menu Tamanho da lista máx. e escolhendo um número.

### Vincular uma identidade de usuário IMS a uma conta de usuário clássica do Dynamic Media {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

Você pode vincular uma identidade de usuário do Adobe IMS a uma conta de usuário clássica do Media Media Classic para que você possa usar SSO (Logon único) para fazer logon e iniciar o Scene 7 Publishing System na Adobe Marketing Cloud.

1. A Adobe já deve ter configurado sua conta com uma organização da Adobe Marketing Cloud e vinculá-la ao seu contexto de produto do Sistema de publicação Scene 7. Se essa configuração ainda não estiver concluída, caso tenha sido feita, entre em contato com o Atendimento ao cliente da Adobe.

   Quando a configuração for concluída, você poderá fazer logon na Adobe Marketing Cloud e vincular sua identidade da Adobe Marketing Cloud à sua conta de usuário clássica do Dynamic Media executando o procedimento a seguir.

1. Na Adobe Marketing Cloud, navegue até suas configurações de conta.
1. Clique **em Gerenciar organizações**.
1. Clique **em Vincular conta** ou **Obter acesso**.
1. Selecione **Experience Manager** e digite suas credenciais.

   Suas credenciais incluem sua região da empresa IPS, endereço de email e senha.

1. Clique **em Link**.
1. Quando o link estiver definido, você poderá iniciar o Scene 7 Publishing System na Adobe Marketing Cloud ou iniciá-lo diretamente.

   Execute um dos procedimentos a seguir:

   * Para iniciar o Dynamic Media Classic na Adobe Marketing Cloud, no trilho esquerdo da Adobe Marketing Cloud, clique **em Soluções** &gt; **Experience Manager**. No cartão Clássico do Media Media, clique **em Iniciar**.
   * Para fazer logon no Sistema de publicação Scene 7 diretamente usando suas credenciais IMS, use o seguinte site:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Substitua «N» no caminho acima pelo número da região de sua empresa IPS. Ou seja, N = 1 para América do Norte; 3 para EMEA; ou 5 para JAPAC.

## Largura de banda e armazenamento {#bandwidth-storage}

Os administradores do SPS podem gerar largura de banda, armazenamento e outros tipos de relatórios para as empresas que eles administram. Esses relatórios estão disponíveis na tela Largura de banda e Armazenamento.

Para abrir esta tela, clique em Configuração &gt; Configuração pessoal. Expanda a Configuração de administração e clique em Largura de banda e armazenamento.

### Tipos de relatórios {#types-of-reports}

A tabela a seguir descreve os relatórios que podem ser gerados na tela Largura de banda e Armazenamento:

| Relatório | Informações | Usar |
|:--- |:--- |:--- |
| Largura de banda | Largura de banda usada por empresa | Rastrear o uso de largura de banda por empresa em intervalos de datas específicos para determinar padrões de tráfego. |
| Armazenamento | Uso de armazenamento | Rastreie a quantidade de dados carregada por empresa. |
| Conteúdo da imagem | O número de solicitações de imagem por tipo | Rastreie o número de solicitações e volume para tipos de imagens diferentes. |
| Domínio | O número de solicitações de URL por domínio | Rastrear o uso de imagem com base no domínio da solicitação de imagem de uma empresa específica. (O Dynamic Media Classic pode fornecer mais de um domínio por conta. Para obter mais informações, entre em contato com o Suporte técnico.) |
| Transmissão de vídeo | Uso de largura de banda para vídeo de transmissão | Rastrear o uso de vídeo de fluxo contínuo por empresa em intervalos de datas específicos para determinar padrões de tráfego. |
| Conteúdo do vídeo | Tempo de reprodução de vídeos diferentes | Determine quais são os vídeos mais visualizados e visualizados. |


O relatório de Conteúdo de imagem fornece informações sobre solicitações para os seguintes tipos de imagem:

**Solicitações de** solicitação de imagem para imagens.

**Solicitações de miniatura** para a amostra ou imagens alternativas nos visualizadores.

**Solicitação de** máscara solicita a imagens retornando máscaras de escala cinza.

**Solicitações** de imagem do visualizador do visualizador carregadas por um visualizador.

**Solicitações de renderização** de Imagem do objeto Vnt que retornam uma imagem com objetos especificados nas vinhetas solicitadas.

**Solicitações de renderização** de imagem Vnt, solicitações de renderização de imagem que retornam informações relacionadas às vinhetas solicitadas.

>[!NOTE]
>
>O relatório de Transmissão de vídeo se aplica somente aos vídeos de transmissão. Ela não rastreia a exibição de vídeos progressivos.

### Geração de um relatório {#generating-a-report}

Para gerar um relatório de largura de banda, armazenamento, conteúdo da imagem, domínio, streaming de vídeo ou conteúdo de vídeo:

1. Escolha Configuração &gt; Configuração pessoal.
1. Expanda a Configuração de administração e clique em Largura de banda e armazenamento.
1. Clique em uma guia: Largura de banda, armazenamento, conteúdo da imagem, domínio, transmissão de vídeo ou conteúdo de vídeo.

   Consulte [Tipos de relatórios](administration-setup.md#types_of_reports).

### Exibição de dados de diferentes formas {#viewing-data-in-different-ways}

Depois de gerar um relatório na página Largura de banda e armazenamento, você pode escolher opções para exibir informações. É possível escolher como as informações são apresentadas, exibir informações em um gráfico ou grade de dados e especificar um período de tempo para capturar as informações. Na exibição de dados, você também pode classificar informações e reorganizar colunas.

**Exibir dados em um gráfico ou grade de dados** clicar na opção Exibição de gráfico para exibir os dados em um gráfico; clique na opção Exibição de dados para exibir os dados em uma grade de dados.

**Escolha um tipo de apresentação de relatório** no menu Tipo de relatório, escolha Resumo, diário ou mensal para organizar os dados no formulário de resumo, por dia ou por mês. Nem todos os relatórios oferecem essa opção.

**Especificar um período de tempo** Escolha Opções para definir um período de tempo para o relatório e clique em Atualizar depois de definir um período de tempo:

**Período predefinido** No menu Relatório pré-definido, escolha uma opção. Por exemplo, escolha Mês passado para capturar dados do mês anterior.

**Período personalizado** No menu Relatório pré-definido, escolha Personalizado. Em seguida, escolha uma data no menu Mês inicial (ou Data inicial) e uma data no menu # of Meses (ou # ou Dias). Para Relatórios de domínio e conteúdo de vídeo, você pode escolher uma data de início e término específico para capturar as informações do relatório.

**Classificação de dados (somente Exibição de dados)** Para classificar informações em uma coluna, clique no cabeçalho da coluna. Clique novamente para classificar em ordem decrescente.

**Reorganização de colunas (somente Exibição de dados)** Para mover uma coluna para um local diferente na grade de dados, arraste seu cabeçalho.

### Exportar e imprimir relatórios {#exporting-and-printing-reports}

Depois de gerar um relatório, você pode exportar seus dados para uso em planilhas e outros aplicativos. Também é possível imprimir relatórios.

**Exportando dados do relatório** na exibição de dados, classifique e organize os dados conforme necessário. Em seguida, abra o menu Exportar e escolha um formato: Delimitado por tabulação, Separado por vírgula ou HTML. Os dados são copiados para a Área de transferência no formato escolhido. Agora é possível colar os dados em uma planilha ou aplicativo.

**Imprimindo um relatório** Clique em Imprimir, escolha as opções desejadas na caixa de diálogo Imprimir e clique em OK.

## Erros de imagem {#image-errors}

Os administradores do SPS podem gerar relatórios de Erro de imagem. Um relatório de Erro de imagem fornece uma lista dos 20 erros de imagem mais frequentes, nas últimas 24 horas, para a empresa na qual você está conectado. Siga estas etapas para gerar um relatório de Erro de imagem:

1. Clique em Configuração &gt; Configuração pessoal.
1. Expanda a Configuração de administração e clique em Erros de imagem.
1. (Opcional) Execute um dos procedimentos a seguir:

   * Clique em um cabeçalho para classificar os erros pelas informações de cabeçalho. Por padrão, os erros são classificados por número de ocorrências, mais alto para o menor.
   * Mova o cursor sobre o campo Resposta para obter um erro para ver a mensagem de erro específica.
   * Mova o cursor sobre o campo URL ou o campo Referenciador para visualizar o link para a imagem ou a página da Web referenciador.
   * Clique em URL Copiar URL para copiar o link para a imagem real. Você pode colar esse link em uma janela do navegador para ir para a imagem e investigar o erro.
   * Clique em Copiar URL de referência para copiar o link para a página da Web referenciador.

Os erros exibidos são para a empresa à qual você está conectado no momento. Cada erro inclui as seguintes informações:

**ID da ID** da imagem para a imagem afetada.

**Hora** O intervalo de tempo da primeira vez que o erro foi relatado na última vez em que o erro foi relatado, nas últimas 24 horas.

**Contabiliza** o número de erros relatados na imagem.

**Resposta** A mensagem de erro específica. Os erros são de 4 xx ou 5 xx.

**Urls** Lista o URL da imagem no Scene 7.

**Referenciador** Especifica o URL do site onde a solicitação inicial veio. O referenciador pode ser qualquer site que tenha um link para a imagem.

As colunas URL e Referenciador têm o URL de cópia associado a eles para simplificar o teste.
