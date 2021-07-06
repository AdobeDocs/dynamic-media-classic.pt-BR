---
title: Adição de legendas ao vídeo
description: Saiba como adicionar legendas ao vídeo
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Visualizadores,Vídeo
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
source-git-commit: 9ff171590c65f55cef8c9e5a2b4e77ddbbfa6895
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 1%

---

# Adição de legendas ao vídeo{#adding-captions-to-video}

Você pode estender o alcance de seus vídeos para os mercados globais adicionando legendas a vídeos individuais ou aos Conjuntos de vídeos adaptáveis. Ao adicionar legendas, você evita a necessidade de dublar o áudio ou a necessidade de usar alto-falantes nativos para regravar o áudio para cada idioma diferente. O vídeo é reproduzido no idioma em que foi gravado. As legendas em idioma estrangeiro são exibidas para que pessoas de idiomas diferentes ainda possam entender a parte de áudio.

As legendas também permitem maior acessibilidade, usando legendas ocultas para pessoas surdas ou com deficiência auditiva.

>[!NOTE]
>
>O reprodutor de vídeo usado deve ser compatível com a exibição de legendas.

Para configurar o Efeito da legenda e editar o próprio Menu da legenda, incluindo o texto do menu para qualquer um dos seguintes visualizadores:

* `Universal_HTML5_Video` visualizador
* `Universal_HTML5_MixedMedia_dark` visualizador
* `Universal_HTML5_MixedMedia_light` visualizador

consulte [Adicionar ou editar uma predefinição do visualizador de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consulte também [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

O Dynamic Media Classic pode converter arquivos de legenda para o formato JSON (JavaScript™ Object Notation). Essa conversão significa que você pode incorporar o texto JSON em uma página da Web como uma transcrição oculta, mas completa, do vídeo. Os mecanismos de pesquisa podem, então, rastrear e indexar o conteúdo para tornar os vídeos mais fáceis de serem descobertos e fornecer aos clientes mais detalhes sobre o conteúdo do vídeo.

Consulte [Serving static (non-image) content](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) na *Ajuda da API de disponibilização de imagens do Adobe* para obter mais informações sobre o uso da função JSON em um URL.

**Para adicionar legendas ao vídeo**

1. Usando um aplicativo de terceiros fora do Dynamic Media Classic, crie seu arquivo de legenda de vídeo com base no tipo de visualizador que você está usando.

   | Tipo de visualizador | Arquivo de legendas |
   |--- |--- |
   | HTML5 | Se você estiver usando um visualizador de vídeo HTML5, certifique-se de que o arquivo de legenda criado siga o padrão WebVTT (Web Video Text Tracks). A extensão de nome de arquivo de legendagem é .vtt. Você pode obter mais informações sobre o padrão de legendagem WebVTT.<br><br>[Consulte WebVTT](https://w3c.github.io/webvtt/): O formato de Rastreamento de texto do vídeo da Web. <br><br>Há ferramentas e serviços gratuitos e pagos que podem ser usados para criar arquivos de legenda fora do Dynamic Media Classic. Por exemplo, para criar um arquivo de legenda de vídeo simples sem estilização, você pode usar a seguinte ferramenta de edição e criação de legendas online gratuitas: <br><br>[Criador de legendas WebVTT](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>Para obter melhores resultados, use a ferramenta no Internet Explorer 9 ou superior, no Google Chrome ou no Safari. <br><br>Na ferramenta, no campo  <b>Inserir URL do </b> arquivo de vídeo, cole o URL do arquivo de vídeo e clique em  <b>Carregar</b>. <br><br>Por exemplo, se estiver usando um URL do Dynamic Media Classic para o arquivo de vídeo, clique duas vezes em um ativo de vídeo individual (não um Conjunto de vídeos adaptáveis ou um vídeo Principal) para abri-lo na Exibição de detalhes. No painel direito da Exibição de detalhes, expanda URLs e Código incorporado. Em seguida, no grupo Mobile , à direita de Mobile (Progressive), clique em Copy URL (Copiar URL). Esse processo fornece o URL para o próprio arquivo de vídeo, que pode ser colado no campo <b>Enter URL of video file</b>. O Internet Explorer, o Chrome ou o Safari podem reproduzir nativamente o vídeo. Agora siga as instruções na tela do site para criar e salvar seu arquivo WebVTT. Quando terminar, copie o conteúdo do arquivo de legenda e o cole em um editor de texto simples e salve com uma extensão de nome de arquivo .vtt. <br><br><b>Observação:</b> para oferecer suporte global a legendas de vídeo em idiomas diferentes do inglês, o padrão WebVTT requer a criação de arquivos .vtt e chamadas separadas para cada idioma que você deseja suportar. <br><br>Geralmente, você deseja nomear o arquivo VTT da legenda com o mesmo nome do arquivo de vídeo e anexá-lo com legendas. Ao fazer isso, ele pode ajudá-lo a automatizar a geração dos URLs de vídeo usando seu sistema de gerenciamento de conteúdo da Web existente. |

1. No Dynamic Media Classic, faça upload de seu arquivo de legenda XML WebVTT, DFXP ou SMPTE.

   Consulte [Upload de arquivos](uploading-files.md#uploading_files).

1. No painel Biblioteca de ativos, à esquerda, navegue até a pasta de ativos que contém o arquivo de vídeo a ser associado ao arquivo de legenda que você enviou.
1. No painel Navegação de ativos, selecione um único ativo de vídeo e, em seguida, abaixo da imagem em miniatura do ativo, clique em **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. Na tabela Lista de visualizadores, localize o visualizador de HTML5 chamado **Universal_HTML5_Video**, **Universal_HTML5_MixedMedia_dark** ou **Universal_HTML5_MixedMedia_light**, siga um destes procedimentos:

   * Para obter uma experiência do visualizador de vídeo pop-up, clique em **[!UICONTROL Copy URL]** na extremidade direita do nome.

      Anexe o URL copiado do vídeo com a seguinte sintaxe para associá-lo ao URL copiado para o arquivo de legenda:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Observe o `,1` no final do caminho do URL da legenda. Imediatamente após a extensão do nome de arquivo .vtt no caminho, é possível ativar ou desativar o botão de legenda na barra do reprodutor de vídeo, definindo para `1` ou `0`, respectivamente.

   * Para obter uma experiência de visualizador de vídeo incorporado, clique em **[!UICONTROL Embed Code]** à direita do nome.

      Na caixa de diálogo Incorporar código , clique em **[!UICONTROL Copy to Clipboard]**.

      Para os visualizadores HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark` ou `Universal_HTML5_MixedMedia_light`, anexe o código incorporado copiado com o seguinte:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Observe o `,1` no final do caminho do URL. Imediatamente após a extensão do nome de arquivo .vtt no caminho do URL, você pode, opcionalmente, ativar ou desativar o botão de legenda na barra do reprodutor de vídeo, definindo para `1` ou `0`, respectivamente.
