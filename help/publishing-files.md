---
title: Publicar arquivos
description: '"Saiba como publicar ativos nos Servidores de imagem da Dynamic Media. Você pode publicar ativos de uma só vez ou organizar o Adobe Dynamic Media Classic para publicar ativos em uma programação recorrente. Após a publicação dos ativos, eles ficam disponíveis para entrega. Você pode copiar as chamadas de URL do Adobe Dynamic Media Classic e adicioná-las ao seu site ou aplicativo."'
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '1678'
ht-degree: 0%

---

# Publicar arquivos{#publishing-files}

Você publica os ativos nos Servidores de imagem da Dynamic Media. Você pode publicar ativos de uma só vez ou organizar o Adobe Dynamic Media Classic para publicar ativos em uma programação recorrente. Após a publicação dos ativos, eles ficam disponíveis para entrega. Você pode copiar as chamadas de URL do Adobe Dynamic Media Classic e adicioná-las ao seu site ou aplicativo.

O Adobe Dynamic Media Classic agora é compatível com a entrega de todas as imagens e vídeos por HTTP/2. Ou seja, um URL publicado ou código incorporado para a imagem ou vídeo está disponível para ser integrado a qualquer aplicativo que aceite um ativo hospedado. Esse ativo publicado é então entregue por meio do protocolo HTTP/2. Esse método de entrega melhora a maneira como os navegadores e servidores se comunicam, permitindo uma melhor resposta e tempos de carregamento de todos os seus ativos Adobe Dynamic Media Classic. Consulte [Perguntas frequentes sobre entrega de conteúdo HTTP2](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic).

## Publicar após o upload {#publish-after-uploading}

Ativos em um estado publicado ou não. Por padrão, todos os ativos carregados no Adobe Dynamic Media Classic são marcados automaticamente para publicação.

Para obter mais informações, consulte o [Aviso de publicação instantânea PDF](/help/assets/rendering-instant-publish-notification.pdf).

Use essas técnicas para marcar ativos para publicação:

* **[!UICONTROL Publish After Uploading]** - Na página Upload , próximo à parte inferior, selecione  **[!UICONTROL Publish After Uploading]**. O padrão é um estado selecionado.

* **[!UICONTROL Publish After Uploading]** - Na caixa de diálogo Opções de trabalho, selecione  **[!UICONTROL Publish After Uploading]**. O padrão é um estado selecionado.

Alguns ativos &quot;secundários&quot; são marcados automaticamente para publicação quando seus pais são marcados para publicação. Esta tabela lista os ativos secundários marcados para publicação automática.

| Item pai (grupo) | Itens filho (membro) |
| --- | --- |
| Conjuntos de imagens | Imagens dentro do conjunto. |
| Conjuntos de amostras | Amostras dentro do conjunto. |
| Conjuntos de rotação | Imagens dentro do conjunto. |
| Modelos | Arquivos de modelo, páginas e imagens. |

Imagens derivadas também são marcadas automaticamente para publicação quando suas imagens pai estão sendo publicadas. As imagens derivadas incluem imagens que você ajustou com as opções de edição de imagens. Você pode ver essas imagens derivadas na Exibição de detalhes em Construir e derivados.

## Criar um trabalho de publicação {#creating-a-publish-job}

Crie um trabalho de publicação para publicar ativos que você carregou nos servidores do Adobe Dynamic Media Classic, mas ainda não deseja publicá-los automaticamente. Você pode executar um trabalho de publicação único ou agendar trabalhos para recorrerem regularmente. O Adobe Dynamic Media Classic oferece opções de publicação avançadas para servidores específicos e opções para republicação de ativos que já foram publicados.

**Para criar um trabalho de publicação:**

1. Na barra Navegação global, selecione **[!UICONTROL Publish]**.
1. Na caixa de diálogo Publicar , escolha se deseja um trabalho de publicação único ou recorrente.

   Consulte [Criar um trabalho de publicação único](publishing-files.md#creating_a_one_time_publish_job) e [Criar um trabalho de publicação recorrente](publishing-files.md#creating_a_recurring_publish_job).

1. Insira um nome de trabalho.
1. Opcionalmente, exiba as opções Avançadas e escolha essas opções.

   Consulte [Opções de publicação avançadas](publishing-files.md#advanced_publish_options).

1. Selecione **[!UICONTROL Submit Publish]**.

O Adobe Dynamic Media Classic acompanha trabalhos de publicação na página Trabalhos . Você pode revisar os trabalhos de publicação nessa página.

>[!NOTE]
>
>Os ativos que você republica (você os publicou antes) não aparecem imediatamente no seu site devido ao mecanismo de armazenamento em cache da Web na rede de entrega de conteúdo (CDN). Consulte [Ativos republicados e atrasos de CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Criar um trabalho de publicação único {#creating-a-one-time-publish-job}

Crie um trabalho de publicação único selecionando a opção **[!UICONTROL One-Time]** na página Publicar .

Se desejar que o trabalho de publicação ocorra posteriormente, na página Publicar , selecione **[!UICONTROL One-Time]** e selecione **[!UICONTROL Schedule For Later]** lista suspensa. Use o Calendário e o controle deslizante Tempo para selecionar um dia e hora para executar o trabalho de publicação.

### Criar um trabalho de publicação recorrente {#creating-a-recurring-publish-job}

Crie um trabalho de publicação recorrente selecionando **[!UICONTROL Recurring]** na página Publicar .

Em seguida, escolha uma opção Repetir de **[!UICONTROL Daily]**, **[!UICONTROL Weekly]**, **[!UICONTROL Monthly]** ou **[!UICONTROL Custom]** e especifique quando deseja que o trabalho de publicação ocorra novamente. O Adobe Dynamic Media Classic apresenta ferramentas de calendário para agendar o trabalho de publicação recorrente. Você pode selecionar a opção **[!UICONTROL Custom]** e inserir uma regra no campo de texto Regra para descrever um intervalo de trabalho personalizado.

Consulte [Criar um intervalo de tempo de trabalho de upload ou publicação personalizado](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Os trabalhos recorrentes de publicação (e upload) são listados na página Trabalhos . Você pode editar ou excluir um trabalho agendado indo até a guia Agendado da página Trabalhos .

### Opções de publicação avançadas {#advanced-publish-options}

Você pode exibir as opções Avançadas na página Publicar e escolher essas opções para lidar com um trabalho de publicação:

* **[!UICONTROL Publish To]** - Para publicar ativos somente em um servidor específico, escolha um tipo de servidor.

* **[!UICONTROL Publish]** - Por padrão, o Adobe Dynamic Media Classic publica apenas ativos que são novos e não foram publicados antes (a opção Novo desde a última publicação ). No entanto, você pode selecionar **[!UICONTROL Full Publish]** para também publicar ativos que foram atualizados ou alterados desde a última publicação. Selecione **[!UICONTROL Full w/ Search Data]** se estiver publicando um eCatalog e quiser que os leitores possam pesquisá-lo por palavra-chave.

* **[!UICONTROL Run Job As]** - Escolha um nome de usuário na lista. Você pode classificar tarefas por nome de usuário na página Trabalhos . Ao escolher um nome, você associa um trabalho de publicação a um usuário.

**[!UICONTROL HTTP Notification]** - Insira um URL para acionar trabalhos de publicação subsequentes.

Consulte [Usar um trabalho de upload ou publicação como um acionador](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Cancelar um trabalho de publicação {#canceling-a-publish-job}

Você pode cancelar um trabalho de publicação em andamento. Além disso, se você for um administrador, poderá cancelar um trabalho de publicação em andamento na página Trabalhos da empresa.

Para cancelar um trabalho de publicação, vá para a página Trabalhos e selecione **[!UICONTROL Cancel]**. Na guia Agendado da página Trabalhos , é possível pausar ou retomar um trabalho ao desmarcar ou marcar a caixa de seleção na coluna Ativo do trabalho.

>[!NOTE]
>
>Após cancelar um trabalho de publicação, seu status é alterado para &quot;parar&quot; até que o trabalho chegue a um ponto em que possa parar com segurança. A interrupção de um trabalho de publicação pode demorar um pouco se o trabalho estiver em processo de obter dados do banco de dados.

## Publicar ativos manualmente {#manually-publishing-assets}

Você pode publicar ativos individuais manualmente em vez de criar um trabalho de publicação. Ao publicar conjuntos, como um Conjunto de imagens ou um Conjunto de vídeos adaptáveis, o conjunto (ou &quot;pai&quot;) e todos os membros (ou &quot;filhos&quot;) desse conjunto são publicados.

Os ativos não publicados são indicados na interface do usuário por um ícone cinza e redondo com uma barra sobre ele (estado não publicado), à esquerda do nome do ativo. Depois que um ativo é publicado, o ícone fica verde e tem uma marca de seleção branca no centro (estado publicado).

**Para publicar ativos manualmente:**

1. Siga um destes procedimentos:

   * Na Exibição de Grade, Exibição de Lista ou Exibição de Detalhes, use os métodos padrão de seleção de arquivo para selecionar um ou mais ativos não publicados.

      Na Barra de Navegação Global, vá para **[!UICONTROL File]** > **[!UICONTROL Publish]**.

   * Na Exibição de grade, Exibição de lista ou Exibição de detalhes, selecione o ícone cinza, arredondado com uma barra à esquerda do nome do ativo.

## Cancelar a publicação manual de ativos {#manually-unpublishing-assets}

Você pode cancelar a publicação de ativos individuais manualmente. Ao cancelar a publicação de conjuntos, como um Conjunto de amostras ou um eCatalog, o próprio conjunto (ou &quot;pai&quot;) entrará em um estado não publicado. No entanto, os membros (ou &quot;filhos&quot;) desse conjunto não são afetados; em vez disso, cada um mantém seu estado publicado ou não publicado.

Os ativos publicados são indicados na interface do usuário por um ícone redondo, verde com uma marca de seleção branca no centro (estado publicado), à esquerda do nome do ativo. Após a publicação de um ativo, o ícone fica cinza com uma barra (estado não publicado),

**Para cancelar a publicação manual de ativos:**

1. Siga um destes procedimentos:

   * Na Exibição de Grade, Exibição de Lista ou Exibição de Detalhes, selecione um ou mais ativos publicados.

      Na Barra de Navegação Global, vá para **[!UICONTROL File]** > **[!UICONTROL Unpublish]**.

   * Na Exibição de grade, Exibição de lista ou Exibição de detalhes, selecione o ícone de marca de seleção arredondado e verde à esquerda do nome do ativo.

## Obter o histórico de publicação de um ativo {#getting-an-asset-s-publish-history}

A última data em que um ativo foi publicado é mostrada na Exibição de detalhes na parte superior do painel. Para obter mais detalhes sobre o histórico de publicação, abra o painel Histórico e Servidores Publicados na Exibição de Detalhes. A partir daí, é possível ver quando o ativo foi publicado e para quais servidores ele foi publicado.

## Ativos republicados e atrasos de CDN {#republished-assets-and-cdn-delays}

Os ativos do Adobe Dynamic Media Classic são distribuídos na rede de entrega de conteúdo (CDN). A CDN é um sistema de servidores de computador em rede que cooperam de forma transparente para fornecer conteúdo, especialmente conteúdo de mídia grande, aos usuários finais. No sistema CDN, o conteúdo da Web é armazenado em caches da Web pela Internet (chamada de rede de cache de borda). O conteúdo da Web é entregue dos caches da Web para os usuários finais para fazer deliveries mais rápidos.

Na primeira vez que alguém baixa uma página da Web, os ativos são entregues a um servidor de cache da Web CDN. Eles são armazenados neste servidor para que na próxima vez que alguém na mesma área acessar a página da Web, o mesmo conteúdo em cache possa ser entregue mais rápido. O conteúdo é entregue mais rápido porque está localizado mais próximo do usuário final. O CDN possibilita exibições de página da Web mais rápidas. Ele reduz as demandas de largura de banda no servidor central porque o conteúdo é fornecido da rede de cache de borda, não de um servidor central em cada instância.

O conteúdo do Adobe Dynamic Media Classic recém-publicado está disponível imediatamente para o usuário final e preenche rapidamente a rede de cache de borda. No entanto, o conteúdo recém-republicado, imagens que têm exatamente os mesmos nomes das imagens publicadas anteriormente em um servidor de imagem, não é atualizado no CDN por até dez horas. Em vez disso, os usuários finais veem o que está em um cache da Web na rede CDN. Por isso, seus ativos republicados do Adobe Dynamic Media Classic não aparecem para os usuários finais por dez horas.

Se quiser que seus ativos de imagem recém-republicados estejam disponíveis antes do atraso de dez horas, é possível liberar caches da Web no CDN. A liberação desses caches da Web remove o conteúdo antigo dos caches da Web CDN e o substitui pelos ativos publicados mais recentemente.

Para liberar o cache, na barra Navegação global, vá para **[!UICONTROL File]** > **[!UICONTROL Invalidate CDN]**. Todos os arquivos selecionados são removidos do cache. Se não houver ativos publicáveis ou se você não for um administrador da empresa, a opção Remover da CDN não estará disponível.

>[!MORELIKETHIS]
>
>* [Verificar arquivos de trabalho](checking-job-files.md)
>* [Editar, excluir, pausar e retomar tarefas recorrentes](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

