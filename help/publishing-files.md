---
title: Publicação de arquivos
seo-title: Publicação de arquivos
description: 'null'
seo-description: Saiba como publicar arquivos.
uuid: cdcf 519 b -4 c 1 e -430 b-b 43 a -2 f 20 f 75071 b 1
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/upload_ and_ publish_ assets
discoiquuid: 39099 bc 0-9228-46 f 0-9 bee -3542059 f 4695
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Publicação de arquivos{#publishing-files}

Publique seus ativos em Servidores de imagem do Dynamic Media. Você pode publicar ativos de uma só vez ou organizar o Dynamic Media Classic para publicar ativos em uma programação recorrente. Após os ativos serem publicados, eles estarão disponíveis para entrega. Você pode copiar as chamadas de URL do Sistema de publicação Scene 7 e adicioná-las ao seu site ou aplicativo.

O Sistema de publicação Scene 7 agora oferece suporte à entrega de todas as imagens e vídeos em HTTP/2. Ou seja, um URL publicado ou um código incorporado para a imagem ou vídeo está disponível para ser integrado a qualquer aplicativo que aceite um ativo hospedado. Esse ativo publicado é disponibilizado por meio do protocolo HTTP/2. Esse método de entrega melhora a maneira como navegadores e servidores se comunicam, permitindo uma melhor resposta e tempo de carregamento de todos os ativos do Dynamic Media Classic. Consulte [HTTP 2 Delivery of Content Faq](https://docs.adobe.com/content/docs/en/aem/6-2/administer/integration/marketing-cloud/scene7/http2faq.html).

## Publicar após o upload {#publish-after-uploading}

Ativos em um estado publicado ou não publicado. Por padrão, quaisquer ativos carregados no Dynamic Media Classic são marcados automaticamente para publicação.

Para obter mais informações, consulte o [PDF Aviso de publicação instantânea](https://marketing.adobe.com/resources/help/en_US/s7/rendering-instant-publish-notification.pdf).

Use essas técnicas para marcar ativos para publicação:

**Publicar após carregar** na página Carregar, perto da parte inferior, selecione Publicar após o upload. O padrão é um estado selecionado.

**Publicar depois de fazer upload** na caixa de diálogo Opções de trabalho, selecione Publicar após o upload. O padrão é um estado selecionado.

Alguns ativos "filho" são marcados automaticamente para publicação quando seus pais estão marcados para publicação. Esta tabela lista os ativos filho marcados para publicação automaticamente.

| Item pai (grupo) | Itens filho (membro) |
|--- |--- |
| Conjuntos de imagens | Imagens no conjunto. |
| Conjuntos de amostras | Amostras dentro do conjunto. |
| Conjuntos de rotação | Imagens no conjunto. |
| Modelos | Arquivos, páginas e imagens modelo. |

Imagens derivadas também são marcadas automaticamente para publicar quando suas imagens pai estão sendo publicadas. Imagens derivadas incluem imagens que você ajustou com opções de edição de imagens. Você pode ver essas imagens derivadas na exibição Detalhe em Criar e derivados.

## Criação de um trabalho de publicação {#creating-a-publish-job}

Crie um trabalho de publicação para publicar ativos que você carregou nos servidores do Dynamic Media Classic, mas optou por não publicá-los automaticamente. Você pode realizar um trabalho de publicação único ou agendar trabalhos para recorrerem regularmente. O Dynamic Media Classic oferece opções avançadas de publicação para publicação em servidores específicos e opções para republicar ativos que já foram publicados.

**Criação de um trabalho de publicação**

1. Na barra de Navegação global, clique **em Publicar**.
1. Na caixa de diálogo Publicar, escolha se deseja um trabalho de publicação único ou recorrente.

   Consulte [Criar um trabalho de publicação único](publishing-files.md#creating_a_one_time_publish_job) e [Criar um trabalho de publicação recorrente](publishing-files.md#creating_a_recurring_publish_job).

1. Insira um nome de serviço.
1. Opcionalmente, exiba as opções Avançadas e escolha estas opções.

   Consulte [Opções de publicação avançadas](publishing-files.md#advanced_publish_options).

1. Clique **em Enviar publicação**.

O SPS rastreia os trabalhos de publicação na página Tarefas. Você pode revisar os trabalhos de publicação nessa página.

>[!NOTE]
>
>Os ativos que você publicar novamente (já publicados antes) não aparecem imediatamente em seu site devido ao mecanismo de armazenamento em cache na rede de entrega de conteúdo (CDN). Consulte [Ativos republicados e atrasos](publishing-files.md#republished_assets_and_cdn_delays)de CDN.

### Criação de um trabalho de publicação único {#creating-a-one-time-publish-job}

Crie um trabalho de publicação único selecionando a opção Única na página Publicar.

Se desejar que o trabalho de publicação ocorra em uma data posterior, selecione o menu Quando e escolha Programar para mais tarde. Em seguida, use o controle deslizante Calendário e Hora para selecionar um dia e um horário para executar o trabalho de publicação.

### Criação de um trabalho de publicação recorrente {#creating-a-recurring-publish-job}

Crie um trabalho de publicação recorrente selecionando a opção Recorrente na página Publicar.

Em seguida, escolha uma opção Repetir: diário, semanal, mensal ou personalizado— para declarar quando deseja que o trabalho de publicação seja reiniciado. O Dynamic Media Classic apresenta ferramentas de calendário para programar o trabalho de publicação recorrente. Você pode escolher a opção Personalizado e inserir uma regra na caixa Regra para descrever um intervalo de trabalho personalizado.

Consulte [Criar um intervalo de tempo de trabalho ou um intervalo de tempo de trabalho personalizado](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>As tarefas de publicação recorrente (e upload) estão listadas na página Tarefas. Você pode editar ou excluir um trabalho programado, acessando a guia Programada da página Tarefas.

### Opções avançadas de publicação {#advanced-publish-options}

Você pode exibir as opções Avançadas na página Publicar e escolher estas opções para lidar com um trabalho de publicação:

**Publicar para** escolher um tipo de servidor para publicar ativos somente em um servidor específico, e não para todos os servidores.

**Publicar** por padrão, o SPS publica apenas os ativos que são novos e não foram publicados antes (a opção Novo desde a publicação). Entretanto, você pode escolher Publicação completa para publicar também ativos que foram atualizados ou alterados desde a última publicação. Escolha Dados completos w/pesquisar se você estiver publicando um ecatalog e quiser que os leitores possam pesquisá-lo por palavra-chave.

**Executar tarefa como** escolha um nome de usuário na lista. Você pode classificar tarefas por nome de usuário na página Tarefas. Ao escolher um nome, você associará um trabalho de publicação a um usuário.

**Notificação HTTP** Insira um URL para acionar trabalhos de publicação subsequentes.

Consulte [Uso de um upload ou publicação de trabalho como disparador](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).

## Cancelamento de um trabalho de publicação {#canceling-a-publish-job}

Você pode cancelar um trabalho de publicação em andamento. Além disso, se for um administrador, você poderá cancelar uma tarefa de publicação em andamento na página Tarefas da empresa.

Para cancelar um trabalho de publicação, vá para a página Tarefas e clique em Cancelar. Na guia Programada da página Tarefas, você pode pausar ou retomar uma tarefa desmarcando ou marcando a caixa de seleção na coluna Ativo do trabalho.

>[!NOTE]
>
>Depois de cancelar um trabalho de publicação, seu status muda para «parar» até que o trabalho atinja um ponto onde ele possa parar com segurança. Interromper um trabalho de publicação pode levar algum tempo se a tarefa estiver no processo de obtenção de dados do banco de dados.

## Publicar ativos manualmente {#manually-publishing-assets}

Você pode publicar ativos individuais manualmente em vez de criar um trabalho de publicação. Quando você publica conjuntos, como um Conjunto de imagens ou um Conjunto de vídeos adaptativo, o conjunto (ou «pai») e todos os membros (ou «filhos») dentro desse conjunto são publicados.

Os ativos não publicados são indicados na interface do usuário por um ícone cinza, de round com uma barra por meio dele (estado não publicado), à esquerda do nome do ativo. Depois que um ativo é publicado, o ícone fica verde e possui uma marca de seleção branca no centro (estado publicado).

**Para publicar ativos manualmente**

1. Execute um dos procedimentos a seguir:

   * Na Exibição de grade, Exibição de lista ou Exibição de detalhes, use métodos padrão de seleção de arquivo para selecionar um ou mais ativos não publicados.

      Na barra de navegação global, clique **em Arquivo** &gt; **Publicar**.

   * Na Exibição de grade, Exibição de lista ou Exibição de detalhes, clique no ícone cinza, com uma barra por meio dele, à esquerda do nome do ativo.

## Cancelar publicação manual de ativos {#manually-unpublishing-assets}

Você pode cancelar a publicação de ativos individuais manualmente. Quando você cancela a publicação de conjuntos, como um Conjunto de amostras ou um ecatalog, o conjunto (ou «pai») é colocado em um estado não publicado. No entanto, os membros (ou «filhos») dentro desse conjunto não serão afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Os ativos publicados são indicados na interface do usuário por um ícone redondo, verde com uma marca de seleção branca no centro (estado publicado), à esquerda do nome do ativo. Depois que um ativo não é publicado, o ícone fica cinza com uma barra por meio dele (estado não publicado),

**Para cancelar a publicação manual de ativos**

1. Execute um dos procedimentos a seguir:

   * Na Exibição de grade, Exibição de lista ou Exibição de detalhes, selecione um ou mais ativos pubados.

      Na barra de navegação global, clique **em Arquivo** &gt; **Cancelar publicação**.

   * No modo de exibição de grade, exibição de lista ou visualização de detalhes, clique no ícone de marca de seleção arredondada e verde à esquerda do nome do ativo.

## Obtenção do histórico de publicação de um ativo {#getting-an-asset-s-publish-history}

A última data em que um ativo foi publicado é mostrado na exibição Detalhe na parte superior do painel. Você pode obter mais detalhes sobre o histórico de publicação abrindo o painel Histórico e servidores publicados na exibição Detail. Lá, você pode ver quando o ativo foi publicado e para quais servidores ele foi publicado.

## Ativos republicados e atrasos de CDN {#republished-assets-and-cdn-delays}

Os ativos do Dynamic Media Classic são distribuídos na rede de entrega de conteúdo (CDN). CDN é um sistema de servidores de computador netamente cooperativos que cooperam de forma transparente para fornecer conteúdo, especialmente conteúdo de mídia grande, para os usuários finais. No sistema CDN, o conteúdo da Web é armazenado em caches da Web na Internet (chamado rede de cache de borda). O conteúdo da Web é disponibilizado desses caches da Web para que os usuários finais façam entregas mais rápidas.

Na primeira vez em que alguém baixa uma página da Web, os ativos são fornecidos para um servidor de cache da Web CDN. Eles são armazenados nesse servidor para que a próxima vez que alguém na mesma área acessa a página da Web, o mesmo conteúdo em cache pode ser entregue mais rapidamente. O conteúdo é entregue mais rapidamente porque está localizado mais próximo do usuário final. O CDN é exibido para exibições de página mais rápidas. Reduz as demanda de largura de banda no servidor central, pois o conteúdo é disponibilizado a partir da rede do cache da borda, e não de um servidor central em cada instância.

O conteúdo recém publicado do Dynamic Media Classic está disponível imediatamente para o usuário final e preenche rapidamente a rede de cache de borda. No entanto, o conteúdo recém-publicado, imagens que têm exatamente os mesmos nomes que as imagens publicadas anteriormente em um servidor de imagens, não é atualizado no CDN por até dez horas. Em vez disso, os usuários finais veem o que está em um cache da Web na rede CDN. Por isso, os ativos republicados do Dynamic Media Classic podem não ser exibidos para os usuários finais por dez horas.

Se quiser que os ativos de imagem recém-publicados estejam disponíveis antes do atraso de dez horas, você pode piscar caches da Web no CDN. A limpeza desses caches da Web remove conteúdo antigo dos caches da Web CDN e o substitui pelos ativos publicados mais recentemente.

Para esvaziar o cache, clique em Arquivo &gt; Invalidar CDN. Todos os arquivos selecionados são removidos do cache. Se não houver ativos editáveis ou se você não for um administrador da empresa, a opção Remover da CDN não estará disponível.

>[!MORELIKETHIS]
>
>* [Verificação de arquivos de trabalho](checking-job-files.md)
>* [Editar, excluir, pausar e retomar trabalhos recorrentes](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

