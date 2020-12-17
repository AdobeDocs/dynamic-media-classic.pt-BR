---
title: Adicionar legendas ao vídeo
seo-title: Adicionar legendas ao vídeo
description: nulo
seo-description: Saiba como adicionar legendas ao vídeo
uuid: 4cc64469-4369-44a9-83db-63bad51aba8a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 1%

---


# Adicionar legendas ao vídeo{#adding-captions-to-video}

Você pode estender o alcance de seus vídeos aos mercados globais adicionando legendas a vídeos únicos ou a Conjuntos de vídeos adaptáveis. Ao adicionar legendas, você evita a necessidade de dublar o áudio ou a necessidade de usar alto-falantes nativos para regravar o áudio para cada idioma diferente. O vídeo é reproduzido no idioma em que foi gravado. As legendas em idioma estrangeiro são exibidas para que pessoas de idiomas diferentes ainda possam entender a parte de áudio.

A legendagem também permite maior acessibilidade ao usar legendagem para pessoas surdas ou com dificuldades auditivas.

>[!NOTE]
>
>O player de vídeo usado deve suportar a exibição de legendas.

Consulte [Adicionar ou editar uma predefinição do visualizador de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) para configurar o efeito de legenda e editar o próprio Menu de legenda, incluindo o texto do menu para qualquer um dos seguintes visualizadores:

* `Universal_HTML5_Video` visualizador.
* `Universal_HTML5_MixedMedia_dark` visualizador.
* `Universal_HTML5_MixedMedia_light` visualizador.

Consulte também [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

O Dynamic Media Classic tem a capacidade de converter arquivos de legenda em formato JSON (JavaScript Object Notation). Essa conversão significa que você pode incorporar o texto JSON em uma página da Web como uma transcrição oculta, mas completa, do vídeo. Os mecanismos de pesquisa podem rastrear e indexar o conteúdo para tornar os vídeos mais facilmente detectáveis e fornecer aos clientes detalhes adicionais sobre o conteúdo do vídeo.

Consulte [Servindo conteúdo estático (não imagem)](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html) na *Ajuda da API de disponibilização de imagem do Adobe* para obter mais informações sobre como usar a função JSON em um URL.

**Para adicionar legendas ao vídeo**

1. Usando um aplicativo de terceiros fora do Dynamic Media Classic, crie seu arquivo de legenda de vídeo com base no tipo de visualizador usado.

   | Tipo de visualizador | Arquivo de legenda |
   |--- |--- |
   | HTML5 | Se você estiver usando um visualizador de vídeo HTML5, verifique se o arquivo de legenda criado segue o padrão WebVTT (Web Video Text Tracks). A extensão de nome de arquivo de legenda é .vtt. Você pode obter mais informações sobre o padrão de legendagem WebVTT.<br><br>[Consulte WebVTT](https://dev.w3.org/html5/webvtt/): O formato Rastreamento de texto de vídeo da Web. <br><br>Há ferramentas e serviços gratuitos e pagos que você pode usar para criar arquivos de legenda fora do Dynamic Media Classic. Por exemplo, para criar um arquivo simples de legenda de vídeo sem estilização, você pode usar a seguinte ferramenta gratuita de criação e edição de legendas online: <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>Para obter melhores resultados, use a ferramenta no Internet Explorer 9 ou superior, Google Chrome ou Safari. <br><br>Na ferramenta, no campo  <b>Inserir URL do </b> arquivo de vídeo, cole o URL do arquivo de vídeo e clique em  <b>Carregar</b>. <br><br>Por exemplo, se você estiver usando um URL do Dynamic Media Classic para seu arquivo de vídeo, no DMC, clique com o duplo em um ativo de vídeo individual (não um Conjunto de vídeos adaptáveis ou um vídeo Principal) para abri-lo na Visualização Detalhe. No painel direito da Visualização Detail, expanda URLs e Incorpore código. Em seguida, no grupo Móvel, à direita de Móvel (Progressivo), clique em Copiar URL. Esse processo fornece o URL para o próprio arquivo de vídeo, que você pode colar no campo <b>Insira o URL do arquivo de vídeo</b>. O Internet Explorer, o Chrome ou o Safari podem reproduzir nativamente o vídeo. Siga as instruções na tela do site para criar e salvar seu arquivo WebVTT. Quando terminar, copie o conteúdo do arquivo de legenda e cole-o em um editor de texto simples e salve-o com uma extensão de nome de arquivo .vtt. <br><br><b>Observação: </b> para obter suporte global às legendas de vídeo em idiomas diferentes do inglês, lembre-se de que o padrão WebVTT requer a criação de arquivos .vtt separados e chamadas para cada idioma que você deseja suportar. <br><br>Geralmente, você deseja nomear o arquivo VTT da legenda com o mesmo nome do arquivo de vídeo e anexá-lo às legendas. Ao fazer isso, ele pode ajudá-lo a automatizar a geração de URLs de vídeo usando seu sistema de gestão de conteúdo da Web existente. |

1. No Dynamic Media Classic, carregue seu arquivo de legenda WebVTT, DFXP ou SMPTE XML.

   Consulte [Carregando arquivos](uploading-files.md#uploading_files).

1. No painel Biblioteca de ativos, à esquerda, navegue até a pasta de ativos que contém o arquivo de vídeo que você deseja associar ao arquivo de legenda que você carregou.
1. No painel Navegação de ativos, selecione um único ativo de vídeo e, abaixo da imagem em miniatura do ativo, clique em **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. Na tabela Lista do visualizador, localize o visualizador HTML5 chamado **Universal_HTML5_Video**, **Universal_HTML5_MixedMedia_black** ou **Universal_HTML5_MixedMedia_light**, em seguida, execute um dos seguintes procedimentos:

   * Para obter uma experiência do visualizador de vídeo pop-up, clique em **[!UICONTROL Copy URL]** na extremidade direita do nome.

      Anexe o URL copiado do vídeo com a sintaxe a seguir para associá-lo ao URL copiado ao arquivo de legenda:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Observe `,1` no final do caminho do URL da legenda. Imediatamente após a extensão de nome de arquivo .vtt no caminho, você tem a opção de ativar ou desativar o botão de legenda na barra do player de vídeo definindo `1` ou `0`, respectivamente.

   * Para obter uma experiência com o visualizador de vídeo incorporado, clique em **[!UICONTROL Embed Code]** na extremidade direita do nome.

      Na caixa de diálogo Incorporar código, clique em **[!UICONTROL Copy to Clipboard]**.

      Para os visualizadores HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark` ou `Universal_HTML5_MixedMedia_light`, anexe o código incorporado copiado com o seguinte:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Observe `,1` no final do caminho do URL. Imediatamente após a extensão de nome de arquivo .vtt no caminho do URL, você tem a opção de ativar ou desativar o botão de legenda na barra do player de vídeo definindo para `1` ou `0`, respectivamente.

