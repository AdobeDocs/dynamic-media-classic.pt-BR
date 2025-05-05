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
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# Adicionar legendas ao vídeo {#add-captions-to-video}

Estenda o alcance de seus vídeos aos mercados globais. Você pode fazer isso adicionando legendas a vídeos únicos ou Conjuntos de vídeos adaptados. Ao adicionar legendas, você evita a necessidade de dublar o áudio ou a necessidade de usar alto-falantes nativos para regravar o áudio para cada idioma diferente. O vídeo é reproduzido no idioma em que foi gravado. Legendas em idiomas estrangeiros aparecem para que pessoas de diferentes idiomas ainda possam entender a parte de áudio.

A legenda também permite maior acessibilidade usando legendas ocultas para pessoas surdas ou com deficiência auditiva.

>[!NOTE]
>
>O reprodutor de vídeo usado deve oferecer suporte à exibição de legendas.

Para configurar o Efeito de legenda e editar o Menu de legenda propriamente dito, incluindo o texto do menu para qualquer um dos seguintes visualizadores:

* Visualizador `Universal_HTML5_Video`
* Visualizador `Universal_HTML5_MixedMedia_dark`
* Visualizador `Universal_HTML5_MixedMedia_light`

Consulte [Adicionar ou Editar uma Predefinição do Visualizador de Vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consulte também [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

O Adobe Dynamic Media Classic pode converter arquivos de legenda para o formato JSON (JavaScript Object Notation). Essa conversão significa que você pode incorporar o texto JSON em uma página da Web como uma transcrição oculta, mas completa, do vídeo. Os mecanismos de pesquisa podem rastrear e indexar o conteúdo para facilitar a descoberta dos vídeos e fornecer aos clientes mais detalhes sobre o conteúdo do vídeo.

Consulte [Conteúdo estático (não de imagem) do servidor](https://experienceleague.adobe.com/pt-br/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api) para obter mais informações sobre como usar a função JSON em uma URL.

**Para adicionar legendas a um vídeo:**

1. Usando um aplicativo de terceiros fora do Adobe Dynamic Media Classic, crie seu arquivo de legenda de vídeo com base no tipo de visualizador que você está usando.

   | Tipo de visualizador | Arquivo de legendas |
   |--- |--- |
   | HTML5 | Se estiver usando um visualizador de vídeo HTML5, certifique-se de que o arquivo de legenda criado segue o padrão WebVTT (Web Video Text Tracks, Rastreamentos de texto de vídeo da Web). A extensão do nome de arquivo de legendagem é `.VTT`. Você pode obter mais informações sobre o padrão de legendagem WebVTT.<br><br>[Consulte WebVTT](https://w3c.github.io/webvtt/): o formato de Rastreamento de Texto de Vídeo da Web. <br><br>Há muitos sites que oferecem ferramentas e serviços gratuitos e pagos que você pode usar para criar arquivos de legenda WebVTT. <br><br>Siga as instruções na tela de um site para criar e salvar seu arquivo WebVTT. Quando terminar, copie o conteúdo do arquivo de legenda e cole-o em um editor de texto sem formatação e salve-o com uma extensão de nome de arquivo VTT. <br><br><b>Observação:</b> para obter suporte global a legendas de vídeo em idiomas diferentes do inglês, o padrão WebVTT exige a criação de `.VTT` arquivos e chamadas separados para cada idioma ao qual você deseja oferecer suporte. <br><br>Geralmente, você deseja nomear o arquivo de legenda VTT com o mesmo nome do arquivo de vídeo e anexá-lo com legendas. Ao fazer isso, ele pode ajudar você a automatizar a geração dos URLs de vídeo usando seu sistema existente de gerenciamento de conteúdo da Web. |

1. No Adobe Dynamic Media Classic, carregue seu arquivo de legenda WebVTT, DFXP ou SMPTE XML.

   Consulte [Carregar arquivos](uploading-files.md#uploading_files).

1. No painel Biblioteca de ativos à esquerda, navegue até a pasta de ativos que contém o arquivo de vídeo a ser associado ao arquivo de legenda carregado.
1. No painel Navegar por ativos, selecione um único ativo de vídeo e, abaixo da imagem em miniatura do ativo, selecione **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. Na tabela Lista do Visualizador, localize o visualizador do HTML5 chamado **Universal_HTML5_Video**, **Universal_HTML5_MixedMedia_dark** ou **Universal_HTML5_MixedMedia_light**, e siga um destes procedimentos:

   * Para uma experiência de visualizador de vídeo pop-up, selecione **[!UICONTROL Copy URL]** na extremidade direita do nome.

     Anexe o URL copiado do vídeo com a seguinte sintaxe para que você possa associá-lo ao URL copiado para o seu arquivo de legenda:

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     Observe o `,1` no final do caminho de URL da legenda. Imediatamente após a extensão de nome de arquivo VTT no caminho, você pode ativar ou desativar o botão de legendas ocultas na barra do reprodutor de vídeo definindo como `1` ou `0`, respectivamente.

   * Para uma experiência de visualizador de vídeo incorporado, selecione **[!UICONTROL Embed Code]** na extremidade direita do nome.

     Na caixa de diálogo Incorporar código, selecione **[!UICONTROL Copy to Clipboard]**.

     Para os visualizadores HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark` ou `Universal_HTML5_MixedMedia_light`, anexe o Código de inserção copiado com o seguinte:

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     Observe o `,1` no final do caminho de URL. Imediatamente após a extensão de nome de arquivo VTT no caminho da URL, você pode, opcionalmente, ativar ou desativar o botão de legenda na barra do reprodutor de vídeo definindo como `1` ou `0`, respectivamente.
