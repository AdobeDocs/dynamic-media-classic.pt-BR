---
title: Trabalhar com arquivos PSD
seo-title: Trabalhar com arquivos PSD
description: 'null'
seo-description: Saiba como trabalhar com arquivos PSD.
uuid: 5836 b 660-6 bca -46 e 7-ab 39-1 a 31 d 1 e 0 cff 2
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/master_ files
discoiquuid: 4086 e 3 db -5 aca -41 a 0-8 f 15-302 afbf 67 ddb
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Trabalhar com arquivos PSD{#working-with-psd-files}

O PSD (arquivos de documento do Photoshop) é usado com mais frequência no Dynamic Media Classic para criar modelos. Ao carregar um arquivo PSD, você pode criar um modelo de Dynamic Media Classic automaticamente do arquivo (selecione a opção Criar modelo na tela Carregar).

O SPS cria várias imagens de um arquivo PSD com camadas se você usar o arquivo para criar um modelo; cria uma imagem para cada camada.

## Opções de upload de PSD {#psd-upload-options}

As opções para fazer upload de arquivos PSD estão localizadas em Opções do Photoshop nas Opções de trabalho de upload. Você pode recortar um arquivo, escolher um perfil de cor para ele, usá-lo para criar um modelo e selecionar uma âncora.

Essas opções estão disponíveis ao fazer upload de arquivos PSD:

**Cortar** (localizado em Opções de corte.) Escolha Aparar para cortar automaticamente o espaço em branco das bordas de um arquivo PSD; escolha Manual para cortar os lados do arquivo PSD:

**Aparar** Selecione o menu Aparar com base em e escolha Cor ou Transparência.

Se escolher a opção Cor, selecione o menu Canto e escolha o canto do PSD com a cor que representa melhor a cor de espaço em branco que você deseja cortar.

Arraste o controle deslizante para especificar uma tolerância de 0 a 1:

Para aparar com base em cor, especifique 0 para cortar pixels apenas se eles corresponderem exatamente à cor selecionada no canto do PSD. Números mais próximos a 1 permitem mais diferença de cor.

Para aparar com base na transparência, especifique 0 para cortar pixels apenas se eles forem totalmente transparentes; os números mais próximos a 1 permitem mais transparência.

**Manual** Digite o número de pixels para cortar de qualquer lado ou cada lado da imagem. A quantidade de cortes da imagem depende da configuração de ppi (pixels por polegada) no arquivo de imagem. Por exemplo, se a imagem exibir 150 ppi e você inserir 75 nas caixas de texto Superior, Direito, Inferior e Esquerda, uma meia polegada será recortada de cada lado da imagem.

**Perfil de cor** (Localizado em Opções de perfil de cores.) Escolha uma opção:

**Converter em srgb (padrão)** Converte para srgb (Vermelho vermelho vermelho padrão). O srgb é o espaço de cores recomendado para exibir imagens em páginas da Web.

**Manter a cor original** Mantém o espaço de cores original da imagem.

**Personalizado de &gt; Para** abrir menus para que você possa escolher um espaço de cores Converter de e Converter para. É possível escolher um espaço de cor padrão do Photoshop ou um espaço de cores carregado no SPS. Consulte Perfis ICC.

**Manter Camadas** Risa as camadas no PSD, se houver, em ativos individuais. As camadas de ativos permanecem associadas ao PSD. É possível exibi-los abrindo o arquivo PSD na exibição Detalhe e selecionando o painel de camadas. Consulte Visualizar e editar camadas em um arquivo PSD.

**Criar modelo** Cria um modelo das camadas no arquivo PSD.

**Extrair texto** Extrai o texto para que os usuários possam pesquisar por texto em um visualizador.

**Estender camadas para tamanho do plano de fundo** Estende o tamanho das camadas de imagem somadas para o tamanho da camada de plano de fundo.

**As** Camadas de nomenclatura de camada no arquivo PSD são carregadas como imagens separadas. Escolha uma opção para nomear essas imagens no Sistema de publicação Scene 7:

**Nome da camada** Nomes das imagens após os nomes de camada no arquivo PSD. Por exemplo, uma camada chamada de Tag de preço no arquivo PSD original se torna uma imagem chamada Tag Price. No entanto, se os nomes de camada no arquivo PSD forem nomes padrão de camadas do Photoshop (Plano de Fundo, Camada 1, Camada 2 e assim por diante), as imagens serão nomeadas após seus números de camada no arquivo PSD, e não seus nomes de camada padrão.

**Photoshop e Número de camada** As imagens após seus números de camada no arquivo PSD, ignorando os nomes de camada originais. As imagens são nomeadas com o nome de arquivo do Photoshop e um número de camada anexado. Por exemplo, a segunda camada de um arquivo chamado Ad Ad. psd é chamada de Ad Ad_ 2, mesmo se ela possuía um nome não padrão no Photoshop.

**Photoshop e Nome de camada** As imagens após o arquivo PSD, seguido pelo nome da camada ou número da camada. O número da camada será usado se os nomes de camada no arquivo PSD forem nomes padrão de camadas do Photoshop. Por exemplo, uma camada chamada de Price Tag em um arquivo PSD chamado springad chama-se Tag Ad_ Price. Uma camada com o nome padrão Camada 2 é chamada de Ad_ 2.

**Âncora** Especifique como as imagens são ancoradas em modelos gerados a partir da composição em camadas obtida a partir do arquivo PSD. Por padrão, a âncora é o centro. Uma âncora central permite que imagens substitutas preencham melhor o mesmo espaço, independentemente da proporção da imagem de substituição. Imagens com um aspecto diferente que substitui essa imagem, ao referenciar o modelo e utilizar a substituição de parâmetros, ocupam efetivamente o mesmo espaço. Mude para uma configuração diferente se seu aplicativo exigir que as imagens substitutas preencham o espaço alocado no modelo.

## Exibição e edição de camadas em um arquivo PSD {#viewing-and-editing-layers-in-a-psd-file}

Se você tiver selecionado a opção Manter camadas quando fizer upload de seu PSD, o Dynamic Media Classic obterá as camadas individuais em ativos. É possível exibir e editar as camadas de ativos pertencentes a um arquivo PSD abrindo o arquivo no painel Procurar na visualização Detalhe.

1. Clique duas vezes no arquivo PSD completo no Painel Procurar para abri-lo na exibição Detalhe.

   ***observação**: Certifique-se de abrir o ativo completo e não de uma das camadas PSD.*

1. Clique em Camadas para abrir o painel Camadas. Todas as camadas aparecem como imagens separadas no painel Camadas.
1. Clique duas vezes em uma camada para abri-la e execute um dos procedimentos a seguir:

   * Clique no ícone do Mapa de imagem para criar um mapa de imagem na camada. (Consulte [Criar mapas de imagem](creating-image-maps.md#creating_image_maps).)
   * Clique no ícone de Metas de zoom para criar metas de zoom na camada. (Consulte [Criar metas de zoom para Zoom guiado](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Clique no ícone Cortar para recortar a camada. (Consulte [Recortar uma imagem](cropping-image.md#cropping_an_image).)
   * Clique em Nitidez para ajustar a camada. (Consulte [Nitidez de uma imagem](sharpening-image.md#sharpening_an_image).)
   * Clique em Ajustar para ajustar a camada. (Consulte [Ajuste de uma imagem](adjusting-image.md#adjusting_an_image).)

1. Clique em Salvar ou Salvar como.
1. Para exibir ou editar uma camada diferente, clique em uma seta na parte inferior da visualização da camada.
1. Para sair da exibição de Detalhe da camada, clique no ícone de modo de exibição de Grade.

