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
autotag-review: '2026-05-13T20:17:45.884Z'
TQID: 'https://experienceleague.adobe.com/I9wTnanImSLtXv4Nff2uW92cNkMhoGf5hc8cXsPFNYc'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: c2296997-5d79-4905-b32e-99b5aa892429id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
source-git-commit: 66b6e10c324d5b154cd39146b5a129f36aa55622
workflow-type: tm+mt
source-wordcount: 1003
ht-degree: 0%

---

# SEO em vídeo (otimização do mecanismo de pesquisa){#video-seo-search-engine-optimization}

SEO é o processo de melhorar o volume de tráfego para um site a partir de mecanismos de pesquisa. Embora os mecanismos de pesquisa sejam eficientes na coleta de informações sobre o conteúdo baseado em texto, eles não conseguem processar adequadamente as informações sobre o vídeo. Essas informações devem ser-lhes fornecidas.

Para fornecer aos mecanismos de pesquisa descrições de seus vídeos, use o Adobe Dynamic Media Classic Video SEO para aplicar metadados de vídeo. O Adobe Dynamic Media Classic oferece a capacidade de criar mapas de site de vídeo e feeds mRSS. Esses arquivos XML padrão são usados para enviar informações de vídeo para mecanismos de pesquisa:

* **Mapa do site de vídeo**: informa ao Google exatamente onde e qual conteúdo de vídeo está em um site. Os vídeos são totalmente pesquisáveis no Google. Por exemplo, um mapa do site de vídeo pode especificar o tempo de execução e as categorias de vídeos. Para obter informações sobre mapas de site de vídeo, consulte [Mapas de site de vídeo e alternativas de mapas de site de vídeo](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1).

* Feed **mRSS (Media Really Simple Syndication)**: usado pelos editores de conteúdo para alimentar arquivos de mídia no Yahoo! Pesquisa de vídeo. Para obter informações sobre feeds mRSS, consulte [Mapas de site de vídeo e alternativas de mapas de site de vídeo](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1).

>[!NOTE]
>
>O Google é compatível com os protocolos Video Sitemap e feed mRSS para o envio de informações para mecanismos de pesquisa.

O Adobe Dynamic Media Classic pode gerar mapas de site de vídeo e feeds mRSS a partir de metadados armazenados em cada vídeo. Ao criar mapas de site de vídeo e feeds mRSS, você decide quais campos de metadados de arquivos de vídeo incluir. Você descreve os vídeos nos mecanismos de pesquisa para que esses mecanismos possam direcionar o tráfego para vídeos com mais precisão em seu site.

>[!NOTE]
>
>Antes de criar um mapa do site de vídeo ou feed mRSS, determine quais campos o mecanismo de pesquisa requer no arquivo XML e como estruturá-los. Para criar um Mapa do site de vídeo ou feed mRSS bem-sucedido, ele deve atender aos requisitos do mecanismo de pesquisa.

O Adobe Dynamic Media Classic cria relatórios sobre mapas de site de vídeo e feeds mRSS após gerá-los. Esses relatórios estão disponíveis na página Video SEO Report.

>[!NOTE]
>
>Para os mapas do site de vídeo e feeds mRSS, o Adobe Dynamic Media Classic captura metadados somente de vídeos marcados para publicação. Marque vídeos para publicação para incluir seus metadados em mapas de site de vídeo e feeds mRSS.

## Escolher configurações de SEO de vídeo

Selecione as configurações de SEO do vídeo para mapas do site de vídeo e feeds mRSS na página **[!UICONTROL Video Search Engine Optimization Settings]**. Para abrir esta página, na barra de Navegação Global, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Settings]**.

Na área **[!UICONTROL General Setting]**, escolha se deseja gerar mapas de site de vídeo, feeds mRSS ou ambos. Para mapear campos de metadados para campos de entrada, use a área **[!UICONTROL Generation Settings]**.

Depois de escolher as configurações, selecione **[!UICONTROL Save]** (ou **[!UICONTROL Save & Generate]**) para criar o Mapa do Site de Vídeo, os feeds mRSS ou ambos.

### Definir configurações gerais {#choosing-general-settings}

Na lista suspensa **[!UICONTROL Generation Mode]**, escolha um modo de relatório:

* **Mapa do site de vídeo**: crie um mapa do site de vídeo.

* **RSS Feed**: criar um RSS feed de mídia (mRSS).

* **Ambos**: criar ambos os tipos de arquivos XML.

* **Desativado**: para parar de gerar mapas de site de vídeo e feeds RSS de mídia (mRSS), escolha esta opção.

Na lista suspensa **[!UICONTROL Automatic/Manual Mode]**, escolha se deseja gerar automática ou manualmente:

* **Modo Automático**: o Adobe Dynamic Media Classic gera automaticamente um mapa do site de vídeo, um feed RSS de mídia (mRSS) ou ambos, todos os dias. Selecione a opção **[!UICONTROL Mark for Publish]** para marcar os arquivos XML gerados pelo Adobe Dynamic Media Classic para publicação.

  * **Marcar para publicação** Marca para publicação o arquivo XML gerado.

* **Modo Manual**: o Adobe Dynamic Media Classic gera o Mapa do Site de Vídeo, o feed RSS de Mídia (mRSS), ou ambos, quando você seleciona **[!UICONTROL Generate]** ou **[!UICONTROL Save & Generate]** na tela Configurações de Otimização do Mecanismo de Pesquisa de Vídeo. Configure também essas opções:

  * **Nenhuma outra configuração**: não marca para publicação o arquivo XML gerado.

  * **Marcar para publicação**: marcas para publicação do arquivo XML gerado.

  * **Permitir Geração Parcial**: os mecanismos de pesquisa podem rejeitar um arquivo XML se ele não contiver informações completas de metadados para todos os vídeos. Essa opção gera o arquivo XML mesmo se os metadados não estiverem disponíveis para alguns vídeos. Um aviso é registrado na tela Relatório. Escolha essa opção se você pretende exportar o arquivo XML e processar as informações ausentes manualmente.

### Escolhendo Configurações de Geração {#choosing-generation-settings}

A área Configurações de geração lista os campos de entrada para o Mapa do site de vídeo, feed mRSS ou ambos. No painel Metadados, os nomes dos campos de metadados são listados. Use a área Configurações gerais para mapear campos de entrada para campos de metadados. Você configura o Adobe Dynamic Media Classic para obter metadados para o Mapa do site de vídeo e/ou feed mRSS.

1. No menu Visualizações de metadados, escolha uma visualização de metadados. Depois de escolher uma visualização, os nomes dos campos de metadados aparecem no painel Metadados.
Consulte [Exibições de Metadados](application-setup.md#metadata_views).
1. Arraste os nomes dos campos de metadados do painel Metadados para os campos de entrada Página inicial, Título, Descrição, Tags e Categoria. Os campos Landing Page, Title e Description são obrigatórios.

   >[!NOTE]
   >
   >Também é possível inserir dados manualmente em campos de entrada.

1. Siga um destes procedimentos:

   * Para salvar suas configurações sem gerar o arquivo XML, selecione **[!UICONTROL Save]**.
   * Para salvar e gerar o arquivo, selecione **[!UICONTROL Save & Generate]**.

     O arquivo XML é gerado e registrado no log de tarefas. O mapa do site de vídeo (mapa do site de vídeo) e um feed de Mídia RSS (mRSS) (feed de mrss) são armazenados na pasta raiz da sua empresa.

>[!NOTE]
>
>Publique o Mapa do site em vídeo ou o feed mRSS antes de enviá-lo para os mecanismos de pesquisa. Os arquivos de mapa do site de vídeo e de feed de Mídia RSS (mRSS) são armazenados na pasta raiz da empresa. Marque esses arquivos XML para publicação, se necessário, e selecione **[!UICONTROL Publish]**.

## Envie arquivos de Mapa do site de vídeo e Feed mRSS para um mecanismo de pesquisa {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Os arquivos de mapa do site de vídeo e de feed de Mídia RSS (mRSS) são armazenados na pasta raiz da empresa:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Para enviar o mapa do site de vídeo ou o arquivo de feed RSS de mídia (mRSS) para os mecanismos de pesquisa, copie um desses URLs nas ferramentas do webmaster do mecanismo de pesquisa.

## Exibir relatórios de vídeo SEO {#viewing-video-seo-reports}

Exiba relatórios de SEO de vídeo na página Relatório de otimização do mecanismo de pesquisa de vídeo. Para abrir esta página, na barra de Navegação Global, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Reports]**.

Se ocorreram erros quando um relatório foi gerado, eles são listados na página Relatório.
