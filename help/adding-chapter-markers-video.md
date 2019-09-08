---
title: Adicionar marcadores de capítulo ao vídeo
seo-title: Adicionar marcadores de capítulo ao vídeo
description: 'null'
seo-description: Saiba como adicionar marcadores de capítulo a um vídeo.
uuid: 4 e 1 e 6 daf-afc 6-49 d 9-ac 90-183 fe 2 a 903 b 2
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/vídeo
discoiquuid: 8 bc 5 e 552-2 abb -41 f 0-89 d 2-bdf 3 ae 5 d 96 c 2
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Adicionar marcadores de capítulo ao vídeo{#adding-chapter-markers-to-video}

É possível tornar os vídeos de formulário longos mais fáceis de assistir e navegar adicionando marcadores de capítulo a vídeos únicos ou a Conjuntos de vídeos adaptativos. Quando um usuário reproduz o vídeo, ele pode clicar nos marcadores de capítulo na linha do tempo do vídeo (também conhecido como depurador de vídeo) para navegar facilmente para o ponto de interesse, ou ir imediatamente para novo conteúdo novo, demonstração, tutoriais etc.

>[!NOTE]
>
>O player de vídeo usado deve suportar o uso de marcadores de capítulo.

Consulte [Adicionar ou editar uma predefinição do visualizador de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) para configurar os pontos de sinalização de navegação do capítulo e o texto pop-up do título do capítulo para o `Universal_HTML5_Video` visualizador (HTML 5).

Consulte [também Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

Crie uma lista de capítulos para seu vídeo de forma semelhante à criação de legendas. Ou seja, você cria um arquivo webvtt. Observe, no entanto, que esse arquivo deve estar separado de qualquer arquivo de legenda webvtt que você também possa usar; não é possível combinar legendas e capítulos em um arquivo webvtt.

Você pode usar a amostra a seguir como um exemplo do formato usado para criar um arquivo webvtt com navegação de capítulo:

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

No exemplo acima, `Chapter 1` é o identificador de sinalização e é opcional. O tempo de sinalização de `00:00:000 --> 01:04:364` especifica a hora de início e a hora de término do capítulo, no formato 00:00:000. Os três últimos dígitos são milissegundos e podem ser deixados como 000, se preferirem. O título do capítulo é `The bicycle store behind it all` a descrição real do conteúdo do capítulo. O identificador de indicação, o tempo de cue inicial e o título do capítulo aparecem em um pop-up no player de vídeo quando um usuário passa o ponteiro do mouse sobre um ponto de sinalização visual na linha do tempo do vídeo.

Como você está usando um visualizador de vídeo HTML 5, certifique-se de que o arquivo de capítulo criado siga o padrão webvtt (Web Video Text Faixas). A extensão de nome de arquivo do capítulo é. vtt. Você pode obter mais informações sobre o padrão de legendagem webvtt.

Consulte [webvtt: O formato Faixas de texto do vídeo na Web](https://dev.w3.org/html5/webvtt/).

**Adicionar marcadores de capítulo ao vídeo**

1. Usando um editor de texto simples fora do Scene 7 Publishing System, crie seu arquivo de capítulo de vídeo.

   >[!NOTE]
   >
   >Para o suporte global de capítulos de vídeo em idiomas diferentes do inglês, esteja ciente de que o padrão webvtt exige que você crie arquivos. vtt separados e chama cada idioma que deseja suportar.

1. Salve o arquivo. vtt na codificação UTF 8 para evitar problemas com a execução de caracteres no texto do título do capítulo.

   Geralmente, você quer nomear o capítulo VTT do mesmo nome que o arquivo de vídeo e anexá-lo `chapters`. Ao fazer isso, ele pode ajudar você com automatizar a geração dos urls de vídeo usando seu sistema existente de gerenciamento de conteúdo da Web.

1. No Scene 7 Publishing System, carregue o arquivo de capítulo do webvtt.

   Consulte [Carregamento de arquivos](uploading-files.md#uploading_files).

1. No painel Biblioteca de ativos do lado esquerdo, navegue até a pasta de ativos que contém o arquivo de vídeo que você deseja associar ao arquivo de capítulo que você carregou.
1. No painel Procurar ativo, selecione um único ativo de vídeo e depois abaixo da imagem em miniatura do ativo, clique **em Visualizar** &gt; Lista **do visualizador**.
1. Na tabela Lista de visualizadores, encontre o visualizador HTML 5 denominado **Mundial_ HTML 5_ Video** e execute um dos procedimentos a seguir:

   * Para uma experiência de visualizador de vídeo pop-up, clique **em Copiar URL** para a extremidade direita do nome.

      Anexe o URL copiado do vídeo com a seguinte sintaxe para associá-la ao URL copiado ao arquivo de legenda:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Para uma experiência de visualizador de vídeo incorporada, clique **em Incorporar código** à direita do nome.

      Na caixa de diálogo Incorporar código, clique **em Copiar para a área de transferência**.

      Para `Universal_HTML5_Video` o visualizador HTML 5, anexe o código incorporado copiado com o seguinte:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`

