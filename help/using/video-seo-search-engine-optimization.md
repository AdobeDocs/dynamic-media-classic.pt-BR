---
title: SEO em vídeo (otimização do mecanismo de pesquisa)
description: Saiba como definir as configurações de SEO do vídeo no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '983'
ht-degree: 0%

---

# SEO em vídeo (otimização do mecanismo de pesquisa){#video-seo-search-engine-optimization}

SEO é o processo de melhorar o volume de tráfego para um site a partir de mecanismos de pesquisa. Embora os mecanismos de pesquisa se sobressaiam na coleta de informações sobre conteúdo baseado em texto, eles não podem adquirir informações adequadamente sobre vídeos. Essas informações devem ser-lhes fornecidas.

Usando o Adobe Dynamic Media Classic Video SEO, você pode aplicar metadados de vídeo para fornecer aos mecanismos de pesquisa descrições de seus vídeos. O Adobe Dynamic Media Classic oferece a capacidade de criar mapas de site de vídeo e feeds mRSS. Esses arquivos XML padrão são usados para enviar informações de vídeo para mecanismos de pesquisa:

* **Mapa do site de vídeo**: informa ao Google exatamente onde e qual é o conteúdo do vídeo em um site. Assim, os vídeos são totalmente pesquisáveis no Google. Por exemplo, um mapa do site de vídeo pode especificar o tempo de execução e as categorias de vídeos. Para obter informações sobre mapas do site de vídeo, consulte [Mapas de site de vídeo e alternativas de mapas de site de vídeo](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **Feed mRSS (Media Really Simple Syndication)**: usado pelos editores de conteúdo para alimentar arquivos de mídia no Yahoo! Pesquisa de vídeo. Para obter informações sobre feeds mRSS, consulte [Mapas de site de vídeo e alternativas de mapas de site de vídeo](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>O Google é compatível com os protocolos Video Sitemap e feed mRSS para o envio de informações para mecanismos de pesquisa.

O Adobe Dynamic Media Classic pode gerar mapas de site de vídeo e feeds mRSS a partir de metadados armazenados em cada vídeo. Ao criar mapas de site de vídeo e feeds mRSS, você decide quais campos de metadados de arquivos de vídeo incluir. Dessa forma, você descreve os vídeos nos mecanismos de pesquisa para que os mecanismos de pesquisa possam direcionar com mais precisão o tráfego para vídeos no seu site.

>[!NOTE]
>
>Antes de criar um Mapa do site de vídeo ou feed mRSS, descubra quais campos o mecanismo de pesquisa requer no arquivo XML e como estruturá-los. Para criar um Mapa do site de vídeo ou feed mRSS bem-sucedido, ele deve atender aos requisitos do mecanismo de pesquisa.

O Adobe Dynamic Media Classic cria relatórios sobre mapas de site de vídeo e feeds mRSS após gerá-los. Esses relatórios estão disponíveis na página Video SEO Report.

>[!NOTE]
>
>Para os mapas do site de vídeo e feeds mRSS, o Adobe Dynamic Media Classic captura metadados somente de vídeos marcados para publicação. Marque vídeos para publicação para incluir seus metadados em mapas de site de vídeo e feeds mRSS.

## Escolher configurações de SEO de vídeo

Selecione as configurações de SEO do vídeo para mapas do site de vídeo e feeds mRSS na **[!UICONTROL Video Search Engine Optimization Settings]** página. Para abrir esta página, na barra de Navegação global, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Settings]**.

No **[!UICONTROL General Setting]** escolha se deseja gerar mapas de site de vídeo, feeds mRSS ou ambos. No **[!UICONTROL Generation Settings]** , mapeie campos de metadados para campos de entrada.

Depois de escolher as configurações, selecione **[!UICONTROL Save]** (ou **[!UICONTROL Save & Generate]**) para criar o mapa do site de vídeo, os feeds mRSS ou ambos.

### Definir configurações gerais {#choosing-general-settings}

No **[!UICONTROL Generation Mode]** escolha um modo de relatório:

* **Mapa do site de vídeo**: crie um mapa do site de vídeo.

* **Feed mRSS**: crie um feed RSS de mídia (mRSS).

* **Ambos**: crie os dois tipos de arquivos XML.

* **Desligado**: para interromper a geração de mapas do site de vídeo e feeds de RSS de mídia (mRSS), escolha esta opção.

No **[!UICONTROL Automatic/Manual Mode]** escolha entre gerar automática ou manualmente:

* **Modo Automático**: o Adobe Dynamic Media Classic gera automaticamente um mapa do site de vídeo, um feed RSS de mídia (mRSS) ou ambos, todos os dias. Selecione o **[!UICONTROL Mark for Publish]** para que você possa marcar automaticamente para publicação o arquivo XML gerado pelo Adobe Dynamic Media Classic.

   * **Marcar para publicação** Marcas para publicar o arquivo XML gerado.

* **Modo Manual**: o Adobe Dynamic Media Classic gera o mapa do site de vídeo, o feed RSS de mídia (mRSS) ou ambos ao selecionar **[!UICONTROL Generate]** ou **[!UICONTROL Save & Generate]** na tela Configurações de otimização de pesquisa de vídeo. Escolha também estas opções:

   * **Sem mais configurações**: não marca para publicação o arquivo XML gerado.

   * **Marcar para publicação**: marcas para publicar o arquivo XML gerado.

   * **Permitir geração parcial**: os mecanismos de pesquisa podem rejeitar um arquivo XML se ele não contiver informações completas de metadados para todos os vídeos. Essa opção gera o arquivo XML mesmo se os metadados não estiverem disponíveis para alguns vídeos. Um aviso é registrado na tela Relatório. Escolha essa opção se você pretende exportar o arquivo XML e processar as informações ausentes manualmente.

### Escolhendo Configurações de Geração {#choosing-generation-settings}

A área Configurações de geração lista os campos de entrada para o Mapa do site de vídeo, feed mRSS ou ambos. No painel Metadados, os nomes dos campos de metadados são listados. Use a área Configurações gerais para mapear campos de entrada para campos de metadados. Ao fazer isso, você informa à Adobe Dynamic Media Classic onde obter metadados para o Mapa do site de vídeo e/ou feed mRSS.

1. No menu Visualizações de metadados, escolha uma visualização de metadados. Depois de escolher uma visualização, os nomes dos campos de metadados aparecem no painel Metadados.
Consulte [Visualizações de metadados](application-setup.md#metadata_views).
1. Arraste os nomes dos campos de metadados do painel Metadados para os campos de entrada Página inicial, Título, Descrição, Tags e Categoria. Os campos Landing Page, Title e Description são obrigatórios.

   >[!NOTE]
   >
   >Também é possível inserir dados manualmente em campos de entrada.

1. Siga um destes procedimentos:

   * Para salvar as configurações sem gerar o arquivo XML, selecione **[!UICONTROL Save]**.
   * Para salvar e gerar o arquivo, selecione **[!UICONTROL Save & Generate]**.

     O arquivo XML é gerado e registrado no log de tarefas. Os arquivos de mapa do site de vídeo (mapa do site de vídeo) e de feed de Mídia RSS (feed de mrss) são armazenados na pasta raiz da sua empresa.

>[!NOTE]
>
>Publique o Mapa do site em vídeo ou o feed mRSS antes de enviá-lo para os mecanismos de pesquisa. Os arquivos de mapa do site de vídeo e de feed de Mídia RSS (mRSS) são armazenados na pasta raiz da empresa. Marque esses arquivos XML para publicação, se necessário, e selecione **[!UICONTROL Publish]**.

## Enviar arquivos de Mapa do site de vídeo e Feed de RSS por meio de um mecanismo de pesquisa {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Os arquivos de mapa do site de vídeo e de feed de Mídia RSS (mRSS) são armazenados na pasta raiz da empresa:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copie um desses URLs nas ferramentas do webmaster do mecanismo de pesquisa para enviar seu mapa do site de vídeo ou arquivo de feed de Mídia RSS (mRSS) para os mecanismos de pesquisa.

## Exibir relatórios de vídeo SEO {#viewing-video-seo-reports}

Exiba relatórios de SEO de vídeo na página Relatório de otimização do mecanismo de pesquisa de vídeo. Para abrir esta página, na barra de Navegação global, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Reports]**.

Se ocorreram erros quando um relatório foi gerado, eles são listados na página Relatório.
