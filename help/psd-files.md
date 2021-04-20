---
title: 'Trabalhar com arquivos PSD '
description: Saiba como trabalhar com arquivos PSD.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---


# Trabalhar com arquivos PSD {#working-with-psd-files}

Os PSD (arquivos de documento do Photoshop) são usados com mais frequência no Dynamic Media Classic para criar modelos. Ao carregar um arquivo PSD, você pode criar um modelo do Dynamic Media Classic automaticamente a partir do arquivo (selecione a opção Criar modelo na tela Upload ).

O Dynamic Media Classic cria várias imagens de um arquivo PSD com camadas se você usar o arquivo para criar um modelo; ele cria uma imagem para cada camada.

## Opções de upload de PSD {#psd-upload-options}

As opções para carregar arquivos PSD estão localizadas em Opções do Photoshop em Opções de upload de trabalho. Você pode recortar um arquivo, escolher um perfil de cor para ele, usá-lo para criar um modelo e selecionar uma âncora.

Essas opções estão disponíveis ao carregar arquivos PSD:

**Recortar**  (localizado em Opções de recorte.) Escolha Aparar para cortar automaticamente o espaço em branco das bordas de um arquivo PSD; escolha Manual para cortar os lados do arquivo PSD:

**** ApararSelecione o menu Aparar com base em e escolha Cor ou Transparência.

Se você escolher a opção Cor, selecione o menu Canto e escolha o canto do PSD com a cor que melhor representa a cor do espaço em branco que deseja recortar.

Arraste o controle deslizante para especificar uma tolerância de 0 a 1:

Para cortar com base na cor, especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto do PSD. Os números mais próximos de 1 permitem mais diferenças de cor.

Para cortar com base na transparência, especifique 0 para cortar pixels somente se eles forem totalmente transparentes; números mais próximos de 1 permitem mais transparência.

**** ManualInsira o número de pixels para cortar de qualquer lado ou de cada lado da imagem. A quantidade de imagens cortadas depende da configuração ppi (pixels por polegada) no arquivo de imagem. Por exemplo, se a imagem exibir 150 ppi e você digitar 75 nas caixas de texto Superior, Direito, Inferior e Esquerdo, meia polegada será cortada de cada lado da imagem.

**Perfil de cor**  (localizado em Opções de perfil de cor.) Escolha uma opção:

**Converter em sRGB (padrão)** Converte em sRGB (Padrão Vermelho Verde Azul). sRGB é o espaço de cores recomendado para exibir imagens nas páginas da Web.

**Manter** espaço de cores originalMantém o espaço de cores original da imagem.

**Personalizar de >** ParaAbrir menus para poder escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores Photoshop padrão ou um espaço de cores carregado no Dynamic Media Classic. Consulte Perfis ICC.

**Manter** camadasLimpa as camadas na PSD, se houver, em ativos individuais. As camadas de ativo permanecem associadas ao PSD. Você pode visualizá-los abrindo o arquivo PSD na exibição de Detalhes e selecionando o painel de camada. Consulte Exibição e edição de camadas em um arquivo PSD.

**Criar** modeloCria um modelo a partir das camadas no arquivo PSD.

**Extrair** textoExtrai o texto para que os usuários possam pesquisá-lo em um visualizador.

**Estender camadas para** tamanho do plano de fundoEstende o tamanho das camadas de imagem cortadas para o tamanho da camada do plano de fundo.

**Camadas** de nomenclatura da camada no arquivo PSD são carregadas como imagens separadas. Escolha uma opção para nomear essas imagens no Dynamic Media Classic:

**Nome da camada** Nomeie as imagens após seus nomes de camada no arquivo PSD. Por exemplo, uma camada chamada Tag de preço no arquivo PSD original se torna uma imagem chamada Tag de preço. No entanto, se os nomes de camada no arquivo PSD forem nomes de camada padrão do Photoshop (Plano de fundo, Camada 1, Camada 2 e assim por diante), as imagens serão nomeadas após seus números de camada no arquivo PSD, não seus nomes de camada padrão.

**Photoshop e** Número da camadaNomes as imagens após seus números de camada no arquivo PSD, ignorando os nomes originais da camada. As imagens são nomeadas com o nome do arquivo Photoshop e um número de camada anexado. Por exemplo, a segunda camada de um arquivo chamado Spring Ad.psd é chamada Spring Ad_2 , mesmo que tenha um nome não padrão no Photoshop.

**Photoshop e** Nome da camadaNomeie as imagens após o arquivo PSD seguido do nome da camada ou do número da camada. O número da camada é usado se os nomes da camada no arquivo PSD forem nomes padrão da camada do Photoshop. Por exemplo, uma camada chamada Tag de preço em um arquivo PSD chamado SpringAd é chamada Tag Ad_Price Primavera. Uma camada com o nome padrão Camada 2 é chamada de Anúncio de primavera_2.

**** ÂncoraEspecifique como as imagens são ancoradas em modelos que são gerados a partir da composição em camadas produzida a partir do arquivo PSD. Por padrão, a âncora é o centro. Uma âncora central permite que imagens de substituição preencham melhor o mesmo espaço, independentemente da proporção da imagem de substituição. Imagens com um aspecto diferente que substituem essa imagem, ao referenciar o modelo e usar substituição de parâmetro, ocupam efetivamente o mesmo espaço. Altere para uma configuração diferente se o aplicativo exigir as imagens de substituição para preencher o espaço alocado no modelo.

## Exibição e edição de camadas em um arquivo PSD {#viewing-and-editing-layers-in-a-psd-file}

Se você selecionou a opção Manter camadas ao fazer upload do PSD, o Dynamic Media Classic recortou as camadas individuais em ativos. Você pode exibir e editar as camadas de ativo pertencentes a um arquivo PSD abrindo o arquivo no Painel de navegação na exibição de Detalhes.

1. Clique duas vezes no arquivo PSD completo no Painel de navegação para abri-lo na exibição de Detalhes.

   ***observação **: Certifique-se de abrir o ativo completo e não uma das camadas de PSD.*

1. Clique em Camadas para abrir o painel Camadas. Todas as camadas são exibidas como imagens separadas no painel Camadas.
1. Clique duas vezes em uma camada para abri-la e fazer o seguinte:

   * Clique no ícone Mapa de imagem para criar um mapa de imagem na camada. (Consulte [Criação de mapas de imagem](creating-image-maps.md#creating_image_maps).)
   * Clique no ícone Zoom Targets para criar zoom na camada. (Consulte [Criação de destinos de zoom para Zoom Guiado](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Clique no ícone Recortar para recortar a camada. (Consulte [Recortar uma imagem](cropping-image.md#cropping_an_image).)
   * Clique em Nitidez para ajustar a nitidez da camada. (Consulte [Nitidez de uma imagem](sharpening-image.md#sharpening_an_image).)
   * Clique em Ajustar para ajustar a camada. (Consulte [Ajustar uma imagem](adjusting-image.md#adjusting_an_image).)

1. Clique em Salvar ou Salvar como.
1. Para exibir ou editar uma camada diferente, clique em uma seta na parte inferior da visualização da camada.
1. Para sair da exibição Detalhes da camada, clique no ícone Exibição de grade.

