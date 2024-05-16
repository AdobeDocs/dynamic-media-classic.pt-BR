---
title: "Início rápido: vídeo no Adobe Dynamic Media Classic"
description: Uma introdução e o Quick Start do Adobe Dynamic Media Classic Video para ajudá-lo a começar a usar o rapidamente.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
topic: Content Management
level: Beginner
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 0%

---

# Início rápido: vídeo no Adobe Dynamic Media Classic{#quick-start-video}

O Adobe Dynamic Media Classic Video é uma solução completa que facilita a publicação de vídeo adaptável de alta qualidade para transmissão em várias telas, incluindo dispositivos móveis para desktop, iOS, Android™, BlackBerry® e Windows®. Um Conjunto de vídeos adaptados agrupa versões do mesmo vídeo codificadas em taxas de bits e formatos diferentes, como 400 kbps, 800 kbps e 1000 kbps. O computador desktop ou dispositivo móvel detecta a largura de banda disponível.

Por exemplo, em um dispositivo móvel iOS, ele detecta uma largura de banda como 3G, 4G ou Wi-Fi. Em seguida, ele seleciona automaticamente o vídeo codificado correto entre as várias taxas de bits de vídeo no Conjunto de vídeos adaptados. O vídeo é transmitido para desktops, dispositivos móveis ou tablets.

Além disso, a qualidade do vídeo é comutada automaticamente de forma dinâmica se as condições da rede forem alteradas no desktop ou no dispositivo móvel. Além disso, se um cliente entrar no modo de tela cheia em um desktop, o Conjunto de vídeos adaptados responderá usando uma resolução melhor, melhorando a experiência de visualização do cliente. O uso dos Conjuntos de vídeos adaptados oferece a melhor reprodução possível. É melhor para clientes que reproduzem o Adobe Dynamic Media Classic Video em várias telas e dispositivos.

A lógica que um reprodutor de vídeo usa para determinar qual vídeo codificado reproduzir ou selecionar durante a reprodução se baseia no seguinte algoritmo:

1. O reprodutor de vídeo carrega o fragmento de vídeo inicial com base na taxa de bits mais próxima do valor definido como &quot;taxa de bits inicial&quot; no próprio reprodutor.
1. O reprodutor de vídeo muda com base nas alterações na velocidade da largura de banda, usando os seguintes critérios:

   1. O player escolhe o fluxo de largura de banda mais alto abaixo ou igual à largura de banda estimada.
   1. O player considera apenas 80% da largura de banda disponível. No entanto, se estiver mudando, é mais conservador em apenas 70% para evitar superestimar e voltar imediatamente.

Consulte a lógica do algoritmo em [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) para obter informações técnicas sobre ele.

Para gerenciar vídeos únicos e Conjuntos de vídeos adaptados, o Adobe Dynamic Media Classic é compatível com o seguinte:

* Fazer upload de vídeo a partir de vários formatos de vídeo compatíveis. E, fazendo upload de formatos de áudio e codificação de vídeo para o formato MP4 H.264 para reprodução em várias telas. Você pode usar predefinições predefinidas do Adobe Dynamic Media Classic Adaptive Video, predefinições de codificação de vídeo único ou personalizar sua própria codificação para controlar a qualidade e o tamanho do vídeo.

Consulte [Ativar ou desativar predefinições de vídeo adaptável](/help/using/application-setup.md#activating-or-deactivating-adaptive-video-presets)

Consulte também [Predefinições de vídeo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) vídeo de treinamento.

Quando um Conjunto de vídeos adaptados é gerado, ele inclui vídeos MP4.

>[!NOTE]
>
>Vídeos primários/de origem e qualquer outro vídeo de formato de origem são *não* adicionado a um Conjunto de vídeos adaptados.

* Legenda de vídeo nos visualizadores Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark e Universal_HTML5_MixedMedia_light e navegação de capítulo de vídeo nos visualizadores Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark e Universal_HTML5_MixedMedia_light.

  Consulte [Adicionar legendas a um vídeo](adding-captions-video.md).

  Consulte [Adicionar marcadores de capítulo a um vídeo](adding-chapter-markers-video.md).

* Organize, navegue e pesquise vídeos com suporte completo a metadados para obter um gerenciamento eficiente dos ativos de vídeo.
* Forneça Conjuntos de vídeos adaptados para a Web e para desktops e dispositivos móveis, incluindo iPhone, iPad, Android™, BlackBerry® e Windows® phone.

  O streaming de vídeo adaptável é suportado em várias plataformas iOS.

  Veja o suporte mais recente na [Guia de referência de visualizadores do Adobe](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources).

  O Adobe Dynamic Media Classic oferece suporte à reprodução de vídeo móvel para vídeo MP4 H.264. <!-- LINK IS 404; NO SUITABLE REPLACEMENT WAS FOUND You can find BlackBerry&reg; devices that support this video format at the following website: -->

  <!-- See [Supported video formats on BlackBerry&reg;](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482). -->

  Você pode encontrar dispositivos Windows® compatíveis com este formato de vídeo no link a seguir:

  [Formatos de vídeo compatíveis com o Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs).

* Reproduza o vídeo usando as Predefinições do visualizador do Adobe Dynamic Media Classic, incluindo o seguinte:

   * Visualizadores de vídeo único.
   * Visualizadores de mídia mista que combinam conteúdo de vídeo e imagem.

* Configure players de vídeo para atender às suas necessidades de marca.
* Integre vídeo ao seu site, site móvel ou aplicativo móvel com um URL simples ou Código incorporado.

Consulte os seguintes vídeos de treinamento:
* [Visão geral do vídeo MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [Pré-visualização de vídeo MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [Upload de vídeo MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [Visão geral do streaming](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**Início rápido**

A descrição do fluxo de trabalho passo a passo a seguir foi projetada para ajudar você a começar a usar rapidamente os Conjuntos de vídeos adaptados no Adobe Dynamic Media Classic. Após cada etapa, há uma referência cruzada a um cabeçalho de tópico onde você pode encontrar mais informações.

## 1. Fazer upload e codificar vídeos

Carregue e gere conjuntos de vídeos adaptáveis usando um dos dois cenários a seguir:

* **Carregar vídeos pré-codificados**: se seus vídeos já tiverem sido codificados externamente a partir do Adobe Dynamic Media Classic, na barra Navegação global, selecione **[!UICONTROL Upload]**. Procure e faça upload de arquivos de vídeo MP4 diretamente para o Adobe Dynamic Media Classic. Em seguida, acesse **[!UICONTROL Build]** > **[!UICONTROL Adaptive Video Sets]**. Navegue até os arquivos de vídeo. Arraste e solte os arquivos de vídeo desejados na tabela Conjunto de vídeos adaptados e salve o conjunto.
* **Fazer upload de vídeos de origem primária**: Se os vídeos não estiverem codificados, na barra de Navegação global, selecione **[!UICONTROL Upload]** para carregar arquivos de origem de vídeo principal (não MP4). O Adobe Dynamic Media Classic os codifica em arquivos MP4 para você. No **[!UICONTROL Upload Job Options]** caixa de diálogo, em **[!UICONTROL EVideo Options]**, selecione **[!UICONTROL Adaptive Video]**.

  Com essa opção preferida, é possível criar Conjuntos de vídeos adaptados. A predefinição de codificação correta é aplicada automaticamente ao vídeo, 16:9 ou 4:3, para corresponder às dimensões do vídeo carregado. Quando você envia seu trabalho de upload, um Conjunto de vídeos adaptados é criado automaticamente para você, que inclui três configurações de codificação de vídeo na taxa de proporção correta.

  Ou, no mesmo **[!UICONTROL Job Options]** caixa de diálogo, em **[!UICONTROL EVideo Options]**, expandir **[!UICONTROL Single Encoding Presets]**. Selecione as predefinições individuais de codificação de vídeo desejadas. É possível selecionar **Desktop**, **Móvel (iPhone, iPad, Android™)**, e **Tablet (iPad, Android™)** para criar os arquivos MP4.

* Ou você pode reprocessar um vídeo principal usando a variável **[!UICONTROL Reprocessing]** recurso. Os vídeos recém-codificados são adicionados ao Conjunto de vídeos adaptados existente.

Consulte [Fazer upload e codificar vídeos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Opcional**

O Adobe Dynamic Media Classic oferece várias predefinições predefinidas de codificação de vídeo. Essas predefinições refletem as configurações de codificação de vídeo mais comuns usadas hoje e são otimizadas para reprodução em páginas de destino.

No entanto, se mais personalizações forem necessárias, os administradores poderão criar Predefinições de vídeo para personalizar o tamanho e a experiência de reprodução de Vídeos para os usuários finais. Os administradores podem adicionar e gerenciar Predefinições de vídeo na página Predefinições de vídeo, disponível em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Single Encoding Presets]**. A página Predefinições de vídeo oferece opções para adicionar, editar, excluir e ativar predefinições de vídeo.

Consulte [Trabalhar com predefinições de codificação de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Visualizar vídeos em um visualizador de vídeo

Para ver como um vídeo é reproduzido para usuários finais em um desktop, site ou dispositivo móvel, selecione o vídeo no Painel de navegação. Em seguida, selecione **[!UICONTROL Preview]**.

Consulte [Visualizar vídeos em um visualizador de vídeo](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Você pode reproduzir o vídeo na página Visualizar. Você também pode escolher visualizadores de vídeo diferentes para descobrir como seu vídeo é exibido em diferentes players. Como prática recomendada, use o reprodutor de vídeo HTML5 para reprodução de várias telas em dispositivos desktop, tablets e dispositivos móveis.

**Opcional**

Personalização da predefinição do visualizador: o Adobe Dynamic Media Classic oferece Predefinições do visualizador predefinidas para entrega de vídeo. Essas predefinições determinam a aparência do Visualizador e como seus controles de reprodução funcionam. Para personalizar o visualizador de vídeo, os administradores podem adicionar e gerenciar Predefinições do visualizador na página Predefinições do visualizador. Para abrir esta página, no canto superior direito do Adobe Dynamic Media Classic, acesse **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**. A página Predefinições do visualizador oferece comandos para adicionar, editar, excluir e ativar as Predefinições do visualizador.

Consulte [Trabalhar com predefinições do visualizador de vídeo](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

Consulte também [Predefinições de vídeo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) vídeo de treinamento.

## 3. Implante vídeos em seus sites e sites móveis

Para integrar vídeos ao seu site, você pode executar um dos seguintes procedimentos:

* Exibir o vídeo em sua própria janela pop-up ou modal; nesse caso, use **[!UICONTROL Copy URL]** recurso.

  Para obter o URL para um vídeo, na Exibição em grade ou na Exibição em lista, selecione-o no Painel de navegação. Selecionar **[!UICONTROL Preview]** e selecione **[!UICONTROL Copy URL]** à direita de `Universal_HTML5_Viewer`.

  Ao selecionar **[!UICONTROL Copy URL]**, o URL é copiado para a Área de transferência. Coloque esse código na HTML do site, site para dispositivos móveis ou aplicativo.

  >[!NOTE]
  >
  >Os URLs são ativados somente após a publicação do vídeo ou do Conjunto de vídeos adaptados.

* Exibir o vídeo incorporado na página da Web, nesse caso, use o **[!UICONTROL Embed Code]** recurso.

  Para obter o código incorporado de um vídeo, na exibição em grade ou em lista, selecione o vídeo no painel Procurar. Ir para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**. Na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]** à direita de `Universal_HTML5_Video`. Não é permitido editar o código.

  Selecionar **[!UICONTROL Close]** e cole o Código de inserção em uma ou mais páginas da Web.

  >[!NOTE]
  >
  >O código de inserção só é ativado após a publicação do vídeo ou do Conjunto de vídeos adaptados.

Consulte [Implantar vídeo em seus sites e sites móveis](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Práticas recomendadas para codificação de vídeo](uploading-encoding-videos.md#best_practices_for_video_encoding)
