---
title: '" Início rápido: Vídeo "'
seo-title: '" Início rápido: Vídeo "'
description: 'null'
seo-description: Uma introdução e início rápido ao vídeo para ajudá-lo a começar a usar rapidamente.
uuid: bf 0 ecf 87-a 1 f 2-4 e 83-8041-df 5192 dd 26 a 1
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/vídeo
discoiquuid: 6 cef 541 b-e 9 df -48 eb -9 a 16-ca 3 e 1 f 07238 e
translation-type: tm+mt
source-git-commit: de7d2608f94935f238a11d8310b97dddc5476f57

---


# Início rápido: Vídeo{#quick-start-video}

O Adobe Dynamic Media Classic Video é uma solução completa que facilita a publicação de vídeo adaptável de alta qualidade para transmissão em várias telas, incluindo dispositivos móveis, iOS, Android, Blackberry e Windows. Uma versão de grupos de vídeo adaptável do mesmo vídeo que são codificados em diferentes taxas de bits e formatos como 400 kbps, 800 kbps e 1000 kbps. O computador desktop ou dispositivo móvel detecta a largura de banda disponível.

Por exemplo, em um dispositivo móvel iOS, detecta uma largura de banda como 3 G, 4 G ou Wi-Fi. Em seguida, ele seleciona automaticamente o vídeo codificado à direita entre as diversas taxas de bits de vídeo no Conjunto de vídeos adaptativo. O vídeo é transmitido para desktops, dispositivos móveis ou tablets.

Além disso, a qualidade do vídeo é alternada dinamicamente se as condições de rede forem alteradas na área de trabalho ou no dispositivo móvel. Além disso, se um cliente entrar no modo de tela cheia em um desktop, o Conjunto de vídeos adaptativo responde usando uma resolução melhor, melhorando dessa forma a experiência de visualização do cliente. O uso de Conjuntos de vídeos adaptativos fornece a melhor reprodução possível para os clientes que reproduzem vídeo do Dynamic Media Classic em várias telas e dispositivos.

A lógica que um player de vídeo usa para determinar qual vídeo codificado deve ser reproduzido ou selecionar durante a reprodução se baseia no seguinte algoritmo:

1. O player de vídeo carrega o fragmento de vídeo inicial com base na taxa de bits que está mais próxima ao valor definido para «taxa inicial inicial» no player em si.
1. O player de vídeo muda com base em alterações à velocidade de largura de banda usando os seguintes critérios:

   1. O player escolhe o fluxo de largura de banda mais alto abaixo ou igual à largura de banda estimada.
   1. O player considera apenas 80% da largura de banda disponível. Entretanto, se estiver alterando, é mais conversivo em apenas 70% para evitar a sobrecarga e ter de voltar imediatamente.

Consulte a lógica do algoritmo em [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) para obter informações técnicas sobre ele.

Para gerenciar vídeos únicos e Conjuntos de vídeos adaptativos, o Dynamic Media Classic oferece suporte para:

* Carregando vídeo de vários formatos de vídeo suportados e formatos de áudio e codificando vídeo como formato MP 4 H .264 para reprodução em várias telas. Você pode usar predefinições de vídeo personalizadas do Dynamic Media clássica predefinidas, predefinições de codificação de vídeo única ou personalizar sua própria codificação para controlar a qualidade e o tamanho do vídeo.

   Quando um conjunto de vídeos adaptável é gerado, ele inclui vídeos MP 4.

   `**Note:**` Vídeos mestre/de origem e outros vídeos de formato de origem *não* são adicionados a um conjunto de vídeos adaptativo.

* Legendas de vídeo nos visualizadores universais_ HTML 5_ Video, Universal_ HTML 5_ mixedmedia_ escuros e Universal_ HTML 5_ mixedmedia_ light e navegação do capítulo de vídeo nos visualizadores universais_ HTML 5_ Video, Universal_ HTML 5_ mixedmedia_ escuros e Universal_ HTML 5_ mixedmedia_ light.

   Consulte [Adicionar legendas ao vídeo](adding-captions-video.md).

   Consulte [Adicionar marcadores de capítulo ao vídeo](adding-chapter-markers-video.md).

* Organize, navegue e pesquise vídeos com suporte total de metadados para gerenciamento eficiente de ativos de vídeo.
* Forneça Conjuntos de vídeos adaptativos para a Web, bem como para desktops e dispositivos móveis, incluindo iphone, ipad, Android™, Blackberry e Windows Phone.

   O streaming de vídeo adaptável é compatível com diversas plataformas iOS.

   Consulte o suporte mais recente no Guia de referência de visualizadores [da Adobe](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/).

   O Dynamic Media Classic oferece suporte à reprodução de vídeo móvel para vídeo MP 4 H .264. É possível encontrar dispositivos Blackberry que oferecem suporte a esse formato de vídeo no seguinte site:

   Consulte [Formatos de vídeo suportados no Blackberry](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   É possível encontrar dispositivos Windows compatíveis com este formato de vídeo:

   Consulte [Formatos de vídeo suportados no Windows Phone](https://msdn.microsoft.com/en-us/library/ff462087(v=vs.92).aspx).

* Reproduza o vídeo usando Predefinições do visualizador do Dynamic Media Classic, incluindo o seguinte:

   * Visualizadores de vídeo único.
   * Visualizadores de mídia mista que combinam conteúdo de vídeo e imagem.

* Configure os players de vídeo para atender às suas necessidades de marca.
* Integre vídeo a seu site, site móvel ou aplicativo móvel com um URL simples ou código incorporado.

**Início rápido**

A descrição de fluxo de trabalho passo a passo a seguir foi projetada para ajudá-lo a começar a usar rapidamente os conjuntos de vídeos adaptativos no Dynamic Media Classic. Depois de cada etapa é uma referência cruzada para um cabeçalho de tópico onde você pode encontrar mais informações.

**1. Upload e codificação de vídeos**

Carregue e gere conjuntos de vídeos adaptativos usando um dos seguintes cenários:

* **Carregar vídeos pré-codificados** - se os vídeos já tiverem sido codificados fora do Dynamic Media Classic, clique **em Carregar** na barra de navegação global para procurar e carregar arquivos de vídeo MP 4 diretamente no Sistema de publicação do Scene 7. Em seguida, clique **em Criar** &gt; **Conjuntos de vídeos adaptativos**. Navegue até seus arquivos de vídeo. Arraste e solte os arquivos de vídeo que deseja na tabela Conjunto de vídeos adaptativos e salve o conjunto.
* **Carregar vídeos de origem principal** - se os vídeos não estiverem codificados, clique **em Carregar** na barra de navegação global para carregar arquivos de origem de vídeo mestre (não MP 4) e faça com que o sistema de publicação Scene 7 os codifice em arquivos MP 4 para você. Na caixa de diálogo Opções de upload de trabalho, em Opções de evideo, selecione **Vídeo adaptativo**.

   Essa opção preferencial permite criar um Conjunto de vídeos adaptativo que aplica automaticamente a predefinição correta de codificação ao vídeo, seja de 16:9 ou 4:3, para corresponder às dimensões do vídeo carregado. Quando você envia seu trabalho de upload, um Conjunto de vídeos adaptativo é criado automaticamente para você, que inclui três codificadores de vídeo na proporção correta.

   Ou, na mesma caixa de diálogo Opções de trabalho, em Opções de evideo, expanda **Predefinições** de codificação única e selecione predefinições de codificação de vídeo individuais desejadas no **Desktop**, **Mobile (iphone, ipad, Android)** e **Tablet (ipad, Android)** para que você crie os arquivos MP 4.

* Ou você pode reprocessar um vídeo mestre usando o recurso Reprocessar. Os vídeos recém codificados são adicionados ao Conjunto de vídeos adaptativo existente.

Consulte [Upload e codificação de vídeos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Opcional**

O Dynamic Media Classic oferece várias predefinições predefinidas de codificação de vídeos. Essas predefinições predefinidas refletem as configurações mais comuns de codificação de vídeo usadas hoje e são otimizadas para reprodução nas telas de destino.

No entanto, se for necessária uma personalização adicional, os administradores poderão criar Predefinições de vídeo para personalizar o tamanho e a experiência de reprodução dos vídeos para os usuários finais. Os administradores podem adicionar e gerenciar predefinições de vídeo na página Predefinições de vídeo disponíveis em Configuração &gt; Configuração do aplicativo &gt; Predefinições de vídeo &gt; Predefinições de codificação única. A página Predefinições de vídeo oferece opções para adicionar, editar, excluir e ativar predefinições de vídeo.

Consulte [Trabalhar com predefinições de codificação de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

**2. Visualização de vídeos em um visualizador de vídeo**

Para ver como um vídeo é reproduzido para os usuários finais em um desktop, seu site ou em um dispositivo móvel, selecione o vídeo no Painel Procurar e clique **em Visualizar**.

Consulte [Visualizar vídeos em um visualizador de vídeo](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Você pode reproduzir o vídeo na tela Visualizar. Você também pode escolher diferentes Visualizadores de vídeo para descobrir a aparência do vídeo em players diferentes. Como prática recomendada, use o player de vídeo HTML 5 para reprodução em várias telas em computadores, tablets e dispositivos móveis.

**Opcional**

Personalização predefinida do visualizador - o Dynamic Media Classic oferece predefinições predefinidas do visualizador para fornecer vídeo. Essas predefinições determinam a aparência do Visualizador e como seus controles de reprodução funcionam. Para personalizar o visualizador de vídeo, os administradores podem adicionar e gerenciar Predefinições do visualizador na página Predefinições do visualizador. Para abrir esta página, no canto superior direito do Sistema de publicação do Scene 7, clique em Configuração &gt; Predefinições do visualizador. A página Predefinições do visualizador oferece comandos para adicionar, editar, excluir e ativar Predefinições do visualizador.

Consulte [Trabalhar com predefinições do visualizador de vídeo](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

**3. Implantação de vídeos em sites e sites móveis**

Para integrar vídeo ao seu site, você pode fazer uma das seguintes ações:

* Exiba o vídeo em sua própria janela pop-up ou modal, e nesse caso você deve usar o recurso Copiar URL.

   Para obter o URL de um vídeo, no modo de exibição de grade ou na exibição de lista, selecione-o no Painel Procurar. Clique em Visualizar e clique em Copiar URL à direita `Universal_HTML5_Viewer`.

   Quando você clica em Copiar URL, o URL é copiado para a Área de transferência. Coloque esse código no HTML de seu site, site móvel ou aplicativo.

   ***observação**: Os urls são ativados somente depois que você publica o vídeo ou o Conjunto de vídeos adaptativo.*

* Exiba o vídeo incorporado na página da Web, nesse caso você deve usar o recurso Incorporar código.

   Para obter o código incorporado para um vídeo, no modo de exibição de grade ou na exibição de lista, selecione o vídeo no Painel Procurar. Clique em Visualizar &gt; Lista do visualizador. Na coluna Ações da tabela, clique em Incorporar código à direita `Universal_HTML5_Video`. Não é permitido editar o código.

   Clique em Fechar e cole o código incorporado em suas páginas da Web.

   ***observação**: O código incorporado é ativado somente depois de publicar o vídeo ou o Conjunto de vídeos adaptativo.*

Consulte [Implantação de vídeo a seus sites e sites móveis](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Práticas recomendadas para codificação de vídeos](uploading-encoding-videos.md#best_practices_for_video_encoding)

