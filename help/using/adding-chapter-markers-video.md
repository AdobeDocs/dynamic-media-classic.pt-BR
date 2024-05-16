---
title: Adicionar marcadores de capítulo ao vídeo
description: Saiba como adicionar marcadores de capítulo a um vídeo no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Adicionar marcadores de capítulo ao vídeo {#adding-chapter-markers-to-video}

Você pode facilitar a visualização e a navegação dos vídeos de formulário longo adicionando marcadores de capítulo a vídeos únicos ou aos Conjuntos de vídeos adaptados. Quando um usuário reproduz o vídeo, ele pode selecionar os marcadores de capítulo na linha do tempo do vídeo (também conhecido como depurador do vídeo). Isso permite que eles naveguem facilmente para o ponto de interesse ou acessem imediatamente novos conteúdos, demonstrações, tutoriais e assim por diante.

>[!NOTE]
>
>O reprodutor de vídeo usado deve aceitar o uso de marcadores de capítulo.

Consulte [Adicionar ou editar uma predefinição do visualizador de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) se quiser configurar os pontos de sinalização de navegação do capítulo e o texto pop-up do título do capítulo para o `Universal_HTML5_Video` (HTML5).

Consulte também [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

Uma lista de capítulos é criada para o vídeo da mesma maneira que as legendas. Ou seja, você cria um arquivo WebVTT. Observe, no entanto, que esse arquivo deve ser separado de qualquer arquivo de legenda WebVTT que você também possa estar usando; não é possível combinar legendas e capítulos em um arquivo WebVTT.

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

No exemplo acima, `Chapter 1` é o identificador de sinalização e é opcional. A hora da indicação de `00:00:000 --> 01:04:364` especifica a hora inicial e final do capítulo, em 00:00:formato 000. Os últimos três dígitos são milissegundos e podem ser deixados como 000, se preferir. O título do capítulo de `The bicycle store behind it all` é a descrição real do conteúdo do capítulo. O identificador de sinalização, o tempo de sinalização inicial e o título do capítulo são exibidos em um pop-up no reprodutor de vídeo quando o ponteiro é posicionado sobre um ponto de sinalização visual na linha do tempo do vídeo.

Como você está usando um visualizador de vídeo HTML5, certifique-se de que o arquivo de capítulo criado segue o padrão WebVTT (Rastreamento de texto de vídeo da Web). A extensão de nome de arquivo do capítulo é `.VTT`. Você pode obter mais informações sobre o padrão de legendagem WebVTT.

Consulte [WebVTT: o formato de rastreamento de texto de vídeo na Web](https://w3c.github.io/webvtt/).

**Para adicionar marcadores de capítulo a um vídeo:**

1. Usando um editor de texto simples fora do Adobe Dynamic Media Classic, crie seu arquivo de capítulo de vídeo.

   >[!NOTE]
   >
   >Para suporte global de capítulos de vídeo em idiomas diferentes do inglês, o padrão WebVTT exige a criação de capítulos separados `.VTT` arquivos e chamadas para cada idioma que você deseja suportar.

1. Salve o arquivo VTT na codificação UTF8 para que você possa evitar problemas com a representação de caracteres no texto do título do capítulo.

   Geralmente, você deseja nomear o arquivo de VTT do capítulo com o mesmo nome do arquivo de vídeo e anexá-lo com `chapters`. Ao fazer isso, ele pode ajudar você a automatizar a geração dos URLs de vídeo usando seu sistema existente de gerenciamento de conteúdo da Web.

1. No Adobe Dynamic Media Classic, carregue seu arquivo de capítulo WebVTT.

   Consulte [Fazer upload de arquivos](uploading-files.md#uploading_files).

1. No painel Biblioteca de ativos à esquerda, navegue até a pasta de ativos que contém o arquivo de vídeo a ser associado ao arquivo de capítulo que você carregou.
1. No painel Navegar por ativos, selecione um único ativo de vídeo e, abaixo da imagem em miniatura do ativo, selecione **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. Na tabela Lista do visualizador, localize o visualizador do HTML5 chamado **Universal_HTML5_Video**, e siga um destes procedimentos:

   * Para obter uma experiência de visualizador de vídeo pop-up, selecione **[!UICONTROL Copy URL]** à direita do nome.

     Anexe o URL copiado do vídeo com a seguinte sintaxe para que você possa associá-lo ao URL copiado para o seu arquivo de legenda:

     `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Para obter uma experiência de visualizador de vídeo incorporado, selecione **[!UICONTROL Embed Code]** à direita do nome.

     Na caixa de diálogo Incorporar código, selecione **[!UICONTROL Copy to Clipboard]**.

     Para o HTML5 `Universal_HTML5_Video` , anexe o Código incorporado copiado com o seguinte:

     `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*"`
