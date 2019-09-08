---
title: Adicionar legendas ao vídeo
seo-title: Adicionar legendas ao vídeo
description: 'null'
seo-description: Saiba como adicionar legendas ao vídeo
uuid: 4 cc 64469-4369-44 a 9-83 db -63 bad 51 tab 8 a
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Adicionar legendas ao vídeo{#adding-captions-to-video}

Você pode estender o alcance dos vídeos para os mercados globais adicionando legendas a vídeos únicos ou a Conjuntos de vídeos adaptativos. Ao adicionar legendas, você evita a necessidade de virar o áudio ou a necessidade de usar alto-falantes nativos para depurar o áudio para cada idioma diferente. O vídeo é reproduzido no idioma que foi registrado. Os legendas de idioma estrangeiro aparecem para que as pessoas de diferentes idiomas possam compreender a parte de áudio.

A legenda também permite maior acessibilidade usando legendas ocultas para pessoas surdas ou difíceis de ouvir.

>[!NOTE]
>
>O player de vídeo usado deve oferecer suporte à exibição de legendas.

Consulte [Adicionar ou editar uma predefinição](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) do visualizador de vídeo para configurar o Efeito de legenda e editar o próprio menu de legenda, incluindo o texto do menu para qualquer um dos seguintes visualizadores:

* `Universal_HTML5_Video` visualizador.
* `Universal_HTML5_MixedMedia_dark` visualizador.
* `Universal_HTML5_MixedMedia_light` visualizador.

Consulte [também Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

O Dynamic Media Classic tem a capacidade de converter arquivos de legenda para o formato JSON (Notascript Object Notation). Essa conversão significa que você pode incorporar o texto JSON em uma página da Web como uma transcrição oculta, mas completa do vídeo. Os mecanismos de pesquisa podem rastrear e indexar o conteúdo para tornar os vídeos mais facilmente detectáveis e fornecer aos clientes detalhes adicionais sobre o conteúdo do vídeo.

Consulte [Conteúdo estático (não imagem)](https://marketing.adobe.com/resources/help/en_US/s7/is_ir_api/is_api/c_serving_static_nonimage_contents.html) na Ajuda da API de disponibilização de imagens *da Adobe* para obter mais informações sobre o uso da função JSON em um URL.

**Adicionar legendas ao vídeo**

1. Usando um aplicativo de terceiros fora do Scene 7 Publishing System, crie o arquivo de legenda de vídeo com base no tipo de visualizador usado.

   | Tipo de visualizador | Arquivo de legenda |
   |--- |--- |
   | HTML5 | Se estiver usando um visualizador de vídeo HTML 5, certifique-se de que o arquivo de legenda criado siga o padrão webvtt (Web Video Text Faixas). A extensão de nome de arquivo de legenda é. vtt. Você pode obter mais informações sobre o padrão de legendagem webvtt.<br><br>[Consulte webvtt](https://dev.w3.org/html5/webvtt/): O formato Faixas de texto do vídeo na Web. <br><br>Há tanto as ferramentas como os serviços que você pode usar para criar arquivos de legenda fora do Scene 7 Publishing System. Por exemplo, para criar um arquivo de legenda de vídeo simples sem estilo, você pode usar a seguinte ferramenta gratuita de criação e edição de legenda online: <br><br>[Criador de legendas webvtt](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>para obter melhores resultados, use a ferramenta no Internet Explorer 9 ou superior, no Google Chrome ou no Safari. <br><br>Na ferramenta, <b>insira o URL do campo de arquivo</b> de vídeo, cole o URL do arquivo de vídeo e clique <b>em Carregar</b>. <br><br>Por exemplo, se você estiver usando um URL do Dynamic Media Classic para seu arquivo de vídeo, no SPS, clique duas vezes em um ativo de vídeo individual (não um Conjunto de vídeos adaptativo ou Vídeo mestre) para abri-lo na Exibição de detalhes. No painel direito da Exibição de detalhes, expanda urls e Código incorporado. Em seguida, no grupo Móvel, à direita do Mobile (Progressivo), clique em Copiar URL. Esse processo fornece a URL para o arquivo de vídeo em si, que é possível colar no <b>campo Inserir URL do campo de arquivo</b> de vídeo. O Internet Explorer, o Chrome ou o Safari pode reproduzir o vídeo de forma nativa. Agora siga as instruções na tela do site para criar e salvar seu arquivo webvtt. Quando terminar, copie o conteúdo do arquivo de legenda e cole-o em um editor de texto sem formatação e salve-o com uma extensão de arquivo. vtt. <br><br><b>Observação:</b> Para o suporte global de legendas de vídeo em idiomas diferentes do inglês, esteja ciente de que o padrão webvtt exige que você crie arquivos. vtt separados e chama cada idioma que deseja suportar. <br><br>Geralmente, você deseja nomear o arquivo de legenda VTT do mesmo nome que o arquivo de vídeo e anexá-lo com legendas. Ao fazer isso, ele pode ajudar você com automatizar a geração dos urls de vídeo usando seu sistema existente de gerenciamento de conteúdo da Web. |

1. No Scene 7 Publishing System, carregue o arquivo de legenda webvtt, DFXP ou SMPTE XML.

   Consulte [Carregamento de arquivos](uploading-files.md#uploading_files).

1. No painel Biblioteca de ativos do lado esquerdo, navegue até a pasta de ativos que contém o arquivo de vídeo que você deseja associar ao arquivo de legenda que você carregou.
1. No painel Procurar ativo, selecione um único ativo de vídeo e depois abaixo da imagem em miniatura do ativo, clique **em Visualizar** &gt; Lista **do visualizador**.
1. Na tabela Lista de visualizadores, localize o visualizador HTML 5 chamado **Mundial_ HTML 5_ Video**, **Universal_ HTML 5_ mixedmedia_ escuro** ou **Universal_ HTML 5_ mixedmedia_ light** e execute um dos procedimentos a seguir:

   * Para uma experiência de visualizador de vídeo pop-up, clique **em Copiar URL** para a extremidade direita do nome.

      Anexe o URL copiado do vídeo com a seguinte sintaxe para associá-la ao URL copiado ao arquivo de legenda:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Observe o `,1` final do caminho de URL de legenda. Imediatamente após a extensão de nome de arquivo. vtt no caminho, você tem a opção de ativar ou desativar o botão de legenda oculta na barra do player de vídeo ao configurar ou `1``0`, respectivamente.

   * Para uma experiência de visualizador de vídeo incorporada, clique **em Incorporar código** à direita do nome.

      Na caixa de diálogo Incorporar código, clique **em Copiar para a área de transferência**.

      Para o HTML 5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`ou `Universal_HTML5_MixedMedia_light` visualizadores, anexe o código incorporado copiado com o seguinte:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Observe o `,1` final do caminho do URL. Imediatamente após a extensão de nome de arquivo. vtt no caminho do URL, você tem a opção de ativar ou desativar o botão da legenda na barra do player de vídeo ao configurar ou `1``0`, respectivamente.

