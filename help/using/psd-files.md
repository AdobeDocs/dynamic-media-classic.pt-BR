---
title: Trabalhar com arquivos do PSD
description: Saiba como trabalhar com arquivos PSD no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# Trabalhar com arquivos do PSD{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)**: Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on Web pages. -->

O PSD (arquivos de documento do Photoshop) é usado com mais frequência no Adobe Dynamic Media Classic para criar modelos. Ao fazer upload de um arquivo do PSD, você pode criar um modelo do Adobe Dynamic Media Classic automaticamente a partir do arquivo (selecione a opção Criar modelo na tela Upload).

O Adobe Dynamic Media Classic cria várias imagens a partir de um arquivo PSD com camadas, se você usar o arquivo para criar um modelo; ele cria uma imagem para cada camada.

## Opções de upload do PSD {#psd-upload-options}

As opções para fazer upload de arquivos do PSD estão localizadas em Opções do Photoshop, na caixa de diálogo Fazer upload das opções de trabalho. Você pode cortar um arquivo, escolher um perfil de cor para ele, usá-lo para criar um modelo e selecionar uma âncora.

Essas opções estão disponíveis ao fazer upload de arquivos PSD:

* **Opções de corte**: Localizadas em **[!UICONTROL Crop Options]**. Selecione **[!UICONTROL Trim]** para que você possa cortar automaticamente o espaço em branco das bordas de um arquivo PSD. Selecione **[!UICONTROL Manual]** para recortar os lados do arquivo PSD:

   * **[!UICONTROL Trim]**: Selecione o menu **[!UICONTROL Trim Away Based On]** e escolha **[!UICONTROL Color]** ou **[!UICONTROL Transparency]**.

  Se você escolher a opção **[!UICONTROL Color]**, selecione o menu Canto e escolha o canto do PSD com a cor que melhor representa a cor do espaço em branco que você deseja cortar.

  Arraste o controle deslizante para especificar uma tolerância de 0 a 1. Para recortar com base na cor, especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto do PSD. Números próximos a 1 permitem mais diferença de cor. Para cortar com base na transparência, especifique 0 para cortar pixels apenas se forem transparentes; números mais próximos de 1 permitem mais transparência.

   * **[!UICONTROL Manual]**: Digite o número de pixels a serem cortados de qualquer lado ou de cada lado da imagem. O quanto da imagem é cortada depende da configuração ppi (pixels por polegada) no arquivo de imagem. Por exemplo, suponha que a imagem exiba 150 ppi. Em seguida, digite 75 nas caixas de texto Superior, Direito, Inferior e Esquerdo. Cada lado da imagem é cortado, 0,5 pol.

* **Opções de Perfil de Cores**: Localizadas em **[!UICONTROL Color Profile Options]**.

   * **[!UICONTROL Default Color Preservation]**

   * **[!UICONTROL Keep Original Color Space]**: retém o espaço de cores original da imagem.

   * **[!UICONTROL Custom From]** > **[!UICONTROL To]**: abre menus para que você possa escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores padrão do Photoshop ou um espaço de cores carregado no Adobe Dynamic Media Classic. Consulte [perfis ICC](/help/using/icc-profiles.md).

* **Opções do Photoshop**

   * **[!UICONTROL Maintain Layers]**: Ripa as camadas na PSD, se houver, em ativos individuais. As camadas de ativos permanecem associadas à PSD. É possível visualizá-las abrindo o arquivo PSD na Exibição de detalhes e selecionando o painel de camada. Consulte Exibição e edição de camadas em um arquivo do PSD.

   * **[!UICONTROL Create Template]**: cria um modelo a partir das camadas no arquivo PSD.

   * **[!UICONTROL Extract Text]**: extrai o texto para que os usuários possam pesquisar texto em um Visualizador.

   * **[!UICONTROL Extend Layers To Background Size]**: Estende o tamanho das camadas de imagem extraídas para o tamanho da camada de plano de fundo.

   * **[!UICONTROL Layer Naming]**: as camadas no arquivo PSD são carregadas como imagens separadas. Para nomear essas imagens no Adobe Dynamic Media Classic, escolha uma das seguintes opções:

      * **[!UICONTROL Layer Name]**: Nomeia as imagens de acordo com seus nomes de camada no arquivo PSD. Por exemplo, uma camada chamada Etiqueta de preço no arquivo original do PSD se torna uma imagem chamada Etiqueta de preço. No entanto, se os nomes das camadas no arquivo do PSD forem nomes de camadas padrão do Photoshop (Plano de fundo, Camada 1, Camada 2 e assim por diante), as imagens serão nomeadas após seus números de camada no arquivo do PSD. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop and layer number]**: Nomeia as imagens de acordo com seus números de camada no arquivo PSD, ignorando os nomes de camada originais. As imagens são nomeadas com o nome de arquivo do Photoshop e um número de camada anexado. Por exemplo, a segunda camada de um arquivo chamado `Spring Ad.psd` é chamada `Spring Ad_2` mesmo se tiver um nome não padrão no Photoshop.

      * **[!UICONTROL Photoshop and layer name]**: Nomeia as imagens após o arquivo PSD seguido pelo nome ou número da camada. O número da camada é usado se os nomes das camadas no arquivo do PSD forem nomes de camadas padrão do Photoshop. Por exemplo, uma camada chamada `Price Tag` em um arquivo PSD chamado `SpringAd` é chamada `Spring Ad_Price Tag`. Uma camada com o nome padrão Layer 2 é chamada `Spring Ad_2`.

   * **[!UICONTROL Anchor]**: especifique como as imagens são ancoradas em modelos que são gerados a partir da composição em camadas produzida a partir do arquivo PSD. Por padrão, a âncora é o centro. Uma âncora central permite substituir imagens que podem preencher melhor o mesmo espaço, independentemente da proporção da imagem de substituição. As imagens com um aspecto diferente que substituem essa imagem, ao referenciar o modelo e usar a substituição de parâmetro, ocupam efetivamente o mesmo espaço. Altere para uma configuração diferente se seu aplicativo exigir que as imagens de substituição preencham o espaço alocado no modelo.

## Exibir e editar camadas em um arquivo PSD {#viewing-and-editing-layers-in-a-psd-file}

Se você selecionou a opção **[!UICONTROL Maintain Layers]** quando carregou o PSD, o Adobe Dynamic Media Classic rasgou as camadas individuais em ativos. É possível visualizar e editar as camadas de ativos pertencentes a um arquivo do PSD abrindo o arquivo no painel Procurar na Exibição de detalhes.

>[!NOTE]
>
>O Adobe Dynamic Media Classic suporta até cinco níveis em um grupo de camadas aninhado.

1. Clique duas vezes no arquivo PSD completo no painel Procurar. O arquivo é aberto na Exibição de Detalhes.

   >[!NOTE]
   >
   >Certifique-se de abrir o ativo completo e não uma das camadas do PSD.

1. Selecione **[!UICONTROL Layers]**. Todas as camadas são exibidas como imagens separadas no painel Camadas.
1. Clique duas vezes em uma camada e siga um destes procedimentos:

   * Para criar um Mapa de Imagem na camada, selecione o ícone **[!UICONTROL Image Map]**. (Consulte [Criar Mapas De Imagens](creating-image-maps.md#creating_image_maps).)
   * Para criar Destinos de Zoom na camada, selecione o ícone **[!UICONTROL Zoom Targets]**. (Consulte [Criar Destinos de Zoom para Zoom Guiado](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Para recortar a camada, selecione o ícone **[!UICONTROL Crop]**. (Consulte [Cortar uma imagem](cropping-image.md#cropping_an_image).)
   * Para ajustar a nitidez da camada, selecione **[!UICONTROL Sharpen]**. (Consulte [Nitidez de uma imagem](sharpening-image.md#sharpening_an_image).)
   * Para ajustar a camada, selecione **[!UICONTROL Adjust]**. (Consulte [Ajustar uma imagem](adjusting-image.md#adjusting_an_image).)

1. Selecione **[!UICONTROL Save]** ou **[!UICONTROL Save As]**.
1. Para visualizar ou editar uma camada diferente, selecione uma seta na parte inferior da visualização da camada.
1. Para sair da Exibição de Detalhes da camada, selecione o ícone **[!UICONTROL Grid View]**.
