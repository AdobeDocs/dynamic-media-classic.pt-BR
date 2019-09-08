---
title: Implantação de vídeos em sites e sites móveis
seo-title: Implantação de vídeos em sites e sites móveis
description: 'null'
seo-description: Saiba como implantar vídeos em seus sites e sites móveis.
uuid: 22 bb 4402-c 0 ab -4 df 0-89 b 9-99707 d 111927
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/vídeo
discoiquuid: 0 d 006314-c 4 cc -4 f 6 c-a 51 c -6075 bb 445 e 39
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Implantação de vídeos em sites e sites móveis{#deploying-video-to-your-websites-and-mobile-sites}

Sites, sites móveis e aplicativos de desktop acessam o conteúdo do servidor do Dynamic Media Classic, incluindo vídeo, usando sequências de URL ou código incorporado. O Dynamic Media Classic ativa essas sequências de caracteres de URL durante o processo de publicação. Para colocar a sequência de URL ou o código incorporado para seu vídeo em suas páginas da Web, páginas móveis e aplicativos de desktop, copie-o do Sistema de publicação Scene 7.

>[!NOTE]
>
>O URL ou o código incorporado não está ativo até que você publique o ativo.

## Publicação de vídeo {#publishing-video}

Publicar um vídeo permite que os servidores do Dynamic Media Classic forneçam vídeo a seu site, site móvel ou aplicativo.

Há dois métodos diferentes que você pode usar para publicar vídeo:

* **Publicar vídeos automaticamente e instantaneamente no upload**

   Como parte do processo de upload de vídeo, o Dynamic Media Classic pode publicar automaticamente vídeos quando eles são carregados e codificados. Essa capacidade de publicar instantaneamente significa que não há necessidade de publicar vídeos separadamente depois do fato.

* **Publicar vídeos manualmente após o upload**

   Se você não quiser publicar vídeos imediatamente, poderá publicar vídeos manualmente a qualquer momento.

Depois de publicar vídeos, o Sistema de publicação Scene 7 ativa as strings de URL para sua página HTML ou código do aplicativo.

**Para publicar vídeo**

1. Execute um dos procedimentos a seguir:

   * Para publicar vídeos automaticamente e instantaneamente no upload, na tela Carregar, clique **em Publicar depois de fazer upload**. Você terminou; não há mais etapas para concluir.
   * Para publicar vídeos manualmente após o upload, no Painel Procurar, selecione os vídeos e, na barra Navegação global, clique **em Publicar**.

## Vincular um URL de vídeo a um site móvel ou a um site {#linking-a-video-url-to-a-mobile-site-or-a-website}

Depois de publicar um vídeo, você pode obter seu URL para uso em seu site, site móvel ou aplicativo de desktop. Use o URL do vídeo quando quiser exibir vídeo em uma janela pop-up ou modal na parte superior da página da Web.

Quando um cliente clica no link, seu dispositivo, largura de banda e tamanho de tela são detectados automaticamente. O vídeo apropriado é exibido para reprodução em um visualizador pré-definido para desktop ou no player de vídeo nativo do dispositivo móvel para smartphones e tablets.

Consulte [também Incorporar o visualizador de vídeo em uma página da Web](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Vincular um URL de vídeo a um site móvel ou a um site**

1. No painel Procurar ativo, na lista suspensa Mostrar, clique em **Vídeo** ou **Conjunto de vídeos adaptativos**.
1. no painel Biblioteca de ativos no lado esquerdo, navegue até a pasta de ativos que contém o vídeo ou o conjunto de vídeos adaptável que você deseja vincular.
1. Acima do painel Navegador de ativos, no lado direito da barra de ferramentas, execute um dos seguintes procedimentos:

   * Clique **em Exibição de grade** ou **Exibição de lista**. No painel Navegador de ativos, clique duas vezes na miniatura de vídeo de um único ativo para abri-lo na Exibição de detalhes. Nos urls e no painel Incorporar código à direita, em Streaming HTTP, clique **em Copiar URL** à direita do visualizador desejado. Como prática recomendada, copie o URL associado ao `Universal_HTML5_Video` visualizador.
   * Clique **em Exibição de grade**. No painel Procurar ativo, selecione um único ativo e depois abaixo da imagem em miniatura, clique **em Visualizar** &gt; Lista **do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique **em Copiar URL**. Como prática recomendada, copie o URL associado ao `Universal_HTML5_Video` visualizador.

   * Clique **em Exibição de lista**. No painel Procurar ativo, selecione um único ativo e, à direita da imagem em miniatura, clique **em Visualizar** &gt; Lista **do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique **em Copiar URL**. Como prática recomendada, copie o URL associado ao `Universal_HTML5_Video` visualizador.

   * Clique **em Exibição de grade**, **Exibição de lista** ou Exibição **de detalhes**. Na mesma barra de ferramentas, clique **em Visualizar** &gt; Lista **de visualizadores**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique **em Copiar URL**. Como prática recomendada, copie o URL associado ao `Universal_HTML5_Video` visualizador.

1. Cole o link de URL do vídeo HTML 5 em seu site e site móvel.

## Incorporação do visualizador de vídeo em uma página da Web {#embedding-the-video-viewer-on-a-web-page}

Use o recurso Incorporar código quando quiser reproduzir o vídeo incorporado na página da Web. Copie o código incorporado para a área de transferência para que você possa colá-lo em suas páginas da Web. A edição do código não é permitida na caixa de diálogo Incorporar código.

Consulte [também Vinculação de um URL de vídeo a um site móvel ou site](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Incorporação do visualizador de vídeo em uma página da Web**

1. No painel Procurar ativo, na lista suspensa Mostrar, clique em **Vídeo** ou **Conjunto de vídeos adaptativos**.
1. no painel Biblioteca de ativos no lado esquerdo, navegue até a pasta de ativos que contém o vídeo ou o vídeo adaptável definido cujo código incorporado você deseja copiar.
1. Acima do painel Navegador de ativos, no lado direito da barra de ferramentas, execute um dos seguintes procedimentos:

   * Clique **em Exibição de grade** ou **Exibição de lista**. No painel Navegador de ativos, clique duas vezes na miniatura de vídeo de um único ativo para abri-lo na Exibição de detalhes. Nos urls e no painel Incorporar código à direita, em Streaming HTTP, clique em **Incorporar código** à direita do visualizador desejado. Como prática recomendada, clique **em Incorporar código** que esteja associado ao `Universal_HTML5_Video` visualizador.
   * Clique **em Exibição de grade**. No painel Procurar ativo, selecione um único ativo e depois abaixo da imagem em miniatura do vídeo, clique **em Visualizar** &gt; Lista **do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique **em Incorporar código**. Como prática recomendada, clique **em Incorporar código** que esteja associado ao `Universal_HTML5_Video` visualizador.

   * Clique **em Exibição de lista**. No painel Procurar ativo, selecione um único ativo e, à direita da imagem em miniatura, clique **em Visualizar** &gt; Lista **do visualizador**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique **em Incorporar código**. Como prática recomendada, clique **em Incorporar código** que esteja associado ao `Universal_HTML5_Video` visualizador.

   * Clique **em Exibição de grade**, **Exibição de lista** ou Exibição **de detalhes**. Na mesma barra de ferramentas, clique **em Visualizar** &gt; Lista **de visualizadores**.

      Na página Lista do visualizador, na coluna Ações da tabela, clique **em Incorporar código**. Como prática recomendada, clique **em Incorporar código** que esteja associado ao `Universal_HTML5_Video` visualizador.

1. Na caixa de diálogo Incorporar código, clique **em Copiar para a área de transferência**.

   A edição do código não é permitida na caixa de diálogo Incorporar código.

1. Clique **em Fechar**.
1. Cole o código incorporado em suas páginas da Web.

### Implementação de código incorporado para uso de vídeo HTML 5 com ativos de vídeo MP 4 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Se você não usar o player de vídeo HTML 5 clássico de Dynamic Media, mas quiser usar a tag NTML 5 nativa `<video>` com os ativos de vídeo MP 4, poderá usar a seguinte amostra de código incorporado:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Substitua `"S7 video thumbnail URL"` pelo URL de miniatura do vídeo. Esta é a imagem em miniatura do vídeo que um usuário vê antes de reproduzir o vídeo.

   Consulte [Obter urls de miniatura de vídeo](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Substitua `"S7 OGG video asset URL (no player)"` pelo URL progressivo do vídeo para vídeo OGG.

   Consulte [Vincular um URL de vídeo a um site móvel ou site](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Substitua `"S7 MP4 mobile progressive video asset URL (no player)"` pelo URL progressivo do vídeo.

   Consulte [Vincular um URL de vídeo a um site móvel ou site](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Implantação de vídeo usando um player de vídeo de terceiros {#deploying-video-using-a-third-party-video-player}

Se você usar um player de vídeo de terceiros ou um player de vídeo personalizado personalizado em vez de um visualizador de vídeo do Dynamic Media Classic, poderá obter o URL de vídeo direto que funciona para streaming de vídeo de multi-bitrate HLS ou download progressivo.

**Implantação de vídeo usando um player de vídeo de terceiros**

1. No Sistema de publicação do Scene 7, na barra Navegação global, clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Configurações gerais**.
1. Dependendo do tipo de URL que deseja usar, execute uma das seguintes tarefas:
* Geração de um URL de vídeo de streaming de HLS direto (multi-bitrate)

   Na página **Configurações** gerais do aplicativo, no grupo **Servidores** , no **campo de texto Nome** do servidor publicado, crie o URL direto usando a seguinte sintaxe: `server/is/content/company/folder/filename.m3u8`
Por exemplo, suponha que o nome do servidor Publicado esteja `https://s7d9.scene7.com/.` usando a sintaxe na etapa 2, o URL direto pode ser semelhante ao seguinte:
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Geração de um URL de vídeo de streaming de HLS direto (taxa de bits única)

   Na **página Configurações** gerais do aplicativo, no grupo **Servidores** , no campo de texto **HLS** Streaming Server Name, crie o URL direto usando a seguinte sintaxe:
   `server/company/folder/filename.ext.m3u8`Por exemplo, suponha que o nome do servidor de streaming HLS esteja `https://s7mbrstream.scene7.com/hls-vod/`. Usando a sintaxe na etapa 2, o URL direto pode ser semelhante ao seguinte:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Geração de um URL de vídeo progressivo direto

   Na página **Configurações** gerais do aplicativo, no grupo **Servidores** , no **campo de texto Nome** do servidor de vídeo progressivo, crie o URL de evideo direto usando a seguinte sintaxe: `server/company/folder/filename`
Por exemplo, suponha que o nome do servidor de vídeo progressivo é `https://s7d9.scene7.com/is/content/`. Usando a sintaxe na etapa 2, o URL direto pode ser semelhante ao seguinte:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Trabalho com miniaturas de vídeo {#working-with-video-thumbnails}

O Dynamic Media Classic gera miniaturas para vídeos codificados e vídeos pré-codificados. Você pode usar miniaturas de vídeo como qualquer ativo de imagem. Além disso, você pode obter urls para as miniaturas de vídeo que o Dynamic Media Classic gera e implantar esses urls fora do SPS. Por exemplo, você pode implantar miniaturas em resultados de pesquisa, listagens de vídeo relacionadas e listas de reprodução de vídeo em um site.

As miniaturas são geradas com base no primeiro quadro heterogêneo (não é um quadro preto ou um quadro branco, e assim por diante) do vídeo.

### Obtenção de urls de miniatura de vídeo {#obtaining-video-thumbnail-urls}

O Dynamic Media Classic gera miniaturas de vídeo automaticamente durante o processo de upload. As miniaturas aparecem no painel Procurar na exibição de Lista e na exibição de Grade.

Para gerar urls para miniaturas de vídeo, realize uma operação de publicação.

Consulte [Publicação de vídeo](deploying-video-websites-mobile-sites.md#publishing_video).

Após a publicação, você pode obter urls de miniatura de vídeo em Exibição detalhada nos urls e no painel Incorporar código. Clique **em Copiar URL** à direita da miniatura do vídeo para copiar o URL

### Modificação de quadros de pôster em visualizadores de vídeo {#modifying-poster-frames-in-video-viewers}

O quadro *de pôster* é o quadro inicial que aparece nos visualizadores de Vídeo antes do vídeo começar a ser reproduzido. O Dynamic Media Classic usa miniaturas de vídeo como quadros de pôster.

Você pode aplicar modificadores de imagem ao quadro de pôster. Por exemplo, você pode cortar o quadro de pôster ou torná-lo transparente. Para modificar o quadro de pôster, abra a tela de configuração do visualizador de vídeo e insira modificadores na seção Modificadores de imagem de cartaz.

Consulte [Adicionar ou editar uma predefinição do visualizador de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consulte [www.adobe.com/go/learn_s7_image_server_guide_en](https://www.adobe.com/go/learn_s7_image_server_guide_en).

Também é possível modificar miniaturas de vídeo anexando modificadores a urls de miniaturas de vídeo.

>[!MORELIKETHIS]
>
>* [Publicação de arquivos](publishing-files.md#publishing_files)

