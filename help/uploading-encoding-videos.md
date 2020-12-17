---
title: Carregamento e codificação de vídeos
seo-title: Carregamento e codificação de vídeos
description: Saiba como carregar e codificar vídeos.
seo-description: Saiba como carregar e codificar vídeos.
uuid: 9a7d6513-b10c-40b0-aebb-18a795c2b8d1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: a0941823-850c-4373-9e37-f32032de3805
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '3938'
ht-degree: 1%

---


# Carregamento e codificação de vídeos{#uploading-and-encoding-videos}

Para criar um único vídeo ou conjuntos de vídeos adaptáveis para o delivery na Web ou em dispositivos móveis, primeiro carregue os arquivos de vídeo principais no Dynamic Media Classic. O Dynamic Media Classic codifica vídeos no formato MP4 e publica vídeos nos seguintes formatos de arquivo:

**O MP4** Dynamic Media Classic recomenda o MP4 como o formato de arquivo de vídeo preferencial. Use arquivos MP4 para o seguinte:

* HTTP Dynamic Streaming em desktops.
* HTTP Live Streaming (protocolo de streaming da Apple).
* Delivery de vídeo progressivo para dispositivos móveis Android, Blackberry e Windows

O Dynamic Media Classic oferta dois workflows para carregar arquivos de vídeo:

**Vídeos pré-codificados** Você carrega arquivos MP4 diretamente no Dynamic Media Classic. Com esse fluxo de trabalho, os arquivos não são codificados no momento em que você os carrega. Os arquivos são pré-codificados em preparação para o delivery para o desktop e para dispositivos móveis.

**Vídeos de origem principalFaça upload de arquivos de vídeo de origem principal e, ao fazer upload, codifique esses arquivos em arquivos MP4.** Os vídeos codificados são rotulados como &quot;Vídeo&quot; no painel Procurar. O Dynamic Media Classic é compatível com a codificação de arquivos de vídeo em vários formatos.

* Verifique se os arquivos de vídeo de origem principal que você deseja codificar são suportados.

   Consulte [Tipos de arquivos de vídeo suportados para codificação](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

* Escolha uma predefinição de codificação de vídeo.

   Consulte [Predefinições de vídeo para codificação de arquivos de vídeo](application-setup.md#video-presets-for-encoding-video-files).

   Consulte [Práticas recomendadas para codificação de vídeo](uploading-encoding-videos.md#best-practices-for-video-encoding).

O Dynamic Media Classic também gera miniaturas de vídeo. Você pode saber mais sobre miniaturas de vídeo, como obter seus URLs e modificar quadros de pôster.

Consulte [Trabalhar com miniaturas de vídeo](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**Para carregar e codificar vídeos**

Execute um dos procedimentos a seguir:

*Se os vídeos já estiverem codificados*

1. Na barra Navegação global, clique em **Carregar**.
1. Na tela Carregar, clique na guia **Da área de trabalho**.
1. Na página Carregar, no painel Selecionar arquivos para upload, clique em **Procurar**, navegue até um arquivo de vídeo MP4 e clique em **Abrir**.
1. No painel Escolher destino da pasta, selecione uma pasta para o arquivo carregado.
1. Na página Carregar, verifique se **Publicar após carregar** está marcada.
1. Clique em **Enviar upload**.

*Se quiser codificar seus vídeos usando o Dynamic Media Classic*

1. Na barra Navegação global, clique em **Carregar**.
1. Na tela Carregar, clique na guia **Da área de trabalho**.
1. No painel Selecionar arquivos para carregar, clique em **Procurar**, navegue até um arquivo de vídeo de origem principal e clique em **Abrir**.
1. No painel Escolher destino da pasta, selecione uma pasta para o arquivo carregado.
1. No canto inferior direito da página, clique em **Opções de Trabalho**,
1. Na caixa de diálogo Carregar opções de trabalho, expanda Opções de vídeo.
   * Execute um dos procedimentos a seguir:
      * A prática recomendada é usar o método a seguir.
Selecione **Codificação de vídeo adaptável**.
Consulte [Vídeo adaptativo (padrão)](application-setup.md#adaptive-video-default).
   * Opcional, se desejar usar configurações de codificação individuais, faça o seguinte.
Expanda **Predefinições de codificação única** e selecione as opções de codificação que deseja para Desktop, Móvel e Tablet.
Consulte [Predefinições de codificação de vídeo do desktop](application-setup.md#desktop-video-encoding-presets), [Predefinições de codificação de vídeo móvel](application-setup.md#mobile-video-encoding-presets), [Predefinições de codificação de vídeo do Tablet](application-setup.md#tablet-video-encoding-presets).
1. Na caixa de diálogo Carregar opções de trabalho, clique em **Salvar**.
1. Na página Carregar, verifique se **Publicar após carregar** está marcada.
1. Na página Carregar, no canto inferior direito, clique em **Enviar upload**.

Se quiser codificar novamente um arquivo de vídeo que você carregou anteriormente

1. No Dynamic Media Classic, no painel Procurar, navegue até o vídeo e selecione-o.
1. Clique em **Arquivo** > **Reprocessar**.
1. Na caixa de diálogo Reprocessar ativos, expanda Opções de vídeo.
1. Execute um dos procedimentos a seguir:
   * A prática recomendada é usar o método a seguir.
Selecione **Vídeo adaptativo**.
Consulte [Vídeo adaptativo (padrão)](application-setup.md#adaptive-video-default).
   * Opcional, se desejar usar configurações de codificação individuais, faça o seguinte.
Expanda **Predefinições de codificação única** e selecione as opções de codificação que deseja para Desktop, Móvel e Tablet.
Consulte [Predefinições de codificação de vídeo do desktop](application-setup.md#desktop-video-encoding-presets), [Predefinições de codificação de vídeo móvel](application-setup.md#mobile-video-encoding-presets), [Predefinições de codificação de vídeo do Tablet](application-setup.md#tablet-video-encoding-presets).
1. Na caixa de diálogo Reprocessar ativos, clique em **Enviar**.

Quando você usa a predefinição de codificação de vídeo adaptável ou usa várias predefinições de codificação única, o resultado é um Conjunto de vídeos adaptáveis que é criado automaticamente com várias codificações de vídeo. Você também pode criar manualmente um Conjunto de vídeos adaptáveis selecionando vídeos individuais.

Somente os tipos de arquivos MP4 e M4V são criados quando você gera um Conjunto de vídeos adaptável automática ou manualmente.

## Tipos de arquivos de vídeo suportados para codificação {#supported-video-file-types-for-encoding}

A tabela a seguir lista os tipos de arquivos de vídeo (com codecs de vídeo permitidos) que você pode codificar no formato MP4 ou OGV ao carregar arquivos. A tabela lista formatos de arquivo e codecs:

**Formatos de arquivo de vídeoSemelhante a um arquivo ZIP, um formato de arquivo de vídeo determina como os arquivos estão contidos no arquivo de vídeo.** Um arquivo de vídeo normalmente contém várias faixas. uma faixa de vídeo (sem áudio) e uma ou mais faixas de áudio (sem vídeo) — que estão inter-relacionados e sincronizados. O formato de arquivo de vídeo determina como esses diferentes rastreamentos de dados e metadados são organizados.

**Codecs** de vídeo Um codec de vídeo descreve o algoritmo pelo qual um vídeo é codificado. Um player de vídeo decodifica o vídeo de acordo com seu codec e exibe uma série de imagens, ou quadros, na tela. Os codecs minimizam a quantidade de informações que os arquivos de vídeo são necessários para armazenar para reproduzir o vídeo. Em vez de informações sobre cada quadro individual, somente as informações sobre as diferenças entre um quadro e o seguinte são armazenadas. Como a maioria dos vídeos muda pouco de um quadro para outro, os codecs permitem altas taxas de compactação, o que resulta em tamanhos menores de arquivos.

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
| ProRes | APCN, APCS, APCO, APCH, AP4H |
| TS | DVCPro 50 |
| VOB | MPEG-2 |
| WMV/ASF | VC-1, Windows Media Video 7, Windows Media Video 8 |

>[!NOTE]
>
>A tela Tarefas alerta você se você fizer upload e tentar codificar um arquivo de vídeo, mas o arquivo for rejeitado, pois ele contém um codec ou container de arquivo incompatível. Para obter mais informações, consulte [Verificando arquivos de trabalho](checking-job-files.md).

## Práticas recomendadas para codificação de vídeo {#best-practices-for-video-encoding}

Veja a seguir dicas de práticas recomendadas para a codificação de arquivos de vídeo de origem no Dynamic Media Classic.

Para obter conselhos sobre a codificação de vídeo, consulte:

* Artigo: *Streaming 101: Os fundamentos... Codecs, largura de banda, taxa de dados e resolução: * [www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en).
* Vídeo: *Conceitos básicos de codificação de vídeo: * [www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en).

### Arquivos de vídeo de origem {#source-video-files}

Ao codificar um arquivo de vídeo, use um arquivo de vídeo de origem com a qualidade mais alta possível. Evite usar arquivos de vídeo previamente codificados, pois esses arquivos já estão compactados, e a codificação adicional cria um vídeo de qualidade inferior.

A tabela a seguir descreve o tamanho recomendado, a proporção e a taxa mínima de bits que seus arquivos de vídeo de origem devem ter ao codificá-los:

| Tamanho | Taxa de proporção | Taxa mínima de bits |
|--- |--- |--- |
| 1024 X 768 | 4:3 | 4500 kbps para a maioria dos vídeos. |
| 1280 X 720 | 16:90 | 3000 - 6000 kbps, dependendo da quantidade de movimento no vídeo. |
| 1920 X 1080 | 16:90 | 6000 - 8000 kbps, dependendo da quantidade de movimento no vídeo. |

### Obtenção dos metadados de um arquivo {#obtaining-a-file-s-metadata}

Você pode obter os metadados de um arquivo visualizando seus metadados no Dynamic Media Classic, usando uma ferramenta de edição de vídeo ou um aplicativo projetado para obter metadados. Veja a seguir as instruções de uso do MediaInfo, um aplicativo de terceiros, para obter os metadados de um arquivo de vídeo:

1. Ir para esta página da Web: [https://mediainfo.sourceforge.net/en/Download](https://mediainfo.sourceforge.net/en/Download).
1. Selecione e baixe o instalador da versão da GUI e siga as instruções de instalação.
1. Após a instalação, clique com o botão direito do mouse no arquivo de vídeo (somente Windows) e selecione MediaInfo, ou abra MediaInfo e arraste o arquivo de vídeo para o aplicativo. Todos os metadados associados ao arquivo de vídeo, incluindo largura, altura e fps.

### Taxa de proporção {#aspect-ratio}

Ao escolher ou criar uma predefinição de codificação de vídeo para o arquivo de vídeo principal, verifique se a predefinição tem a mesma proporção do arquivo de vídeo principal. A *proporção* é a proporção entre a largura e a altura do vídeo.

Para determinar a proporção de um arquivo de vídeo, obtenha os metadados do arquivo e observe a largura e a altura do arquivo (consulte [Obtenção dos metadados do arquivo](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Em seguida, use essa fórmula para determinar a proporção:

largura/altura = proporção

A tabela a seguir descreve como os resultados da fórmula se traduzem em opções de proporção comuns:

| Resultado da fórmula | Taxa de proporção |
|--- |--- |
| 1,33 | 4:3 |
| 0,75 | 3:4 |
| 1,78 | 16:90 |
| 0,56 | 09:16 |

Por exemplo, um vídeo com largura de 1440 x altura de 1080 tem uma proporção largura/altura de 1440/1080 ou 1,33. Nesse caso, escolha uma predefinição de codificação de vídeo com uma proporção de 4:3 para codificar o arquivo de vídeo.

### Taxa de dados {#data-rate}

A *taxa de dados* (também chamada de* bit rate*) é a quantidade de dados que é codificada para formar um único segundo de reprodução de vídeo. A taxa de dados é medida em kilobits por segundo (Kbps).

>[!NOTE]
>
>Como todos os codecs usam compactação com perdas, a taxa de dados é o fator mais importante na qualidade do vídeo. Com a compactação com perdas, quanto mais você compacta um arquivo de vídeo, mais a qualidade é degradada. Por isso, todas as outras características são iguais (resolução, taxa de quadros e codec), quanto menor a taxa de dados, menor a qualidade do arquivo compactado.

Ao escolher uma predefinição de codificação de vídeo, considere a velocidade de conexão do usuário final do público alvo. Escolha uma predefinição com uma taxa de dados que seja 80% dessa velocidade. Por exemplo, se a velocidade de conexão do usuário final do público alvo for de 1000 Kbps, a melhor predefinição será aquela com uma taxa de dados de vídeo de 800 Kbps.

Esta tabela descreve a taxa de dados de velocidades de conexão típicas.

| Velocidade (Kbps) | Tipo de conexão |
|--- |--- |
| 256 | Conexão dial-up. |
| 600 | Conexão móvel típica. Para essa conexão, público alvo uma taxa de dados no intervalo de 400 a um máximo de 800 para experiências 3G. |
| 2000 | Conexão típica de desktop de banda larga. Para esta conexão, público alvo uma taxa de dados no intervalo de 800 a 2000 Kbps, com a maioria dos públicos alvos, em média, de 1200 a 1500 Kbps. |
| 5000 | Conexão típica de banda larga alta. Não é recomendável a codificação nesse intervalo superior, pois o delivery de vídeo nessa velocidade não está disponível para a maioria dos consumidores. |

### Resolução {#resolution}

*A* resolução descreve a altura e a largura de um arquivo de vídeo em pixels. A maioria dos vídeos de origem é armazenada em alta resolução (por exemplo, 1920 x 1080). Para fins de streaming, o vídeo de origem é compactado em uma resolução menor (640 x 480 ou menor).

A resolução e a taxa de dados são dois fatores totalmente ligados que determinam a qualidade do vídeo. Para manter a mesma qualidade de vídeo, quanto maior o número de pixels em um arquivo de vídeo (quanto maior a resolução), maior deve ser a taxa de dados. Por exemplo, considere o número de pixels por quadro em uma resolução 320 x 240 e um arquivo de vídeo de resolução 640 x 480:

| Resolução | Pixels por quadro |
|--- |--- |
| 320 x 240 | 76 800 |
| 640 x 480 | 307 200 |

O arquivo 640 x 480 tem quatro vezes mais pixels por quadro. Para obter a mesma taxa de dados para essas duas resoluções de exemplo, aplique quatro vezes a compactação ao arquivo 640 x 480, o que pode reduzir a qualidade do vídeo. Portanto, uma taxa de dados de vídeo de 250 Kbps produz uma visualização de alta qualidade em uma resolução de 320 x 240, mas não em uma resolução de 640 x 480.

>[!NOTE]
>
>Em geral, quanto maior for a taxa de dados, melhor será a aparência do vídeo e maior será a resolução usada, maior será a taxa de dados necessária para manter a qualidade de exibição (em comparação com resoluções mais baixas).

Como a resolução e a taxa de dados estão vinculadas, você tem duas opções ao codificar o vídeo:

* Escolha uma taxa de dados e, em seguida, codifique na resolução mais alta que tenha boa aparência na taxa de dados escolhida.
* Escolha uma resolução e, em seguida, codifique na taxa de dados necessária para obter vídeo de alta qualidade na resolução escolhida.

Ao escolher (ou criar) uma predefinição de codificação de vídeo para o arquivo de vídeo principal, use esta tabela para público alvo da resolução correta:

| Resolução | Altura (pixels) | Tamanho da tela |
|--- |--- |--- |
| 240 p | 240 | Tela pequena |
| 300 p | 300 | Tela pequena geralmente para dispositivos móveis |
| 360 p | 360 | Tela pequena |
| 480 p | 480 | Tela média |
| 720p | 720 | Tela grande |
| 1080p | 1080 | Tela grande de alta definição |

### Fps (quadros por segundo) {#fps-frames-per-second}

Nos Estados Unidos e no Japão, a maioria dos vídeos é fotografados a 29,97 quadros por segundo (fps); na Europa, a maioria dos vídeos são gravados a 25 qps. O filme é filmado a 24 fps.

Escolha uma predefinição de codificação de vídeo que corresponda à taxa fps do arquivo de vídeo principal. Por exemplo, se o vídeo principal for 25 fps, escolha uma predefinição de codificação com 25 fps. Por padrão, toda codificação personalizada usa o fps do arquivo de vídeo principal. Por isso, não é necessário especificar explicitamente a configuração fps ao criar uma predefinição de codificação de vídeo.

### Dimensões de codificação de vídeo {#video-encoding-dimensions}

Para obter resultados ideais, selecione dimensões de codificação de modo que o vídeo de origem seja um múltiplo completo de todos os vídeos codificados.

Para calcular essa proporção, divida a largura de origem por largura codificada para obter a proporção de largura. Em seguida, divida a altura de origem por altura codificada para obter a proporção de altura.

Se a proporção resultante for um inteiro inteiro, isso significa que o vídeo é dimensionado de forma ideal. Se a proporção resultante não for um inteiro, isso afeta a qualidade do vídeo, deixando artefatos de pixel restantes na tela. Esse efeito é mais visível quando o vídeo tem texto.

Por exemplo, suponha que o vídeo de origem seja 1920 x 1080. Na tabela a seguir, os três vídeos codificados fornecem as configurações de codificação ideais a serem usadas.

| Tipo de vídeo | Largura x altura | Proporção de largura | Taxa de altura |
|--- |--- |--- |--- |
| Fonte | 1920 x 1080 | 1 | 1 |
| Codificado | 960 x 540 | 2 | 2 |
| Codificado | 640 x 360 | 3 | 1 |
| Codificado | 480 x 270 | 4 | 4 |

### Formato de arquivo de vídeo codificado {#encoded-video-file-format}

O Adobe Dynamic Media Classic recomenda o uso de predefinições de codificação de vídeo MP4 H.264. Como os arquivos MP4 usam o codec de vídeo H.264, ele fornece vídeo de alta qualidade, mas em um tamanho de arquivo compactado.

## Trabalhar com predefinições de codificação de vídeo {#working-with-video-encoding-presets}

Arquivos de vídeo principais criados com equipamento de produção de vídeo e software de edição de vídeo são muitas vezes muito grandes e não estão no formato adequado para delivery para destinos online. Para converter vídeo digital no formato e especificações adequados para reprodução em telas diferentes, você pode *transcodificar* arquivos de vídeo (um processo também conhecido como *encoding*). Durante o processo de codificação, o vídeo é compactado em um tamanho de arquivo menor e eficiente para um delivery ideal da Web e para dispositivos móveis.

Consulte [Carregar e codificar vídeos](uploading-encoding-videos.md#uploading-and-encoding-videos).

O Dynamic Media Classic oferece uma biblioteca de predefinições de codificação de vídeo predefinidas que refletem as configurações de codificação mais comuns usadas atualmente. Essas predefinições de codificação são otimizadas para reprodução em telas de público alvo. Além disso, os administradores podem criar suas próprias predefinições de codificação de vídeo para personalizar o tamanho e a qualidade de reprodução dos vídeos para os usuários finais. Todas as predefinições de codificação de vídeo, sejam prontas para uso no Dynamic Media Classic ou personalizadas, exibem o vídeo no formato de arquivo MP4.

Na tela Predefinições de vídeo, os administradores podem configurar e gerenciar a codificação de vídeo. Eles podem fazer o seguinte:

* Ative e desative as predefinições de codificação de vídeo.
* Crie uma predefinição de codificação de vídeo.
* Edite predefinições de codificação de vídeo.
* Exclua predefinições de vídeo.

Qualquer vídeo que você carregar no Dynamic Media Classic ou que você codificar no Dynamic Media Classic será tratado como &quot;vídeo&quot;. Em outras palavras, essa classificação de ativo significa que você pode fornecer o vídeo para reprodução em desktops, dispositivos móveis ou ambos. Por exemplo, você pode pré-visualização esses tipos de vídeos no Dynamic Media Classic. Você também pode gerar URLs (usando o recurso Copiar URL) e código que podem ser incorporados (usando o recurso Incorporar código) para uso com players de vídeo, sites e assim por diante.

Consulte [Visualizar vídeos em um visualizador de vídeo](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Consulte [Vincular um URL de vídeo a um site móvel ou a um site](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Consulte [Incorporar o visualizador de vídeo em uma página da Web](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Para ativos de vídeo que você carrega e codifica no Dynamic Media Classic, o vídeo é entregue no seguinte formato de arquivo:

**MP4 H.264** Use arquivos MP4 para o seguinte:

* HTTP Dynamic Streaming em desktops.
* HLS (HTTP Live Streaming, protocolo de streaming da Apple).
* Delivery de vídeo progressivo para dispositivos móveis Android, Blackberry e Windows.

Qualquer outro formato de vídeo e codec é tratado como um &quot;Vídeo Principal&quot;. Essa classificação de ativo significa que o vídeo é um arquivo de vídeo de origem e não pode ser usado para reprodução de delivery em desktops ou dispositivos móveis. Por exemplo, você não pode pré-visualização esses tipos de vídeos no Dynamic Media Classic. Você também não pode gerar Copiar URLs ou Incorporar código para usar em players de vídeo, sites e assim por diante.

### Filtrar a lista das predefinições de codificação de vídeo {#filtering-the-list-of-video-encoding-presets}

As páginas Predefinições de vídeo e Predefinições de vídeo adaptáveis consistem em uma tabela que lista o status ativo, o nome predefinido, o dispositivo de reprodução pretendido, a dimensão de vídeo e a taxa de dados do público alvo de cada predefinição de vídeo.

Você pode refinar a lista escolhendo filtrar em Ambos, Ativo ou Inativo, para ver todas as predefinições de vídeo ou restringir a lista a predefinições que estejam ativas ou inativas.

Você também pode filtrar com base na opção de um dispositivo de reprodução para restringir a lista às predefinições de vídeo projetadas para reprodução de vídeos em todos os dispositivos, desktop, dispositivos móveis ou tablets.

**Para filtrar a lista das predefinições de codificação de vídeo**

1. No Dynamic Media Classic, clique em **Configuração** > **Configuração de Aplicativo** > **Predefinições de Vídeo** > **Predefinições de Vídeo Adaptive** ou **Predefinições de Codificação Únicas**.

   As páginas para Predefinições de vídeo adaptáveis e Predefinições de codificação única incluem uma tabela que lista o status ativo, o nome da predefinição, o dispositivo de reprodução pretendido, as dimensões de vídeo e a taxa de dados do Público alvo de cada predefinição de vídeo.

1. Na página Predefinições de codificação única chamada Predefinições de vídeo, na barra de ferramentas Predefinições de vídeo, use as duas listas suspensas para refinar a lista das predefinições na tabela com base no status Ativo e no dispositivo de reprodução.

   * Na primeira lista suspensa mais estreita, escolha **Ambos** para ver todas as predefinições de vídeo, ou escolha **Ativo** ou **Inativo** ou restrinja a lista a predefinições que estejam ativas ou inativas.
   * Na segunda lista suspensa mais ampla, escolha uma opção de dispositivo de reprodução para restringir a lista às Predefinições de vídeo projetadas para reprodução de vídeos em desktops. ou para reproduzir vídeos em dispositivos móveis ou tablets.

### Ativar ou desativar as predefinições de codificação de vídeo {#activating-or-deactivating-video-encoding-presets}

As predefinições de vídeo ativadas são exibidas na caixa de diálogo Opções de trabalho de upload. Essa é a caixa de diálogo que aparece quando um usuário carrega arquivos de vídeo durante o processo de upload. Eles podem escolher entre uma lista de todas as predefinições de codificação ativadas.

**Para ativar ou desativar predefinições de codificação de vídeo**

1. No Dynamic Media Classic, clique em **Configuração** > **Configuração de Aplicativo** > **Predefinições de Vídeo**.
1. Execute um dos procedimentos a seguir:

   * Clique em **Predefinições de vídeo adaptáveis**.
   * Clique em **Predefinições de codificação única**.

1. Execute um dos procedimentos a seguir:

   * Para ativar uma predefinição de vídeo, na página de predefinições, na coluna Ativo, selecione a caixa ao lado de um nome predefinido.
   * Para desativar uma predefinição de vídeo, desmarque a caixa ao lado das predefinições de vídeo que você deseja tornar inativas.

      ***nota**: As predefinições de vídeo inativas não aparecem na caixa de diálogo Opções de trabalho de upload. *

1. No canto inferior direito da página, clique em **Fechar**.

### Adicionar ou editar uma predefinição de codificação de vídeo {#adding-or-editing-a-video-encoding-preset}

Você pode criar suas próprias predefinições de vídeo personalizadas de codificação única e adicioná-las à tabela Predefinições de vídeo. Você também pode fazer alterações em qualquer predefinição de codificação única pré-definida de vídeo que acompanha o Dynamic Media Classic, desde que salve a predefinição editada com um novo nome.

O Dynamic Media Classic definiu limites máximos para a taxa de dados do público alvo, a altura da resolução e a largura da resolução para garantir uma experiência de reprodução adequada. As mensagens de aviso serão exibidas se você exceder esses limites, que são os seguintes:

* Para a reprodução do computador, os limites são: (Largura/16) * (Altura/16) &lt; 8192.
* Para reprodução móvel, os limites são: (Largura/16) * (Altura/16) &lt; 660; Taxa de dados do público alvo &lt; 4000.
* Para reprodução em tablet, os limites são: (Largura/16) * (Altura/16) &lt; 3600.

**Para adicionar ou editar uma predefinição de codificação de vídeo**

1. No Dynamic Media Classic, clique em **Configuração** > **Configuração de Aplicativo** > **Predefinições de Vídeo**.
1. Clique em **Predefinições de codificação única** para abrir a página Predefinições de vídeo.
1. Na página Predefinições de vídeo, execute um dos procedimentos a seguir:

   * Na barra de ferramentas Predefinições de vídeo, clique em **Adicionar** para adicionar uma nova Predefinição de vídeo.
   * Selecione uma predefinição de vídeo. Na barra de ferramentas, clique em **Editar**.

      Não é possível editar predefinições predefinidas do Dynamic Media Classic; você só pode criar uma predefinição a partir de uma existente escolhendo **Salvar como**.

1. Na página Adicionar predefinição de vídeo ou Editar predefinição de vídeo, defina as opções de Predefinição de vídeo desejadas.

   Consulte [Práticas recomendadas para codificação de vídeo](uploading-encoding-videos.md#best-practices-for-video-encoding) para obter as configurações recomendadas.

   | Opção Predefinição de vídeo | Descrição |
   |--- |--- |
   | Nome da predefinição | Digite um nome descritivo para a predefinição de vídeo. O nome digitado é exibido na caixa de diálogo Carregar opções de trabalho, na qual os usuários escolhem opções de transcodificação. |
   | Descrição | Descreva a predefinição de vídeo. O que você inserir aparecerá como uma dica de ferramenta quando você mover o ponteiro sobre o nome da predefinição na caixa de diálogo Carregar opções de trabalho, na qual os usuários escolhem opções de transcodificação. |
   | Dispositivo de reprodução | Escolha o dispositivo no qual o vídeo deve ser reproduzido. As opções são Computador (desktops), Móvel (iPhone, iPad, Android); ou Tablet (apenas para iPad). Essa configuração determina automaticamente o codec de áudio e vídeo apropriado usado durante a codificação. |
   | Taxa de dados do público alvo | Digite a velocidade média de conexão com a Internet (em quilobits por segundo) do usuário final do público alvo. Você pode inserir a taxa ou arrastar o controle deslizante para inseri-la. O espectro de velocidade de conexão do usuário lista velocidades típicas para conexões de banda larga, DSL, móveis e dial-up. Essa configuração determina automaticamente a taxa de dados de áudio e vídeo combinados. Em outras palavras, a quantidade de dados que é codificada para formar um único segundo de reprodução de vídeo. Quanto maior a taxa de dados, melhor será a qualidade do vídeo resultante. No entanto, as taxas de dados muito altas resultam em arquivos de tamanho grande que criam experiências de visualização de subpares para usuários com largura de banda baixa. Como prática recomendada, encontre um equilíbrio entre taxas de dados altas e baixas. Pretende criar uma experiência de reprodução de qualidade adequada sem afastar os usuários que têm larguras de banda estreitas. |
   | Proporção | Proporção é a proporção entre a largura e a altura do vídeo. As duas primeiras proporções listadas abaixo são comumente usadas para exibir o vídeo horizontalmente:<ul><li> 4:3 - Usado para quase todo o conteúdo de transmissão de TV de definição padrão.</li><li>16:9 - Usado para quase todos os filmes e conteúdo de TV de alta definição (HDTV) de tela larga.</li><li>Escala automática - (Padrão) uma única predefinição de codificação que funciona com qualquer proporção para criar vídeos para delivery para móvel, tablet e desktop. Os vídeos de origem carregados que são codificados com essa predefinição são definidos com uma altura fixa. Entretanto, a largura é dimensionada automaticamente para preservar a proporção do vídeo (proporção largura/altura).</li><li>Personalizado - usado quando você deseja definir um tamanho de vídeo não padrão.</li><li>A proporção escolhida determina as configurações de largura e altura para o Tamanho da resolução; o valor de largura e altura é automaticamente dimensionado para a proporção correta.</li></ul> |
   | Tamanho da resolução | O tamanho da resolução, expresso pelo número de pixels de largura pelo número de pixels de altura, determina a dimensão. Insira um valor de largura e altura em pixels ou arraste o controle deslizante para inserir esses valores. O espectro de resolução lista tamanhos de resolução típicos. Os valores de largura e altura seguem automaticamente a proporção selecionada. Por exemplo, se você selecionar 4:3 como proporção e digitar 400 como largura, 300 será inserido automaticamente como altura.Se você selecionou Escala automática para a configuração Proporção, o valor Largura para o Tamanho da resolução será automaticamente definido como Pré-visualização de Auto.Clique em  para abrir uma janela do navegador e ver suas opções de resolução lá. |
   | Codificar sufixo de arquivo | Insira um sufixo. Esse sufixo é anexado ao arquivo de vídeo codificado resultante. É possível inserir um hífen e um sublinhado no nome; espaços em branco e caracteres especiais não são permitidos. |
   | Outras configurações | O Dynamic Media Classic determina todas as outras configurações de codificação automaticamente de acordo com as diretrizes de codificação de práticas recomendadas. |

1. Execute um dos procedimentos a seguir:

   * Clique em **Salvar** se tiver adicionado ou editado uma predefinição de vídeo.
   * Clique em **Salvar como** se tiver adicionado uma predefinição de vídeo iniciando a partir de uma predefinição existente.

### Excluindo uma predefinição de codificação de vídeo {#deleting-a-video-encoding-preset}

Os administradores podem excluir predefinições de vídeo personalizadas. As predefinições de vídeo que vêm com o Dynamic Media Classic não podem ser excluídas.

**Para excluir uma predefinição de codificação de vídeo**

1. No Dynamic Media Classic, clique em **Configuração** > **Configuração de Aplicativo** > **Predefinições de Vídeo**.
1. Clique em **Predefinições de codificação única** para abrir a página Predefinições de vídeo.
1. Na página Predefinições de vídeo, selecione uma Predefinição de vídeo na tabela que não deseja mais ou não precisa.
1. Na barra de ferramentas Predefinições de vídeo, clique em **Excluir**.
1. Na caixa de diálogo Excluir predefinição, clique em **Excluir**.

>[!MORELIKETHIS]
>
>* [Start rápido: Vídeo](quick-start-video.md#quick-start-video)
>* [Carregamento e codificação de vídeos](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Trabalhar com predefinições do visualizador de vídeo](previewing-videos-video-viewer.md#working-with-video-viewer-presets)

