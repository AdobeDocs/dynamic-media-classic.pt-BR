---
title: 'Publicação de arquivos '
seo-title: 'Publicação de arquivos '
description: nulo
seo-description: Saiba como publicar arquivos.
uuid: cdcf519b-4c1e-430b-b43a-2f20f75071b1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 39099bc0-9228-46f0-9bee-3542059f4695
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1657'
ht-degree: 0%

---


# Publicação de arquivos {#publishing-files}

Você publica seus ativos em Dynamic Media Image Servers. Você pode publicar ativos de uma só vez ou fazer com que o Dynamic Media Classic publique ativos em uma programação recorrente. Depois que seus ativos forem publicados, eles estarão disponíveis para você para delivery. Você pode copiar as chamadas de URL do Dynamic Media Classic e adicioná-las ao seu site ou aplicativo.

O Dynamic Media Classic agora oferece suporte ao delivery de todas as imagens e vídeos por HTTP/2. Ou seja, um URL publicado ou um código incorporado para a imagem ou o vídeo está disponível para ser integrado a qualquer aplicativo que aceite um ativo hospedado. Esse ativo publicado é então entregue por meio do protocolo HTTP/2. Este método de delivery melhora a maneira como os navegadores e servidores se comunicam, permitindo uma melhor resposta e tempos de carregamento de todos os seus ativos do Dynamic Media Classic. Consulte [Delivery HTTP2 de Perguntas frequentes sobre conteúdo](https://docs.adobe.com/content/docs/en/aem/6-2/administer/integration/marketing-cloud/scene7/http2faq.html).

## Publicar após carregar {#publish-after-uploading}

Ativos em um estado publicado ou não publicado. Por padrão, todos os ativos carregados no Dynamic Media Classic são marcados automaticamente para publicação.

Para obter mais informações, consulte o [Aviso de publicação instantânea PDF](/help/assets/rendering-instant-publish-notification.pdf).

Use estas técnicas para marcar ativos para publicação:

* **Publicar após**
uploadNa página Carregar, perto da parte inferior, selecione Publicar após upload. O padrão é um estado selecionado.

* **Publicar após**
uploadNa caixa de diálogo Opções de trabalho, selecione Publicar após upload. O padrão é um estado selecionado.

Alguns ativos &quot;filho&quot; são marcados automaticamente para publicação quando seus pais são marcados para publicação. Esta tabela lista ativos secundários marcados para publicação automaticamente.

| Item pai (grupo) | Itens filho (membro) |
|--- |--- |
| Conjuntos de imagens | Imagens dentro do conjunto. |
| Conjuntos de amostras | Amostras dentro do conjunto. |
| Conjuntos de rotação | Imagens dentro do conjunto. |
| Modelos | Arquivos de modelo, páginas e imagens. |

As imagens derivadas também são marcadas automaticamente para publicação quando suas imagens pai estão sendo publicadas. As imagens derivadas incluem imagens ajustadas com opções de edição de imagens. Você pode ver essas imagens derivadas na visualização Detalhe em Construir e derivados.

## Criando um trabalho de publicação {#creating-a-publish-job}

Crie um trabalho de publicação para publicar ativos que você carregou nos servidores Dynamic Media Classic, mas optou por não publicá-los automaticamente ainda. Você pode executar tarefas de publicação única ou programar tarefas para que possam ser repetidas regularmente. Opções avançadas de publicação do Dynamic Media Classic oferta para publicação em servidores específicos e opções para republicação de ativos que já foram publicados.

**Para criar um trabalho de publicação**

1. Na barra Navegação global, clique em **Publicar**.
1. Na caixa de diálogo Publicar, escolha se deseja um trabalho de publicação único ou recorrente.

   Consulte [Criação de um trabalho de publicação única](publishing-files.md#creating_a_one_time_publish_job) e [Criação de um trabalho de publicação recorrente](publishing-files.md#creating_a_recurring_publish_job).

1. Insira um nome de tarefa.
1. Opcionalmente, exiba as opções Avançadas e escolha essas opções.

   Consulte [Opções avançadas de publicação](publishing-files.md#advanced_publish_options).

1. Clique em **Enviar publicação**.

O Dynamic Media Classic acompanha os trabalhos de publicação na página Tarefas. Você pode revisar trabalhos de publicação nessa página.

>[!NOTE]
>
>Os ativos que você publicar novamente (você já os publicou antes) não aparecem imediatamente em seu site devido ao mecanismo de armazenamento em cache da Web na rede de delivery de conteúdo (CDN). Consulte [Ativos republicados e atrasos CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Criando um trabalho de publicação única {#creating-a-one-time-publish-job}

Crie um trabalho de publicação única selecionando a opção Uma vez na página Publicar.

Se desejar que a tarefa de publicação ocorra em uma data posterior, selecione o menu Quando e escolha Agendar para mais tarde. Em seguida, use o controle deslizante Calendário e Hora para selecionar um dia e hora para executar o trabalho de publicação.

### Criando um trabalho de publicação recorrente {#creating-a-recurring-publish-job}

Crie um trabalho de publicação recorrente selecionando a opção Recorrente na página Publicar.

Em seguida, escolha uma opção Repetir (Diário, Semanal, Mensal ou Personalizado) para declarar quando deseja que o trabalho de publicação seja repetido. O Dynamic Media Classic apresenta ferramentas de calendário para agendar o trabalho de publicação recorrente. Você pode escolher a opção Personalizado e inserir uma regra na caixa Regra para descrever um intervalo de trabalho personalizado.

Consulte [Criação de um carregamento personalizado ou um intervalo de tempo de trabalho de publicação](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Os trabalhos recorrentes de publicação (e upload) são listados na página Tarefas. Você pode editar ou excluir um trabalho programado indo até a guia Agendado da página Tarefas.

### Opções de publicação avançadas {#advanced-publish-options}

Você pode exibir as opções avançadas na página Publicar e escolher estas opções para lidar com um trabalho de publicação:

* **Publicar**
paraEscolha um tipo de servidor para publicar ativos somente em um servidor específico, não em todos os servidores.

* ****
PublicarPor padrão, o Dynamic Media Classic publica somente ativos que são novos e não foram publicados antes (a opção Nova desde a última publicação). No entanto, você pode escolher Publicação completa para também publicar ativos que foram atualizados ou alterados desde a última publicação. Escolha Completo com Dados de pesquisa se você estiver publicando um eCatalog e quiser que os leitores possam pesquisá-lo por palavra-chave.

* **Executar trabalho**
comoEscolha um nome de usuário na lista. Você pode classificar trabalhos por nome de usuário na página Tarefas. Ao escolher um nome, você associa um trabalho de publicação a um usuário.

**Notificação**
HTTPnsira um URL para acionar trabalhos de publicação subsequentes.

Consulte [Usar um trabalho de upload ou publicação como um acionador](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Cancelando um trabalho de publicação {#canceling-a-publish-job}

Você pode cancelar um trabalho de publicação em andamento. Além disso, se você for um administrador, poderá cancelar um trabalho de publicação em andamento na página Tarefas de empresa.

Para cancelar um trabalho de publicação, vá para a página Tarefas e clique em Cancelar. Na guia Agendado da página Tarefas, você pode pausar ou retomar uma tarefa desmarcando ou desmarcando a caixa de seleção na coluna Ativo da ordem de produção.

>[!NOTE]
>
>Depois que você cancela um trabalho de publicação, seu status muda para &quot;parar&quot; até que o trabalho chegue a um ponto em que possa parar com segurança. Parar um trabalho de publicação pode levar algum tempo se o trabalho estiver no processo de obter dados do banco de dados.

## Publicar manualmente ativos {#manually-publishing-assets}

Você pode publicar ativos individuais manualmente em vez de criar um trabalho de publicação. Quando você publica conjuntos, como um Conjunto de imagens ou um Conjunto de vídeos adaptáveis, o conjunto (ou &quot;pai&quot;) e todos os membros (ou &quot;filhos&quot;) dentro desse conjunto são publicados.

Os ativos não publicados são indicados na interface do usuário por um ícone cinza e redondo com uma barra sobre ele (estado não publicado), à esquerda do nome do ativo. Depois que um ativo é publicado, o ícone fica verde e tem uma marca de seleção branca no centro (estado publicado).

**Para publicar ativos manualmente**

1. Execute um dos procedimentos a seguir:

   * Na Visualização de grade, Visualização de Lista ou Visualização de detalhes, use os métodos padrão de seleção de arquivos para selecionar um ou mais ativos não publicados.

      Na barra de navegação global, clique em **Arquivo > Publicar**.

   * Na Visualização Grade, na Visualização de Lista ou na Visualização Detalhes, clique no ícone cinza, redondo com uma barra sobre ele, à esquerda do nome do ativo.

## Cancelar a publicação manual de ativos {#manually-unpublishing-assets}

Você pode cancelar a publicação de ativos individuais manualmente. Quando você cancela a publicação de conjuntos, como um Conjunto de amostras ou um eCatalog, o próprio conjunto (ou &quot;pai&quot;) entra em um estado não publicado. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um deles mantém seu estado publicado ou não publicado.

Os ativos publicados são indicados na interface do usuário por um ícone redondo e verde com uma marca de seleção branca no centro (estado publicado), à esquerda do nome do ativo. Depois que um ativo não é publicado, o ícone fica cinza com uma barra nele (estado não publicado),

**Para cancelar a publicação manual de ativos**

1. Execute um dos procedimentos a seguir:

   * Na Visualização de grade, Visualização de Lista ou Detalhes, selecione um ou mais ativos publicados.

      Na barra de navegação global, clique em **Arquivo > **Cancelar a publicação**.

   * Na Visualização de grade, na Visualização de Lista ou na Visualização Detalhes, clique no ícone de marca de seleção redonda e verde à esquerda do nome do ativo.

## Obter o histórico de publicação de um ativo {#getting-an-asset-s-publish-history}

A última data em que um ativo foi publicado é mostrada na visualização Detalhe na parte superior do painel. Você pode obter mais detalhes sobre o histórico de publicação abrindo o painel Histórico e servidores publicados em visualização de detalhes. Daí, você pode ver quando o ativo foi publicado e para quais servidores ele foi publicado.

## Ativos republicados e atrasos de CDN {#republished-assets-and-cdn-delays}

Os ativos do Dynamic Media Classic são distribuídos na rede de delivery de conteúdo (CDN). O CDN é um sistema de servidores de computador em rede que cooperam de forma transparente para fornecer conteúdo, especialmente conteúdo de mídia grande, aos usuários finais. No sistema CDN, o conteúdo da Web é armazenado em caches da Web pela Internet (chamado de rede de cache de borda). O conteúdo da Web é disponibilizado desses caches da Web para usuários finais para delivery mais rápidos.

Na primeira vez que alguém baixa uma página da Web, os ativos são entregues a um servidor de cache da Web CDN. Eles são armazenados neste servidor para que na próxima vez que alguém na mesma área acessar a página da Web, o mesmo conteúdo em cache possa ser entregue mais rapidamente. O conteúdo é disponibilizado mais rapidamente porque está localizado mais perto do usuário final. A CDN permite exibições de página da Web mais rápidas. Diminui as demandas de largura de banda no servidor central porque o conteúdo é fornecido da rede de cache de borda, não de um servidor central em cada instância.

O conteúdo recém-publicado do Dynamic Media Classic está disponível imediatamente para o usuário final e preenche rapidamente a rede de cache de borda. No entanto, o conteúdo recém-publicado (imagens com os mesmos nomes das imagens publicadas anteriormente em um servidor de imagens) não é atualizado no CDN por até dez horas. Em vez disso, os usuários finais veem o que está em um cache da Web na rede CDN. Por esse motivo, seus ativos republicados do Dynamic Media Classic podem parecer aos usuários finais por dez horas.

Se você quiser que seus ativos de imagem republicados recentemente estejam disponíveis antes do atraso de dez horas, é possível liberar caches da Web no CDN. A descarga desses caches da Web remove o conteúdo antigo dos caches da Web CDN e o substitui pelos ativos publicados mais recentemente.

Para limpar o cache, clique em Arquivo > Invalidar CDN. Todos os arquivos selecionados são removidos do cache. Se não houver ativos publicáveis, ou se você não for um administrador de empresa, a opção Remover da CDN não estará disponível.

>[!MORELIKETHIS]
>
>* [Verificando arquivos de trabalho](checking-job-files.md)
>* [Editar, excluir, pausar e retomar trabalhos recorrentes](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

