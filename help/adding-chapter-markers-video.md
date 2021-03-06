---
title: Adicionar marcadores de capítulo ao vídeo
description: Saiba como adicionar marcadores de capítulo a um vídeo no Adobe Dynamic Media Classic.
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 0%

---

# Adicionar marcadores de capítulo ao vídeo {#adding-chapter-markers-to-video}

Você pode tornar seus vídeos de formulário longos mais fáceis de assistir e navegar adicionando marcadores de capítulo a vídeos individuais ou aos Conjuntos de vídeos adaptáveis. Quando um usuário reproduz o vídeo, ele pode selecionar os marcadores de capítulo na linha do tempo do vídeo (também conhecidos como depurador de vídeo). Isso permite que eles naveguem facilmente em seu ponto de interesse ou pulem imediatamente para novos conteúdos, demonstrações, tutoriais e assim por diante.

>[!NOTE]
>
>O reprodutor de vídeo usado deve suportar o uso de marcadores de capítulo.

Consulte [Adicionar ou editar uma predefinição do visualizador de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) se desejar configurar os pontos de sinalização de navegação do capítulo e o texto pop-up do título do capítulo para o visualizador `Universal_HTML5_Video` (HTML5).

Consulte também [Adicionar e editar Predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

Você cria uma lista de capítulo para o vídeo da mesma forma que cria legendas. Ou seja, você cria um arquivo WebVTT. Observe, no entanto, que esse arquivo deve ser separado de qualquer arquivo de legenda WebVTT que você também possa estar usando; não é possível combinar legendas e capítulos em um arquivo WebVTT.

Você pode usar a seguinte amostra como exemplo do formato usado para criar um arquivo WebVTT com navegação de capítulo:

```as3
WEBVTT 
Chapter 1 
00:00.000 --> 01:04.364 
The bicycle store behind it all. 
Chapter 2 
01:04.364 --> 02:00.944 
Creative Cloud. 
Chapter 3 
02:00.944 --> 03:02.937 
Ease of management for a working solution. 
Chapter 4 
03:02.937 --> 03:35.000 
Cost-efficient access to rapidly evolving technology.
```

No exemplo acima, `Chapter 1` é o identificador de sinalização e é opcional. A hora de sinalização de `00:00:000 --> 01:04:364` especifica a hora de início e a hora de término do capítulo, no formato 00:00:000. Os últimos três dígitos são milissegundos e podem ser deixados como 000, se preferir. O título do capítulo de `The bicycle store behind it all` é a descrição real do conteúdo do capítulo. O identificador de sinalização, a hora de início e o título do capítulo são exibidos em uma pop-up no reprodutor de vídeo quando o ponteiro é posicionado sobre um ponto de sinalização visual na linha do tempo do vídeo.

Como você está usando um visualizador de vídeo HTML5, certifique-se de que o arquivo de capítulo criado siga o padrão WebVTT (Web Video Text Tracks). A extensão do nome de arquivo do capítulo é .VTT. Você pode obter mais informações sobre o padrão de legendagem WebVTT.

Consulte [WebVTT: O Texto de Vídeo da Web Rastreia o Formato](https://w3c.github.io/webvtt/).

**Para adicionar marcadores de capítulo ao vídeo:**

1. Usando um editor de texto simples fora do Adobe Dynamic Media Classic, crie seu arquivo de capítulo de vídeo.

   >[!NOTE]
   >
   >Para oferecer suporte global a capítulos de vídeo em idiomas diferentes do inglês, o padrão WebVTT requer a criação de arquivos .vtt e chamadas separados para cada idioma que você deseja suportar.

1. Salve o arquivo VTT na codificação UTF8 para evitar problemas com a representação de caracteres no texto do título do capítulo.

   Geralmente, você deseja nomear o arquivo VTT do capítulo com o mesmo nome do arquivo de vídeo e anexá-lo com `chapters`. Ao fazer isso, ele pode ajudá-lo a automatizar a geração dos URLs de vídeo usando seu sistema de gerenciamento de conteúdo da Web existente.

1. No Adobe Dynamic Media Classic, faça o upload do arquivo de capítulo WebVTT.

   Consulte [Fazer upload de arquivos](uploading-files.md#uploading_files).

1. No painel Biblioteca de ativos, à esquerda, navegue até a pasta de ativos que contém o arquivo de vídeo a ser associado ao arquivo de capítulo carregado.
1. No painel Navegação de ativos , selecione um único ativo de vídeo e, em seguida, abaixo da imagem em miniatura do ativo, selecione **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. Na tabela Lista de visualizadores , localize o visualizador HTML5 chamado **Universal_HTML5_Video** e siga um destes procedimentos:

   * Para obter uma experiência do visualizador de vídeo pop-up, selecione **[!UICONTROL Copy URL]** na extremidade direita do nome.

      Anexe o URL copiado do vídeo com a seguinte sintaxe para associá-lo ao URL copiado para o arquivo da legenda:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Para uma experiência de visualizador de vídeo incorporado, selecione **[!UICONTROL Embed Code]** na extremidade direita do nome.

      Na caixa de diálogo Incorporar código, selecione **[!UICONTROL Copy to Clipboard]**.

      Para o visualizador HTML5 `Universal_HTML5_Video`, anexe o código incorporado copiado com o seguinte:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
