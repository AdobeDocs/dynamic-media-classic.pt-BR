---
title: '"Início rápido: Vídeo"'
description: Uma introdução e o Início rápido para o Adobe Dynamic Media Classic Video para ajudá-lo a ativar e executar rapidamente.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 0%

---


# Início rápido: Vídeo{#quick-start-video}

O Adobe Dynamic Media Classic Video é uma solução completa que facilita a publicação de vídeo adaptável de alta qualidade para transmissão em várias telas, incluindo dispositivos móveis para desktop, iOS, Android, Blackberry e Windows. Um Conjunto de vídeos adaptáveis agrupa versões do mesmo vídeo codificadas em diferentes formatos e taxas de bits, como 400 kbps, 800 kbps e 1000 kbps. O computador desktop ou dispositivo móvel detecta a largura de banda disponível.

Por exemplo, em um dispositivo móvel iOS, ele detecta uma largura de banda como 3G, 4G ou Wi-Fi. Em seguida, ele seleciona automaticamente o vídeo codificado direito dentre as várias taxas de bits de vídeo no Conjunto de vídeos adaptáveis. O vídeo é transmitido em desktops, dispositivos móveis ou tablets.

Além disso, a qualidade do vídeo é alternada dinamicamente automaticamente se as condições da rede mudarem no desktop ou no dispositivo móvel. Além disso, se um cliente entrar no modo de tela cheia em um desktop, o Adaptive Video Set responde usando uma resolução melhor, melhorando assim a experiência de visualização do cliente. O uso de conjuntos de vídeos adaptáveis fornece a melhor reprodução possível para os clientes que reproduzem o vídeo do Dynamic Media Classic em várias telas e dispositivos.

A lógica usada por um reprodutor de vídeo para determinar qual vídeo codificado reproduzir ou selecionar durante a reprodução é baseada no seguinte algoritmo:

1. O reprodutor de vídeo carrega o fragmento de vídeo inicial com base na taxa de bits mais próxima do valor definido para &quot;taxa de bits inicial&quot; no próprio reprodutor.
1. O reprodutor de vídeo é alternado com base em alterações na velocidade da largura de banda usando os seguintes critérios:

   1. O reprodutor escolhe o fluxo de largura de banda mais alto abaixo ou igual à largura de banda estimada.
   1. O Player considera apenas 80% da largura de banda disponível. No entanto, se estiver mudando, é mais conversível em apenas 70% para evitar a sobrestimação e a necessidade de voltar imediatamente.

Consulte a lógica do algoritmo em [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) para obter informações técnicas sobre ele.

Para gerenciar vídeos únicos e conjuntos de vídeos adaptáveis, o Dynamic Media Classic oferece suporte ao seguinte:

* Upload de vídeo de vários formatos de vídeo e formatos de áudio suportados e codificação de vídeo para o formato MP4 H.264 para reprodução em várias telas. Você pode usar predefinições de vídeo adaptável predefinidas do Dynamic Media Classic, predefinições de codificação de vídeo único ou personalizar sua própria codificação para controlar a qualidade e o tamanho do vídeo.

   Quando um conjunto de vídeo adaptável é gerado, ele inclui vídeos MP4.

   `**Note:**` Vídeos principais/de origem e qualquer outro vídeo no formato de origem  ** não são adicionados a um Conjunto de vídeos adaptáveis.

* As legendas de vídeo em Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark e Universal_HTML5_MixedMedia_light e a navegação de capítulo de vídeo em Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark e Universal_HTML5_MixedMedia_light.

   Consulte [Adicionar legendas ao vídeo](adding-captions-video.md).

   Consulte [Adicionar marcadores de capítulo a vídeo](adding-chapter-markers-video.md).

* Organize, navegue e pesquise vídeos com suporte completo a metadados para o gerenciamento eficiente dos ativos de vídeo.
* Forneça Conjuntos de Vídeos Adaptativos para a Web, bem como para desktops e dispositivos móveis, incluindo iPhone, iPad, Android™, Blackberry e Windows phone.

   O streaming de vídeo adaptável é compatível com diversas plataformas iOS.

   Consulte o suporte mais recente no [Adobe Viewers Reference Guide](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/home.html).

   O Dynamic Media Classic é compatível com a reprodução de vídeo móvel para vídeo MP4 H.264. Você pode encontrar dispositivos Blackberry que suportam esse formato de vídeo no seguinte site:

   Consulte [Formatos de vídeo suportados no Blackberry](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   Você pode encontrar dispositivos Windows compatíveis com este formato de vídeo no seguinte endereço:

   Consulte [Formatos de vídeo suportados no Windows Phone](https://msdn.microsoft.com/en-us/library/ff462087(v=vs.92).aspx).

* Reproduzir o vídeo usando as Predefinições do visualizador do Dynamic Media Classic, incluindo o seguinte:

   * Visualizadores de vídeo individuais.
   * Visualizadores de mídia mista que combinam conteúdo de vídeo e imagem.

* Configure players de vídeo para atender às suas necessidades de marca.
* Integre vídeo ao seu site, site móvel ou aplicativo móvel com um URL simples ou código incorporado.

**Início rápido**

A seguinte descrição passo a passo do fluxo de trabalho foi criada para ajudá-lo a ativar e executar rapidamente com conjuntos de vídeos adaptáveis no Dynamic Media Classic. Após cada etapa é uma referência cruzada a um cabeçalho de tópico, onde você pode encontrar mais informações.

**1. Upload e codificação de vídeos**

Faça upload e gere conjuntos de vídeos adaptáveis usando um dos dois cenários a seguir:

* **Fazer upload de**
vídeos pré-codificadosSe os vídeos já tiverem sido codificados fora do Dynamic Media Classic, clique em 
**** Faça upload da barra de navegação global para procurar e carregar arquivos de vídeo MP4 diretamente no Dynamic Media Classic. Em seguida, clique em **Build > Adaptive Video Sets**. Navegue até seus arquivos de vídeo. Arraste e solte os arquivos de vídeo desejados na tabela Adaptive Video Set e salve o conjunto.
* **Carregar**
vídeos de origem principalSe os vídeos não estiverem codificados, clique em 
**** Faça upload da barra de navegação global para fazer upload de arquivos de fonte de vídeo principais (não MP4) e solicite que o Dynamic Media Classic os codifique em arquivos MP4 para você. Na caixa de diálogo Upload Job Options , em Opções de EVideo, selecione **Adaptive Video**.

   Essa opção preferida permite criar um Conjunto de vídeos adaptáveis que aplica automaticamente a predefinição de codificação correta ao vídeo, seja 16:9 ou 4:3, para corresponder às dimensões do vídeo que você enviou. Quando você envia seu trabalho de upload, um Conjunto de vídeos adaptáveis é criado automaticamente para você, o que inclui três codificações de vídeo na proporção correta.

   Ou, na mesma caixa de diálogo Opções de trabalho, em Opções de vídeo, expanda **Predefinições de codificação única** e selecione predefinições de codificação de vídeo individuais desejadas em **Desktop**, **Dispositivo móvel (iPhone, iPad, Android)** e **Tablet (iPad, Android id)** para criar os arquivos MP4.

* Ou você pode reprocessar um vídeo principal usando o recurso Reprocessar . Os vídeos recém-codificados são adicionados ao Conjunto de vídeos adaptáveis existente.

Consulte [Fazer upload e codificar vídeos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Opcional**

O Dynamic Media Classic oferece várias predefinições de codificação de vídeo predefinidas. Essas predefinições predefinidas refletem as configurações mais comuns de codificação de vídeo usadas hoje e são otimizadas para reprodução nas telas de destino.

No entanto, se for necessária uma personalização adicional, os administradores podem criar Predefinições de vídeo para personalizar o tamanho e a experiência de reprodução de Vídeos para os usuários finais. Os administradores podem adicionar e gerenciar Predefinições de vídeo na página Predefinições de vídeo disponível em Configuração > Configuração do aplicativo > Predefinições de vídeo > Predefinições de codificação única. A página Predefinições de vídeo oferece opções para adicionar, editar, excluir e ativar Predefinições de vídeo.

Consulte [Trabalhar com predefinições de codificação de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

**2. Visualização de vídeos em um visualizador de vídeo**

Para ver como um vídeo é reproduzido para usuários finais em um desktop, site ou em um dispositivo móvel, selecione o vídeo no Painel Procurar e clique em **Visualizar**.

Consulte [Visualização de vídeos em um visualizador de vídeo](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Você pode reproduzir o vídeo na tela Preview. Você também pode escolher visualizadores de vídeo diferentes para descobrir como o vídeo se parece em diferentes players. Como prática recomendada, use o reprodutor de vídeo HTML5 para reprodução de várias telas em desktops, tablets e dispositivos móveis.

**Opcional**

Personalização de predefinições do visualizador - o Dynamic Media Classic oferece predefinições do visualizador predefinidas para entrega de vídeo. Essas predefinições determinam a aparência do Visualizador e como seus controles de reprodução funcionam. Para personalizar o visualizador de vídeo, os administradores podem adicionar e gerenciar as Predefinições do visualizador na página Predefinições do visualizador. Para abrir esta página, no canto superior direito do Dynamic Media Classic, clique em Configuração > Predefinições do visualizador. A página Predefinições do visualizador oferece comandos para adicionar, editar, excluir e ativar as Predefinições do visualizador.

Consulte [Trabalhar com predefinições do visualizador de vídeo](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

**3. Implantação de vídeos em seus sites e sites móveis**

Para integrar vídeo ao seu site, você pode fazer um dos seguintes procedimentos:

* Exiba o vídeo em sua própria janela pop-up ou modal, nesse caso, você deve usar o recurso Copiar URL.

   Para obter o URL de um vídeo, na Exibição de grade ou Exibição de lista, selecione-o no Painel de navegação. Clique em Preview e, em seguida, clique em Copy URL à direita de `Universal_HTML5_Viewer`.

   Ao clicar em Copiar URL, o URL é copiado para a Área de Transferência. Coloque esse código no HTML do seu site, site móvel ou aplicativo.

   >[!NOTE]
   >
   >Os URLs são ativados somente após a publicação do vídeo ou do Conjunto de vídeos adaptáveis.

* Exiba o vídeo incorporado na página da Web, nesse caso, você deve usar o recurso Código incorporado.

   Para obter o código incorporado de um vídeo, na Exibição de grade ou Exibição de lista, selecione o vídeo no Painel de navegação. Clique em Visualizar > Lista de visualizadores. Na coluna Ações da tabela, clique em Incorporar código à direita de `Universal_HTML5_Video`. Não é permitido editar o código.

   Clique em Fechar e cole o código incorporado nas páginas da Web.

   >[!NOTE]
   >
   >O código Incorporado só é ativado após a publicação do vídeo ou do Conjunto de vídeos adaptáveis.

Consulte [Implantação de vídeo em seus sites e sites móveis](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Práticas recomendadas para codificação de vídeo](uploading-encoding-videos.md#best_practices_for_video_encoding)

