---
title: 'Trabalhar com arquivos PSD '
description: Saiba como trabalhar com arquivos PSD.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Gerenciamento de ativos
role: Business Practitioner
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '964'
ht-degree: 0%

---

# Trabalhar com arquivos PSD {#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

Os PSD (arquivos de documento do Photoshop) são usados com mais frequência no Dynamic Media Classic para criar modelos. Ao carregar um arquivo PSD, você pode criar um modelo do Dynamic Media Classic automaticamente a partir do arquivo (selecione a opção Criar modelo na tela Upload ).

O Dynamic Media Classic cria várias imagens de um arquivo PSD com camadas se você usar o arquivo para criar um modelo; ele cria uma imagem para cada camada.

## Opções de upload de PSD {#psd-upload-options}

As opções para carregar arquivos PSD estão localizadas em Opções do Photoshop na caixa de diálogo Upload Job Options . Você pode recortar um arquivo, escolher um perfil de cor para ele, usá-lo para criar um modelo e selecionar uma âncora.

Essas opções estão disponíveis ao carregar arquivos PSD:

* **Opções de corte**  - Localizado em  **[!UICONTROL Crop Options]**. Escolha Aparar para cortar automaticamente o espaço em branco das bordas de um arquivo PSD; clique em **[!UICONTROL Manual]** para cortar as laterais do arquivo PSD:

   * **Aparar**  - Selecione o  **[!UICONTROL Trim Away Based On]** menu e escolha  **[!UICONTROL Color]** ou  **[!UICONTROL Transparency]**.

      Se você escolher a opção Cor, selecione o menu Canto e escolha o canto do PSD com a cor que melhor representa a cor do espaço em branco que deseja recortar.

      Arraste o controle deslizante para especificar uma tolerância de 0 a 1. Para cortar com base na cor, especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto do PSD. Os números mais próximos de 1 permitem mais diferenças de cor. Para cortar com base na transparência, especifique 0 para cortar pixels somente se eles forem transparentes; números mais próximos de 1 permitem mais transparência.

   * **Manual**  - Insira o número de pixels para cortar de qualquer lado ou de cada lado da imagem. A quantidade de imagens cortadas depende da configuração ppi (pixels por polegada) no arquivo de imagem. Por exemplo, se a imagem exibir 150 ppi e você digitar 75 nas caixas de texto Superior, Direito, Inferior e Esquerdo, meia polegada será cortada de cada lado da imagem.

* **Opções de perfil de cor**  - Localizado em  **[!UICONTROL Color Profile Options]**.

   * **Preservação de cores padrão**

   * **Manter espaço de cor original**  - Mantém o espaço de cor original da imagem.

   * **Personalizado de > Para**  - abre menus para que você possa escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores Photoshop padrão ou um espaço de cores carregado no Dynamic Media Classic. Consulte [Perfis ICC](/help/icc-profiles.md).

* **Opções do Photoshop**

   * **Manter camadas**  - Pega as camadas na PSD, se houver, em ativos individuais. As camadas de ativo permanecem associadas ao PSD. Você pode visualizá-los abrindo o arquivo PSD na exibição de Detalhes e selecionando o painel de camada. Consulte Exibição e edição de camadas em um arquivo PSD.

   * **Criar modelo**  - Cria um modelo a partir das camadas no arquivo PSD.

   * **Extrair texto**  - Extrai o texto para que os usuários possam pesquisá-lo em um visualizador.

   * **Estender camadas ao tamanho do plano de fundo**  - Estende o tamanho das camadas de imagem cortadas ao tamanho da camada de plano de fundo.

   * **Nomenclatura de camada**  - as camadas no arquivo PSD são carregadas como imagens separadas. Para nomear essas imagens no Dynamic Media Classic, escolha uma das seguintes opções:

      * **Nome da camada**  - Nomeia as imagens após seus nomes de camada no arquivo PSD. Por exemplo, uma camada chamada Tag de preço no arquivo PSD original se torna uma imagem chamada Tag de preço. No entanto, se os nomes de camada no arquivo PSD forem nomes de camada padrão do Photoshop (Plano de fundo, Camada 1, Camada 2 e assim por diante), as imagens serão nomeadas após seus números de camada no arquivo PSD, não seus nomes de camada padrão.

      * **Photoshop e número de camada**  - Nomeia as imagens após seus números de camada no arquivo PSD, ignorando os nomes originais da camada. As imagens são nomeadas com o nome do arquivo Photoshop e um número de camada anexado. Por exemplo, a segunda camada de um arquivo chamado `Spring Ad.psd` é chamada de `Spring Ad_2` mesmo que tenha um nome não padrão no Photoshop.

      * **Photoshop e nome da camada**  - Nomeia as imagens após o arquivo PSD seguido do nome da camada ou do número da camada. O número da camada é usado se os nomes da camada no arquivo PSD forem nomes padrão da camada do Photoshop. Por exemplo, uma camada chamada `Price Tag` em um arquivo PSD chamado `SpringAd` é chamada de `Spring Ad_Price Tag`. Uma camada com o nome padrão Camada 2 é chamada `Spring Ad_2`.
   * **Âncora**  - Especifique como as imagens são ancoradas em modelos que são gerados a partir da composição em camadas produzida a partir do arquivo PSD. Por padrão, a âncora é o centro. Uma âncora central permite que imagens de substituição preencham melhor o mesmo espaço, independentemente da proporção da imagem de substituição. Imagens com um aspecto diferente que substituem essa imagem, ao referenciar o modelo e usar substituição de parâmetro, ocupam efetivamente o mesmo espaço. Altere para uma configuração diferente se o aplicativo exigir as imagens de substituição para preencher o espaço alocado no modelo.


## Exibição e edição de camadas em um arquivo PSD {#viewing-and-editing-layers-in-a-psd-file}

Se você selecionou a opção Manter camadas ao fazer upload do PSD, o Dynamic Media Classic recortou as camadas individuais em ativos. Você pode exibir e editar as camadas de ativo pertencentes a um arquivo PSD abrindo o arquivo no Painel de navegação na exibição de Detalhes.

1. Clique duas vezes no arquivo PSD completo no painel Procurar. O arquivo é aberto na exibição de Detalhes.

   >[!NOTE]
   >
   >Certifique-se de abrir o ativo completo e não uma das camadas de PSD.

1. Clique em **[!UICONTROL Layers]**. Todas as camadas são exibidas como imagens separadas no painel Camadas.
1. Clique duas vezes em uma camada e siga um destes procedimentos:

   * Para criar um mapa de imagem na camada, clique no ícone **[!UICONTROL Image Map]**. (Consulte [Criação de mapas de imagem](creating-image-maps.md#creating_image_maps).)
   * Para criar destinos de zoom na camada, clique no ícone **[!UICONTROL Zoom Targets]**. (Consulte [Criação de destinos de zoom para Zoom Guiado](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Para recortar a camada, clique no ícone **[!UICONTROL Crop]**. (Consulte [Recortar uma imagem](cropping-image.md#cropping_an_image).)
   * Para ajustar a nitidez da camada, clique em **[!UICONTROL Sharpen]**. (Consulte [Nitidez de uma imagem](sharpening-image.md#sharpening_an_image).)
   * Para ajustar a camada, clique em **[!UICONTROL Adjust]**. (Consulte [Ajustar uma imagem](adjusting-image.md#adjusting_an_image).)

1. Clique em **[!UICONTROL Save]** ou **[!UICONTROL Save As]**.
1. Para exibir ou editar uma camada diferente, clique em uma seta na parte inferior da visualização da camada.
1. Para sair da exibição Detalhes da camada, clique no ícone **[!UICONTROL Grid view]**.
