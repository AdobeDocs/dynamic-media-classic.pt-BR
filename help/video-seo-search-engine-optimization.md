---
title: SEO de vídeo (Otimização do mecanismo de pesquisa)
seo-title: SEO de vídeo (Otimização do mecanismo de pesquisa)
description: 'null'
seo-description: Saiba como configurar as configurações de SEO de vídeo.
uuid: bac 2 c 6 a 9-8466-4 b 8 f-b 835-6 cb 0 b 4168513
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/configuração
discoiquuid: 34 asu 868-775 f -452 b-b 26 e-d 139 f 0 e 280 ae
translation-type: tm+mt
source-git-commit: de7d2608f94935f238a11d8310b97dddc5476f57

---


# SEO de vídeo (Otimização do mecanismo de pesquisa){#video-seo-search-engine-optimization}

A SEO é o processo de aprimoramento do volume do tráfego para um site a partir de mecanismos de pesquisa. Embora os mecanismos de pesquisa excel sejam coletados na coleta de informações sobre conteúdo baseado em texto, eles não podem adquirir informações sobre o vídeo adequadamente, a menos que essas informações sejam fornecidas a eles.

Usando o Dynamic Media Classic SEO, você pode aproveitar os metadados de vídeo para fornecer mecanismos de pesquisa com descrições de seus vídeos. O Dynamic Media Classic fornece a capacidade de criar mapas do site de vídeo e feeds de mrss. Estes são arquivos XML padrão para enviar informações de vídeo para mecanismos de pesquisa:

**O Mapa do Sitemap** informa exatamente onde e qual conteúdo de vídeo está em um site. Consequentemente, os vídeos podem ser completamente pesquisados no Google. Por exemplo, um Mapa do site de vídeo pode especificar o tempo de execução e categorias de vídeos. Para obter informações sobre mapas do site, consulte https://www.google.com/support/webmasters/bin/answer.py?answer=80471.

**Feed de mrss (Mídia simples de mídia)** usado pelos editores de conteúdo para feed de arquivos de mídia para o Yahoo! Pesquisa de vídeo. Para obter informações sobre feeds de mrss, consulte https://www.rssboard.org/media-rss.

>[!NOTE]
>
>O Google suporta o protocolo de feed do Sitemap e o protocolo de feed mrss para enviar informações para mecanismos de pesquisa.

O Dynamic Media Classic pode gerar mapas do site de vídeo e feeds de mrss de metadados armazenados com cada vídeo. Ao criar mapas do site de vídeo e feeds de mrss, você decide quais campos de metadados serão incluídos nos arquivos de vídeo. Dessa forma, você descreve seus vídeos em mecanismos de pesquisa para que os mecanismos de pesquisa possam direcionar o tráfego com precisão para vídeos em seu site

>[!NOTE]
>
>Antes de criar um feed do site de vídeo ou de mrss, descubra quais campos o mecanismo de pesquisa requer no arquivo XML e como estruturar esses campos. Para criar um feed de vídeo com êxito ou feed de mrss, ele deve atender às exigências do mecanismo de pesquisa.

O Dynamic Media Classic cria relatórios sobre mapas do site de vídeo e feeds de mrss depois de gerá-los. Esses relatórios estão disponíveis na tela Relatório de SEO de vídeo.

>[!NOTE]
>
>Para os feeds do site de vídeo e os feeds de mrss, o Dynamic Media Classic captura somente metadados de vídeos marcados para publicação. Marque vídeos para publicar para incluir seus metadados nos mapas do site e nos feeds de mrss.

## Como escolher configurações de SEO de vídeo {#choosing-video-seo-settings}

Escolha Configurações de SEO de vídeo para mapas do site de vídeo e feeds de mrss na tela Configurações de otimização do mecanismo de pesquisa do vídeo. Para abrir esta tela, escolha Configuração &gt; Configuração do aplicativo &gt; SEO &gt; Configurações.

Na área Configuração geral, escolha se deseja gerar Mapas do site do vídeo, feeds de mrss ou ambos. Na área Configurações de geração, mapeie campos de metadados para campos de entrada.

Depois de escolher configurações, clique em Gerar (ou Salvar e gerar) para criar o Mapa do site de vídeo, os feeds de mrss ou ambos.

### Como escolher configurações gerais {#choosing-general-settings}

Na lista suspensa Modo de geração, escolha um modo de relatório:

**Criação de um** mapa do site do vídeo do Sitemap.

**Feed de feed mrss** Criar um feed RSS (mrss).

**** Ambos criam ambos os tipos de arquivos XML.

**Desativar** escolha esta opção para parar a geração de mapas do site de vídeo e de um feed RSS (mrss).

Na lista suspensa Modo Automático/Manual, escolha se será gerado automaticamente ou manualmente:

**O modo** automático Media Media Classic gera automaticamente um feed do Video Sitemap, feed RSS (mrss) ou ambos os dias. Escolha a opção Marcar para publicar para marcar automaticamente a publicação do arquivo XML gerado pelo Dynamic Media Classic.

**O Modo** manual Media Media Classic gera o feed do Video Sitemap, RSS de mídia (mrss) ou ambos, quando você clica em Gerar ou Salvar e gerar na tela Configurações de otimização de pesquisa do vídeo. Escolha estas opções também:

**Nenhuma configuração** não indica para publicar o arquivo XML gerado.

**Marca para Exportar** marcas para publicar o arquivo XML gerado.

**Permitir mecanismos** de pesquisa de geração parcial pode rejeitar um arquivo XML se não contiver informações completas de metadados para todos os vídeos. Essa opção gera o arquivo XML mesmo que os metadados não estejam disponíveis para alguns vídeos. Um aviso é registrado na tela Relatório. Escolha essa opção se pretende exportar o arquivo XML e processar as informações ausentes manualmente.

### Escolher configurações de geração {#choosing-generation-settings}

A área de Configurações de geração lista campos de entrada para o feed de Video Sitemap e/ou mrss, e no painel Metadados, os nomes dos campos de metadados. Use a área Configurações gerais para mapear campos de entrada para campos de metadados. Ao fazer isso, você diz o Dynamic Media Classic onde obter metadados para o feed do Sitemap Vídeo e/ou mrss.

1. No menu Exibições de metadados, escolha uma exibição de metadados. Depois de escolher uma exibição, os nomes dos campos de metadados aparecem no painel Metadados. (Para obter informações sobre exibições de metadados, consulte [Exibições de metadados](application-setup.md#metadata_views).)
1. Arraste os nomes de campo de metadados do painel Metadados para os campos de entrada de página inicial, Título, Descrição, Tags e Categoria. Os campos Página inicial, Título e Descrição são obrigatórios.

   >[!NOTE]
   >
   >Você também pode inserir manualmente dados nos campos de entrada.

1. Clique em Salvar (para salvar as configurações sem gerar o arquivo XML), Gerar (para gerar o arquivo XML) ou Salvar e gerar (para salvar e gerar o arquivo).

   O arquivo XML é gerado e registrado no log de trabalho. Arquivos de vídeo do mapa de vídeo (do site do vídeo) e de um feed RSS (mrss) de mídia (mrss) são armazenados na pasta raiz de sua empresa.

>[!NOTE]
>
>Você deve publicar o feed do Sitemap ou o feed mrss antes de enviá-lo para mecanismos de pesquisa. Os arquivos de feed de vídeo do Sitemap e RSS (mrss) são armazenados na pasta raiz da empresa. Marque esses arquivos XML para publicação, se necessário, e clique em Publicar.

## Envio de arquivos do Sitemap de vídeo e de intervalos de feed para mecanismos de pesquisa {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Os arquivos de feed de vídeo do Sitemap e RSS (mrss) são armazenados na pasta raiz da empresa:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copie um desses urls nas ferramentas webmestre do mecanismo de pesquisa para enviar o arquivo de feed do Sitemap ou RSS (mrss) de vídeo para mecanismos de pesquisa.

## Exibindo relatórios de SEO de vídeo {#viewing-video-seo-reports}

Exiba relatórios de SEO de vídeo na tela Relatório de otimização do mecanismo de pesquisa de vídeo. Para abrir esta tela, clique em Configuração &gt; Configuração do aplicativo &gt; SEO &gt; Relatórios.

Se os erros ocorreram quando um relatório foi gerado, eles são listados na tela Relatório.
