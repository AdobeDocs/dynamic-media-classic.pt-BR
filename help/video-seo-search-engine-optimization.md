---
title: SEO de vídeo (Otimização do mecanismo de pesquisa)
seo-title: SEO de vídeo (Otimização do mecanismo de pesquisa)
description: nulo
seo-description: Saiba como configurar as configurações de SEO de vídeo.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 0%

---


# SEO de vídeo (Otimização do mecanismo de pesquisa){#video-seo-search-engine-optimization}

SEO é o processo de melhorar o volume de tráfego de mecanismos de pesquisa para um site. Embora os mecanismos de pesquisa se superem ao coletar informações sobre o conteúdo baseado em texto, eles não podem adquirir informações adequadamente sobre o vídeo, a menos que essas informações lhes sejam fornecidas.

Usando o Dynamic Media Classic Video SEO, você pode aproveitar os metadados de vídeo para fornecer aos mecanismos de pesquisa descrições de seus vídeos. O Dynamic Media Classic fornece a capacidade de criar feeds de Sitemaps de vídeo e mRSS. Estes são arquivos XML padrão para enviar informações de vídeo para mecanismos de pesquisa:

**Mapa do site** de vídeo Informa o Google exatamente onde e qual conteúdo de vídeo está em um site. Consequentemente, os vídeos podem ser totalmente pesquisados no Google. Por exemplo, um Mapa do site de vídeo pode especificar o tempo de execução e as categorias dos vídeos. Para obter informações sobre mapas de site de vídeo, consulte https://www.google.com/support/webmasters/bin/answer.py?answer=80471.

**Feed** mRSS (Media Really Simple Syndication) usado por editores de conteúdo para alimentar arquivos de mídia no Yahoo! Pesquisa de vídeo. Para obter informações sobre feeds mRSS, consulte https://www.rssboard.org/media-rss.

>[!NOTE]
>
>O Google suporta o mapa do site de vídeo e o protocolo de feed mRSS para enviar informações aos mecanismos de pesquisa.

O Dynamic Media Classic pode gerar mapas do site de vídeo e feeds mRSS de metadados armazenados com cada vídeo. Ao criar mapas do site de vídeo e feeds mRSS, você decide quais campos de metadados dos arquivos de vídeo devem ser incluídos. Dessa forma, você descreve seus vídeos para mecanismos de pesquisa, de modo que os mecanismos de pesquisa possam direcionar o tráfego para vídeos do site com mais precisão

>[!NOTE]
>
>Antes de criar um mapa do site de vídeo ou feed mRSS, descubra quais campos o mecanismo de pesquisa requer no arquivo XML e como estruturar esses campos. Para criar um mapa do site de vídeo ou feed mRSS bem-sucedido, ele deve atender aos requisitos do mecanismo de pesquisa.

O Dynamic Media Classic cria relatórios sobre os mapas do site de vídeo e os feeds mRSS depois que você os gera. Esses relatórios estão disponíveis na tela Relatório de SEO de Vídeo.

>[!NOTE]
>
>Para os feeds de Sitemaps de vídeo e mRSS, o Dynamic Media Classic captura metadados somente de vídeos que estão marcados para publicação. Marque vídeos para publicação para incluir seus metadados em mapas do site de vídeo e feeds mRSS.

## Seleção das configurações de SEO de vídeo {#choosing-video-seo-settings}

Escolha as configurações de SEO de vídeo para os feeds de Sitemaps de vídeo e mRSS na tela Configurações de otimização do mecanismo de pesquisa de vídeo. Para abrir essa tela, escolha Configuração > Configuração do aplicativo > SEO de vídeo > Configurações.

Na área Configuração geral, escolha se deseja gerar mapas de site de vídeo, feeds mRSS ou ambos. Na área Configurações de geração, mapeie os campos de metadados para os campos de entrada.

Depois de escolher as configurações, clique em Gerar (ou Salvar e gerar) para criar o Mapa do site de vídeo, os feeds mRSS ou ambos.

### Escolhendo Configurações Gerais {#choosing-general-settings}

Na lista suspensa Modo de geração, escolha um modo de relatório:

**Mapa do site** de vídeo Crie um mapa do site de vídeo.

**Feed** mRSS Crie um feed RSS de mídia (mRSS).

**Ambos** criam os dois tipos de arquivos XML.

**Desligado** Escolha esta opção para parar de gerar os mapas do site de vídeo e os feeds RSS de mídia (mRSS).

Na lista suspensa Modo automático/manual, escolha se deseja gerar automática ou manualmente:

**Modo** automático O Dynamic Media Classic gera automaticamente um mapa do site de vídeo, feed RSS de mídia (mRSS) ou ambos, a cada dia. Escolha a opção Marcar para publicação para marcar automaticamente para publicar o arquivo XML gerado pelo Dynamic Media Classic.

**Modo** manual O Dynamic Media Classic gera o mapa do site de vídeo, o feed RSS de mídia (mRSS) ou ambos, quando você clica em Gerar ou Salvar e gerar na tela Configurações de otimização da pesquisa de vídeo. Escolha também estas opções:

**Nenhuma configuração** adicional não marca para publicar o arquivo XML gerado.

**Marcar para Marcas de publicação** para publicar o arquivo XML gerado.

**Permitir mecanismos de pesquisa de geração** parcial pode rejeitar um arquivo XML se ele não contiver informações completas de metadados para todos os vídeos. Essa opção gera o arquivo XML mesmo se os metadados não estiverem disponíveis para alguns vídeos. Um aviso é registrado na tela Relatório. Escolha essa opção se você deseja exportar o arquivo XML e processar as informações ausentes manualmente.

### Escolhendo Configurações de Geração {#choosing-generation-settings}

A área Configurações de geração lista campos de entrada para o mapa do site do vídeo e/ou feed mRSS e, no painel Metadados, os nomes dos campos de metadados. Use a área Configurações gerais para mapear campos de entrada para campos de metadados. Ao fazer isso, você informa ao Dynamic Media Classic onde obter metadados para o mapa do site de vídeo e/ou feed mRSS.

1. No menu Visualizações de metadados, escolha uma visualização de metadados. Depois de escolher uma visualização, os nomes dos campos de metadados são exibidos no painel Metadados. (Para obter informações sobre visualizações de metadados, consulte Visualizações [de metadados](application-setup.md#metadata_views).)
1. Arraste os nomes dos campos de metadados do painel Metadados para os campos de entrada Landing page, Título, Descrição, Tags e Categoria. Os campos Landing page, Título e Descrição são obrigatórios.

   >[!NOTE]
   >
   >Você também pode inserir dados manualmente nos campos de entrada.

1. Clique em Salvar (para salvar suas configurações sem gerar o arquivo XML), Gerar (para gerar o arquivo XML) ou Salvar e gerar (para salvar e gerar o arquivo).

   O arquivo XML é gerado e gravado no log Trabalho. Os arquivos de mapa do site de vídeo (mapa do site de vídeo) e de feed RSS de mídia (mRSS) (mrss-feed) são armazenados na pasta raiz da sua empresa.

>[!NOTE]
>
>Você deve publicar o mapa do site do vídeo ou o feed mRSS antes de enviá-lo para os mecanismos de pesquisa. Os arquivos de feed RSS (mRSS) e do mapa do site de vídeo são armazenados na pasta raiz da empresa. Marque esses arquivos XML para publicação, se necessário, e clique em Publicar.

## Envio de arquivos do mapa do site de vídeo e do feed RSS para mecanismos de pesquisa {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Os arquivos de feed RSS (mRSS) e do mapa do site de vídeo são armazenados na pasta raiz da empresa:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copie um desses URLs nas ferramentas webmaster do mecanismo de pesquisa para enviar o seu arquivo de feed Video Sitemap ou Media RSS (mRSS) para mecanismos de pesquisa.

## Exibição de relatórios de SEO de vídeo {#viewing-video-seo-reports}

Visualização relatórios de SEO de vídeo na tela Relatório de otimização do mecanismo de pesquisa de vídeo. Para abrir essa tela, clique em Configuração > Configuração do aplicativo > SEO de vídeo > Relatórios.

Se ocorreram erros quando um relatório foi gerado, eles são listados na tela Relatório.
