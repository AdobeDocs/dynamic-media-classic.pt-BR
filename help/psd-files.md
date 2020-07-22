---
title: 'Trabalhar com arquivos PSD '
seo-title: 'Trabalhar com arquivos PSD '
description: nulo
seo-description: Saiba como trabalhar com arquivos PSD.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 1%

---


# Trabalhar com arquivos PSD {#working-with-psd-files}

Os arquivos PSD (Documento do Photoshop) são usados com mais frequência no Dynamic Media Classic para criar modelos. Ao carregar um arquivo PSD, você pode criar um modelo do Dynamic Media Classic automaticamente a partir do arquivo (selecione a opção Criar modelo na tela Carregar).

O Dynamic Media Classic cria várias imagens de um arquivo PSD com camadas se você usar o arquivo para criar um modelo; cria uma imagem para cada camada.

## Opções de carregamento de PSD {#psd-upload-options}

As opções para carregar arquivos PSD estão localizadas em Opções do Photoshop em Opções de trabalho de upload. Você pode recortar um arquivo, escolher um perfil colorido para ele, usá-lo para criar um modelo e selecionar uma âncora.

Essas opções estão disponíveis ao carregar arquivos PSD:

**Recortar** (localizado em Opções de corte). Escolha Aparar para cortar automaticamente o espaço em branco das bordas de um arquivo PSD; escolha Manual para cortar os lados do arquivo PSD:

**Aparar** Selecione o menu Aparar para longe com base em e escolha Cor ou Transparência.

Se você escolher a opção Cor, selecione o menu Canto e escolha o canto do PSD com a cor que melhor representa a cor do espaço em branco que deseja cortar.

Arraste o controle deslizante para especificar uma tolerância de 0 a 1:

Para aparar com base na cor, especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto do PSD. Números próximos a 1 permitem mais diferenças de cor.

Para aparar com base na transparência, especifique 0 para cortar pixels somente se eles forem totalmente transparentes. números mais próximos de 1 permitem mais transparência.

**Manual** Digite o número de pixels a serem cortados de qualquer lado ou de cada lado da imagem. A quantidade de imagens cortadas depende da configuração ppi (pixels por polegada) no arquivo de imagem. Por exemplo, se a imagem exibir 150 ppi e você digitar 75 nas caixas de texto Superior, Direita, Inferior e Esquerda, meia polegada será cortada de cada lado da imagem.

**Perfil** colorido (localizado em Opções de Perfil colorido). Escolha uma opção:

**Converter em sRGB (padrão)** Converte em sRGB (Padrão Vermelho Verde Azul). O sRGB é o espaço de cores recomendado para exibir imagens em páginas da Web.

**Manter espaço** de cor original Mantém o espaço de cor original da imagem.

**Os menus Personalizado de > Para** abre para que você possa escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores padrão do Photoshop ou um espaço de cores carregado no Dynamic Media Classic. Consulte perfis ICC.

**Manter camadas** Limpa as camadas no PSD, se houver, em ativos individuais. As camadas de ativo permanecem associadas ao PSD. É possível visualização-los abrindo o arquivo PSD na visualização Detalhe e selecionando o painel de camadas. Consulte Visualização e edição de camadas em um arquivo PSD.

**Criar modelo** Cria um modelo a partir das camadas no arquivo PSD.

**Extrair texto** Extrai o texto para que os usuários possam pesquisar por texto em um visualizador.

**Estender camadas ao tamanho** do plano de fundo Estende o tamanho das camadas de imagem recortadas até o tamanho da camada de plano de fundo.

**Camadas de nomenclatura** de camada no arquivo PSD são carregadas como imagens separadas. Escolha uma opção para nomear essas imagens no Dynamic Media Classic:

**Nome** da camada Nomeia as imagens após seus nomes de camada no arquivo PSD. Por exemplo, uma camada chamada Tag de preço no arquivo PSD original se torna uma imagem chamada Tag de preço. No entanto, se os nomes de camada no arquivo PSD forem nomes de camada padrão do Photoshop (Plano de fundo, Camada 1, Camada 2 e assim por diante), as imagens serão nomeadas após seus números de camada no arquivo PSD, não seus nomes de camada padrão.

**Photoshop e número** de camada Nomeie as imagens após seus números de camada no arquivo PSD, ignorando os nomes de camada originais. As imagens são nomeadas com o nome de arquivo do Photoshop e um número de camada anexado. Por exemplo, a segunda camada de um arquivo chamado Spring Ad.psd é chamada Spring Ad_2 mesmo se ela tiver um nome não padrão no Photoshop.

**Nome** do Photoshop e da camada Nomeie as imagens após o arquivo PSD seguido do nome da camada ou do número da camada. O número da camada será usado se os nomes de camada no arquivo PSD forem nomes de camada padrão do Photoshop. Por exemplo, uma camada chamada Marca de preço em um arquivo PSD chamado SpringAd é chamada Marca Ad_Price Primavera. Uma camada com o nome padrão Camada 2 é chamada Primavera Ad_2.

**Âncora** Especifique como as imagens são ancoradas em modelos que são gerados a partir da composição em camadas produzida a partir do arquivo PSD. Por padrão, a âncora é o centro. Uma âncora central permite que as imagens de substituição preencham melhor o mesmo espaço, independentemente da proporção da imagem de substituição. Imagens com um aspecto diferente que substituem essa imagem, ao referenciar o modelo e usar substituição de parâmetro, ocupam efetivamente o mesmo espaço. Altere para uma configuração diferente se o aplicativo exigir as imagens de substituição para preencher o espaço alocado no modelo.

## Exibição e edição de camadas em um arquivo PSD {#viewing-and-editing-layers-in-a-psd-file}

Se você selecionou a opção Manter camadas ao carregar seu PSD, o Dynamic Media Classic copiou as camadas individuais em ativos. É possível visualização e editar as camadas de ativos pertencentes a um arquivo PSD abrindo o arquivo no Painel de navegação em visualização de detalhes.

1. Clique com o Duplo no arquivo PSD completo no Painel de navegação para abri-lo na visualização Detalhe.

   ***observação **: Certifique-se de abrir o ativo completo e não uma das camadas de PSD.*

1. Clique em Camadas para abrir o painel Camadas. Todas as camadas são exibidas como imagens separadas no painel Camadas.
1. Clique em uma camada com o Duplo para abri-la e execute um dos procedimentos a seguir:

   * Clique no ícone Mapa de imagem para criar um mapa de imagem na camada. (Consulte [Criação de mapas](creating-image-maps.md#creating_image_maps)de imagem.)
   * Clique no ícone Zoom de Públicos alvos para criar públicos alvos de zoom na camada. (Consulte [Criação de públicos alvos de zoom para o zoom](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)guiado.)
   * Clique no ícone Cortar para cortar a camada. (Consulte [Recortar uma imagem](cropping-image.md#cropping_an_image).)
   * Clique em Nitidez para aumentar a nitidez da camada. (Consulte [Como aumentar a nitidez de uma imagem](sharpening-image.md#sharpening_an_image).)
   * Clique em Ajustar para ajustar a camada. (Consulte [Ajustar uma imagem](adjusting-image.md#adjusting_an_image).)

1. Clique em Salvar ou Salvar como.
1. Para visualização ou editar uma camada diferente, clique em uma seta na parte inferior da pré-visualização da camada.
1. Para sair da visualização Detalhes da camada, clique no ícone visualização Grade.

