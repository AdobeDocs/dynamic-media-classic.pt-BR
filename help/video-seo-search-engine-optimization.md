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
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 0%

---

# SEO de vídeo (Otimização do mecanismo de pesquisa){#video-seo-search-engine-optimization}

SEO é o processo de melhorar o volume de tráfego para um site a partir de mecanismos de pesquisa. Enquanto os mecanismos de pesquisa se excitam na coleta de informações sobre o conteúdo baseado em texto, eles não podem adquirir informações adequadamente sobre o vídeo, a menos que essas informações sejam fornecidas a eles.

Usando o SEO de vídeo do Dynamic Media Classic, você pode aplicar metadados de vídeo para fornecer aos mecanismos de pesquisa descrições de seus vídeos. O Dynamic Media Classic oferece a capacidade de criar mapas de site de vídeo e feeds de mRSS. Esses arquivos XML padrão são usados para enviar informações de vídeo para mecanismos de pesquisa:

* **Mapa do site de vídeo**  - Informa o Google exatamente onde e qual é o conteúdo do vídeo em um site. Assim, os vídeos são totalmente pesquisáveis no Google. Por exemplo, um Mapa do site de vídeo pode especificar o tempo de execução e as categorias de vídeos. Para obter informações sobre os mapas do site de vídeo, consulte [Mapas do site de vídeo e alternativas do mapa do site de vídeo](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **Feed**  mRSS (Media realmente Simple Syndication) - Usado por editores de conteúdo para alimentar arquivos de mídia no Yahoo! Pesquisa de vídeo. Para obter informações sobre feeds mRSS, consulte [Mapas de site de vídeo e alternativas de mapa de site de vídeo](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>O Google oferece suporte ao Mapa do Site de Vídeo e ao protocolo de feed de RSS para enviar informações para mecanismos de pesquisa.

O Dynamic Media Classic pode gerar mapas de sites de vídeo e feeds de mRSS de metadados armazenados com cada vídeo. Ao criar mapas do site de vídeo e feeds de mRSS, você decide quais campos de metadados dos arquivos de vídeo devem ser incluídos. Dessa forma, você descreve seus vídeos para mecanismos de pesquisa, de modo que os mecanismos de pesquisa possam direcionar o tráfego para vídeos em seu site com mais precisão

>[!NOTE]
>
>Antes de criar um mapa do site de vídeo ou feed mRSS, descubra quais campos o mecanismo de pesquisa requer no arquivo XML e como estruturar esses campos. Para criar um mapa do site de vídeo ou feed mRSS bem-sucedido, ele deve atender aos requisitos do mecanismo de pesquisa.

O Dynamic Media Classic cria relatórios sobre mapas de site de vídeo e feeds de mRSS depois que você os gera. Esses relatórios estão disponíveis na página Relatório de SEO de Vídeo .

>[!NOTE]
>
>Para os feeds do Site de Vídeo e do mRSS, o Dynamic Media Classic captura metadados somente de vídeos que estão marcados para publicação. Marque vídeos para publicação para incluir seus metadados em Mapas de vídeo e feeds de mRSS.

## Escolha das configurações de SEO do vídeo {#choosing-video-seo-settings}

Clique em Configurações de SEO de vídeo para obter os mapas de site de vídeo e os feeds de mRSS na página **[!UICONTROL Video Search Engine Optimization Settings]**. Para abrir esta página, na barra Navegação global, clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Settings]**.

Na área **[!UICONTROL General Setting]**, escolha se deseja gerar mapas do Site de Vídeo, feeds de RSS ou ambos. Na área **[!UICONTROL Generation Settings]**, mapeie os campos de metadados para campos de entrada.

Depois de escolher as configurações, clique em **[!UICONTROL Save]** (ou **[!UICONTROL Save & Generate]**) para criar o Mapa do Site de Vídeo, os feeds de RSS ou ambos.

### Como escolher configurações gerais {#choosing-general-settings}

Na lista suspensa **[!UICONTROL Generation Mode]**, escolha um modo de relatório:

* **Mapa do site de vídeo**  - Criar um mapa do site de vídeo.

* **Feed mRSS**  - Crie um feed RSS de mídia (mRSS).

* **Ambos**  - Crie ambos os tipos de arquivos XML.

* **Off**  - Para parar de gerar os feeds de Sitemaps de vídeo e RSS de mídia (mRSS), escolha essa opção.

Na lista suspensa **[!UICONTROL Automatic/Manual Mode]**, escolha se deseja gerar automaticamente ou manualmente:

* **Modo automático**  - O Dynamic Media Classic gera automaticamente um mapa do site de vídeo, um feed RSS de mídia (mRSS) ou ambos, a cada dia. Escolha a opção Marcar para publicação para marcar automaticamente para publicar o arquivo XML gerado pelo Dynamic Media Classic.

   * **Marque para** PublicarMarcas para publicar o arquivo XML gerado.

* **Modo manual**  - O Dynamic Media Classic gera o Mapa do site de vídeo, o RSS da mídia (mRSS) ou ambos, quando você clica em Gerar ou Salvar e gerar na tela Configurações de otimização da pesquisa de vídeo. Escolha também essas opções:

   * **Sem mais configurações**  - Não marca para publicar o arquivo XML gerado.

   * **Marcar para publicar**  - Marca para publicar o arquivo XML gerado.

   * **Permitir geração parcial**  - os mecanismos de pesquisa podem rejeitar um arquivo XML se ele não contiver informações completas de metadados para todos os vídeos. Essa opção gera o arquivo XML mesmo se os metadados não estiverem disponíveis para alguns vídeos. Um aviso é registrado na tela Relatório. Escolha essa opção se deseja exportar o arquivo XML e processar as informações ausentes manualmente.

### Escolhendo Configurações de Geração {#choosing-generation-settings}

A área Configurações de geração lista os campos de entrada do Mapa do Site de Vídeo, ou feed de RSS, ou ambos, e no painel Metadados, os nomes dos campos de metadados. Use a área Configurações gerais para mapear campos de entrada para campos de metadados. Ao fazer isso, você informa ao Dynamic Media Classic onde obter metadados para o Mapa do Site de Vídeo e/ou feed mRSS.

1. No menu Visualizações de metadados, escolha uma visualização de metadados. Após escolher uma exibição, os nomes dos campos de metadados são exibidos no painel Metadados.
Consulte [Visualizações de metadados](application-setup.md#metadata_views).
1. Arraste os nomes dos campos de metadados do painel Metadados para os campos de entrada Página inicial, Título, Descrição, Tags e Categoria . Os campos Página de aterrissagem, Título e Descrição são obrigatórios.

   >[!NOTE]
   >
   >Também é possível inserir dados manualmente nos campos de entrada.

1. Siga um destes procedimentos:

   * Para salvar suas configurações sem gerar o arquivo XML, clique em **[!UICONTROL Save]**.
   * Para salvar e gerar o arquivo, clique em **[!UICONTROL Save & Generate]**.

      O arquivo XML é gerado e registrado no log Trabalho. Os arquivos do Mapa do site de vídeo (video-sitemap) e de um feed RSS de mídia (mRSS) (mrss-feed) são armazenados na pasta raiz da sua empresa.

>[!NOTE]
>
>Publique o Mapa do Site de Vídeo ou o feed do mRSS antes de enviá-lo para os mecanismos de pesquisa. Os arquivos de feed do Mapa do Site de Vídeo e do RSS do Media (mRSS) são armazenados na pasta raiz da empresa. Marque esses arquivos XML para publicação, se necessário, e clique em **[!UICONTROL Publish]**.

## Envio de arquivos de Sitemap de vídeo e Feed de RSS para mecanismos de pesquisa {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Os arquivos de feed do Mapa do Site de Vídeo e do RSS do Media (mRSS) são armazenados na pasta raiz da empresa:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copie um desses URLs nas ferramentas do webmaster do mecanismo de pesquisa para enviar seu arquivo de feed Video Sitemap ou Media RSS (mRSS) para mecanismos de pesquisa.

## Exibição de relatórios de SEO de vídeo {#viewing-video-seo-reports}

Visualize relatórios de SEO de vídeo na página Relatório de otimização do mecanismo de pesquisa de vídeo . Para abrir esta página, na barra Navegação global, clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Reports]**.

Se ocorreram erros quando um relatório foi gerado, eles são listados na página Relatório .
