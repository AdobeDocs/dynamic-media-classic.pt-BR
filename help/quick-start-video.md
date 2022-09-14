---
title: "Início rápido: Vídeo no Adobe Dynamic Media Classic"
description: Uma introdução e o Quick Start para Adobe Dynamic Media Classic Video para ajudá-lo a ativar e executar rapidamente.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1760'
ht-degree: 0%

---

# Início rápido: Vídeo no Adobe Dynamic Media Classic{#quick-start-video}

O Adobe Dynamic Media Classic Video é uma solução completa que facilita a publicação de Vídeo adaptável de alta qualidade para transmissão em várias telas, incluindo dispositivos móveis de desktop, iOS, Android™, BlackBerry® e Windows®. Um Conjunto de vídeos adaptáveis agrupa versões do mesmo vídeo codificadas em diferentes formatos e taxas de bits, como 400 kbps, 800 kbps e 1000 kbps. O computador desktop ou dispositivo móvel detecta a largura de banda disponível.

Por exemplo, em um dispositivo móvel iOS, ele detecta uma largura de banda como 3G, 4G ou Wi-Fi. Em seguida, ele seleciona automaticamente o vídeo codificado direito dentre as várias taxas de bits de vídeo no Conjunto de vídeos adaptáveis. O vídeo é transmitido em desktops, dispositivos móveis ou tablets.

Além disso, a qualidade do vídeo é alternada dinamicamente automaticamente se as condições da rede mudarem no desktop ou no dispositivo móvel. Além disso, se um cliente entrar no modo de tela cheia em um desktop, o Adaptive Video Set responde usando uma resolução melhor, melhorando a experiência de visualização do cliente. O uso de conjuntos de vídeos adaptáveis fornece a melhor reprodução possível para os clientes que reproduzem o vídeo do Adobe Dynamic Media Classic em várias telas e dispositivos.

A lógica usada por um reprodutor de vídeo para determinar qual vídeo codificado reproduzir ou selecionar durante a reprodução é baseada no seguinte algoritmo:

1. O reprodutor de vídeo carrega o fragmento de vídeo inicial com base na taxa de bits mais próxima do valor definido para &quot;taxa de bits inicial&quot; no próprio reprodutor.
1. O reprodutor de vídeo é alternado com base em alterações na velocidade da largura de banda usando os seguintes critérios:

   1. O reprodutor escolhe o fluxo de largura de banda mais alto abaixo ou igual à largura de banda estimada.
   1. O Player considera apenas 80% da largura de banda disponível. No entanto, se estiver mudando, é mais conservador a apenas 70% para evitar a sobrestimação e a necessidade imediata de voltar.

Veja a lógica do algoritmo em [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) para obter informações técnicas sobre ele.

Para gerenciar vídeos únicos e conjuntos de vídeos adaptáveis, o Adobe Dynamic Media Classic suporta o seguinte:

* Upload de vídeo de vários formatos de vídeo e formatos de áudio compatíveis e codificação de vídeo para o formato MP4 H.264 para reprodução em várias telas. Você pode usar predefinições de vídeo adaptáveis predefinidas do Adobe Dynamic Media Classic, predefinições de codificação de vídeo único ou personalizar sua própria codificação para controlar a qualidade e o tamanho do vídeo.

Consulte [Ativar ou desativar predefinições de vídeo adaptável](/help/application-setup.md#activating-or-deactivating-adaptive-video-presets)

Consulte também [Predefinições de vídeo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) vídeo de treinamento.

Quando um conjunto de vídeo adaptável é gerado, ele inclui vídeos MP4.

>[!NOTE]
>
>Vídeos primários/de origem e qualquer outro vídeo de formato de origem são *not* adicionado a um Conjunto de vídeos adaptáveis.

* Legenda de vídeo nos visualizadores Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark e Universal_HTML5_MixedMedia_light e navegação de capítulo de vídeo nos visualizadores Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark e Universal_HTML5_MixedMedia_light.

   Consulte [Adicionar legendas ao vídeo](adding-captions-video.md).

   Consulte [Adicionar marcadores de capítulo ao vídeo](adding-chapter-markers-video.md).

* Organize, navegue e pesquise vídeos com suporte completo a metadados para o gerenciamento eficiente dos ativos de vídeo.
* Forneça Conjuntos de Vídeos Adaptativos para a Web e para desktops e dispositivos móveis, incluindo iPhone, iPad, Android™, BlackBerry® e o telefone Windows®.

   O streaming de vídeo adaptável é compatível com várias plataformas iOS.

   Consulte o suporte mais recente no [Guia de referência de visualizadores de Adobe](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

   O Adobe Dynamic Media Classic oferece suporte para reprodução de vídeo móvel para vídeo MP4 H.264. Você pode encontrar dispositivos BlackBerry® que suportam este formato de vídeo no seguinte site:

   Consulte [Formatos de vídeo compatíveis com o BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   Você pode encontrar dispositivos Windows® que suportam este formato de vídeo no seguinte endereço:

   Consulte [Formatos de vídeo compatíveis com o Windows® Phone](https://docs.microsoft.com/en-us/).

* Reproduzir o vídeo usando as Predefinições do visualizador do Adobe Dynamic Media Classic, incluindo o seguinte:

   * Visualizadores de vídeo individuais.
   * Visualizadores de mídia mista que combinam conteúdo de vídeo e imagem.

* Configure players de vídeo para atender às suas necessidades de marca.
* Integre vídeo ao seu site, site móvel ou aplicativo móvel com um URL simples ou código incorporado.

Veja os seguintes vídeos de treinamento:
* [Visão geral do vídeo MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [Pré-visualização de vídeo MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [Upload de vídeo MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [Visão geral de streaming](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**Início rápido**

A seguinte descrição passo a passo do fluxo de trabalho foi criada para ajudá-lo a ativar e executar rapidamente com conjuntos de vídeos adaptáveis no Adobe Dynamic Media Classic. Após cada etapa, há uma referência cruzada em um cabeçalho de tópico no qual você pode encontrar mais informações.

## 1. Fazer upload e codificar vídeos

Faça upload e gere conjuntos de vídeos adaptáveis usando um dos dois cenários a seguir:

* **Fazer upload de vídeos pré-codificados** - Se os vídeos já tiverem sido codificados fora do Adobe Dynamic Media Classic, na barra de navegação global, selecione **[!UICONTROL Upload]** para procurar e carregar arquivos de vídeo MP4 diretamente no Adobe Dynamic Media Classic. Em seguida, vá para **[!UICONTROL Build]** > **[!UICONTROL Adaptive Video Sets]**. Navegue até seus arquivos de vídeo. Arraste e solte os arquivos de vídeo que deseja na tabela Adaptive Video Set e salve o conjunto.
* **Fazer upload de vídeos de origem primária** - Se os vídeos não estiverem codificados, na barra Navegação global, selecione **[!UICONTROL Upload]** para carregar arquivos de fonte de vídeo primária (não MP4). O Adobe Dynamic Media Classic os codifica em arquivos MP4 para você. No **[!UICONTROL Upload Job Options]** caixa de diálogo, em **[!UICONTROL EVideo Options]**, selecione **[!UICONTROL Adaptive Video]**.

   Essa opção preferida permite criar um Conjunto de vídeos adaptáveis que aplica automaticamente a predefinição de codificação correta ao vídeo, seja 16:9 ou 4:3, para corresponder às dimensões do vídeo que você enviou. Quando você envia seu trabalho de upload, um Conjunto de vídeos adaptativos é criado automaticamente para você, o que inclui três configurações de vídeo codificadas na proporção correta.

   Ou, no mesmo **[!UICONTROL Job Options]** caixa de diálogo, em **[!UICONTROL EVideo Options]**, expandir **[!UICONTROL Single Encoding Presets]**. Selecione as predefinições de codificação de vídeo individuais das quais deseja **Desktop**, **Móvel (iPhone, iPad, Android™)** e **Tablet (iPad, Android™)** para criar os arquivos MP4.

* Ou você pode reprocessar um vídeo principal usando o **[!UICONTROL Reprocess]** recurso. Os vídeos recém-codificados são adicionados ao Conjunto de vídeos adaptáveis existente.

Consulte [Fazer upload e codificar vídeos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Opcional**

O Adobe Dynamic Media Classic oferece várias predefinições de codificação de vídeo predefinidas. Essas predefinições predefinidas refletem as configurações mais comuns de codificação de vídeo usadas hoje e são otimizadas para reprodução nas páginas de destino.

No entanto, se for necessária uma personalização adicional, os administradores podem criar Predefinições de vídeo para personalizar o tamanho e a experiência de reprodução de Vídeos para os usuários finais. Os administradores podem adicionar e gerenciar as Predefinições de vídeo na página Predefinições de vídeo , disponível em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Single Encoding Presets]**. A página Predefinições de vídeo oferece opções para adicionar, editar, excluir e ativar Predefinições de vídeo.

Consulte [Trabalhar com predefinições de codificação de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Visualizar vídeos em um visualizador de vídeo

Para ver como um vídeo é reproduzido para usuários finais em um desktop, site ou em um dispositivo móvel, selecione o vídeo no Painel de navegação e selecione **[!UICONTROL Preview]**.

Consulte [Visualizar vídeos em um visualizador de vídeo](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Você pode reproduzir o vídeo na página Visualização. Você também pode escolher visualizadores de vídeo diferentes para descobrir como o vídeo aparece em diferentes players. Como prática recomendada, use o reprodutor de vídeo HTML5 para reprodução de várias telas em desktops, tablets e dispositivos móveis.

**Opcional**

Personalização da predefinição do visualizador - a Adobe Dynamic Media Classic oferece predefinições predefinidas do visualizador para entrega de vídeo. Essas predefinições determinam a aparência do Visualizador e como seus controles de reprodução funcionam. Para personalizar o visualizador de vídeo, os administradores podem adicionar e gerenciar as Predefinições do visualizador na página Predefinições do visualizador. Para abrir esta página, no canto superior direito do Adobe Dynamic Media Classic, acesse **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**. A página Predefinições do visualizador oferece comandos para adicionar, editar, excluir e ativar as Predefinições do visualizador.

Consulte [Trabalhar com predefinições do visualizador de vídeo](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

Consulte também [Predefinições de vídeo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) vídeo de treinamento.

## 3. Implante vídeos em seus sites e sites móveis

Para integrar vídeo ao seu site, você pode fazer um dos seguintes procedimentos:

* Exiba o vídeo em sua própria janela pop-up ou modal, nesse caso, use a variável **[!UICONTROL Copy URL]** recurso.

   Para obter o URL de um vídeo, na Exibição de grade ou Exibição de lista, selecione-o no Painel de navegação. Selecionar **[!UICONTROL Preview]** e selecione **[!UICONTROL Copy URL]** à direita de `Universal_HTML5_Viewer`.

   Ao selecionar **[!UICONTROL Copy URL]**, o URL é copiado para a Área de transferência. Coloque esse código na HTML do site, site móvel ou aplicativo.

   >[!NOTE]
   >
   >Os URLs são ativados somente após a publicação do vídeo ou do Conjunto de vídeos adaptáveis.

* Exiba o vídeo incorporado na página da Web, nesse caso, use a variável **[!UICONTROL Embed Code]** recurso.

   Para obter o código incorporado de um vídeo, na Exibição de grade ou Exibição de lista, selecione o vídeo no Painel de navegação. Ir para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**. Na coluna Actions da tabela, selecione **[!UICONTROL Embed Code]** à direita de `Universal_HTML5_Video`. Não é permitido editar o código.

   Selecionar **[!UICONTROL Close]** e cole o código incorporado nas páginas da Web.

   >[!NOTE]
   >
   >O código Incorporado só é ativado após a publicação do vídeo ou do Conjunto de vídeos adaptáveis.

Consulte [Implantar vídeo em seus sites e sites móveis](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Práticas recomendadas para codificação de vídeo](uploading-encoding-videos.md#best_practices_for_video_encoding)

