---
title: Upload e codificação de vídeos
seo-title: Upload e codificação de vídeos
description: Saiba como fazer upload e codificar vídeos.
seo-description: Saiba como fazer upload e codificar vídeos.
uuid: 9a7d6513-b10c-40b0-aebb-18a795c2b8d1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: a0941823-850c-4373-9e37-f32032de3805
feature: Dynamic Media Classic,Visualizadores,Vídeo
role: Business Practitioner
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '3778'
ht-degree: 1%

---

# Upload e codificação de vídeos{#uploading-and-encoding-videos}

Para criar um único vídeo ou conjuntos de vídeos adaptáveis para entrega na Web ou em dispositivos móveis, primeiro carregue seus arquivos de vídeo principais no Dynamic Media Classic. O Dynamic Media Classic codifica vídeos para o formato MP4 e publica vídeo nos seguintes formatos de arquivo:

* **MP4**  - O Dynamic Media Classic recomenda o MP4 como o formato de arquivo de vídeo preferencial. Use arquivos MP4 para o seguinte:

   * HTTP Dynamic Streaming em desktops.
   * HTTP Live Streaming (protocolo de transmissão da Apple).
   * Entrega de vídeo progressivo para dispositivos móveis Android™, BlackBerry® e Windows®

   O Dynamic Media Classic oferece dois fluxos de trabalho para carregar arquivos de vídeo:

* **Vídeos pré-codificados**  - Você carrega arquivos MP4 diretamente no Dynamic Media Classic. Com esse fluxo de trabalho, os arquivos não são codificados no momento em que você os carrega. Os arquivos são pré-codificados em preparação para entrega no desktop e em dispositivos móveis.

* **Vídeos de origem principal**  - Faça upload de arquivos de vídeo de origem principal e, ao fazer upload, codifique esses arquivos em arquivos MP4. Os vídeos codificados são rotulados como &quot;Vídeo&quot; no painel Procurar. O Dynamic Media Classic é compatível com a codificação de arquivos de vídeo em vários formatos.

   * Verifique se os arquivos de vídeo de origem principal que você deseja codificar são compatíveis.

      Consulte [Tipos de arquivo de vídeo suportados para codificação](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

   * Escolha uma predefinição de codificação de vídeo.

      Consulte [Predefinições de vídeo para codificação de arquivos de vídeo](application-setup.md#video-presets-for-encoding-video-files).

      Consulte [Práticas recomendadas para codificação de vídeo](uploading-encoding-videos.md#best-practices-for-video-encoding).

O Dynamic Media Classic também gera miniaturas de vídeo. Saiba mais sobre miniaturas de vídeo, como obter URLs e modificar quadros de pôster.

Consulte [Trabalhar com miniaturas de vídeo](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**Para fazer upload e codificar vídeos:**

Siga qualquer um destes procedimentos.

*Se os vídeos já estiverem codificados*

1. Na barra Navegação global, clique em **[!UICONTROL Upload]**.
1. Na página Upload , clique na guia **[!UICONTROL From Desktop]** .
1. Na página Upload , no painel **[!UICONTROL Select Files for Upload]**, clique em **[!UICONTROL Browse]**, navegue até um arquivo de vídeo MP4 e clique em **[!UICONTROL Open]**.
1. No painel **[!UICONTROL Choose Folder Destination]**, selecione uma pasta para o arquivo carregado.
1. Na página Upload , verifique se **[!UICONTROL Publish After Uploading]** está marcado.
1. Clique em **[!UICONTROL Submit Upload]**.

*Se quiser codificar seus vídeos usando o Dynamic Media Classic*

1. Na barra Navegação global, clique em **[!UICONTROL Upload]**.
1. Na página Upload , clique na guia **[!UICONTROL From Desktop]** .
1. No painel **[!UICONTROL Select Files to Upload]**, clique em **[!UICONTROL Browse]**, navegue até um arquivo de vídeo de fonte principal e clique em **[!UICONTROL Open]**.
1. No painel **[!UICONTROL Choose Folder Destination]**, selecione uma pasta para o arquivo carregado.
1. No canto inferior direito da página, clique em **[!UICONTROL Job Options]**,
1. Na caixa de diálogo Upload Job Options , expanda **[!UICONTROL EVideo Options]** e siga um destes procedimentos:

   * A prática recomendada é selecionar **[!UICONTROL Adaptive Video Encoding]**. Consulte [Vídeo adaptável (padrão)](application-setup.md#adaptive-video-default).
   * Opcional. Se desejar usar configurações de codificação individuais, expanda **[!UICONTROL Single Encoding Presets]** e selecione as opções de codificação desejadas para Desktop, Móvel e Tablet.
Consulte [Predefinições de codificação de vídeo de desktop](application-setup.md#desktop-video-encoding-presets), [Predefinições de codificação de vídeo móvel](application-setup.md#mobile-video-encoding-presets), [Predefinições de codificação de vídeo de tablet](application-setup.md#tablet-video-encoding-presets).
1. Na caixa de diálogo Upload Job Options , clique em **[!UICONTROL Save]**.
1. Na página Upload , verifique se **[!UICONTROL Publish After Uploading]** está marcado.
1. Na página Upload , no canto inferior direito, clique em **[!UICONTROL Submit Upload]**.

*Se quiser codificar novamente um arquivo de vídeo que você carregou anteriormente*

1. No Dynamic Media Classic, no painel Procurar, navegue até o vídeo e selecione-o.
1. Clique em **[!UICONTROL File]** > **[!UICONTROL Reprocess]**.
1. Na caixa de diálogo Reprocessar ativos , expanda **[!UICONTROL EVideo Options]** e siga um destes procedimentos:
   * A prática recomendada é usar o seguinte método. Selecione **Adaptive Video**.
Consulte [Vídeo adaptável (padrão)](application-setup.md#adaptive-video-default).
   * Opcional. Se desejar usar configurações de codificação individuais, expanda ****[!UICONTROL Single Encoding Presets]**** e selecione as opções de codificação desejadas para Desktop, Móvel e Tablet.
Consulte [Predefinições de codificação de vídeo de desktop](application-setup.md#desktop-video-encoding-presets), [Predefinições de codificação de vídeo móvel](application-setup.md#mobile-video-encoding-presets), [Predefinições de codificação de vídeo de tablet](application-setup.md#tablet-video-encoding-presets).
1. Na caixa de diálogo Reprocessar ativos , clique em **[!UICONTROL Submit]**.

Quando você usa a predefinição de codificação Vídeo adaptativo ou usa várias predefinições de codificação única, o resultado é um Conjunto de vídeos adaptáveis criado automaticamente com várias codificações de vídeo. Você também pode criar manualmente um Conjunto de vídeos adaptativos selecionando vídeos individuais.

Somente os tipos de arquivos MP4 e M4V são criados quando você gera um Conjunto de Vídeos Adaptativos de forma automática ou manual.

## Tipos de arquivo de vídeo compatíveis para codificação {#supported-video-file-types-for-encoding}

A tabela a seguir lista os tipos de arquivos de vídeo (com codecs de vídeo permitidos) que podem ser codificados no formato MP4 ou OGV ao carregar arquivos. A tabela lista os formatos de arquivo e codecs:

* **Formatos de arquivo de vídeo**  - Semelhante a um arquivo ZIP, o formato de arquivo de vídeo determina como os arquivos estão contidos no arquivo de vídeo. Um arquivo de vídeo geralmente contém várias faixas — uma faixa de vídeo (sem áudio) e uma ou mais faixas de áudio (sem vídeo) — que são interrelacionadas e sincronizadas. O formato de arquivo de vídeo determina como essas diferentes faixas de dados e metadados são organizados.

* **Codecs de vídeo**  - Um codec de vídeo descreve o algoritmo pelo qual um vídeo é codificado. Um reprodutor de vídeo decodifica o vídeo de acordo com seu codec e exibe uma série de imagens, ou quadros, na tela. Os codecs minimizam a quantidade de informações que os arquivos de vídeo precisam armazenar para reproduzir vídeo. Em vez de informações sobre cada quadro individual, somente as informações sobre as diferenças entre um quadro e o próximo são armazenadas. Como a maioria dos vídeos muda pouco de um quadro para outro, os codecs permitem altas taxas de compactação, o que resulta em tamanhos de arquivo menores.

   | Formato de arquivo de vídeo | Codecs de vídeo |
   |:--- |:--- |
   | 3GP | H.263, H.264 |
   | AVI | DivX, DV |
   | M2P | MPEG-2 PS |
   | M2T | MPEG-2 TS |
   | M2TS | MPEG-2 TS |
   | M2V | MPEG-2 ES |
   | M4V | H.264 |
   | MOV | DV, DVCPro 50, H.261, H.263, H.264, Sorenson Video 1 |
   | MP4 | H.264/MPEG-4 AVC |
   | MPEG | MPEG-2 SS |
   | MPG | MPEG-2 SS |
   | MTS | MPEG-2 |
   | ProRes | APCN , APCS, APCO, APCH, AP4H |
   | TS | DVCPro 50 |
   | VOB | MPEG-2 |
   | WMV/ASF | VC-1, Windows® Media Video 7, Windows® Media Video 8 |

   >[!NOTE]
   >
   >A tela Trabalhos o alerta se você fizer upload e tentar codificar um arquivo de vídeo, mas o arquivo for rejeitado, pois ele contém um codec ou um contêiner de arquivo incompatível. Para obter mais informações, consulte [Verificando arquivos de trabalho](checking-job-files.md).

## Práticas recomendadas para codificação de vídeo {#best-practices-for-video-encoding}

A seguir estão dicas de práticas recomendadas para a codificação de arquivos de vídeo de origem no Dynamic Media Classic.

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### Arquivos de vídeo de origem {#source-video-files}

Ao codificar um arquivo de vídeo, use um arquivo de vídeo de origem com a maior qualidade possível. Evite usar arquivos de vídeo previamente codificados, pois esses arquivos já estão compactados, e uma codificação adicional criará um vídeo de qualidade inferior.

A tabela a seguir descreve o tamanho recomendado, a proporção e a taxa mínima de bits que seus arquivos de vídeo de origem devem ter ao codificá-los:

| Tamanho | Proporção | Taxa mínima de bits |
|--- |--- |--- |
| 1024 X 768 | 4:3 | 4500 kbps para a maioria dos vídeos. |
| 1280 X 720 | 16:99 | 3000 - 6000 kbps, dependendo da quantidade de movimento no vídeo. |
| 1920 X 1080 | 16:99 | 6000 - 8000 kbps, dependendo da quantidade de movimento no vídeo. |

### Obter os metadados de um arquivo {#obtaining-a-file-s-metadata}

Você pode obter os metadados de um arquivo ao exibir os metadados no Dynamic Media Classic, usando uma ferramenta de edição de vídeo ou um aplicativo projetado para obter metadados. A seguir estão as instruções para usar MediaInfo, um aplicativo de terceiros, para obter os metadados de um arquivo de vídeo:

1. Vá para esta página da Web: [https://mediainfo.sourceforge.net/en/Download](https://mediainfo.sourceforge.net/en/Download).
1. Selecione e baixe o instalador da versão da GUI e siga as instruções de instalação.
1. Após a instalação, clique com o botão direito do mouse no arquivo de vídeo (somente Windows®) e selecione MediaInfo ou abra MediaInfo e arraste o arquivo de vídeo para o aplicativo. Você verá todos os metadados associados ao arquivo de vídeo, incluindo largura, altura e fps.

### Proporção {#aspect-ratio}

Ao escolher ou criar uma predefinição de codificação de vídeo para o arquivo de vídeo principal, verifique se a predefinição tem a mesma proporção do vídeo principal. A *proporção* é a relação da largura com a altura do vídeo.

Para determinar a proporção de um arquivo de vídeo, obtenha os metadados do arquivo e anote a largura e a altura do arquivo (consulte [Obter os metadados de um arquivo](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Em seguida, use essa fórmula para determinar a proporção:

largura/altura = proporção

A tabela a seguir descreve como os resultados da fórmula são traduzidos para opções comuns de proporção:

| Resultado da fórmula | Proporção |
|--- |--- |
| 1,33 | 4:3 |
| 0,75 | 3:4 |
| 1,78 | 16:99 |
| 0,56 | 9:16 |

Por exemplo, um vídeo com 1440 largura x 1080 altura tem uma proporção largura/altura de 1440/1080 ou 1,33. Nesse caso, você escolhe uma predefinição de codificação de vídeo com uma proporção de aspecto 4:3 para codificar o arquivo de vídeo.

### Taxa de dados {#data-rate}

A *data rate* (também chamada de *bit rate*) é a quantidade de dados codificada para formar um único segundo de reprodução de vídeo. A taxa de dados é medida em kilobits por segundo (Kbps).

>[!NOTE]
>
>Como todos os codecs usam compactação com perdas, a taxa de dados é o fator mais importante na qualidade do vídeo. Com a compactação com perdas, quanto mais você compacta um arquivo de vídeo, mais a qualidade é degradada. Por isso, todas as outras características são iguais (resolução, taxa de quadros e codec), quanto menor a taxa de dados, menor a qualidade do arquivo compactado.

Ao escolher uma predefinição de codificação de vídeo, lembre-se de considerar a velocidade de conexão do usuário final de destino. Escolha uma predefinição com uma taxa de dados de 80% dessa velocidade. Por exemplo, se a velocidade de conexão do usuário final de destino for 1000 Kbps, a melhor predefinição é aquela com uma taxa de dados de vídeo de 800 Kbps.

Esta tabela descreve a taxa de dados de velocidades de conexão típicas.

| Velocidade (Kbps) | Tipo de conexão |
|--- |--- |
| 256 | Conexão discada. |
| 800 | Conexão móvel típica. Para essa conexão, direcione uma taxa de dados no intervalo de 400 a um máximo de 800 para experiências 3G. |
| 2000 | Conexão típica de desktop de banda larga. Para esta conexão, direcione uma taxa de dados no intervalo de 800-2000 Kbps, com a maioria dos destinos com média de 1200-1500 Kbps. |
| 5000 | Conexão típica de alta banda larga. A codificação nesse intervalo superior não é recomendada porque a entrega de vídeo nessa velocidade não está disponível para a maioria dos consumidores. |

### Resolução {#resolution}

** A solução descreve a altura e a largura de um arquivo de vídeo em pixels. A maioria dos vídeos de origem é armazenada em alta resolução (por exemplo, 1920 x 1080). Para fins de transmissão, o vídeo de origem é compactado em uma resolução menor (640 x 480 ou menor).

A resolução e a taxa de dados são dois fatores totalmente vinculados que determinam a qualidade do vídeo. Para manter a mesma qualidade de vídeo, quanto maior o número de pixels em um arquivo de vídeo (quanto maior a resolução), maior deverá ser a taxa de dados. Por exemplo, considere o número de pixels por quadro em uma resolução de 320 x 240 e um arquivo de vídeo de resolução de 640 x 480:

| Resolução | Pixels por quadro |
|--- |--- |
| 320 x 240 | 76 800 |
| 640 x 480 | 307 200 |

O arquivo de 640 x 480 tem quatro vezes mais pixels por quadro. Para atingir a mesma taxa de dados para essas duas resoluções de exemplo, aplique quatro vezes a compactação no arquivo 640 x 480, o que pode reduzir a qualidade do vídeo. Portanto, uma taxa de dados de vídeo de 250 Kbps produz uma exibição de alta qualidade com uma resolução de 320 x 240, mas não com resolução de 640 x 480.

>[!NOTE]
>
>Em geral, quanto maior for a taxa de dados, melhor será a exibição do vídeo e, quanto maior for a resolução usada, maior será a taxa de dados que deve manter a qualidade de visualização (em comparação com resoluções mais baixas).

Como a resolução e a taxa de dados estão vinculadas, você tem duas opções ao codificar o vídeo:

* Escolha uma taxa de dados e, em seguida, codifique na resolução mais alta que apareça melhor na taxa de dados escolhida.
* Escolha uma resolução e, em seguida, codifique na taxa de dados necessária para obter vídeo de alta qualidade na resolução escolhida.

Ao escolher (ou criar) uma predefinição de codificação de vídeo para o arquivo de vídeo principal, use esta tabela para direcionar a resolução correta:

| Resolução | Altura (pixels) | Tamanho da tela |
|--- |--- |--- |
| 240p | 240 | Tela pequena |
| 300p | 300 | Tela pequena normalmente para dispositivos móveis |
| 360p | 360 | Tela pequena |
| 480p | 480 | Tela média |
| 720p | 720 | Tela grande |
| 1080p | 1080 | Tela grande de alta definição |

### Fps (quadros por segundo) {#fps-frames-per-second}

Nos Estados Unidos e Japão, a maioria dos vídeos é capturada a 29,97 quadros por segundo (fps); na Europa, a maioria dos vídeos é filmada a 25 fps. O filme é filmado a 24 fps.

Escolha uma predefinição de codificação de vídeo que corresponda à taxa fps do arquivo de vídeo principal. Por exemplo, se o vídeo principal tiver 25 fps, escolha uma predefinição de codificação com 25 fps. Por padrão, toda codificação personalizada usa o fps do arquivo de vídeo principal. Por isso, não é necessário especificar explicitamente a configuração fps ao criar uma predefinição de codificação de vídeo.

### Dimensões de codificação de vídeo {#video-encoding-dimensions}

Para obter resultados ideais, selecione dimensões de codificação de modo que o vídeo de origem seja um múltiplo completo de todos os vídeos codificados.

Para calcular essa proporção, você divide a largura da origem por largura codificada para obter a relação de largura. Em seguida, divida a altura da origem por altura codificada para obter a proporção de altura.

Se a proporção resultante for um inteiro, significa que o vídeo é dimensionado de maneira ideal. Se a proporção resultante não for um inteiro, ela afetará a qualidade do vídeo, deixando artefatos de pixel à esquerda na exibição. Esse efeito é mais notável quando o vídeo tem texto.

Por exemplo, suponha que o vídeo de origem seja 1920 x 1080. Na tabela a seguir, os três vídeos codificados fornecem as configurações de codificação ideais para usar.

| Tipo de vídeo | Largura x altura | Proporção de largura | Taxa de altura |
|--- |--- |--- |--- |
| Origem | 1920 x 1080 | 1 | 1 |
| Codificado | 960 x 540 | 2 | 2 |
| Codificado | 640 x 360 | 3 | 1 |
| Codificado | 480 x 270 | 4 | 4 |

### Formato de arquivo de vídeo codificado {#encoded-video-file-format}

O Adobe Dynamic Media Classic recomenda o uso de predefinições de codificação de vídeo MP4 H.264. Como os arquivos MP4 usam o codec de vídeo H.264, ele fornece vídeo de alta qualidade, mas em um tamanho de arquivo compactado.

## Trabalhar com predefinições de codificação de vídeo {#working-with-video-encoding-presets}

Os arquivos de vídeo principais criados com equipamento de produção de vídeo e software de edição de vídeo geralmente são muito grandes e não estão no formato adequado para entrega em destinos online. Para converter vídeo digital no formato e especificações adequados para reprodução em diferentes telas, você pode *transcodificar* arquivos de vídeo (um processo também conhecido como *encoding*). Durante o processo de codificação, o vídeo é compactado em um tamanho de arquivo menor e eficiente para proporcionar a entrega ideal à Web e a dispositivos móveis.

Consulte [Fazer upload e codificar vídeos](uploading-encoding-videos.md#uploading-and-encoding-videos).

O Dynamic Media Classic oferece uma biblioteca de predefinições de codificação de vídeo predefinidas que refletem as configurações de codificação mais comuns usadas hoje. Essas predefinições de codificação são otimizadas para reprodução nas telas de destino. Além disso, os administradores podem criar suas próprias predefinições de codificação de vídeo para personalizar o tamanho e a qualidade da reprodução dos vídeos para os usuários finais. Todas as predefinições de codificação de vídeo, sejam elas prontas para uso do Dynamic Media Classic ou personalizadas, exibem vídeo no formato de arquivo MP4.

Na tela Predefinições de vídeo, os administradores podem configurar e gerenciar a codificação de vídeo. Eles podem fazer o seguinte:

* Ative e desative as predefinições de codificação de vídeo.
* Crie uma predefinição de codificação de vídeo.
* Edite as predefinições de codificação de vídeo.
* Excluir predefinições de vídeo.

Qualquer vídeo que você faça upload para o Dynamic Media Classic ou que codifique no Dynamic Media Classic será tratado como &quot;vídeo&quot;. Em outras palavras, essa classificação de ativos significa que você pode fornecer o vídeo para reprodução em desktops, dispositivos móveis ou ambos. Por exemplo, você pode visualizar esses tipos de vídeos no Dynamic Media Classic. Também é possível gerar URLs (usando o recurso Copiar URL) e código que você pode incorporar (usando o recurso Incorporar código) para usar com players de vídeo, em sites e assim por diante.

Consulte [Visualização de vídeos em um visualizador de vídeo](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Consulte [Vincular um URL de vídeo a um site para dispositivos móveis ou a um site](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Consulte [Incorporar o visualizador de vídeo em uma página da Web](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Para ativos de vídeo que você faz upload e codifica no Dynamic Media Classic, o vídeo é entregue no seguinte formato de arquivo:

**MP4 H.264** Use arquivos MP4 para o seguinte:

* HTTP Dynamic Streaming em desktops.
* HLS (HTTP Live Streaming, protocolo de transmissão da Apple).
* Entrega de vídeo progressivo para dispositivos móveis Android™, BlackBerry® e Windows®.

Qualquer outro formato e codec de vídeo é tratado como um &quot;Vídeo Principal&quot;. Essa classificação de ativo significa que o vídeo é um arquivo de vídeo de origem e não pode ser usado para reprodução de delivery em desktops ou dispositivos móveis. Por exemplo, você não pode visualizar esses tipos de vídeos no Dynamic Media Classic. Também não é possível gerar Copiar URLs ou Incorporar código para uso em players de vídeo, sites e assim por diante.

### Filtragem da lista de predefinições de codificação de vídeo {#filtering-the-list-of-video-encoding-presets}

A página Predefinições de vídeo e a página Predefinições de vídeo adaptáveis consistem em uma tabela que lista o status ativo, o nome predefinido, o dispositivo de reprodução pretendido, o tamanho do vídeo e a taxa de dados de cada predefinição de vídeo.

Você pode refinar a lista optando por filtrar em Ambos, Ativo ou Inativo, para ver todas as Predefinições de vídeo ou restringir a lista a predefinições que estão ativas ou inativas.

Também é possível filtrar com base em uma opção de dispositivo de reprodução para restringir a lista a Predefinições de vídeo criadas para reprodução de vídeos em todos os dispositivos, desktops, dispositivos móveis ou tablets.

**Para filtrar a lista de predefinições de codificação de vídeo:**

1. No Dynamic Media Classic, na barra Navegação global, clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Adaptive Video Presets]** ou **[!UICONTROL Single Encoding Presets]**.

   As páginas para Predefinições de vídeo adaptativo e Predefinições de codificação única incluem uma tabela que lista o status Ativo, o nome predefinido, o Dispositivo de reprodução pretendido, as dimensões do vídeo e a taxa de dados de cada predefinição de vídeo.

1. Na página Predefinições de codificação única chamada Predefinições de vídeo, na barra de ferramentas Predefinições de vídeo, use as duas listas suspensas para refinar a lista de predefinições na tabela com base no status Ativo e no dispositivo de reprodução.

   * Na primeira lista suspensa mais estreita, escolha **[!UICONTROL Both]** para visualizar todas as Predefinições de vídeo, escolha **[!UICONTROL Active]** ou **[!UICONTROL Inactive]** ou restrinja a lista a predefinições que estão ativas ou inativas.
   * Na segunda lista suspensa mais ampla, escolha uma opção de dispositivo de reprodução para limitar a lista às Predefinições de vídeo criadas para reprodução de vídeos em desktops. ou para reproduzir vídeos em dispositivos móveis ou tablets.

### Ativação ou desativação das predefinições de codificação de vídeo {#activating-or-deactivating-video-encoding-presets}

As predefinições de vídeo ativadas são exibidas na caixa de diálogo Opções de trabalho de upload . A caixa de diálogo é exibida quando um usuário carrega arquivos de vídeo durante o processo de upload. Eles podem escolher em uma lista de todas as predefinições de codificação ativadas.

1. No Dynamic Media Classic, na barra Navegação global, clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]**.
1. Siga um destes procedimentos:

   * Clique em **[!UICONTROL Adaptive Video Presets]**.
   * Clique em **[!UICONTROL Single Encoding Presets]**.

1. Siga um destes procedimentos:

   * Para ativar uma predefinição de vídeo, na página predefinições, na coluna Ativo , selecione a caixa ao lado de um nome predefinido.
   * Para desativar uma predefinição de vídeo, desmarque a caixa ao lado das predefinições de vídeo que você deseja tornar inativas.

      >[!NOTE]
      >
      >As predefinições de vídeo inativas não são exibidas na caixa de diálogo Opções de trabalho de upload .

1. No canto inferior direito da página, clique em **[!UICONTROL Close]**.

### Adicionar ou editar uma predefinição de codificação de vídeo {#adding-or-editing-a-video-encoding-preset}

Você pode criar suas próprias predefinições de vídeo de codificação única personalizadas e adicioná-las à tabela de Predefinições de vídeo. Também é possível alterar qualquer predefinição de vídeo de codificação única e predefinida que vem com o Dynamic Media Classic, desde que você salve a predefinição editada com um novo nome.

O Dynamic Media Classic definiu limites máximos para a taxa de dados do target, a altura da resolução e a largura da resolução para garantir uma experiência de reprodução adequada. As mensagens de aviso são exibidas se você exceder esses limites, que são os seguintes:

* Para reprodução de computador, os limites são: (Largura/16) * (Altura/16) &lt; 8192.
* Para reprodução móvel, os limites são: (Largura/16) * (Altura/16) &lt; 660; taxa de dados pretendida &lt; 4000.
* Para a reprodução do tablet, os limites são: (Largura/16) * (Altura/16) &lt; 3600.

**Para adicionar ou editar uma predefinição de codificação de vídeo:**

1. No Dynamic Media Classic, na barra Navegação global, clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]**.
1. Clique em **[!UICONTROL Single Encoding Presets]**.
1. Na página Predefinições de vídeo , siga um destes procedimentos:

   * Na barra de ferramentas Predefinições de vídeo, clique em **[!UICONTROL Add]** para adicionar uma Predefinição de vídeo.
   * Selecione uma predefinição de vídeo. Na barra de ferramentas, clique em **[!UICONTROL Edit]**.

      Não é possível editar predefinições predefinidas do Dynamic Media Classic; você só pode criar uma predefinição a partir de uma predefinição existente escolhendo **[!UICONTROL Save As]**.

1. Na página Adicionar predefinição de vídeo ou Editar predefinição de vídeo , defina as opções de Predefinição de vídeo desejadas.

   Consulte [Práticas recomendadas para codificação de vídeo](uploading-encoding-videos.md#best-practices-for-video-encoding) para obter as configurações recomendadas.

   | Opção Predefinição de vídeo | Descrição |
   |--- |--- |
   | Nome da predefinição | Insira um nome descritivo para a predefinição de vídeo. O nome inserido é exibido na caixa de diálogo Upload Job Options , na qual os usuários escolhem opções de transcodificação. |
   | Descrição | Descreva a predefinição de vídeo. O item inserido aparece como uma dica de ferramenta ao mover o ponteiro sobre o nome da predefinição na caixa de diálogo Upload Job Options , na qual os usuários escolhem opções de transcodificação. |
   | Dispositivo de reprodução | Escolha o dispositivo no qual o vídeo deve ser reproduzido. As opções são Computador (desktops), Móvel (iPhone, iPad, Android™); ou Tablet (somente iPad). Essa configuração determina automaticamente o codec de áudio e vídeo apropriado usado durante a codificação. |
   | Taxa de dados do Target | Insira a velocidade média de conexão com a Internet (em kilobits por segundo) do usuário final do target. É possível inserir a taxa ou arrastar o controle deslizante para inseri-la. O espectro Velocidade de Conexão do Usuário lista as velocidades típicas para banda larga, DSL, dispositivos móveis e conexões dial-up. Essa configuração determina automaticamente a taxa de dados de áudio e vídeo combinados. Em outras palavras, a quantidade de dados que é codificada para formar um único segundo de reprodução de vídeo. Quanto maior a taxa de dados, melhor a qualidade do vídeo resultante. No entanto, as taxas de dados muito altas resultam em tamanhos de arquivo grandes que criam experiências de visualização de subpar para usuários com uma largura de banda baixa. Como prática recomendada, encontre um equilíbrio entre taxas de dados altas e baixas. Pretende criar uma experiência de reprodução de qualidade adequada sem alienar os usuários que têm larguras de banda estreitas. |
   | Proporção | Proporção é a relação entre a largura e a altura do vídeo. As duas primeiras proporções listadas abaixo são normalmente usadas para exibir o vídeo horizontalmente:<ul><li> 4:3 - Usado para quase todo o conteúdo de transmissão de TV de definição padrão.</li><li>16:9 - Usado para quase todos os conteúdos de TV de alta definição (HDTV) e filmes em tela larga.</li><li>Dimensionamento automático - (Padrão) Uma única predefinição de codificação que funciona com qualquer proporção para criar vídeos para entrega em dispositivos móveis, tablets e desktops. Os vídeos de origem carregados codificados com essa predefinição são definidos com uma altura fixa. No entanto, a largura é dimensionada automaticamente para preservar a proporção do aspecto do vídeo (relação largura/altura).</li><li>Personalizado - Usado quando você deseja definir um tamanho de vídeo não padrão.</li><li>A proporção escolhida determina as configurações de largura e altura do Tamanho da Resolução; o valor de largura e altura é dimensionado automaticamente para a proporção correta.</li></ul> |
   | Tamanho da Resolução | O tamanho da resolução, expresso pelo número de pixels de largura pelo número de pixels de altura, determina o tamanho. Insira um valor de largura e altura em pixels ou arraste o controle deslizante para inserir esses valores. O espectro de resolução lista os tamanhos de resolução típicos. Os valores de largura e altura aderem automaticamente à proporção selecionada. Por exemplo, se você selecionar 4:3 como proporção e inserir 400 para largura, 300 será inserido automaticamente para altura. Se você selecionou Dimensionamento automático para a configuração Proporção de aspecto , o valor de Largura para o Tamanho da resolução é automaticamente definido como Automático. Clique em Visualizar para que você possa abrir uma janela do navegador e ver suas opções de resolução lá. |
   | Codificar sufixo do arquivo | Insira um sufixo. Esse sufixo é anexado ao arquivo de vídeo codificado resultante. Você pode inserir um hífen e um sublinhado no nome; espaços em branco e caracteres especiais não são permitidos. |
   | Outras configurações | O Dynamic Media Classic determina todas as outras configurações de codificação automaticamente de acordo com as diretrizes de codificação de práticas recomendadas. |

1. Siga um destes procedimentos:

   * Clique em **[!UICONTROL Save]** se tiver adicionado ou editado uma Predefinição de vídeo.
   * Clique em **[!UICONTROL Save As]** se tiver adicionado uma Predefinição de vídeo iniciando em uma predefinição existente.

### Exclusão de uma predefinição de codificação de vídeo {#deleting-a-video-encoding-preset}

Os administradores podem excluir predefinições de vídeo personalizadas. As predefinições de vídeo fornecidas com o Dynamic Media Classic não podem ser excluídas.

1. No Dynamic Media Classic, na barra Navegação global, clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]**.
1. Clique em **[!UICONTROL Single Encoding Presets]**.
1. Na página Predefinições de vídeo , selecione uma Predefinição de vídeo na tabela que não deseja mais nem precisa.
1. Na barra de ferramentas Predefinições de vídeo, clique em **[!UICONTROL Delete]**.
1. Na caixa de diálogo Excluir predefinição, clique em **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [Início rápido: Vídeo](quick-start-video.md#quick-start-video)
* [Upload e codificação de vídeos](uploading-encoding-videos.md#uploading-and-encoding-videos)
* [Trabalhar com predefinições do visualizador de vídeo](previewing-videos-video-viewer.md#working-with-video-viewer-presets)

