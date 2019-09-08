---
title: Upload e codificação de vídeos
seo-title: Upload e codificação de vídeos
description: Saiba como carregar e codificar vídeos.
seo-description: Saiba como carregar e codificar vídeos.
uuid: 9 a 7 d 6513-b 10 c -40 b 0-aebb -18 a 795 c 2 b 8 d 1
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: a 0941823-850 c -4373-9 e 37-f 32032 de 3805
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Upload e codificação de vídeos{#uploading-and-encoding-videos}

Para criar conjuntos de vídeos exclusivos ou de vídeo adaptáveis para distribuição na Web ou dispositivos móveis, carregue primeiro os arquivos de vídeo mestre no Sistema de publicação Scene 7. O Dynamic Media Classic codifica vídeos em formato MP 4 e publica vídeos nos seguintes formatos de arquivo:

**MP 4** Dynamic Media Classic recomenda MP 4 como o formato de arquivo de vídeo preferencial. Use arquivos MP 4 para o seguinte:

* HTTP Dynamic Streaming em desktops.
* HTTP Live Streaming (protocolo de transmissão de streaming da Apple).
* Fornecimento progressivo de vídeo para dispositivos móveis Android, Blackberry e Windows

O Dynamic Media Classic oferece dois fluxos de trabalho para fazer upload de arquivos de vídeo:

**Vídeos pré-codificados** Carrega arquivos MP 4 diretamente no Dynamic Media Classic. Com esse fluxo de trabalho, os arquivos não são codificados no momento em que você os carrega. Os arquivos são pré-codificados em preparação para distribuição na área de trabalho e para dispositivos móveis.

**Vídeos de origem principal** Carregue os arquivos de vídeo de origem principal e, no upload, codificue esses arquivos para arquivos MP 4. Os vídeos codificados são rotulados como "Vídeo" no painel Procurar. O Dynamic Media Classic oferece suporte à codificação de arquivos de vídeo em diversos formatos.

* Verifique se os arquivos de vídeo de origem principal que deseja codificar são suportados.

   Consulte [Tipos de arquivo de vídeo suportados para codificação](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

* Escolha uma predefinição de codificação de vídeo.

   Consulte [Predefinições de vídeo para codificação de arquivos de vídeo](application-setup.md#video-presets-for-encoding-video-files).

   Consulte [Práticas recomendadas para codificação de vídeos](uploading-encoding-videos.md#best-practices-for-video-encoding).

O Dynamic Media Classic também gera miniaturas de vídeo. Você pode saber mais sobre miniaturas de vídeo, como obter seus urls e modificar quadros de pôster.

Consulte [Trabalhar com miniaturas de vídeo](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**Para carregar e codificar vídeos**

Execute um dos procedimentos a seguir:

*Se os vídeos já estiverem codificados*

1. Na barra de Navegação global, clique **em Carregar**.
1. Na tela Upload, clique na guia **da área de trabalho** .
1. Na página Upload, no painel Selecionar arquivos para upload, clique **em Procurar**, navegue até um arquivo de vídeo MP 4 e clique **em Abrir**.
1. No painel Escolher destino da pasta, selecione uma pasta para o arquivo carregado.
1. Na página Upload, certifique-se de **que Publicar depois de fazer upload** esteja marcado.
1. Clique **em Enviar upload**.

*Se você quiser codificar seus vídeos usando o Scene 7 Publishing System*

1. Na barra de Navegação global, clique **em Carregar**.
1. Na tela Upload, clique na guia **da área de trabalho** .
1. No painel Selecionar arquivos para upload, clique **em Procurar**, navegue até um arquivo de vídeo de origem principal e clique **em Abrir**.
1. No painel Escolher destino da pasta, selecione uma pasta para o arquivo carregado.
1. No canto inferior direito da página, clique em Opções **de trabalho**,
1. Na caixa de diálogo Carregar opções de trabalho, expanda as Opções de evideo.
   * Execute um dos procedimentos a seguir:
      * A prática recomendada é usar o método a seguir.
Selecione **Codificação de vídeo adaptável**.
Consulte [Vídeo adaptativo (padrão)](application-setup.md#adaptive-video-default).
   * Opcional, se desejar usar configurações de codificação individuais, faça o seguinte.
Expanda **as Predefinições de codificação única**e selecione as opções de codificação desejadas para Desktop, Dispositivos móveis e Tablet.
Consulte [Predefinições de codificação de vídeo para desktop](application-setup.md#desktop-video-encoding-presets), [predefinições de codificação de vídeo móvel](application-setup.md#mobile-video-encoding-presets), [predefinições de codificação de vídeos em tablet](application-setup.md#tablet-video-encoding-presets).
1. Na caixa de diálogo Carregar opções de trabalho, clique **em Salvar**.
1. Na página Upload, certifique-se de **que Publicar depois de fazer upload** esteja marcado.
1. Na página Upload, no canto inferior direito, clique **em Enviar upload**.

Se você quiser codificar novamente um arquivo de vídeo carregado anteriormente

1. No Dynamic Media Classic, no painel Procurar, navegue até o vídeo e selecione-o.
1. Clique **em Arquivo** &gt; **Reprocessar**.
1. Na caixa de diálogo Reprocessar ativos, expanda as Opções de evideo.
1. Execute um dos procedimentos a seguir:
   * A prática recomendada é usar o método a seguir.
Selecione **Vídeo adaptativo**.
Consulte [Vídeo adaptativo (padrão)](application-setup.md#adaptive-video-default).
   * Opcional, se desejar usar configurações de codificação individuais, faça o seguinte.
Expanda **as Predefinições de codificação única**e selecione as opções de codificação desejadas para Desktop, Dispositivos móveis e Tablet.
Consulte [Predefinições de codificação de vídeo para desktop](application-setup.md#desktop-video-encoding-presets), [predefinições de codificação de vídeo móvel](application-setup.md#mobile-video-encoding-presets), [predefinições de codificação de vídeos em tablet](application-setup.md#tablet-video-encoding-presets).
1. Na caixa de diálogo Reprocessar ativos, clique **em Enviar**.

Quando você usa predefinição de codificação de Vídeo adaptável ou usa várias predefinições de codificação única, o resultado é um Conjunto de vídeos adaptativo criado automaticamente com várias codificações de vídeo. Você também pode criar manualmente um Conjunto de vídeos adaptativos selecionando vídeos individuais.

Apenas tipos de arquivo MP 4 e M 4 V são criados quando você gera um Conjunto de vídeos adaptativo de forma automática ou manual.

## Tipos de arquivo de vídeo suportados para codificação {#supported-video-file-types-for-encoding}

A tabela a seguir lista os tipos de arquivo de vídeo (com codecs de vídeo permitidos) que podem ser codificados para o formato MP 4 ou OGV quando você carrega arquivos. A tabela lista os formatos de arquivo e os codecs:

**Formatos de arquivo de vídeo** semelhantes a um arquivo ZIP, um formato de arquivo de vídeo determina como os arquivos estão contidos no arquivo de vídeo. Um arquivo de vídeo geralmente contém várias faixas— uma faixa de vídeo (sem áudio) e uma ou mais faixas de áudio (sem vídeo)— que são interrelacionados e sincronizadas. O formato de arquivo de vídeo determina como esses dados e metadados diferentes são organizados.

**Codecs de vídeo** Um codec de vídeo descreve o algoritmo pelo qual um vídeo é codificado. Um player de vídeo decodifica o vídeo de acordo com seu codec e exibe uma série de imagens, ou quadros, na tela. Os codecs reduzem a quantidade de informações que os arquivos de vídeo precisam armazenar para reproduzir vídeo. Em vez de informações sobre cada quadro individual, apenas informações sobre as diferenças entre um quadro e o próximo são armazenadas. Como a maioria dos vídeos muda pouco de um quadro para o seguinte, os codecs permitem altas taxas de compressão, o que resulta em tamanhos de arquivo menores.

| Formato de arquivo de vídeo | Codecs de vídeo |
|:--- |:--- |
| 3GP | H .263, H .264 |
| AVI | Divx, DV |
| M2P | MPEG -2 PS |
| M2T | MPEG -2 TS |
| M2TS | MPEG -2 TS |
| M2V | MPEG -2 ES |
| M4V | H .264 |
| MOV | DV, dvcpro 50, H .261, H .263, H .264, Sorenson Video 1 |
| MP4 | H .264/MPEG -4 AVC |
| MPEG | MPEG -2 SS |
| MPG | MPEG -2 SS |
| MTS | MPEG -2 |
| Prores | APCN, APCS, APCO, APCH, AP 4 H |
| TS | Dvcpro 50 |
| VOB | MPEG -2 |
| WMV/ASF | VC -1, Windows Media Video 7, Windows Media Video 8 |

>[!NOTE]
>
>A tela de Tarefas alerta se você carrega e tenta codificar um arquivo de vídeo, mas o arquivo é rejeitado porque ele contém um codec ou contêiner de arquivo incompatível. Para obter mais informações, consulte [Verificação de arquivos de trabalho](checking-job-files.md).

## Práticas recomendadas para codificação de vídeos {#best-practices-for-video-encoding}

Veja a seguir dicas de práticas recomendadas para codificação de arquivos de vídeo de origem no Sistema de publicação Scene 7.

Para obter conselhos sobre codificação de vídeo, consulte o seguinte:

* Artigo: * Streaming 101: Noções básicas— Codecs, largura de banda, taxa de dados e resolução: * [www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en).
* Vídeo: * Noções básicas sobre codificação de vídeo: * [www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en).

### Arquivos de vídeo de origem {#source-video-files}

Ao codificar um arquivo de vídeo, use um arquivo de vídeo de origem com a maior qualidade possível. Evite usar arquivos de vídeo codificados anteriormente porque esses arquivos já estão compactados, e a codificação adicional cria um vídeo de qualidade de subpar.

A tabela a seguir descreve o tamanho, a proporção e a taxa de bits recomendados que os arquivos de vídeo de origem devem ter ao codificá-los:

| Tamanho | Proporção de aspecto | Taxa mínima de bits |
|--- |--- |--- |
| 1024 X 768 | 4:3 | 4500 kbps para a maioria dos vídeos. |
| 1280 X 720 | 16:9 | 3000 - 6000 kbps, dependendo da quantidade de movimento no vídeo. |
| 1920 X 1080 | 16:9 | 6000 - 8000 kbps, dependendo da quantidade de movimento no vídeo. |

### Obtenção de metadados de um arquivo {#obtaining-a-file-s-metadata}

Você pode obter os metadados de um arquivo exibindo seus metadados no Dynamic Media Classic, usando uma ferramenta de edição de vídeo ou usando um aplicativo projetado para obter metadados. Veja a seguir instruções para usar o mediainfo, um aplicativo de terceiros, para obter os metadados do arquivo de vídeo:

1. Ir para esta página da Web: [https://mediainfo.sourceforge.net/en/Download](https://mediainfo.sourceforge.net/en/Download).
1. Selecione e baixe o instalador da versão GUI e siga as instruções de instalação.
1. Após a instalação, clique com o botão direito do mouse no arquivo de vídeo (somente Windows), selecione mediainfo ou abra o mediainfo e arraste o arquivo de vídeo para o aplicativo. Você verá todos os metadados associados ao seu arquivo de vídeo, incluindo sua largura, altura e fps.

### Proporção de aspecto {#aspect-ratio}

Ao escolher ou criar uma predefinição de codificação de vídeo para o arquivo de vídeo mestre, certifique-se de que a predefinição tenha a mesma proporção que o arquivo mestre de vídeo. A proporção ** é a proporção da largura do vídeo.

Para determinar a proporção de um arquivo de vídeo, obtenha os metadados do arquivo e observe a largura e altura do arquivo (consulte [Obter metadados de um arquivo](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Em seguida, use essa fórmula para determinar a proporção:

largura/altura = proporção

A tabela a seguir descreve como os resultados da fórmula são traduzidos para escolhas comuns de proporção:

| Resultado da fórmula | Proporção de aspecto |
|--- |--- |
| 1.33 | 4:3 |
| 0.75 | 3:4 |
| 1.78 | 16:9 |
| 0.56 | 9:16 |

Por exemplo, um vídeo com width 440 largura x 1080 altura tem uma proporção de aspect 440/1080 ou 1.33. Nesse caso, escolha uma predefinição de codificação de vídeo com uma proporção de 4:3 para codificar o arquivo de vídeo.

### Taxa de dados {#data-rate}

A taxa *de dados* (também chamada de * taxa de bits *) é a quantidade de dados codificada para formar um único segundo da reprodução do vídeo. A taxa de dados é medida em quilobits por segundo (Kbps).

>[!NOTE]
>
>Como todos os codecs usam a compactação com perdas, a taxa de dados é o fator mais importante na qualidade do vídeo. Com a compactação com perdas, quanto mais compactar um arquivo de vídeo, mais a qualidade é degradada. Por isso, todas as outras características são iguais (a resolução, a taxa de quadros e o codec), quanto menor a taxa de dados, menor será a qualidade do arquivo compactado.

Ao escolher uma predefinição de codificação de vídeo, considere a velocidade de conexão de destino do usuário final. Escolha uma predefinição com uma taxa de dados que é 80 % dessa velocidade. Por exemplo, se a velocidade de conexão do usuário final de destino for de 1000 Kbps, a melhor predefinição será uma com uma taxa de dados de vídeo de 800 Kbps.

Esta tabela descreve a taxa de dados das velocidades comuns de conexão.

| Velocidade (Kbps) | Tipo de conexão |
|--- |--- |
| 256 | Conexão discada. |
| 800 | Conexão móvel típica. Para essa conexão, direcione uma taxa de dados no intervalo de 400 a um máximo de 800 para experiências 3 G. |
| 2000 | Conexão típica de desktop de banda larga. Para essa conexão, defina uma taxa de dados no intervalo de K00-2000 Kbps, com a maior parte dos destinos a média de 1200-1500 Kbps. |
| 5000 | Conexão típica de alta banda. A codificação neste intervalo superior não é recomendada porque a entrega de vídeo com esta velocidade não está disponível para a maioria dos consumidores. |

### Resolução {#resolution}

*A resolução* descreve a altura e largura de um arquivo de vídeo em pixels. A maioria dos vídeos de origem é armazenada em uma resolução alta (por exemplo, 1920 x 1080). Para fins de streaming, o vídeo de origem é compactado para uma resolução menor (640 x 480 ou menor).

A resolução e a taxa de dados são dois fatores vinculados verticalmente que determinam a qualidade do vídeo. Para manter a mesma qualidade de vídeo, quanto maior for o número de pixels em um arquivo de vídeo (quanto mais alta a resolução), maior será a taxa de dados. Por exemplo, considere o número de pixels por quadro em uma resolução de 320 x 240 e um arquivo de vídeo de resolução de 640 x 480:

| Resolução | Pixels por quadro |
|--- |--- |
| 320 x 240 | 76,800 |
| 640 x 480 | 307,200 |

O arquivo 640 x 480 tem quatro vezes mais pixels por quadro. Para obter a mesma taxa de dados para estas duas resoluções de exemplo, você aplica quatro vezes a compactação ao arquivo de 640 x 480, o que pode reduzir a qualidade do vídeo. Portanto, uma taxa de dados de vídeo de 250 Kbps produz visualização de alta qualidade em uma resolução de 320 x 240, mas não em uma resolução de 640 x 480.

>[!NOTE]
>
>Em geral, quanto mais taxa de dados você usar, melhor será o seu vídeo e quanto maior for a resolução usada, maior será a taxa de dados necessária para manter a qualidade da visualização (comparada com resoluções mais baixas).

Como a resolução e a taxa de dados são vinculadas, há duas opções ao codificar vídeo:

* Escolha uma taxa de dados e codifique na mais alta resolução que tenha boa aparência na taxa de dados escolhida.
* Escolha uma resolução e codifique na taxa de dados necessária para obter vídeo de alta qualidade na resolução escolhida.

Ao escolher (ou criar) uma predefinição de codificação de vídeo para o arquivo de vídeo mestre, use esta tabela para definir a resolução correta:

| Resolução | Altura (pixels) | Tamanho da tela |
|--- |--- |--- |
| 240p | 240 | Tela pequena |
| 300p | 300 | Tela pequena geralmente para dispositivos móveis |
| 360p | 360 | Tela pequena |
| 480p | 480 | Tela média |
| 720p | 720 | Tela grande |
| 1080p | 1080 | Tela grande de alta definição |

### Fps (quadros por segundo) {#fps-frames-per-second}

Nos Estados Unidos e no Japão, a maioria dos vídeos é capturada a 29.97 quadros por segundo (fps); na Europa, a maioria do vídeo é capturada em 25 fps. Filme é capturado em 24 fps.

Escolha uma predefinição de codificação de vídeo que corresponda à taxa de fps do arquivo de vídeo mestre. Por exemplo, se o vídeo mestre for 25 fps, escolha uma predefinição de codificação com 25 fps. Por padrão, toda a codificação personalizada usa os fps do arquivo de vídeo mestre. Por isso, você não precisa especificar explicitamente a configuração de fps quando criar uma predefinição de codificação de vídeo.

### Dimensões de codificação de vídeo {#video-encoding-dimensions}

Para obter melhores resultados, selecione a codificação de dimensões de forma que o vídeo de origem seja vários de todos os vídeos codificados.

Para calcular essa proporção, você divide a largura da fonte por largura codificada para obter a proporção de largura. Em seguida, você divide a altura da fonte por altura codificada para obter a proporção de altura.

Se a proporção resultante for inteiro, significa que o vídeo é dimensionado de forma otimizada. Se a proporção resultante não for inteiro, ela afeta a qualidade do vídeo deixando os artefatos de pixel vazios na exibição. Esse efeito é mais visível quando o vídeo tem texto.

Por exemplo, suponha que o vídeo de origem seja 1920 x 1080. Na tabela a seguir, os três vídeos codificados fornecem as configurações de codificação ideais a serem usadas.

| Tipo de vídeo | Largura x altura | Proporção de largura | Proporção de altura |
|--- |--- |--- |--- |
| Fonte | 1920 x 1080 | 1 | 1 |
| Codificado | 960 x 540 | 2 | 2 |
| Codificado | 640 x 360 | 3 | 3 |
| Codificado | 480 x 270 | 4 | 4 |

### Formato de arquivo de vídeo codificado {#encoded-video-file-format}

O Adobe Dynamic Media Classic recomenda usar predefinições de codificação de vídeo MP 4 H .264. Como os arquivos MP 4 usam o codec de vídeo H .264, ele fornece vídeo de alta qualidade, mas em um tamanho de arquivo compactado.

## Trabalho com predefinições de codificação de vídeo {#working-with-video-encoding-presets}

Os arquivos de vídeo mestre criados com equipamento de produção de vídeo e software de edição de vídeo geralmente são muito grandes e não estão no formato apropriado para a entrega em destinos online. Para converter vídeos digitais em formato e especificações apropriadas para reprodução em telas diferentes, é possível *transcodificar arquivos* de vídeo (um processo também conhecido como *codificação*). Durante o processo de codificação, o vídeo é compactado para um tamanho de arquivo menor e eficiente para uma melhor entrega na Web e para dispositivos móveis.

Consulte [Upload e codificação de vídeos](uploading-encoding-videos.md#uploading-and-encoding-videos).

O Dynamic Media Classic fornece uma biblioteca de predefinições de codificação de vídeo predefinidas que refletem as configurações de codificação mais comuns usadas hoje. Essas predefinições de codificação são otimizadas para reprodução nas telas de destino. Além disso, os administradores podem criar suas próprias predefinições de codificação de vídeo para personalizar o tamanho e a qualidade da reprodução dos vídeos para os usuários finais. Todas as predefinições de codificação de vídeo, independentemente da caixa de entrada clássica clássica ou personalizada, de saída no formato de arquivo MP 4.

Na tela Predefinições de vídeo, os administradores podem configurar e gerenciar a codificação de vídeos. Eles podem fazer o seguinte:

* Ativar e desativar predefinições de codificação de vídeos.
* Crie uma predefinição de codificação de vídeo.
* Editar predefinições de codificação de vídeos.
* Excluir predefinições de vídeo.

Qualquer vídeo carregado no Sistema de publicação Scene 7 ou que você codifica no Scene 7 Publishing System é tratado como «vídeo». Em outras palavras, essa classificação de ativo significa que você pode fornecer o vídeo para reprodução em desktops, dispositivos móveis ou ambos. Por exemplo, você pode visualizar esses tipos de vídeos no Sistema de publicação Scene 7. Você também pode gerar urls (usando o recurso Copiar URL) e o código que pode ser incorporado (usando o recurso Incorporar código) para uso com players de vídeo, nos sites e assim por diante.

Consulte [Visualizar vídeos em um visualizador de vídeo](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Consulte [Vincular um URL de vídeo a um site móvel ou site](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Consulte [Incorporação do visualizador de vídeo em uma página da Web](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Para os ativos de vídeo que você carrega e codifica no Sistema de publicação Scene 7, o vídeo é entregue no seguinte formato de arquivo:

**MP 4 H .264** Use arquivos MP 4 para o seguinte:

* HTTP Dynamic Streaming em desktops.
* HLS (HTTP Live Streaming, protocolo de transmissão de streaming da Apple).
* Distribuição progressiva de vídeo para dispositivos móveis Android, Blackberry e Windows.

Qualquer outro formato de vídeo e codec é tratado como um «Vídeo mestre». Essa classificação de ativo significa que o vídeo é um arquivo de vídeo de origem e não pode ser usado para a reprodução de entrega em desktops ou dispositivos móveis. Por exemplo, você não pode visualizar esses tipos de vídeos no Sistema de publicação Scene 7. Você também não pode gerar urls Copiar urls ou Incorporar código para uso em players de vídeo, sites e assim por diante.

### Filtragem da lista de predefinições de codificação de vídeos {#filtering-the-list-of-video-encoding-presets}

A página Predefinições de vídeo e a página Predefinições de vídeo adaptável consistem em uma tabela que lista o status ativo, o nome predefinido, o dispositivo de reprodução pretendido, a dimensão do vídeo e a taxa de dados de destino de cada predefinição de vídeo.

Você pode refinar a lista escolhendo filtrar tanto no ativo como no Inativo, para ver todas as predefinições de vídeo ou restringir a lista às predefinições ativas ou inativas.

Você também pode filtrar com base em uma opção de dispositivo de reprodução para restringir a lista às Predefinições de vídeo projetadas para reproduzir vídeos em todos os dispositivos, computadores, dispositivos móveis ou tablets.

**Para filtrar a lista de predefinições de codificação de vídeos**

1. No Dynamic Media Classic, clique **em Configuração** &gt; Configuração **do aplicativo** &gt; **Predefinições de vídeo** &gt; **Predefinições de vídeo adaptável** ou **Predefinições de codificação única**.

   As páginas para Predefinições de vídeo adaptativas e Predefinições de codificação única incluem uma tabela que lista o status Ativo, Nome da predefinição, Dispositivo de reprodução pretendido, dimensões do vídeo e Taxa de dados do Target de cada predefinição de vídeo.

1. Na página Predefinições de codificação única chamada Predefinições de vídeo, na barra de ferramentas Predefinições de vídeo, use as duas listas suspensas para refinar a lista de predefinições na tabela com base no status Ativo e no dispositivo de reprodução.

   * Na primeira, lista suspensa mais estreita, escolha **Ambas** para ver todas as predefinições de vídeo ou escolha **Ativa** ou **Inativa** ou limitar a lista às predefinições ativas ou inativas.
   * Na segunda lista suspensa mais ampla, escolha uma opção de dispositivo de reprodução para restringir a lista às Predefinições de vídeo projetadas para reproduzir vídeos em desktops. ou para reproduzir vídeos em dispositivos móveis ou tablets.

### Ativar ou desativar predefinições de codificação de vídeos {#activating-or-deactivating-video-encoding-presets}

As predefinições de vídeo ativadas aparecem na caixa de diálogo Carregar opções de trabalho. Essa é a caixa de diálogo que aparece quando um usuário carrega arquivos de vídeo durante o processo de upload. Eles podem escolher em uma lista de todas as predefinições de codificação ativadas.

**Para ativar ou desativar predefinições de codificação de vídeos**

1. No Dynamic Media Classic, clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Predefinições de vídeo**.
1. Execute um dos procedimentos a seguir:

   * Clique **em Predefinições de vídeo adaptável**.
   * Clique **em Predefinições de codificação única**.

1. Execute um dos procedimentos a seguir:

   * Para ativar uma predefinição de vídeo, na página de predefinições, na coluna Ativa, selecione a caixa ao lado de um nome predefinido.
   * Para desativar uma predefinição de vídeo, desmarque a caixa ao lado das predefinições de vídeo que você deseja tornar inativas.

      ***observação**: As predefinições de vídeo inativas não aparecem na caixa de diálogo Opções de upload de trabalho. *

1. No canto inferior direito da página, clique **em Fechar**.

### Adicionar ou editar uma predefinição de codificação de vídeo {#adding-or-editing-a-video-encoding-preset}

Você pode criar suas próprias predefinições de vídeo personalizadas personalizadas e adicioná-las à tabela Predefinições de vídeo. Também é possível fazer alterações em quaisquer predefinições de vídeo único pré-definidas que tenham vindo com o Dynamic Media Classic, desde que você salve a predefinição editada com um novo nome.

O Dynamic Media Classic definiu limites máximos para a taxa de dados de destino, a altura da resolução e a largura da resolução para garantir uma experiência de reprodução adequada. As mensagens de aviso aparecerão se você exceder os limites que são os seguintes:

* Para a reprodução do computador, os limites são: (Largura/16) * (Altura/16) &lt; 8192.
* Para reprodução móvel, os limites são: (Largura/16) * (Altura/16) &lt; 660; taxa de dados de destino &lt; 4000.
* Para a reprodução do tablet, os limites são: (Largura/16) * (Altura/16) &lt; 3600.

**Para adicionar ou editar uma predefinição de codificação de vídeo**

1. No Dynamic Media Classic, clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Predefinições de vídeo**.
1. Clique **em Predefinições de codificação única** para abrir a página Predefinições de vídeo.
1. Na página Predefinições de vídeo, execute um dos seguintes procedimentos:

   * Na barra de ferramentas Predefinições de vídeo, clique **em Adicionar** para adicionar uma nova predefinição de vídeo.
   * Selecione uma predefinição de vídeo. Na barra de ferramentas, clique **em Editar**.

      Não é possível editar predefinições predefinidas do Media Media Classic; você pode criar apenas uma predefinição de uma existente escolhendo **Salvar como**.

1. Na página Adicionar predefinição de vídeo ou Editar predefinição de vídeo, defina as opções Predefinidas de vídeo desejadas.

   Consulte [Práticas recomendadas para codificação de vídeo](uploading-encoding-videos.md#best-practices-for-video-encoding) para configurações recomendadas.

   | Opção Predefinição de vídeo | Descrição |
   |--- |--- |
   | Nome da predefinição | Insira um nome descritivo para a predefinição de vídeo. O nome inserido aparece na caixa de diálogo Opções de upload de trabalho, no qual os usuários escolhem opções de transcodificação. |
   | Descrição | Descreva a Predefinição de vídeo. O que você insere é uma dica de ferramenta quando você move o ponteiro sobre o nome da predefinição na caixa de diálogo Opções de trabalho de upload, no qual os usuários escolhem opções de transcodificação. |
   | Dispositivo de reprodução | Escolha o dispositivo no qual o vídeo deve ser reproduzido. As opções são Computador (desktops), Mobile (iphone, ipad, Android); ou tablet (somente ipad). Essa configuração determina automaticamente o codec de áudio e vídeo apropriado usado durante a codificação. |
   | Taxa de dados de destino | Insira a velocidade média de conexão da Internet (em quilobits por segundo) do usuário final de destino. Você pode inserir a taxa ou arrastar o controle deslizante para inseri-lo. O espectro Velocidade da conexão do usuário lista velocidades típicas para conexões de banda larga, DSL, móvel e discagem. Essa configuração determina automaticamente a taxa de dados de áudio e vídeo combinada. Em outras palavras, a quantidade de dados codificada para formar um único segundo da reprodução do vídeo. Quanto maior for a taxa de dados, melhor será a qualidade do vídeo resultante. No entanto, as taxas de dados muito altas resultam em grandes tamanhos de arquivo que criam experiências de visualização de subpar para usuários com baixa largura de banda. Como prática recomendada, acesse o equilíbrio entre taxas de dados altas e baixas. Crie uma experiência de reprodução de qualidade adequada sem alienar usuários que têm larguras de banda restritas. |
   | Proporção | A proporção é a proporção da largura da altura do vídeo. As primeiras duas proporções listadas abaixo são usadas frequentemente para exibir vídeo horizontalmente:<ul><li> 4:3 - Usado para quase todo o conteúdo de transmissão de TV de definição padrão.</li><li>16:9 - Usado para quase toda a tela ampla, conteúdo de TV de alta definição (HDTV) e filmes.</li><li>Autoescala - (Padrão) Uma predefinição de codificação única que funciona com qualquer proporção para criar vídeos para distribuição em dispositivos móveis, tablet e desktop. Os vídeos de origem carregados que são codificados com essa predefinição são definidos com uma altura fixa. No entanto, a largura é dimensionada automaticamente para preservar a proporção do vídeo (largura da altura).</li><li>Personalizado - Usado quando você deseja definir um tamanho de vídeo não padrão.</li><li>A proporção de aspecto escolhida determina as configurações de largura e altura para o Tamanho da resolução; o valor de largura e altura automaticamente escala para a proporção adequada.</li></ul> |
   | Tamanho da resolução | O tamanho da resolução, expresso pelo número de pixels de largura pelo número de pixels de altura, determina a dimensão. Insira um valor de largura e altura em pixels ou arraste o controle deslizante para inserir esses valores. O espectro de Resolução lista tamanhos de resolução típicos. Os valores de largura e altura seguem automaticamente a proporção que você selecionou. Por exemplo, se você selecionar 4:3 como proporção de aspecto e digitar 400 para largura, 300 será inserido automaticamente para a altura. Se você selecionou Autoescala para a configuração Taxa de proporção, então o valor Largura para o Tamanho da resolução é automaticamente definido como Automático. Clique em Visualizar para abrir uma janela do navegador e ver as opções de resolução ali. |
   | Codificar sufixo do arquivo | Insira um sufixo. Esse sufixo é anexado ao arquivo de vídeo codificado resultante. É possível inserir um hífen e sublinhado no nome; espaços em branco e caracteres especiais não são permitidos. |
   | Outras configurações | O Dynamic Media Classic determina todas as outras configurações de codificação automaticamente de acordo com as diretrizes de codificação de práticas recomendadas. |

1. Execute um dos procedimentos a seguir:

   * Clique **em Salvar** se tiver adicionado ou editado uma Predefinição de vídeo.
   * Clique **em Salvar como** se você tiver adicionado uma Predefinição de vídeo, começando por uma predefinição existente.

### Exclusão de uma predefinição de codificação de vídeo {#deleting-a-video-encoding-preset}

Os administradores podem excluir predefinições de vídeo personalizadas. As predefinições de vídeo que vêm com o Dynamic Media Classic não podem ser excluídas.

**Exclusão de uma predefinição de codificação de vídeo**

1. No Dynamic Media Classic, clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Predefinições de vídeo**.
1. Clique **em Predefinições de codificação única** para abrir a página Predefinições de vídeo.
1. Na página Predefinições de vídeo, selecione uma Predefinição de vídeo na tabela que não deseja mais ou que precise.
1. Na barra de ferramentas Predefinições de vídeo, clique **em Excluir**.
1. Na caixa de diálogo Excluir predefinição, clique **em Excluir**.

>[!MORELIKETHIS]
>
>* [Início rápido: Vídeo](quick-start-video.md#quick-start-video)
>* [Upload e codificação de vídeos](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Como trabalhar com predefinições do visualizador de vídeo](previewing-videos-video-viewer.md#working-with-video-viewer-presets)

