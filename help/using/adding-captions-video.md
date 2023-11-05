---
title: Adicionar legendas ao vídeo
description: Saiba como adicionar legendas a vídeos no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 0%

---

# Adicionar legendas ao vídeo {#adding-captions-to-video}

Você pode estender o alcance de seus vídeos para mercados globais adicionando legendas a vídeos únicos ou a Conjuntos de vídeos adaptados. Ao adicionar legendas, você evita a necessidade de dublar o áudio ou a necessidade de usar alto-falantes nativos para regravar o áudio para cada idioma diferente. O vídeo é reproduzido no idioma em que foi gravado. Legendas em idiomas estrangeiros aparecem para que pessoas de diferentes idiomas ainda possam entender a parte de áudio.

A legenda também permite maior acessibilidade usando legendas ocultas para pessoas surdas ou com deficiência auditiva.

>[!NOTE]
>
>O reprodutor de vídeo usado deve oferecer suporte à exibição de legendas.

Para configurar o Efeito de legenda e editar o Menu de legenda propriamente dito, incluindo o texto do menu para qualquer um dos seguintes visualizadores:

* `Universal_HTML5_Video` visualizador
* `Universal_HTML5_MixedMedia_dark` visualizador
* `Universal_HTML5_MixedMedia_light` visualizador

Consulte [Adicionar ou editar uma predefinição do visualizador de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consulte também [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

O Adobe Dynamic Media Classic pode converter arquivos de legenda para o formato JSON (JavaScript Object Notation). Essa conversão significa que você pode incorporar o texto JSON em uma página da Web como uma transcrição oculta, mas completa, do vídeo. Os mecanismos de pesquisa podem rastrear e indexar o conteúdo para facilitar a descoberta dos vídeos e fornecer aos clientes mais detalhes sobre o conteúdo do vídeo.

Consulte [Veicular conteúdo estático (não imagem)](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) no *Ajuda da API do Adobe Image Serving* para obter mais informações sobre como usar a função JSON em um URL.

**Para adicionar legendas ao vídeo:**

1. Usando um aplicativo de terceiros fora do Adobe Dynamic Media Classic, crie seu arquivo de legenda de vídeo com base no tipo de visualizador que você está usando.

   | Tipo de visualizador | Arquivo de legendas |
   |--- |--- |
   | HTML5 | Se estiver usando um visualizador de vídeo HTML5, certifique-se de que o arquivo de legenda criado segue o padrão WebVTT (Web Video Text Tracks, Rastreamentos de texto de vídeo da Web). A extensão do nome de arquivo das legendas é .vtt. Você pode obter mais informações sobre o padrão de legendagem WebVTT.<br><br>[Consulte WebVTT](https://w3c.github.io/webvtt/): o formato de faixas de texto do vídeo da Web. <br><br>Há ferramentas e serviços gratuitos e pagos que você pode usar para criar arquivos de legenda fora do Adobe Dynamic Media Classic. Por exemplo, para criar um arquivo simples de legenda de vídeo sem estilo, é possível usar a seguinte ferramenta online gratuita de criação e edição de legendas: <br><br>[Criador de legendas WebVTT](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>Para obter melhores resultados, use a ferramenta no Internet Explorer 9 ou superior, Google Chrome ou Safari. <br><br>Na ferramenta, no campo <b>Inserir URL do arquivo de vídeo</b> cole o URL do arquivo de vídeo e selecione <b>Carregar</b>. <br><br>Por exemplo, se estiver usando um URL do Adobe Dynamic Media Classic para o arquivo de vídeo, clique duas vezes em um ativo de vídeo individual (não em um Conjunto de vídeos adaptados ou em um Vídeo principal) para abri-lo na Exibição de detalhes. No painel direito da Exibição de detalhes, expanda URLs e Código incorporado. Em seguida, no grupo Mobile, à direita de Mobile (Progressive), selecione <b>Copiar URL</b>. Esse processo fornece o URL para o próprio arquivo de vídeo, que você pode colar na tag <b>Inserir URL do arquivo de vídeo</b> campo. O Internet Explorer, o Chrome ou o Safari podem reproduzir nativamente o vídeo. Agora siga as instruções na tela do site para criar e salvar seu arquivo WebVTT. Quando terminar, copie o conteúdo do arquivo de legenda e cole-o em um editor de texto sem formatação e salve-o com uma extensão de nome de arquivo VTT. <br><br><b>Nota:</b> Para suporte global a legendas de vídeo em idiomas diferentes do inglês, o padrão WebVTT exige a criação de arquivos .vtt separados e chamadas para cada idioma ao qual você deseja oferecer suporte. <br><br>Geralmente, você deseja nomear o arquivo de legenda VTT com o mesmo nome do arquivo de vídeo e anexá-lo com legendas. Ao fazer isso, ele pode ajudar você a automatizar a geração dos URLs de vídeo usando seu sistema existente de gerenciamento de conteúdo na Web. |

1. No Adobe Dynamic Media Classic, carregue seu arquivo de legenda WebVTT, DFXP ou SMPTE XML.

   Consulte [Fazer upload de arquivos](uploading-files.md#uploading_files).

1. No painel Biblioteca de ativos à esquerda, navegue até a pasta de ativos que contém o arquivo de vídeo que você deseja associar ao arquivo de legenda carregado.
1. No painel Navegar por ativos, selecione um único ativo de vídeo e, abaixo da imagem em miniatura do ativo, selecione **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. Na tabela Lista do visualizador, localize o visualizador do HTML5 chamado **Universal_HTML5_Video**, **Universal_HTML5_MixedMedia_dark** ou **Universal_HTML5_MixedMedia_light**, siga um destes procedimentos:

   * Para obter uma experiência de visualizador de vídeo pop-up, selecione **[!UICONTROL Copy URL]** à direita do nome.

     Anexe o URL copiado do vídeo com a seguinte sintaxe para que você possa associá-lo ao URL copiado para o seu arquivo de legenda:

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     Observe que `,1` no final da legenda URL path. Imediatamente após a extensão de nome de arquivo VTT no caminho, é possível ativar ou desativar o botão de legendas ocultas na barra do reprodutor de vídeo, definindo como `1` ou `0`, respectivamente.

   * Para obter uma experiência de visualizador de vídeo incorporado, selecione **[!UICONTROL Embed Code]** à direita do nome.

     Na caixa de diálogo Incorporar código, selecione **[!UICONTROL Copy to Clipboard]**.

     Para o HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`ou `Universal_HTML5_MixedMedia_light` , anexe o código incorporado copiado com o seguinte:

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     Observe que `,1` no final do caminho do URL. Imediatamente após a extensão de nome de arquivo VTT no caminho do URL, é possível ativar ou desativar o botão de legenda na barra do reprodutor de vídeo, definindo como `1` ou `0`, respectivamente.
