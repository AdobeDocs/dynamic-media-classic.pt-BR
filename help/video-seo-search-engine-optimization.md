---
title: SEO de vídeo (Otimização do mecanismo de pesquisa)
description: Saiba como definir as configurações de SEO de vídeo.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Administrator
translation-type: tm+mt
source-git-commit: 3def4a02eda8dc36f2811b3d4f0e870fff1994e4
workflow-type: tm+mt
source-wordcount: '982'
ht-degree: 0%

---


# SEO de vídeo (Otimização do mecanismo de pesquisa){#video-seo-search-engine-optimization}

SEO é o processo de melhorar o volume de tráfego para um site a partir de mecanismos de pesquisa. Enquanto os mecanismos de pesquisa se excitam na coleta de informações sobre o conteúdo baseado em texto, eles não podem adquirir informações adequadamente sobre o vídeo, a menos que essas informações sejam fornecidas a eles.

Usando o SEO de vídeo do Dynamic Media Classic, você pode aplicar metadados de vídeo para fornecer aos mecanismos de pesquisa descrições de seus vídeos. O Dynamic Media Classic oferece a capacidade de criar mapas de site de vídeo e feeds de mRSS. Esses arquivos XML padrão são usados para enviar informações de vídeo para mecanismos de pesquisa:

**Mapa do** site de vídeoInforma o Google exatamente onde e qual conteúdo de vídeo está em um site. Assim, os vídeos são totalmente pesquisáveis no Google. Por exemplo, um Mapa do site de vídeo pode especificar o tempo de execução e as categorias de vídeos. Para obter informações sobre os mapas do site de vídeo, consulte https://www.google.com/support/webmasters/bin/answer.py?answer=80471.

**** Feed mRSS (Media realmente Simple Syndication) usado por editores de conteúdo para alimentar arquivos de mídia no Yahoo! Pesquisa de vídeo. Para obter informações sobre feeds de RSS, consulte https://www.rssboard.org/media-rss.

>[!NOTE]
>
>O Google oferece suporte ao Mapa do Site de Vídeo e ao protocolo de feed de RSS para enviar informações para mecanismos de pesquisa.

O Dynamic Media Classic pode gerar mapas de sites de vídeo e feeds de mRSS de metadados armazenados com cada vídeo. Ao criar mapas do site de vídeo e feeds de mRSS, você decide quais campos de metadados dos arquivos de vídeo devem ser incluídos. Dessa forma, você descreve seus vídeos para mecanismos de pesquisa, de modo que os mecanismos de pesquisa possam direcionar o tráfego para vídeos em seu site com mais precisão

>[!NOTE]
>
>Antes de criar um mapa do site de vídeo ou feed mRSS, descubra quais campos o mecanismo de pesquisa requer no arquivo XML e como estruturar esses campos. Para criar um mapa do site de vídeo ou feed mRSS bem-sucedido, ele deve atender aos requisitos do mecanismo de pesquisa.

O Dynamic Media Classic cria relatórios sobre mapas de site de vídeo e feeds de mRSS depois que você os gera. Esses relatórios estão disponíveis na tela Relatório de SEO de vídeo .

>[!NOTE]
>
>Para os feeds do Site de Vídeo e do mRSS, o Dynamic Media Classic captura metadados somente de vídeos que estão marcados para publicação. Marque vídeos para publicação para incluir seus metadados em Mapas de vídeo e feeds de mRSS.

## Escolher configurações de SEO de vídeo {#choosing-video-seo-settings}

Escolha as configurações de SEO de vídeo para os mapas de site de vídeo e os feeds de mRSS na tela Configurações de otimização do mecanismo de pesquisa de vídeo . Para abrir esta tela, escolha Configuração > Configuração do aplicativo > SEO de vídeo > Configurações.

Na área Configuração geral , escolha se deseja gerar mapas do site de vídeo, feeds de mRSS ou ambos. Na área Configurações de geração , mapeie os campos de metadados para campos de entrada.

Depois de escolher as configurações, clique em Gerar (ou Salvar e gerar) para criar o Mapa do Site de Vídeo, os feeds de RSS ou ambos.

### Como escolher configurações gerais {#choosing-general-settings}

Na lista suspensa Modo de geração , escolha um modo de relatório:

**Mapa do** site de vídeoCriar um mapa do site de vídeo.

**Feed** de RSScriar um feed RSS de mídia (mRSS).

**** Ambos os tipos de arquivos XML.

**** DesativadoPara parar de gerar os feeds de Sitemaps de vídeo e RSS de mídia (mRSS), escolha essa opção.

Na lista suspensa Modo automático/manual , escolha se deseja gerar automaticamente ou manualmente:

**Modo** automáticoO Dynamic Media Classic gera automaticamente um Mapa do Site de Vídeo, feed RSS de mídia (mRSS), ou ambos, a cada dia. Escolha a opção Marcar para publicação para marcar automaticamente para publicar o arquivo XML gerado pelo Dynamic Media Classic.

**** Modo manualO Dynamic Media Classic gera o Mapa do site de vídeo, o feed RSS de mídia (mRSS) ou ambos, quando você clica em Gerar ou Salvar e gerar na tela Configurações de otimização da pesquisa de vídeo. Escolha também essas opções:

**Sem mais** configuraçõesNão marca para publicar o arquivo XML gerado.

**Marque para** PublicarMarcas para publicar o arquivo XML gerado.

**Permitir mecanismos** de pesquisa de geração parcial pode rejeitar um arquivo XML se ele não contiver informações completas de metadados para todos os vídeos. Essa opção gera o arquivo XML mesmo se os metadados não estiverem disponíveis para alguns vídeos. Um aviso é registrado na tela Relatório. Escolha essa opção se deseja exportar o arquivo XML e processar as informações ausentes manualmente.

### Escolhendo Configurações de Geração {#choosing-generation-settings}

A área Configurações de geração lista os campos de entrada do Mapa do Site de Vídeo e/ou feed de RSS e, no painel Metadados, os nomes dos campos de metadados. Use a área Configurações gerais para mapear campos de entrada para campos de metadados. Ao fazer isso, você informa ao Dynamic Media Classic onde obter metadados para o Mapa do Site de Vídeo e/ou feed mRSS.

1. No menu Visualizações de metadados, escolha uma visualização de metadados. Após escolher uma exibição, os nomes dos campos de metadados são exibidos no painel Metadados. (Para obter informações sobre visualizações de metadados, consulte [Visualizações de metadados](application-setup.md#metadata_views).)
1. Arraste os nomes dos campos de metadados do painel Metadados para os campos de entrada Página inicial, Título, Descrição, Tags e Categoria . Os campos Página de aterrissagem, Título e Descrição são obrigatórios.

   >[!NOTE]
   >
   >Também é possível inserir dados manualmente nos campos de entrada.

1. Clique em Salvar (para salvar suas configurações sem gerar o arquivo XML), Gerar (para gerar o arquivo XML) ou Salvar e gerar (para salvar e gerar o arquivo).

   O arquivo XML é gerado e registrado no log Trabalho. Os arquivos do Mapa do site de vídeo (video-sitemap) e de um feed RSS de mídia (mRSS) (mrss-feed) são armazenados na pasta raiz da sua empresa.

>[!NOTE]
>
>Publique o Mapa do Site de Vídeo ou o feed do mRSS antes de enviá-lo para os mecanismos de pesquisa. Os arquivos de feed do Mapa do Site de Vídeo e do RSS do Media (mRSS) são armazenados na pasta raiz da empresa. Marque esses arquivos XML para publicação, se necessário, e clique em Publicar.

## Envio de arquivos do SiteVídeo e do FeedRSS para mecanismos de pesquisa {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Os arquivos de feed do Mapa do Site de Vídeo e do RSS do Media (mRSS) são armazenados na pasta raiz da empresa:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copie um desses URLs nas ferramentas do webmaster do mecanismo de pesquisa para enviar seu arquivo de feed Video Sitemap ou Media RSS (mRSS) para mecanismos de pesquisa.

## Exibição dos relatórios de SEO de vídeo {#viewing-video-seo-reports}

Visualize relatórios de SEO de vídeo na tela Relatório de otimização do mecanismo de pesquisa de vídeo . Para abrir esta tela, clique em Configuração > Configuração do aplicativo > SEO de vídeo > Relatórios.

Se ocorreram erros quando um relatório foi gerado, eles são listados na tela Relatório.
