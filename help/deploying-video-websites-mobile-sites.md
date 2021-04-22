---
title: Implantação de vídeo em seus sites e sites móveis
description: Saiba como implantar vídeo em seus sites e sites móveis.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Visualizadores,Vídeo
role: Business Practitioner
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
translation-type: tm+mt
source-git-commit: 4e79c98b92dfa4e1a9890ed8a291cdf564126466
workflow-type: tm+mt
source-wordcount: '1567'
ht-degree: 2%

---

# Implantação de vídeo em seus sites e sites móveis{#deploying-video-to-your-websites-and-mobile-sites}

Sites, sites móveis e aplicativos de desktop acessam o conteúdo do servidor Dynamic Media Classic, incluindo vídeo, usando strings de URL ou código incorporado. O Dynamic Media Classic ativa essas cadeias de caracteres de URL durante o processo de publicação. Para colocar a string do URL ou o código incorporado do vídeo nas páginas da Web, páginas móveis e aplicativos de desktop, copie-o do Dynamic Media Classic.

>[!NOTE]
>
>O URL ou código incorporado não fica ativo até que você publique o ativo.

## Publicação de vídeo {#publishing-video}

A publicação de um vídeo permite que os servidores Dynamic Media Classic forneçam vídeo ao seu site, site para dispositivos móveis ou aplicativo.

Há dois métodos diferentes que você pode usar para publicar vídeos:

* **Publicar vídeos automaticamente e instantaneamente no upload**  - Como parte do processo de upload de vídeos, o Dynamic Media Classic pode publicar vídeos automaticamente quando eles forem carregados e codificados. Essa capacidade de publicar instantaneamente significa que não há necessidade de publicar vídeos separadamente após o fato.

* **Publicar vídeo manualmente após o upload**  - se você não quiser publicar vídeos imediatamente, publique vídeos manualmente a qualquer momento.

Após publicar vídeos, o Dynamic Media Classic ativa as cadeias de caracteres do URL para sua página HTML ou código do aplicativo.

**Para publicar vídeo:**

1. Siga um destes procedimentos:

   * Para publicar vídeos automaticamente e instantaneamente no upload, na página Upload , clique em **[!UICONTROL Publish after uploading]**. Você terminou; não há outras etapas a serem concluídas.
   * Para publicar vídeos manualmente após o upload, no Painel de navegação, selecione os vídeos e, em seguida, na barra Navegação global, clique em **Publicar**.

## Vincular um URL de vídeo a um site móvel ou {#linking-a-video-url-to-a-mobile-site-or-a-website}

Após publicar um vídeo, você pode obter o URL para uso no seu site, site para dispositivos móveis ou aplicativo de desktop. Use o URL do vídeo quando quiser exibir o vídeo em uma janela pop-up ou modal na parte superior da página da Web.

Quando um cliente clica no link, o dispositivo, a largura de banda e o tamanho da tela são automaticamente detectados. O vídeo apropriado é exibido para reprodução em um visualizador predefinido para desktop ou no reprodutor de vídeo nativo do dispositivo móvel para smartphones e tablets.

Consulte também [Incorporar o visualizador de vídeo em uma página da Web](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Para vincular um URL de vídeo a um site para dispositivos móveis ou a um site:**

1. No painel Navegação de ativos , na lista suspensa **[!UICONTROL Show]**, clique em **[!UICONTROL Video]** ou **[!UICONTROL Adaptive Video Set]**.
1. no painel Biblioteca de ativos, à esquerda, navegue até a pasta de ativos que contém o vídeo ou o conjunto de vídeos adaptáveis que você deseja vincular.
1. Acima do painel Navegação de ativos , no lado direito da barra de ferramentas, execute um dos seguintes procedimentos:

   * Clique em **[!UICONTROL Grid View]** ou **[!UICONTROL List View]**. No painel Navegação de ativos, clique duas vezes na miniatura de vídeo de um único ativo para abri-lo na Exibição de detalhes. No painel URLs e Código incorporado à direita, em HTTP Streaming (Transmissão HTTP), clique em **[!UICONTROL Copy URL]** à direita do visualizador desejado. Como prática recomendada, copie o URL associado ao visualizador `Universal_HTML5_Video`.
   * Clique em **[!UICONTROL Grid View]**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem em miniatura, clique em **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Na página Lista de visualizadores , na coluna Ações da tabela, clique em **[!UICONTROL Copy URL]**. Como prática recomendada, copie o URL associado ao visualizador `Universal_HTML5_Video`.

   * Clique em **[!UICONTROL List View]**. No painel Navegação de ativos , selecione um único ativo e, à direita da imagem em miniatura, clique em **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Na página Lista de visualizadores , na coluna Ações da tabela, clique em **[!UICONTROL Copy URL]**. Como prática recomendada, copie o URL associado ao visualizador `Universal_HTML5_Video`.

   * Clique em **[!UICONTROL Grid View]**, **[!UICONTROL List View]** ou **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, clique em **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Na página Lista de visualizadores , na coluna Ações da tabela, clique em **[!UICONTROL Copy URL]**. Como prática recomendada, copie o URL associado ao visualizador `Universal_HTML5_Video`.

1. Cole o link HTML5 video URL no seu site e site móvel.

## Incorporação do visualizador de vídeo em uma página da Web {#embedding-the-video-viewer-on-a-web-page}

Use o recurso Incorporar código quando quiser reproduzir o vídeo incorporado na página da Web. Copie o código incorporado na área de transferência para poder colá-lo nuas páginas da Web. A edição do código não é permitida na caixa de diálogo Incorporar código.

Consulte também [Vincular um URL de vídeo a um site para dispositivos móveis ou a um site](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Para incorporar o visualizador de vídeo em uma página da Web:**

1. No painel Navegação de ativos , na lista suspensa Mostrar , clique em **[!UICONTROL Video]** ou **[!UICONTROL Adaptive Video Set]**.
1. no painel Biblioteca de ativos, à esquerda, navegue até a pasta de ativos que contém o vídeo ou conjunto de vídeos adaptáveis cujo código incorporado você deseja copiar.
1. Acima do painel Navegação de ativos , no lado direito da barra de ferramentas, execute um dos seguintes procedimentos:

   * Clique em **[!UICONTROL Grid View]** ou **[!UICONTROL List View]**. No painel Navegação de ativos, clique duas vezes na miniatura de vídeo de um único ativo para abri-lo na Exibição de detalhes. No painel URLs e Código incorporado à direita, em HTTP Streaming (Transmissão HTTP), clique em **[!UICONTROL Embed Code]** à direita do visualizador desejado. Como prática recomendada, clique em **[!UICONTROL Embed Code]** que está associado ao visualizador `Universal_HTML5_Video`.
   * Clique em **[!UICONTROL Grid View]**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem de miniatura do vídeo, clique em **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Na página Lista de visualizadores , na coluna Ações da tabela, clique em **[!UICONTROL Embed Code]**. Como prática recomendada, clique em **[!UICONTROL Embed Code]** que está associado ao visualizador `Universal_HTML5_Video`.

   * Clique em **[!UICONTROL List View]**. No painel Navegação de ativos , selecione um único ativo e, à direita da imagem em miniatura, clique em **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Na página Lista de visualizadores , na coluna Ações da tabela, clique em **[!UICONTROL Embed Code]**. Como prática recomendada, clique em **[!UICONTROL Embed Code]** que está associado ao visualizador `Universal_HTML5_Video`.

   * Clique em **[!UICONTROL Grid View]**, **[!UICONTROL List View]** ou **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, clique em **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Na página Lista de visualizadores , na coluna Ações da tabela, clique em **[!UICONTROL Embed Code]**. Como prática recomendada, clique em **[!UICONTROL Embed Code]** que está associado ao visualizador `Universal_HTML5_Video`.

1. Na caixa de diálogo Incorporar código , clique em **[!UICONTROL Copy to Clipboard]**.

   A edição do código não é permitida na caixa de diálogo Incorporar código .

1. Clique em **[!UICONTROL Close]**.
1. Cole o código incorporado nas páginas da Web.

### Implementação do código incorporado para usar vídeo HTML5 com ativos de vídeo MP4 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Se você não usar o reprodutor de vídeo HTML5 do Dynamic Media Classic, mas quiser usar a tag HTML5 nativa `<video>` com ativos de vídeo MP4, poderá usar a seguinte amostra de código integrado:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Substitua `"S7 video thumbnail URL"` pelo URL de miniatura do vídeo, que é a imagem de miniatura do vídeo que um usuário vê antes de reproduzir o vídeo.

   Consulte [Obter URLs de miniatura de vídeo](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Substitua `"S7 OGG video asset URL (no player)"` pelo URL progressivo do vídeo para o vídeo OGG.

   Consulte [Vincular um URL de vídeo a um site para dispositivos móveis ou a um site](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Substitua `"S7 MP4 mobile progressive video asset URL (no player)"` pelo URL progressivo do vídeo.

   Consulte [Vincular um URL de vídeo a um site para dispositivos móveis ou a um site](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Implantação de vídeo usando um reprodutor de vídeo de terceiros {#deploying-video-using-a-third-party-video-player}

Se você usar um reprodutor de vídeo de terceiros ou um reprodutor de vídeo personalizado em vez de um visualizador de vídeo do Dynamic Media Classic, poderá obter o URL do vídeo direto que funciona para streaming de vídeo com taxa de bits múltipla HLS ou download progressivo.

**Para implantar vídeo usando um reprodutor de vídeo de terceiros:**

1. No Dynamic Media Classic, na barra Navegação global, clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]**.
1. Dependendo do tipo de URL que deseja usar, execute uma das seguintes tarefas:

* Para gerar um URL de vídeo de transmissão direta de HLS (taxa de bits múltipla)

   Na página **[!UICONTROL Application General Settings]**, no grupo **[!UICONTROL Servers]**, no campo de texto **[!UICONTROL Published Server Name]**, construa o URL direto. Use a seguinte sintaxe: `server/is/content/company/folder/filename.m3u8`

   Por exemplo, suponha que o nome do servidor Publicado seja `https://s7d9.scene7.com/.` Usando a sintaxe na etapa 2, o URL direto poderia ter a seguinte aparência:
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Para gerar um URL de vídeo de transmissão direta de HLS (taxa de bits única)

   Na página **[!UICONTROL Application General Settings]**, no grupo **[!UICONTROL Servers]**, no campo de texto **[!UICONTROL HLS Streaming Server Name]**, construa o URL direto usando a seguinte sintaxe:

   `server/company/folder/filename.ext.m3u8`

   Por exemplo, suponha que o nome do servidor de transmissão HLS seja `https://s7mbrstream.scene7.com/hls-vod/`. Usando a sintaxe na etapa 2, o URL direto pode ser semelhante ao seguinte:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Para gerar um URL de vídeo progressivo direto

   Na página **[!UICONTROL Application General Settings]**, no grupo **[!UICONTROL Servers]**, no campo de texto **[!UICONTROL Progressive Video Server Name]**, construa o URL direto do eVideo usando a seguinte sintaxe:

   `server/company/folder/filename`

   Por exemplo, suponha que o nome do servidor de vídeo progressivo seja `https://s7d9.scene7.com/is/content/`. Usando a sintaxe na etapa 2, o URL direto pode ser semelhante ao seguinte:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Trabalhar com miniaturas de vídeo {#working-with-video-thumbnails}

O Dynamic Media Classic gera miniaturas para vídeos codificados e vídeos pré-codificados. Você pode usar miniaturas de vídeo como qualquer ativo de imagem. Além disso, você pode obter URLs para as miniaturas de vídeo geradas pelo Dynamic Media Classic e implantar esses URLs fora do Dynamic Media Classic. Por exemplo, você pode implantar as miniaturas em resultados de pesquisa, listas de vídeos relacionadas e listas de reprodução de vídeo em um site.

As miniaturas são geradas com base no primeiro quadro heterogêneo (não um quadro totalmente preto, ou um quadro totalmente branco, e assim por diante) do vídeo.

### Obter URLs de miniatura de vídeo {#obtaining-video-thumbnail-urls}

O Dynamic Media Classic gera miniaturas de vídeo automaticamente durante o processo de upload. As miniaturas são exibidas no painel Procurar na exibição em Lista e na exibição em Grade.

Para gerar URLs para miniaturas de vídeo, execute uma operação de publicação.

Consulte [Publicação de vídeo](deploying-video-websites-mobile-sites.md#publishing_video).

Após a publicação, é possível obter os URLs de miniatura do vídeo na Exibição de detalhes nos URLs e no painel Código incorporado . Clique em **[!UICONTROL Copy URL]** à direita da miniatura do vídeo para copiar o URL.

### Modificação de quadros de pôster em visualizadores de vídeo {#modifying-poster-frames-in-video-viewers}

O *quadro de pôster* é o quadro inicial exibido nos visualizadores de Vídeo antes da reprodução do vídeo. O Dynamic Media Classic usa miniaturas de vídeo como quadros de pôster.

Você pode aplicar modificadores de imagem ao quadro de pôster. Por exemplo, você pode cortar o quadro do pôster ou torná-lo transparente. Para modificar o quadro de pôster, abra a tela de configuração do visualizador de vídeo e insira modificadores na seção Poster Image Modifiers .

Consulte [Adicionar ou editar uma predefinição do visualizador de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consulte [Guia de disponibilização de imagens](https://experienceleague.corp.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api).

Também é possível modificar as miniaturas de vídeo ao anexar modificadores aos URLs de miniatura de vídeo.

>[!MORELIKETHIS]
>
>* [Publicação de arquivos ](publishing-files.md#publishing_files)