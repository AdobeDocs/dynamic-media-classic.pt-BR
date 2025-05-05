---
title: Arquivos do Publish
description: Saiba como publicar seus ativos nos servidores de imagem da Dynamic Media.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1626'
ht-degree: 0%

---

# Arquivos do Publish{#publishing-files}

Publique seus ativos nos Dynamic Media Image Servers. Você pode publicar ativos de uma só vez ou combinar o Adobe Dynamic Media Classic para publicar ativos em uma programação recorrente. Após a publicação dos ativos, eles ficam disponíveis para entrega. Você pode copiar as chamadas de URL do Adobe Dynamic Media Classic e adicioná-las ao seu site ou aplicativo.

O Adobe Dynamic Media Classic agora é compatível com o delivery de todas as imagens e vídeos por HTTP/2. Ou seja, um URL publicado ou código incorporado para a imagem ou vídeo está disponível para ser integrado a qualquer aplicativo que aceite um ativo hospedado. Esse ativo publicado usa o protocolo HTTP/2 para entregá-lo. Esse método de entrega melhora a maneira como os navegadores e servidores se comunicam, permitindo melhores tempos de resposta e carregamento de todos os ativos do Adobe Dynamic Media Classic. Consulte as [Perguntas frequentes sobre entrega de conteúdo HTTP2](https://experienceleague.adobe.com/pt-br/docs/experience-manager-65/content/assets/dynamic/http2).

## Publish depois do upload {#publish-after-uploading}

Assets em um estado publicado ou não publicado. Por padrão, todos os ativos carregados na Adobe Dynamic Media Classic são marcados automaticamente para publicação.

Para obter mais informações, consulte o [PDF de Aviso Instantâneo do Publish](/help/using/assets/rendering-instant-publish-notification.pdf).

Use essas técnicas para marcar ativos para publicação:

* **[!UICONTROL Publish After Uploading]**: Na página Upload, próximo à parte inferior, selecione **[!UICONTROL Publish After Uploading]**. O padrão é um estado selecionado.

* **[!UICONTROL Publish After Uploading]**: Na caixa de diálogo Opções de Trabalho, selecione **[!UICONTROL Publish After Uploading]**. O padrão é um estado selecionado.

Alguns ativos &quot;secundários&quot; são marcados automaticamente para publicação quando seus pais são marcados para publicação. Esta tabela lista os ativos filhos marcados para publicação automática.

| Item (de grupo) principal | Itens filhos (membro) |
| --- | --- |
| Conjuntos de imagem | Imagens no conjunto. |
| Conjuntos de amostras | Amostras dentro do conjunto. |
| Conjuntos de rotação | Imagens no conjunto. |
| Modelos | Arquivos de modelo, páginas e imagens. |

As imagens derivadas também são marcadas automaticamente para publicação quando as imagens principais são publicadas. As imagens derivadas incluem imagens ajustadas com opções de edição de imagens. Você pode ver essas imagens derivadas na Exibição de detalhes em Construído e derivados.

## Criar um trabalho de publicação {#creating-a-publish-job}

Crie um trabalho de publicação para publicar ativos carregados nos servidores do Adobe Dynamic Media Classic, mas não deseja que eles sejam publicados automaticamente ainda. Você pode executar um trabalho de publicação único ou agendar trabalhos para que se repitam regularmente. O Adobe Dynamic Media Classic oferece opções avançadas de publicação para publicação em servidores específicos e opções para republicação de ativos que já foram publicados.

**Para criar um trabalho de publicação:**

1. Na barra de Navegação Global, selecione **[!UICONTROL Publish]**.
1. Na caixa de diálogo Publicação, escolha se deseja um trabalho de publicação único ou recorrente.

   Consulte [Criar um trabalho de publicação único](publishing-files.md#creating_a_one_time_publish_job) e [Criar um trabalho de publicação recorrente](publishing-files.md#creating_a_recurring_publish_job).

1. Insira um nome de trabalho.
1. Como opção, exiba as opções Avançadas e escolha essas opções.

   Consulte [Opções de publicação avançadas](publishing-files.md#advanced_publish_options).

1. Selecione **[!UICONTROL Submit Publish]**.

O Adobe Dynamic Media Classic rastreia trabalhos de publicação na página Trabalhos. Você pode revisar os trabalhos de publicação nessa página.

>[!NOTE]
>
>O Assets republicado (publicado antes) não é exibido imediatamente no site devido ao mecanismo de cache da Web na rede de entrega de conteúdo (CDN). Consulte [Ativos republicados e atrasos de CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Criar um trabalho de publicação único {#creating-a-one-time-publish-job}

Crie um trabalho de publicação único selecionando a opção **[!UICONTROL One-Time]** na página Publicação.

Se desejar que o trabalho de publicação ocorra posteriormente, na página Publicação, selecione **[!UICONTROL One-Time]**. Na lista suspensa, selecione **[!UICONTROL Schedule For Later]**. Use o controle deslizante Calendário e Tempo para selecionar um dia e hora para executar o trabalho de publicação.

### Criar um trabalho de publicação recorrente {#creating-a-recurring-publish-job}

Crie um trabalho de publicação recorrente selecionando **[!UICONTROL Recurring]** na página Publicação.

Em seguida, escolha uma opção de Repetição de **[!UICONTROL Daily]**, **[!UICONTROL Weekly]**, **[!UICONTROL Monthly]** ou **[!UICONTROL Custom]** e especifique quando deseja que o trabalho de publicação se repita. O Adobe Dynamic Media Classic apresenta as ferramentas de calendário para agendar o trabalho de publicação recorrente. Você pode selecionar a opção **[!UICONTROL Custom]** e inserir uma regra no campo de texto Regra para descrever um intervalo de trabalho personalizado.

Consulte [Criar um intervalo de tempo de trabalho de carregamento ou publicação personalizado](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Os trabalhos de publicação (e upload) recorrentes são listados na página Trabalhos. Você pode editar ou excluir um job agendado acessando a guia Scheduled da página Jobs.

### Opções de publicação avançadas {#advanced-publish-options}

É possível exibir as opções avançadas na página Publicação e escolher essas opções para manipular um trabalho de publicação:

* **[!UICONTROL Publish To]**: para publicar ativos somente em um servidor específico, escolha um tipo de servidor.

* **[!UICONTROL Publish]**: por padrão, o Adobe Dynamic Media Classic publica somente ativos novos e que não foram publicados antes (a opção Novo desde a última Publish). No entanto, você pode selecionar **[!UICONTROL Full Publish]** para poder publicar ativos que foram atualizados ou alterados desde a última publicação. Selecione **[!UICONTROL Full w/ Search Data]** se estiver publicando um eCatalog e quiser que os leitores possam pesquisá-lo por palavra-chave.

* **[!UICONTROL Run Job As]**: Escolha um nome de usuário na lista. Você pode classificar trabalhos por nome de usuário na página Trabalhos. Ao escolher um nome, você associa um trabalho de publicação a um usuário.

**[!UICONTROL HTTP Notification]**: Insira uma URL para acionar trabalhos de publicação subsequentes.

Consulte [Usar um trabalho de carregamento ou publicação como acionador](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Cancelar um trabalho de publicação {#canceling-a-publish-job}

Você pode cancelar um trabalho de publicação em andamento. Além disso, se você for um administrador, poderá cancelar um trabalho de publicação em andamento na página Trabalhos da empresa.

Para cancelar um trabalho de publicação, vá para a página Trabalhos e selecione **[!UICONTROL Cancel]**. Na guia Programado da página Jobs, você pode pausar ou retomar um job desmarcando ou marcando a caixa de seleção na coluna Ativo do job.

>[!NOTE]
>
>Depois de cancelar um trabalho de publicação, seu status muda para &quot;parando&quot; até que o trabalho atinja um ponto em que possa parar com segurança. A interrupção de um trabalho de publicação pode levar algum tempo se o trabalho estiver no processo de obtenção de dados do banco de dados.

## Ativos do Publish manualmente {#manually-publishing-assets}

Você pode publicar ativos individuais manualmente em vez de criar um trabalho de publicação. Ao publicar conjuntos, como um Conjunto de imagens ou um Conjunto de vídeos adaptados, o conjunto (ou &quot;pai&quot;) e todos os membros (ou &quot;filhos&quot;) dentro desse conjunto são publicados.

Os ativos não publicados são indicados na interface do usuário por um ícone cinza redondo com uma barra (estado não publicado) à esquerda do nome do ativo. Depois que um ativo é publicado, o ícone fica verde e tem uma marca de seleção branca no centro (estado publicado).

**Para publicar ativos manualmente:**

1. Siga um destes procedimentos:

   * Na Exibição em grade, Exibição em lista ou Exibição de detalhes, use os métodos padrão de seleção de arquivos para selecionar um ou mais ativos não publicados.

     Na barra de Navegação Global, vá para **[!UICONTROL File]** > **[!UICONTROL Publish]**.

   * Na Exibição em grade, Exibição em lista ou Exibição de detalhes, selecione o ícone cinza e redondo com uma barra sobre ele, à esquerda do nome do ativo.

## Cancelar a publicação de ativos manualmente {#manually-unpublishing-assets}

Você pode cancelar a publicação de ativos individuais manualmente. Ao cancelar a publicação de conjuntos, como um Conjunto de amostras ou um eCatalog, o conjunto (ou &quot;principal&quot;) entra em um estado não publicado. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Os ativos publicados são indicados na interface do usuário por um ícone verde e redondo com uma marca de seleção branca no centro (estado publicado), à esquerda do nome do ativo. Depois que a publicação de um ativo é desfeita, o ícone fica cinza com uma barra (estado não publicado),

**Para desfazer a publicação manual de ativos:**

1. Siga um destes procedimentos:

   * Na Exibição em grade, Exibição em lista ou Exibição de detalhes, selecione um ou mais ativos publicados.

     Na barra de Navegação Global, vá para **[!UICONTROL File]** > **[!UICONTROL Unpublish]**.

   * Na Exibição em grade, Exibição em lista ou Exibição de detalhes, selecione o ícone de marca de seleção arredondado e verde à esquerda do nome do ativo.

## Obter um histórico de publicação do ativo {#getting-an-asset-s-publish-history}

A última data em que um ativo foi publicado é mostrada na Exibição de detalhes na parte superior do painel. Para obter mais detalhes sobre o histórico de publicação, abra o painel Histórico e Servidores publicados na Exibição de detalhes. A partir daí, você pode ver quando o ativo foi publicado e em quais servidores ele foi publicado.

## Ativos republicados e atrasos de CDN {#republished-assets-and-cdn-delays}

Os ativos do Adobe Dynamic Media Classic são distribuídos na rede de entrega de conteúdo (CDN). O CDN é um sistema de servidores de computador em rede que cooperam de forma transparente para fornecer conteúdo, especialmente conteúdo de mídia grande, aos usuários finais. No sistema CDN, o conteúdo da Web é armazenado em caches da Web na Internet (chamado de rede de cache de borda). O conteúdo da Web é fornecido a partir dos caches da Web para os usuários finais, para entregas mais rápidas.

Na primeira vez que alguém baixa uma página da Web, os ativos são entregues a um servidor de cache da Web CDN. Esse servidor os armazena para que na próxima vez que alguém na mesma área acessar a página da Web, o mesmo conteúdo em cache seja entregue mais rapidamente. O conteúdo é entregue mais rápido porque está localizado mais próximo do usuário final. O CDN possibilita exibições mais rápidas da página da Web. Ele diminui as demandas de largura de banda no servidor central, porque o conteúdo é entregue a partir da rede de cache de borda, não a partir de um servidor central em cada instância.

O conteúdo recém-publicado do Adobe Dynamic Media Classic está disponível imediatamente para o usuário final e preenche rapidamente a rede de cache de borda. No entanto, o conteúdo recém-republicado, ou seja, imagens que têm os mesmos nomes que as imagens publicadas anteriormente em um Servidor de imagens, não é atualizado no CDN por até dez horas. Em vez disso, os usuários finais veem o que está em um cache da Web na rede CDN. Por esse motivo, os ativos republicados do Adobe Dynamic Media Classic não aparecem para os usuários finais por dez horas.

Se quiser que os ativos de imagem recém-publicados estejam disponíveis antes do atraso de dez horas, você poderá liberar caches da Web no CDN. A limpeza desses caches da Web remove o conteúdo antigo dos caches da Web CDN e o substitui pelos ativos publicados mais recentemente.

Para liberar o cache, na barra Navegação Global, vá para **[!UICONTROL File]** > **[!UICONTROL Invalidate CDN]**. Todos os arquivos selecionados são removidos do cache. Se não houver ativos publicáveis ou se você não for um administrador de empresa, a opção Remover do CDN não estará disponível.

>[!MORELIKETHIS]
>
>* [Verificar arquivos do trabalho](checking-job-files.md)
>* [Editar, excluir, pausar e retomar trabalhos recorrentes](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
