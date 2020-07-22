---
title: '"Start rápido: Vídeo"'
seo-title: '"Start rápido: Vídeo"'
description: nulo
seo-description: Uma introdução e um Start rápido para o Video para ajudá-lo a começar a trabalhar rapidamente.
uuid: bf0ecf87-a1f2-4e83-8041-df5192dd26a1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 6cef541b-e9df-48eb-9a16-ca3e1f07238e
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1443'
ht-degree: 0%

---


# Start rápido: Vídeo{#quick-start-video}

O Adobe Dynamic Media Classic Video é uma solução completa que facilita a publicação de vídeo adaptável de alta qualidade para streaming em várias telas, incluindo dispositivos móveis para desktop, iOS, Android, Blackberry e Windows. Um Conjunto de vídeos adaptáveis agrupa versões do mesmo vídeo que são codificadas em diferentes taxas de bits e formatos, como 400 kbps, 800 kbps e 1000 kbps. O computador desktop ou dispositivo móvel detecta a largura de banda disponível.

Por exemplo, em um dispositivo móvel iOS, ele detecta uma largura de banda como 3G, 4G ou Wi-Fi. Em seguida, seleciona automaticamente o vídeo codificado direito entre as várias taxas de bits de vídeo no Conjunto de vídeos adaptáveis. O vídeo é transmitido para desktops, dispositivos móveis ou tablets.

Além disso, a qualidade do vídeo é automaticamente alternada se as condições da rede mudarem no desktop ou no dispositivo móvel. Além disso, se um cliente entrar no modo de tela cheia em um desktop, o Conjunto de vídeos adaptáveis responderá usando uma resolução melhor, melhorando assim a experiência de visualização do cliente. O uso de Conjuntos de vídeo adaptáveis oferece a melhor reprodução possível para os clientes que reproduzem o vídeo do Dynamic Media Classic em várias telas e dispositivos.

A lógica que um player de vídeo usa para determinar qual vídeo codificado reproduzir ou selecionar durante a reprodução é baseada no seguinte algoritmo:

1. O player de vídeo carrega o fragmento de vídeo inicial com base na taxa de bits mais próxima ao valor definido para &quot;taxa de bits inicial&quot; no próprio player.
1. O player de vídeo muda com base nas alterações na velocidade da largura de banda, usando os seguintes critérios:

   1. O player escolhe o fluxo de largura de banda mais alta abaixo ou igual à largura de banda estimada.
   1. O player considera apenas 80% da largura de banda disponível. No entanto, se ele estiver se aproximando, é mais conversível em apenas 70% para evitar sobrestimações e ter que voltar imediatamente.

Consulte a lógica do algoritmo em [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) para obter informações técnicas sobre ele.

Para gerenciar um único vídeo e Conjuntos de vídeos adaptáveis, o Dynamic Media Classic oferece suporte ao seguinte:

* Carregar vídeo de vários formatos de vídeo e formatos de áudio suportados e codificar vídeo para o formato MP4 H.264 para reprodução em várias telas. Você pode usar predefinições de vídeo adaptáveis predefinidas do Dynamic Media Classic, predefinições de codificação de vídeo único ou personalizar sua própria codificação para controlar a qualidade e o tamanho do vídeo.

   Quando um conjunto de vídeo adaptável é gerado, ele inclui vídeos MP4.

   `**Note:**` Os vídeos Principais/de origem e qualquer outro vídeo de formato de origem *não* são adicionados a um Conjunto de vídeos adaptáveis.

* As legendas de vídeo em Universal_HTML5_Video, Universal_HTML5_MixedMedia_black e Universal_HTML5_MixedMedia_light visualizadores e a navegação de capítulo de vídeo em Universal_HTML5_Video, Universal_HTML5_MixedMedia_black e Universal_HTML5_MixedMedia_light visualizadores.

   Consulte [Adicionar legendas ao vídeo](adding-captions-video.md).

   Consulte [Adicionar marcadores de capítulo ao vídeo](adding-chapter-markers-video.md).

* Organize, navegue e pesquise vídeos com suporte total a metadados para o gerenciamento eficiente dos ativos de vídeo.
* Forneça Conjuntos de vídeo adaptáveis para a Web, desktops e dispositivos móveis, incluindo iPhone, iPad, Android™, Blackberry e telefone Windows.

   O streaming de vídeo adaptativo é suportado em várias plataformas iOS.

   Consulte o suporte mais recente no Guia [de referência do](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/library/home.html)Adobe Viewers.

   O Dynamic Media Classic oferece suporte à reprodução de vídeo móvel para vídeo MP4 H.264. Você pode encontrar dispositivos Blackberry compatíveis com este formato de vídeo no seguinte site:

   Consulte Formatos de vídeo [suportados no Blackberry](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   Você pode encontrar dispositivos Windows compatíveis com este formato de vídeo no seguinte endereço:

   Consulte Formatos de vídeo [suportados no Windows Phone](https://msdn.microsoft.com/en-us/library/ff462087(v=vs.92).aspx).

* Reproduza o vídeo usando as predefinições do Dynamic Media Classic Viewer, incluindo:

   * Visualizadores de vídeo individuais.
   * Visualizadores de mídia mista que combinam conteúdo de vídeo e imagem.

* Configure players de vídeo para atender às suas necessidades de marca.
* Integre vídeo ao seu site, site móvel ou aplicativo móvel com um URL simples ou código incorporado.

**Start rápido**

A seguinte descrição passo a passo do fluxo de trabalho foi projetada para ajudá-lo a começar a usar rapidamente os conjuntos de vídeo adaptáveis no Dynamic Media Classic. Depois de cada etapa é uma referência cruzada para um cabeçalho de tópico no qual você pode encontrar mais informações.

**1. Carregamento e codificação de vídeos**

Carregue e gere conjuntos de vídeo adaptáveis usando um dos dois cenários a seguir:

* **Carregar vídeos pré-codificados** Se os vídeos já tiverem sido codificados fora do Dynamic Media Classic, clique em 
**Carregue** na barra de navegação global para navegar e carregar arquivos de vídeo MP4 diretamente para o Dynamic Media Classic. Em seguida, clique em **Criar > Conjuntos** de vídeos adaptáveis. Navegue até seus arquivos de vídeo. Arraste e solte os arquivos de vídeo desejados na tabela Conjunto de vídeos adaptáveis e salve o conjunto.
* **Carregar vídeos** de origem principais Se os vídeos não estiverem codificados, clique em 
**Faça upload** na barra Navegação global para fazer upload de arquivos de fonte de vídeo principais (não MP4) e codifique-os para arquivos MP4 para você. Na caixa de diálogo Carregar opções de trabalho, em Opções de vídeo, selecione Vídeo **** adaptável.

   Essa opção preferencial permite criar um Conjunto de vídeos adaptáveis que aplica automaticamente a predefinição de codificação correta ao vídeo, seja 16:9 ou 4:3, para corresponder às dimensões do vídeo que você carregou. Quando você envia seu trabalho de upload, um Conjunto de vídeos adaptáveis é criado automaticamente para você, o que inclui três codificações de vídeo na proporção correta.

   Ou, na mesma caixa de diálogo Opções de trabalho, em Opções de vídeo, expanda Predefinições **de codificação** única e selecione as predefinições **individuais de codificação de vídeo que você deseja em** Desktop **,** Mobile (iPhone, iPad, Android) **e** Tablet (iPad, Android)para criar os arquivos MP4.

* Ou você pode reprocessar um vídeo principal usando o recurso Reprocessar. Os vídeos recém-codificados são adicionados ao Conjunto de vídeos adaptáveis existente.

Consulte [Carregamento e codificação de vídeos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Opcional**

O Dynamic Media Classic oferta contém várias predefinições de codificação de vídeo predefinidas. Essas predefinições predefinidas refletem as configurações mais comuns de codificação de vídeo usadas hoje e são otimizadas para reprodução em telas de público alvo.

No entanto, se for necessária uma personalização adicional, os administradores podem criar predefinições de vídeo para personalizar o tamanho e a experiência de reprodução de vídeos para os usuários finais. Os administradores podem adicionar e gerenciar Predefinições de vídeo na página Predefinições de vídeo disponível em Configuração > Configuração do aplicativo > Predefinições de vídeo > Predefinições de codificação única. A página Predefinições de vídeo oferta opções para adicionar, editar, excluir e ativar Predefinições de vídeo.

Consulte [Trabalhar com predefinições](uploading-encoding-videos.md#working_with_video_encoding_presets)de codificação de vídeo.

**2. Visualização de vídeos em um visualizador de vídeo**

Para ver como um vídeo é reproduzido para usuários finais em um desktop, site ou dispositivo móvel, selecione-o no Painel de navegação e clique em **Pré-visualização**.

Consulte [Visualizar vídeos em um visualizador](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer)de vídeo.

Você pode reproduzir o vídeo na tela de Pré-visualização. Você também pode escolher visualizadores de vídeo diferentes para descobrir como o vídeo é exibido em diferentes players. Como prática recomendada, use o player de vídeo HTML5 para reprodução em várias telas em dispositivos móveis, tablets e desktop.

**Opcional**

Personalização do visualizador predefinido - Predefinições predefinidas do visualizador do Dynamic Media Classic oferta para entrega de vídeo. Essas predefinições determinam a aparência do visualizador e como seus controles de reprodução funcionam. Para personalizar o visualizador de vídeo, os administradores podem adicionar e gerenciar as predefinições do visualizador na página de predefinições do visualizador. Para abrir esta página, no canto superior direito do Dynamic Media Classic, clique em Configuração > Predefinições do visualizador. A página Predefinições do visualizador oferta comandos para adicionar, editar, excluir e ativar as Predefinições do visualizador.

Consulte [Trabalhar com predefinições](previewing-videos-video-viewer.md#working_with_video_viewer_presets)do visualizador de vídeo.

**3. Implantação de vídeos em seus sites e sites móveis**

Para integrar vídeos ao seu site, você pode executar um dos seguintes procedimentos:

* Exiba o vídeo em sua própria janela pop-up ou modal, caso em que você deve usar o recurso Copiar URL.

   Para obter o URL de um vídeo, na Visualização de grade ou na Visualização de Lista, selecione-o no painel Procurar. Clique em Pré-visualização e, em seguida, clique em Copiar URL à direita de `Universal_HTML5_Viewer`.

   Quando você clica em Copiar URL, o URL é copiado para a Área de transferência. Coloque esse código no HTML do seu site, site móvel ou aplicativo.

   >[!NOTE]
   >
   >Os URLs são ativados somente após a publicação do vídeo ou do Conjunto de vídeos adaptáveis.

* Exiba o vídeo incorporado na página da Web, caso em que você deve usar o recurso Incorporar código.

   Para obter o código incorporado de um vídeo, na Visualização de grade ou na Visualização de Lista, selecione o vídeo no painel Procurar. Clique em Pré-visualização > Lista do visualizador. Na coluna Ações da tabela, clique em Incorporar código à direita de `Universal_HTML5_Video`. A edição do código não é permitida.

   Clique em Fechar e cole o código incorporado em suas páginas da Web.

   >[!NOTE]
   >
   >O código incorporado só é ativado após a publicação do vídeo ou do Conjunto de vídeos adaptáveis.

Consulte [Implantação de vídeo em seus sites e sites](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites)móveis.

>[!MORELIKETHIS]
>
>* [Práticas recomendadas para codificação de vídeo](uploading-encoding-videos.md#best_practices_for_video_encoding)

