---
title: Implantação de vídeo em seus sites e sites móveis
description: Saiba como implantar vídeos em seus sites e sites móveis.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1680'
ht-degree: 2%

---


# Implantação de vídeo em seus sites e sites móveis{#deploying-video-to-your-websites-and-mobile-sites}

Sites, sites móveis e aplicativos de desktop acessam o conteúdo do servidor Dynamic Media Classic, incluindo vídeo, usando strings de URL ou código incorporado. O Dynamic Media Classic ativa essas sequências de caracteres de URL durante o processo de publicação. Para colocar a string de URL ou o código incorporado do seu vídeo em suas páginas da Web, páginas móveis e aplicativos de desktop, copie-o do Dynamic Media Classic.

>[!NOTE]
>
>O URL ou o código incorporado não estará ativo até que você publique o ativo.

## Publicando vídeo {#publishing-video}

A publicação de um vídeo permite que os Dynamic Media Classic Servers forneçam vídeo para seu site, site móvel ou aplicativo.

Existem dois métodos diferentes que você pode usar para publicar vídeo:

* **Publique vídeos automaticamente e instantaneamente ao fazer upload**

   Como parte do processo de upload de vídeo, o Dynamic Media Classic pode publicar vídeos automaticamente quando eles forem carregados e codificados. Essa capacidade de publicar instantaneamente significa que não há necessidade de publicar vídeos separadamente após o fato.

* **Publicar vídeo manualmente após o upload**

   Se você não quiser publicar vídeos imediatamente, poderá publicar os vídeos manualmente a qualquer momento.

Depois de publicar vídeos, o Dynamic Media Classic ativa as sequências de caracteres do URL para sua página HTML ou código do aplicativo.

**Para publicar vídeo**

1. Execute um dos procedimentos a seguir:

   * Para publicar vídeos automaticamente e instantaneamente no upload, na tela Carregar, clique em **Publicar depois de fazer upload**. Você terminou. não há outras etapas a serem concluídas.
   * Para publicar vídeos manualmente após o upload, no Painel de navegação, selecione os vídeos e, na barra Navegação global, clique em **Publicar**.

## Vincular um URL de vídeo a um site móvel ou a um site {#linking-a-video-url-to-a-mobile-site-or-a-website}

Depois de publicar um vídeo, você pode obter o URL para uso em seu site, site móvel ou aplicativo de desktop. Use o URL do vídeo quando quiser exibir o vídeo em uma janela pop-up ou modal na parte superior da página da Web.

Quando um cliente clica no link, o dispositivo, a largura de banda e o tamanho da tela são detectados automaticamente. O vídeo apropriado é exibido para reprodução em um visualizador predefinido para desktop ou no player de vídeo nativo do dispositivo móvel para smartphones e tablets.

Consulte também [Incorporar o visualizador de vídeo em uma página da Web](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Para vincular um URL de vídeo a um site móvel ou a um site**

1. No painel Navegação de ativos, na lista suspensa Mostrar, clique em **Vídeo** ou **Conjunto de vídeos adaptáveis**.
1. no painel Biblioteca de ativos, à esquerda, navegue até a pasta de ativos que contém o vídeo ou o conjunto de vídeos adaptáveis que você deseja vincular.
1. Acima do painel Navegação de ativos, no lado direito da barra de ferramentas, execute um dos procedimentos a seguir:

   * Clique em **Visualização de grade** ou **Visualização de Lista**. No painel Navegação de ativos, clique com o duplo na miniatura de vídeo de um único ativo para abri-lo na Visualização Detalhe. No painel URLs e Código incorporado à direita, em HTTP Streaming, clique em **Copiar URL** à direita do visualizador desejado. Como prática recomendada, copie o URL associado ao visualizador `Universal_HTML5_Video`.
   * Clique em **Visualização de grade**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem em miniatura, clique em **Pré-visualização** > **Lista do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique em **Copiar URL**. Como prática recomendada, copie o URL associado ao visualizador `Universal_HTML5_Video`.

   * Clique em **Visualização de Lista**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, clique em **Pré-visualização** > **Lista do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique em **Copiar URL**. Como prática recomendada, copie o URL associado ao visualizador `Universal_HTML5_Video`.

   * Clique em **Visualização de grade**, **Visualização de Lista** ou **Visualização de detalhes**. Na mesma barra de ferramentas, clique em **Pré-visualização** > **Lista do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique em **Copiar URL**. Como prática recomendada, copie o URL associado ao visualizador `Universal_HTML5_Video`.

1. Cole o link do URL do vídeo HTML5 em seu site e site móvel.

## Incorporação do visualizador de vídeo em uma página da Web {#embedding-the-video-viewer-on-a-web-page}

Use o recurso Incorporar código quando quiser reproduzir o vídeo incorporado na página da Web. Copie o código incorporado na área de transferência para poder colá-lo nuas páginas da Web. A edição do código não é permitida na caixa de diálogo Incorporar código.

Consulte também [Vincular um URL de vídeo a um site móvel ou a um site](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Para incorporar o visualizador de vídeo em uma página da Web**

1. No painel Navegação de ativos, na lista suspensa Mostrar, clique em **Vídeo** ou **Conjunto de vídeos adaptáveis**.
1. no painel Biblioteca de ativos, à esquerda, navegue até a pasta de ativos que contém o vídeo ou o conjunto de vídeos adaptáveis cujo código de incorporação você deseja copiar.
1. Acima do painel Navegação de ativos, no lado direito da barra de ferramentas, execute um dos procedimentos a seguir:

   * Clique em **Visualização de grade** ou **Visualização de Lista**. No painel Navegação de ativos, clique com o duplo na miniatura de vídeo de um único ativo para abri-lo na Visualização Detalhe. No painel URLs e Código incorporado à direita, em HTTP Streaming, clique em **Código incorporado** à direita do visualizador desejado. Como prática recomendada, clique em **Incorporar código** associado ao visualizador `Universal_HTML5_Video`.
   * Clique em **Visualização de grade**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem em miniatura do vídeo, clique em **Pré-visualização** > **Lista do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique em **Código incorporado**. Como prática recomendada, clique em **Incorporar código** associado ao visualizador `Universal_HTML5_Video`.

   * Clique em **Visualização de Lista**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, clique em **Pré-visualização** > **Lista do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique em **Código incorporado**. Como prática recomendada, clique em **Incorporar código** associado ao visualizador `Universal_HTML5_Video`.

   * Clique em **Visualização de grade**, **Visualização de Lista** ou **Visualização de detalhes**. Na mesma barra de ferramentas, clique em **Pré-visualização** > **Lista do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique em **Código incorporado**. Como prática recomendada, clique em **Incorporar código** associado ao visualizador `Universal_HTML5_Video`.

1. Na caixa de diálogo Incorporar código, clique em **Copiar para a área de transferência**.

   A edição do código não é permitida na caixa de diálogo Incorporar código.

1. Clique em **Fechar**.
1. Cole o código incorporado em suas páginas da Web.

### Implementação do código incorporado para uso de vídeo HTML5 com ativos de vídeo MP4 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Se você não usar o player de vídeo HTML5 do Dynamic Media Classic, mas quiser usar a tag HTML5 nativa `<video>` com ativos de vídeo MP4, poderá usar a seguinte amostra de código incorporado:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Substitua `"S7 video thumbnail URL"` pelo URL de miniatura do vídeo. Esta é a imagem em miniatura do vídeo que um usuário vê antes de reproduzir o vídeo.

   Consulte [Obtendo URLs de miniatura de vídeo](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Substitua `"S7 OGG video asset URL (no player)"` pelo URL progressivo do vídeo para o vídeo OGG.

   Consulte [Vincular um URL de vídeo a um site móvel ou a um site](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Substitua `"S7 MP4 mobile progressive video asset URL (no player)"` pelo URL progressivo móvel do vídeo.

   Consulte [Vincular um URL de vídeo a um site móvel ou a um site](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Implantação de vídeo usando um player de vídeo de terceiros {#deploying-video-using-a-third-party-video-player}

Se você usar um player de vídeo de terceiros ou um player de vídeo personalizado em vez de um visualizador de vídeo Dynamic Media Classic, você pode obter o URL de vídeo direto que funciona para streaming de vídeo com vários bits de HLS ou download progressivo.

**Implantação de vídeo usando um player de vídeo de terceiros**

1. No Dynamic Media Classic, na barra Navegação global, clique em **Configuração** > **Configuração de aplicação** > **Definições gerais**.
1. Dependendo do tipo de URL que você deseja usar, execute uma das seguintes tarefas:
* Para gerar um URL de vídeo de transmissão direta HLS (multi-bitrate)

   Na página **Configurações gerais do aplicativo**, no grupo **Servidores**, no campo de texto **Nome do servidor publicado**, crie o URL direto usando a seguinte sintaxe: `server/is/content/company/folder/filename.m3u8`
Por exemplo, suponha que o nome do servidor publicado seja `https://s7d9.scene7.com/.` Ao usar a sintaxe na etapa 2, o URL direto pode ser semelhante ao seguinte:
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Para gerar um URL de vídeo de transmissão direta HLS (taxa de bits única)

   Na página **Configurações gerais do aplicativo**, no grupo **Servidores**, no campo de texto **HLS Streaming Server Name**, crie o URL direto usando a seguinte sintaxe:
   `server/company/folder/filename.ext.m3u8`
Por exemplo, suponha que o nome do servidor de streaming HLS seja  `https://s7mbrstream.scene7.com/hls-vod/`. Usando a sintaxe na etapa 2, o URL direto pode ser semelhante ao seguinte:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Para gerar um URL de vídeo progressivo direto

   Na página **Configurações gerais do aplicativo**, no grupo **Servidores**, no campo de texto **Nome do servidor de vídeo progressivo**, crie o URL direto do eVideo usando a seguinte sintaxe: `server/company/folder/filename`
Por exemplo, suponha que o nome do servidor de vídeo progressivo seja `https://s7d9.scene7.com/is/content/`. Usando a sintaxe na etapa 2, o URL direto pode ser semelhante ao seguinte:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Trabalhar com miniaturas de vídeo {#working-with-video-thumbnails}

O Dynamic Media Classic gera miniaturas para vídeos codificados e vídeos pré-codificados. Você pode usar miniaturas de vídeo como qualquer ativo de imagem. Além disso, você pode obter URLs para as miniaturas de vídeo que o Dynamic Media Classic gera e implantar esses URLs fora do Dynamic Media Classic. Por exemplo, você pode implantar as miniaturas em resultados de pesquisa, listagens de vídeo relacionadas e listas de reprodução de vídeo em um site.

As miniaturas são geradas com base no primeiro quadro heterogêneo (não um quadro totalmente preto, ou um quadro totalmente branco, e assim por diante) do vídeo.

### Obter URLs de miniatura de vídeo {#obtaining-video-thumbnail-urls}

O Dynamic Media Classic gera miniaturas de vídeo automaticamente durante o processo de upload. As miniaturas são exibidas no painel Procurar na visualização da Lista e na visualização da grade.

Para gerar URLs para miniaturas de vídeo, execute uma operação de publicação.

Consulte [Publicar vídeo](deploying-video-websites-mobile-sites.md#publishing_video).

Após a publicação, você pode obter URLs de miniatura de vídeo na Visualização Detalhe nos URLs e no painel Código incorporado. Clique em **Copiar URL** à direita da miniatura do vídeo para copiar o URL

### Modificação de quadros de pôster em visualizadores de vídeo {#modifying-poster-frames-in-video-viewers}

O *quadro de pôster* é o quadro inicial que aparece nos visualizadores de Vídeo antes da reprodução do vídeo. O Dynamic Media Classic usa miniaturas de vídeo como quadros de pôster.

É possível aplicar modificadores de imagem ao quadro de pôster. Por exemplo, você pode cortar o quadro do pôster ou torná-lo transparente. Para modificar o quadro de pôster, abra a tela de configuração do visualizador de vídeo e digite modificadores na seção Modificadores de imagem de pôster.

Consulte [Adicionar ou editar uma predefinição do visualizador de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consulte [www.adobe.com/go/learn_s7_image_server_guide_en](https://www.adobe.com/go/learn_s7_image_server_guide_en).

Também é possível modificar miniaturas de vídeo anexando modificadores aos URLs de miniatura de vídeo.

>[!MORELIKETHIS]
>
>* [Publicação de arquivos ](publishing-files.md#publishing_files)

