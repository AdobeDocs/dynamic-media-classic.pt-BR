---
title: Fazer upload e codificar vídeos
description: Saiba como carregar e codificar vídeos no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '3886'
ht-degree: 0%

---

# Fazer upload e codificar vídeos{#uploading-and-encoding-videos}

Para criar vídeos únicos ou conjuntos de vídeos adaptados para entrega na Web ou em dispositivos móveis, primeiro você faz upload dos arquivos de vídeo principais para o Adobe Dynamic Media Classic. O Adobe Dynamic Media Classic codifica vídeos no formato MP4 e publica vídeos nos seguintes formatos de arquivo:

* **MP4**: a Adobe Dynamic Media Classic recomenda MP4 como o formato de arquivo de vídeo preferido. Use arquivos MP4 para o seguinte:

   * HTTP Dynamic Streaming em desktops.
   * HTTP Live Streaming (protocolo de transmissão do Apple).
   * Entrega de vídeo progressiva para dispositivos móveis Android™, BlackBerry® e Windows®

  O Adobe Dynamic Media Classic oferece dois fluxos de trabalho para fazer upload de arquivos de vídeo:

* **Vídeos pré-codificados**: é possível fazer upload de arquivos MP4 diretamente no Adobe Dynamic Media Classic. Com esse fluxo de trabalho, os arquivos não são codificados no momento em que você os carrega. Os arquivos são pré-codificados em preparação para entrega no desktop e em dispositivos móveis.

* **Vídeos de origem primária**: carregue os arquivos de vídeo de origem principal e, no upload, codifique esses arquivos em arquivos MP4. Os vídeos codificados são rotulados como &quot;Vídeo&quot; no painel Procurar. O Adobe Dynamic Media Classic é compatível com a codificação de arquivos de vídeo em vários formatos.

   * Verifique se os arquivos de vídeo de origem primária que você deseja codificar são suportados.

     Consulte [Tipos de arquivo de vídeo suportados para codificação](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

   * Escolha uma predefinição de codificação de vídeo.

     Consulte [Predefinições de vídeo para codificar arquivos de vídeo](application-setup.md#video-presets-for-encoding-video-files).

     Consulte [Práticas recomendadas para codificação de vídeo](uploading-encoding-videos.md#best-practices-for-video-encoding).

O Adobe Dynamic Media Classic também gera miniaturas de vídeo. Você pode saber mais sobre miniaturas de vídeo, como obter seus URLs e modificar quadros de pôster.

Consulte [Trabalhar com miniaturas de vídeo](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**Para carregar e codificar vídeos:**

Siga qualquer um destes procedimentos.

*Se os vídeos já estiverem codificados*

1. Na barra Navegação global, selecione **[!UICONTROL Upload]**.
1. Na página Upload, selecione a variável **[!UICONTROL From Desktop]** guia.
1. Na página Upload, no campo **[!UICONTROL Select Files for Upload]** , selecione **[!UICONTROL Browse]**, navegue até um arquivo de vídeo MP4 e selecione **[!UICONTROL Open]**.
1. No escolhido **[!UICONTROL Folder Destination]** selecione uma pasta para o arquivo carregado.
1. Na página Upload, verifique se **[!UICONTROL Publish After Uploading]** está marcado.
1. Selecionar **[!UICONTROL Submit Upload]**.

*Se quiser codificar seus vídeos usando o Adobe Dynamic Media Classic*

1. Na barra Navegação global, selecione **[!UICONTROL Upload]**.
1. Na página Upload, selecione a variável **[!UICONTROL From Desktop]** guia.
1. No **[!UICONTROL Select Files to Upload]** , selecione **[!UICONTROL Browse]**, navegue até um arquivo de vídeo de origem principal e selecione **[!UICONTROL Open]**.
1. No escolhido **[!UICONTROL Folder Destination]** selecione uma pasta para o arquivo carregado.
1. No canto inferior direito da página, selecione **[!UICONTROL Job Options]**,
1. Na caixa de diálogo Fazer Upload das Opções de Job, expanda **[!UICONTROL EVideo Options]**, siga um destes procedimentos:

   * A prática recomendada é selecionar **[!UICONTROL Adaptive Video Encoding]**. Consulte [Vídeo adaptável (padrão)](application-setup.md#adaptive-video-default).
   * Opcional. Se quiser usar configurações de codificação individuais, expanda **[!UICONTROL Single Encoding Presets]**e selecione as opções de codificação desejadas para Desktop, Mobile e Tablet.
Consulte [Predefinições de codificação de vídeo da área de trabalho](application-setup.md#desktop-video-encoding-presets), [Predefinições de codificação de vídeo para dispositivos móveis](application-setup.md#mobile-video-encoding-presets), [Predefinições de codificação de vídeo do tablet](application-setup.md#tablet-video-encoding-presets).
1. Na caixa de diálogo Fazer Upload das Opções de Job, selecione **[!UICONTROL Save]**.
1. Na página Upload, verifique se **[!UICONTROL Publish After Uploading]** está marcado.
1. Na página Upload, no canto inferior direito, selecione **[!UICONTROL Submit Upload]**.

*Se quiser codificar novamente um arquivo de vídeo carregado anteriormente,*

1. No Adobe Dynamic Media Classic, no painel Procurar, navegue até o vídeo e selecione-o.
1. Ir para **[!UICONTROL File]** > **[!UICONTROL Reprocess]**.
1. Na caixa de diálogo Reprocessar ativos, expanda **[!UICONTROL EVideo Options]**, siga um destes procedimentos:
   * A prática recomendada é usar o método a seguir. Selecionar **Vídeo adaptável**.
Consulte [Vídeo adaptável (padrão)](application-setup.md#adaptive-video-default).
   * Opcional. Se quiser usar configurações de codificação individuais, expanda **[!UICONTROL Single Encoding Presets]**e selecione as opções de codificação desejadas para Desktop, Mobile e Tablet.
Consulte [Predefinições de codificação de vídeo da área de trabalho](application-setup.md#desktop-video-encoding-presets), [Predefinições de codificação de vídeo para dispositivos móveis](application-setup.md#mobile-video-encoding-presets), [Predefinições de codificação de vídeo do tablet](application-setup.md#tablet-video-encoding-presets).
1. Na caixa de diálogo Reprocessar ativos, selecione **[!UICONTROL Submit]**.

Quando você usa uma predefinição de codificação de Vídeo adaptável ou várias predefinições de codificação única, o resultado é um Conjunto de vídeos adaptados que é criado automaticamente com várias codificações de vídeo. Você também pode criar manualmente um Conjunto de vídeos adaptados selecionando vídeos individuais.

Somente os tipos de arquivo MP4 e M4V são criados ao gerar um Conjunto de vídeos adaptados automática ou manualmente.

## Tipos de arquivo de vídeo suportados para codificação {#supported-video-file-types-for-encoding}

A tabela a seguir lista os tipos de arquivos de vídeo (com codecs de vídeo permitidos) que você pode codificar para o formato MP4 ou OGV ao fazer upload de arquivos. A tabela lista os formatos de arquivo e os codecs:

* **Formatos de arquivo de vídeo**: assim como um arquivo ZIP, um formato de arquivo de vídeo determina como os arquivos são contidos no arquivo de vídeo. Um arquivo de vídeo geralmente contém várias faixas — uma faixa de vídeo (sem áudio) e uma ou mais faixas de áudio (sem vídeo) — que são inter-relacionadas e sincronizadas. O formato do arquivo de vídeo determina como esses diferentes controles de dados e metadados são organizados.

* **Codecs de vídeo**: um codec de vídeo descreve o algoritmo pelo qual um vídeo é codificado. Um player de vídeo decodifica o vídeo de acordo com seu codec e exibe uma série de imagens, ou quadros, na tela. Os codecs minimizam a quantidade de informações que os arquivos de vídeo precisam armazenar para reproduzir vídeo. Em vez de informações sobre cada quadro individual, somente as informações sobre as diferenças entre um quadro e o próximo são armazenadas. Como a maioria dos vídeos muda pouco de um quadro para o próximo, os codecs permitem altas taxas de compactação, o que resulta em tamanhos de arquivo menores.

  | Formato de arquivo de vídeo | Codecs de vídeo |
  | --- | --- |
  | 3GP | H.263, H.264 |
  | AVI | DivX, DV |
  | M2P | MPEG-2 PS |
  | M2T | TS MPEG-2 |
  | M2TS | TS MPEG-2 |
  | M2V | MPEG-2 ES |
  | M4V | H.264 |
  | MOV | DV, DVCPro 50, H.261, H.263, H.264, Sorenson Vídeo 1 |
  | MP4 | `H.264/MPEG-4` AVC |
  | MPEG | MPEG-2 SS |
  | MPG | MPEG-2 SS |
  | MTS | MPEG-2 |
  | ProRes | APCN, APCS, APCO, APCH, AP4H |
  | TS | DVCPro 50 |
  | VOB | MPEG-2 |
  | WMV/ASF | VC-1, Windows® Media Video 7, Windows® Media Video 8 |

  >[!NOTE]
  >
  >A tela Trabalhos alerta se você fizer upload e tentar codificar um arquivo de vídeo, mas o arquivo é rejeitado porque contém um codec ou contêiner de arquivo incompatível. Para obter mais informações, consulte [Verificar arquivos de trabalho](checking-job-files.md).

## Práticas recomendadas para codificação de vídeo {#best-practices-for-video-encoding}

Veja a seguir as dicas de práticas recomendadas para a codificação de arquivos de vídeo de origem no Adobe Dynamic Media Classic.

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### Arquivos de vídeo de origem {#source-video-files}

Ao codificar um arquivo de vídeo, use um arquivo de vídeo de origem com a mais alta qualidade possível. Evite usar arquivos de vídeo codificados anteriormente, pois esses arquivos já estão compactados, e codificações adicionais criam um vídeo de qualidade inferior.

A tabela a seguir descreve o tamanho recomendado, a taxa de proporção e a taxa de bits mínima que seus arquivos de vídeo de origem devem ter ao codificá-los:

| Tamanho | Taxa de proporção | Taxa de bits mínima |
| --- | --- | --- |
| 1024 X 768 | 4:3 | 4500 kbps para a maioria dos vídeos. |
| 1280 X 720 | 16:9 | 3000: 6000 kbps, dependendo da quantidade de movimento no vídeo. |
| 1920 X 1080 | 16:9 | 6000: 8000 kbps, dependendo da quantidade de movimento no vídeo. |

### Obter os metadados de um arquivo {#obtaining-a-file-s-metadata}

Você pode obter os metadados de um arquivo visualizando os metadados no Adobe Dynamic Media Classic, usando uma ferramenta de edição de vídeo ou usando um aplicativo projetado para obter metadados. A seguir estão as instruções para usar o MediaInfo, um aplicativo de terceiros, para obter os metadados de um arquivo de vídeo:

1. Ir para esta página da Web: [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo).
1. Selecione e baixe o instalador para a versão da GUI e siga as instruções de instalação.
1. Após a instalação, clique com o botão direito no arquivo de vídeo (somente Windows®) e selecione MediaInfo, ou abra MediaInfo e arraste o arquivo de vídeo para o aplicativo. Você verá todos os metadados associados ao arquivo de vídeo, incluindo largura, altura e fps.

### Taxa de proporção {#aspect-ratio}

Ao escolher ou criar uma predefinição de codificação de vídeo para o arquivo de vídeo principal, verifique se a predefinição tem a mesma proporção do arquivo de vídeo principal. A variável *taxa de proporção* é a relação entre a largura e a altura do vídeo.

Para determinar a proporção de um arquivo de vídeo, obtenha os metadados do arquivo e observe a largura e a altura do arquivo (consulte [Obter os metadados de um arquivo](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Em seguida, use esta fórmula para determinar a proporção:

Largura / Altura = Taxa de proporção

A tabela a seguir descreve como os resultados da fórmula são convertidos em opções comuns de taxa de proporção:

| Resultado da fórmula | Taxa de proporção |
| --- | --- |
| 1,33 | 4:3 |
| 0,75 | 3:4 |
| 1,78 | 16:9 |
| 0,56 | 9:16 |

Por exemplo, um vídeo com 1440 de largura × 1080 de altura tem uma proporção largura/altura de 1440/1080 ou 1,33. Nesse caso, você escolhe uma predefinição de codificação de vídeo com uma proporção 4:3 para codificar o arquivo de vídeo.

### Taxa de dados {#data-rate}

A variável *taxa de dados* (também chamado de *taxa de bits*) é a quantidade de dados codificada para compor um segundo único de reprodução de vídeo. A taxa de dados é medida em kilobits por segundo (Kbps).

>[!NOTE]
>
>Como todos os codecs usam compactação com perdas, a taxa de dados é o fator mais importante na qualidade do vídeo. Com a compactação com perdas, quanto mais você compacta um arquivo de vídeo, mais a qualidade é degradada. Por isso, todas as outras características são iguais (resolução, taxa de quadros e codec), quanto menor a taxa de dados, menor a qualidade do arquivo compactado.

Ao escolher uma predefinição de codificação de vídeo, lembre-se de levar em conta a velocidade de conexão do usuário final de destino. Escolha uma predefinição com uma taxa de dados que seja 80% dessa velocidade. Por exemplo, se a velocidade de conexão do usuário final de destino for 1000 Kbps, a melhor predefinição é aquela com uma taxa de dados de vídeo de 800 Kbps.

Esta tabela descreve a taxa de dados de velocidades de conexão típicas.

| Velocidade (Kbps) | Tipo de conexão |
| --- | --- |
| 256 | Conexão dial-up. |
| 800 | Conexão móvel típica. Para essa conexão, direcione uma taxa de dados na faixa de 400 a no máximo 800 para experiências 3G. |
| 2000 | Conexão típica de desktop de banda larga. Para essa conexão, direcione uma taxa de dados na faixa de 800-2000 Kbps, com a média da maioria dos targets de 1200-1500 Kbps. |
| 5000 | Conexão típica de alta banda larga. A codificação nesse intervalo superior não é recomendada porque a entrega de vídeo nessa velocidade não está disponível para a maioria dos consumidores. |

### Resolução {#resolution}

*Resolução* descreve a altura e a largura de um arquivo de vídeo em pixels. A maioria dos vídeos de origem é armazenada em alta resolução (por exemplo, 1920 × 1080). Para fins de transmissão, o vídeo de origem é compactado para uma resolução menor (640 × 480 ou menor).

Resolução e taxa de dados são dois fatores vinculados integralmente que determinam a qualidade do vídeo. Para manter a mesma qualidade de vídeo, quanto maior o número de pixels em um arquivo de vídeo (quanto maior a resolução), maior deverá ser a taxa de dados. Por exemplo, considere o número de pixels por quadro em um arquivo de vídeo de resolução 320 × 240 e resolução 640 × 480:

| Resolução | Pixels por quadro |
| --- | --- |
| 320 × 240 | 76.800 |
| 640 × 480 | 307.200 |

O arquivo de 640 × 480 tem quatro vezes mais pixels por quadro. Para obter a mesma taxa de dados para essas duas resoluções de exemplo, aplique a compactação quatro vezes maior ao arquivo 640 × 480, o que pode reduzir a qualidade do vídeo. Portanto, uma taxa de dados de vídeo de 250 Kbps produz uma visualização de alta qualidade com resolução de 320 × 240, mas não com resolução de 640 × 480.

>[!NOTE]
>
>Em geral, quanto maior a taxa de dados usada, melhor será a exibição do vídeo e maior será a resolução usada, maior será a taxa de dados que você deve manter a qualidade da visualização (em comparação com resoluções mais baixas).

Como a resolução e a taxa de dados são vinculadas, você tem duas opções ao codificar vídeos:

* Escolha uma taxa de dados e, em seguida, codifique na resolução mais alta que seja exibida melhor na taxa de dados escolhida.
* Escolha uma resolução e codifique na taxa de dados necessária para obter um vídeo de alta qualidade na resolução escolhida.

Ao escolher (ou criar) uma predefinição de codificação de vídeo para o arquivo de vídeo principal, use essa tabela para direcionar a resolução correta:

| Resolução | Altura (pixels) | Tamanho da tela |
| --- | --- | --- |
| 240p | 240 | Tela pequena |
| 300p | 300 | Telas pequenas normalmente para dispositivos móveis |
| 360p | 360 | Tela pequena |
| 480p | 480 | Tela média |
| 720p | 720 | Tela grande |
| 1080p | 1080 | Tela grande de alta definição |

### FPS (quadros por segundo) {#fps-frames-per-second}

Nos Estados Unidos e no Japão, a maioria dos vídeos é filmada a 29,97 quadros por segundo (FPS); na Europa, a maioria dos vídeos é filmada a 25 FPS. O filme é filmado em 24 FPS.

Escolha uma predefinição de codificação de vídeo que corresponda à taxa de FPS do arquivo de vídeo principal. Por exemplo, se o vídeo principal tiver 25 quadros/s, escolha uma predefinição de codificação com 25 quadros/s. Por padrão, todas as codificações personalizadas usam o FPS do arquivo de vídeo principal. Por esse motivo, não é necessário especificar a configuração de FPS ao criar uma predefinição de codificação de vídeo.

### Dimensões de codificação de vídeo {#video-encoding-dimensions}

Para obter resultados ideais, selecione dimensões de codificação de forma que o vídeo de origem seja um múltiplo inteiro de todos os vídeos codificados.

Para calcular essa proporção, divida a largura da origem pela largura codificada para obter a proporção da largura. Em seguida, divida a altura da origem pela altura codificada para obter a proporção da altura.

Se a proporção resultante for um inteiro, significa que o vídeo está dimensionado de maneira ideal. Se a proporção resultante não for um número inteiro, ela afetará a qualidade do vídeo, deixando artefatos de pixel restantes na exibição. Esse efeito é mais perceptível quando o vídeo tem texto.

Por exemplo, suponha que a fonte de vídeo seja 1920 × 1080. Na tabela a seguir, os três vídeos codificados fornecem as configurações de codificação ideais para usar.

| Tipo de vídeo | Largura × altura | Proporção de largura | Taxa de altura |
| --- | --- | --- | --- |
| Origem | 1920 × 1080 | 1 | 1 |
| Codificado | 960 × 540 | 2 | 2 |
| Codificado | 640 × 360 | 3 | 3 |
| Codificado | 480 × 270 | 4 | 4 |

### Formato de arquivo de vídeo codificado {#encoded-video-file-format}

A Adobe Dynamic Media Classic recomenda usar predefinições de codificação de vídeo MP4 H.264. Como os arquivos MP4 usam o codec de vídeo H.264, ele fornece vídeo de alta qualidade, mas em um tamanho de arquivo compactado.

## Trabalhar com predefinições de codificação de vídeo {#working-with-video-encoding-presets}

Arquivos de vídeo primários criados com equipamentos de produção de vídeo e software de edição de vídeo geralmente são muito grandes e não estão no formato adequado para entrega em destinos online. Para converter vídeo digital para o formato e as especificações adequados para reprodução em telas diferentes, você pode *transcode* arquivos de vídeo (um processo também conhecido como *codificação*). Durante o processo de codificação, o vídeo é compactado para um tamanho de arquivo menor e eficiente. Ele faz isso para uma entrega ideal na Web e em dispositivos móveis.

Consulte [Fazer upload e codificar vídeos](uploading-encoding-videos.md#uploading-and-encoding-videos).

O Adobe Dynamic Media Classic oferece uma biblioteca de predefinições predefinidas de codificação de vídeo que refletem as configurações de codificação mais comuns usadas atualmente. Essas predefinições de codificação são otimizadas para reprodução nas telas de destino. Além disso, os administradores podem criar suas próprias predefinições de codificação de vídeo para personalizar o tamanho e a qualidade de reprodução dos vídeos para os usuários finais. Todas as predefinições de codificação de vídeo, seja pronta para uso do Adobe Dynamic Media Classic ou personalizada, exibem o vídeo no formato de arquivo MP4.

Na tela Predefinições de vídeo, os administradores podem configurar e gerenciar a codificação de vídeo. Eles podem fazer o seguinte:

* Ative e desative as predefinições de codificação de vídeo.
* Crie uma predefinição de codificação de vídeo.
* Editar predefinições de codificação de vídeo.
* Excluir predefinições de vídeo.

Qualquer vídeo que você carregar no Adobe Dynamic Media Classic ou codificar no Adobe Dynamic Media Classic será tratado como &quot;vídeo&quot;. Em outras palavras, essa classificação de ativos significa que você pode fornecer o vídeo para reprodução em desktops, dispositivos móveis ou ambos. Por exemplo, você pode visualizar esses tipos de vídeos no Adobe Dynamic Media Classic. Você também pode gerar URLs (usando o recurso Copiar URL ) e código que pode ser incorporado (usando o recurso Incorporar código ) para uso com reprodutores de vídeo, em sites e assim por diante.

Consulte [Visualizar vídeos em um visualizador de vídeo](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Consulte [Vincular um URL de vídeo a um site para dispositivos móveis ou site](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Consulte [Incorporar o visualizador de vídeo em uma página da Web](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Para ativos de vídeo que você carrega e codifica no Adobe Dynamic Media Classic, o vídeo é fornecido no seguinte formato de arquivo:

**MP4 H.264** Use arquivos MP4 para o seguinte:

* HTTP Dynamic Streaming em desktops.
* HLS (HTTP Live Streaming, protocolo de transmissão do Apple).
* Entrega de vídeo progressiva para dispositivos móveis Android™, BlackBerry® e Windows®.

Qualquer outro formato de vídeo e codec é tratado como um &quot;Vídeo principal&quot;. Essa classificação de ativos significa que o vídeo é um arquivo de vídeo de origem e não pode ser usado para a reprodução do delivery em desktops ou dispositivos móveis. Por exemplo, não é possível visualizar esses tipos de vídeos no Adobe Dynamic Media Classic. Não é possível gerar Copiar URLs ou Incorporar código para uso em players de vídeo, em sites e assim por diante.

### Filtrar a lista de predefinições de codificação de vídeo {#filtering-the-list-of-video-encoding-presets}

A página Predefinições de vídeo e a página Predefinições de vídeo adaptado consistem em uma tabela que lista o status ativo, o nome predefinido, o dispositivo de reprodução pretendido, o tamanho do vídeo e a taxa de dados de cada Predefinição de vídeo.

É possível refinar a lista optando por filtrar por Ambas, Ativas ou Inativas, para ver todas as Predefinições de vídeo ou restringir a lista a predefinições que estejam ativas ou inativas.

Você também pode filtrar com base em uma opção de dispositivo de reprodução para restringir a lista a Predefinições de vídeo projetadas para reproduzir vídeos em todos os dispositivos, computadores, dispositivos móveis ou tablets.

**Para filtrar a lista de predefinições de codificação de vídeo:**

1. No Adobe Dynamic Media Classic, na barra Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Adaptive Video Presets]** ou **[!UICONTROL Single Encoding Presets]**.

   As páginas de Predefinições de vídeo adaptado e Predefinições de codificação única incluem uma tabela que lista o status Ativo, o nome da predefinição, o dispositivo de reprodução pretendido, as dimensões do vídeo e a taxa de dados de cada Predefinição de vídeo.

1. Na página Predefinições de codificação única, chamada Predefinições de vídeo, na barra de ferramentas Predefinições de vídeo, use as duas listas suspensas para refinar a lista de predefinições na tabela com base no status Ativo e no dispositivo de reprodução.

   * Na primeira lista suspensa mais estreita, escolha **[!UICONTROL Both]** para ver todas as predefinições de vídeo, ou escolha **[!UICONTROL Active]** ou **[!UICONTROL Inactive]** ou restrinja a lista a predefinições que estejam ativas ou inativas.
   * Na segunda lista suspensa mais ampla, escolha uma opção de dispositivo de reprodução para restringir a lista às Predefinições de vídeo projetadas para reproduzir vídeos em desktops. ou para reproduzir vídeos em dispositivos móveis ou tablets.

### Ativar ou desativar predefinições de codificação de vídeo {#activating-or-deactivating-video-encoding-presets}

As Predefinições de vídeo ativado são exibidas na caixa de diálogo Fazer upload das opções de trabalho. A caixa de diálogo é exibida quando um usuário carrega arquivos de vídeo durante o processo de upload. Eles podem escolher em uma lista de todas as predefinições de codificação ativadas.

1. No Adobe Dynamic Media Classic, na barra Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]**.
1. Siga um destes procedimentos:

   * Selecionar **[!UICONTROL Adaptive Video Presets]**.
   * Selecionar **[!UICONTROL Single Encoding Presets]**.

1. Siga um destes procedimentos:

   * Para ativar uma Predefinição de vídeo, na página Predefinições, na coluna Ativo, selecione a caixa ao lado de um nome predefinido.
   * Para desativar uma Predefinição de vídeo, desmarque a caixa ao lado da Predefinição de vídeo que você deseja tornar inativa.

     >[!NOTE]
     >
     >Predefinições de vídeo inativo não aparecem na caixa de diálogo Fazer upload das opções de trabalho.

1. No canto inferior direito da página, selecione **[!UICONTROL Close]**.

### Adicionar ou editar uma predefinição de codificação de vídeo {#adding-or-editing-a-video-encoding-preset}

É possível criar predefinições de vídeo personalizadas em codificação única e adicioná-las à tabela Predefinições de vídeo. Você também pode alterar qualquer predefinição predefinida de vídeo de codificação única fornecida com o Adobe Dynamic Media Classic, desde que salve a predefinição editada com um novo nome.

A Adobe Dynamic Media Classic definiu limites máximos para a taxa de dados de destino, a altura da resolução e a largura da resolução para garantir uma experiência de reprodução adequada. As mensagens de aviso serão exibidas se você exceder esses limites, que são os seguintes:

* Para a reprodução do computador, os limites são: (Largura/16) &#42; (Altura/16) &lt; 8192.
* Para reprodução móvel, os limites são: (Largura/16) &#42; (Altura/16) &lt; 660; taxa de dados alvo &lt; 4000.
* Para a reprodução de tablets, os limites são: (Largura/16) &#42; (Altura/16) &lt; 3600.

**Para adicionar ou editar uma predefinição de codificação de vídeo:**

1. No Adobe Dynamic Media Classic, na barra Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]**.
1. Selecionar **[!UICONTROL Single Encoding Presets]**.
1. Na página Predefinições de vídeo, siga um destes procedimentos:

   * Na barra de ferramentas Predefinições de vídeo, selecione **[!UICONTROL Add]** para adicionar uma predefinição de vídeo.
   * Selecione uma predefinição de vídeo. Na barra de ferramentas, selecione **[!UICONTROL Edit]**.

     Não é possível editar predefinições predefinidas do Adobe Dynamic Media Classic; você só pode criar uma predefinição a partir de uma predefinição existente escolhendo **[!UICONTROL Save As]**.

1. Na página Adicionar predefinição de vídeo ou Editar predefinição de vídeo, defina as opções desejadas de Predefinição de vídeo.

   Consulte [Práticas recomendadas para codificação de vídeo](uploading-encoding-videos.md#best-practices-for-video-encoding) para configurações recomendadas.

   | Opção de Predefinição de vídeo | Descrição |
   | --- | --- |
   | Nome da predefinição | Digite um nome descritivo para a predefinição de vídeo. O nome informado é exibido na caixa de diálogo Fazer Upload das Opções de Job, na qual os usuários escolhem as opções de transcodificação. |
   | Descrição | Descreva a predefinição de vídeo. O que você digitar aparecerá como uma dica de ferramenta. Quando os usuários escolhem opções de transcodificação, a dica de ferramenta é exibida quando eles movem o ponteiro sobre o nome da predefinição na caixa de diálogo Fazer upload das opções de trabalho. |
   | Dispositivo de reprodução | Escolha o dispositivo no qual o vídeo deve ser reproduzido. As opções são Computador (desktops), Dispositivo móvel (iPhone, iPad, Android™) ou Tablet (somente iPad). Essa configuração determina automaticamente o codec de áudio e vídeo apropriado usado durante a codificação. |
   | Taxa de dados de público alvo | Insira a velocidade média de conexão com a Internet (em quilobits por segundo) do usuário final de destino. Você pode inserir a taxa ou arrastar o controle deslizante para inseri-la. O espectro Velocidade de conexão do usuário lista as velocidades típicas para conexões de banda larga, DSL, portáteis e dial-up. Essa configuração determina automaticamente a taxa de dados de vídeo e áudio combinados. Em outras palavras, a quantidade de dados codificada para compor um único segundo de reprodução de vídeo. Quanto maior a taxa de dados, melhor a qualidade do vídeo resultante. No entanto, taxas de dados muito altas resultam em arquivos grandes que criam experiências de visualização discretas para usuários com baixa largura de banda. Como prática recomendada, encontre um equilíbrio entre taxas de dados altas e baixas. Tente criar uma experiência de reprodução de qualidade adequada sem alienar os usuários que têm larguras de banda estreitas. |
   | Taxa de proporção | A taxa de proporção é a relação entre a largura e a altura do vídeo. As duas primeiras proporções listadas abaixo são normalmente usadas para exibir vídeo horizontalmente:<ul><li> 4:3: Usado para quase todos os conteúdos de transmissão de TV de definição padrão.</li><li>16:9: Usado para quase todos os conteúdos e filmes de tela larga na High-Definition Television (HDTV).</li><li>Dimensionamento automático: (padrão) uma predefinição de codificação única que funciona com qualquer taxa de proporção para criar vídeos, permitindo sua entrega em dispositivos móveis, tablets e computadores de mesa. Os vídeos de origem carregados codificados com essa predefinição são definidos com uma altura fixa. No entanto, a largura é dimensionada automaticamente para preservar a proporção do vídeo (proporção largura e altura).</li><li>Personalizado: usado quando você deseja definir um tamanho de vídeo não padrão.</li><li>A taxa de proporção escolhida determina as configurações de largura e altura para o Tamanho da resolução. O valor de largura e altura é dimensionado automaticamente de acordo com a taxa de proporção adequada.</li></ul> |
   | Tamanho da resolução | O tamanho da resolução, expresso pelo número de pixels de largura pelo número de pixels de altura, determina o tamanho. Insira um valor de largura e altura em pixels ou arraste o controle deslizante para inserir esses valores. O espectro de Resolução lista os tamanhos típicos de resolução. O valor da largura e o valor da altura aderem automaticamente à taxa de proporção selecionada. Por exemplo, se você selecionar 4:3 como taxa de proporção e inserir 400 para largura, 300 será inserido automaticamente para altura. Se tiver selecionado Dimensionar automaticamente para a configuração Proporção, o valor Largura do Tamanho da Resolução será automaticamente definido como Automático. Selecionar **[!UICONTROL Preview]** para que você possa abrir uma janela do navegador e ver suas opções de resolução lá. |
   | Codificar sufixo do arquivo | Insira um sufixo. Esse sufixo é anexado ao arquivo de vídeo codificado resultante. Você pode inserir um hífen e um sublinhado no nome; espaços em branco e caracteres especiais não são permitidos. |
   | Outras configurações | O Adobe Dynamic Media Classic determina todas as outras configurações de codificação automaticamente de acordo com as diretrizes de codificação de práticas recomendadas. |

1. Siga um destes procedimentos:

   * Selecionar **[!UICONTROL Save]** se você adicionou ou editou uma Predefinição de vídeo.
   * Selecionar **[!UICONTROL Save As]** se você tiver adicionado uma predefinição de vídeo iniciando com uma predefinição existente.

### Excluir uma predefinição de codificação de vídeo {#delete-a-video-encoding-preset}

Os administradores podem excluir predefinições de vídeo personalizadas. As predefinições de vídeo que acompanham o Adobe Dynamic Media Classic não podem ser excluídas.

1. No Adobe Dynamic Media Classic, na barra Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]**.
1. Selecionar **[!UICONTROL Single Encoding Presets]**.
1. Na página Predefinições de vídeo, selecione na tabela uma Predefinição de vídeo que não é mais desejada ou necessária.
1. Na barra de ferramentas Predefinições de vídeo, selecione **[!UICONTROL Delete]**.
1. Na caixa de diálogo Excluir predefinição, selecione **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [Início rápido: vídeo no Adobe Dynamic Media Classic](quick-start-video.md#quick-start-video)
>* [Fazer upload e codificar vídeos](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Trabalhar com predefinições do visualizador de vídeo](previewing-videos-video-viewer.md#working-with-video-viewer-presets)
>* [Predefinições de vídeo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) vídeo de treinamento
