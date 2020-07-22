---
title: Adicionar marcadores de capítulo ao vídeo
seo-title: Adicionar marcadores de capítulo ao vídeo
description: nulo
seo-description: Saiba como adicionar marcadores de capítulo a um vídeo.
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---


# Adicionar marcadores de capítulo ao vídeo{#adding-chapter-markers-to-video}

Você pode facilitar a visualização e navegação de seus vídeos de formulário longos adicionando marcadores de capítulo a vídeos únicos ou a Conjuntos de vídeos adaptáveis. Quando um usuário reproduz o vídeo, ele pode clicar nos marcadores de capítulo na linha do tempo do vídeo (também conhecido como depurador de vídeo) para navegar facilmente até seu ponto de interesse ou imediatamente pular para novo conteúdo, demonstrações, tutoriais e assim por diante.

>[!NOTE]
>
>O player de vídeo usado deve suportar o uso de marcadores de capítulo.

Consulte [Adicionar ou editar uma predefinição](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) do visualizador de vídeo para configurar os pontos de sinalização de navegação do capítulo e o texto pop-up do título do capítulo para o `Universal_HTML5_Video` visualizador (HTML5).

Consulte também [Adicionar e editar predefinições](application-setup.md#adding_and_editing_viewer_presets)do visualizador.

Você cria uma lista de capítulo para o seu vídeo da mesma forma que cria legendas. Ou seja, você cria um arquivo WebVTT. Observe, no entanto, que esse arquivo deve ser separado de qualquer arquivo de legenda WebVTT que você também esteja usando; não é possível combinar legendas e capítulos em um arquivo WebVTT.

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

No exemplo acima, `Chapter 1` é o identificador de sinalização e é opcional. A hora de sinalização de `00:00:000 --> 01:04:364` especifica a hora de start e a hora de término do capítulo, no formato 00:00:00. Os últimos três dígitos são milissegundos e podem ser deixados como 000, se preferir. O título do capítulo é `The bicycle store behind it all` a descrição real do conteúdo do capítulo. O identificador de sinalização, a hora de início e o título do capítulo são exibidos em um pop-up no player de vídeo quando um usuário posiciona o ponteiro do mouse sobre um ponto de sinalização visual na linha do tempo do vídeo.

Como você está usando um visualizador de vídeo HTML5, verifique se o arquivo de capítulo criado segue o padrão WebVTT (Web Video Text Tracks). A extensão do nome do arquivo do capítulo é .vtt. Você pode obter mais informações sobre o padrão de legendagem WebVTT.

Consulte [WebVTT: O formato](https://dev.w3.org/html5/webvtt/)de Rastreamento de texto de vídeo da Web.

**Para adicionar marcadores de capítulo ao vídeo**

1. Usando um editor de texto simples fora do Dynamic Media Classic, crie seu arquivo de capítulo de vídeo.

   >[!NOTE]
   >
   >Para obter suporte global para capítulos de vídeo em idiomas diferentes do inglês, esteja ciente de que o padrão WebVTT exige a criação de arquivos .vtt separados e chamadas para cada idioma que você deseja suportar.

1. Salve o arquivo .vtt na codificação UTF8 para evitar problemas com renderização de caracteres no texto do título do capítulo.

   Geralmente, você deseja nomear o arquivo VTT do capítulo com o mesmo nome do arquivo de vídeo e anexá-lo a `chapters`. Ao fazer isso, ele pode ajudá-lo a automatizar a geração de URLs de vídeo usando seu sistema de gestão de conteúdo da Web existente.

1. No Dynamic Media Classic, carregue seu arquivo de capítulo WebVTT.

   Consulte [Upload de arquivos](uploading-files.md#uploading_files).

1. No painel Biblioteca de ativos, à esquerda, navegue até a pasta de ativos que contém o arquivo de vídeo que você deseja associar ao arquivo de capítulo que você carregou.
1. No painel Navegação de ativos, selecione um único ativo de vídeo e, abaixo da imagem em miniatura do ativo, clique em **Pré-visualização** > Lista **do** visualizador.
1. Na tabela Lista do visualizador, localize o visualizador HTML5 chamado **Universal_HTML5_Video** e execute um dos procedimentos a seguir:

   * Para obter uma experiência com o visualizador de vídeo pop-up, clique em **Copiar URL** à direita do nome.

      Anexe o URL copiado do vídeo com a sintaxe a seguir para associá-lo ao URL copiado ao arquivo de legenda:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Para obter uma experiência com o visualizador de vídeo incorporado, clique em **Incorporar código** à extrema direita do nome.

      Na caixa de diálogo Incorporar código, clique em **Copiar para a área de transferência**.

      Para o visualizador HTML5 `Universal_HTML5_Video` , anexe o código incorporado copiado com o seguinte:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`

