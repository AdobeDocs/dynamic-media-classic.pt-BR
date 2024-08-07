---
title: Opções de ajuste de imagem no upload
description: Saiba mais sobre as opções de ajuste de imagem disponíveis no momento do upload no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
topic: Administration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1169'
ht-degree: 0%

---

# Opções de ajuste de imagem no upload{#image-editing-options-at-upload}

Ao fazer upload de arquivos de imagem, incluindo arquivos AI, EPS e PSD, você pode realizar as seguintes ações de edição na caixa de diálogo Fazer upload das opções de tarefa:

* Cortar espaço em branco a partir da borda das imagens.
* Recortar manualmente nas laterais das imagens.
* Escolha um perfil de cores.
* Criar uma máscara a partir de um traçado de recorte.
* Nitidez de imagens com opções de máscara sem nitidez
* Plano de fundo de separação

Essas opções estão na página de Carregamento sob o cabeçalho **[!UICONTROL Imaging Edit Options]**.

## Cortar espaço em branco a partir de imagens

Você pode cortar automaticamente pixels de espaço em branco de uma imagem. Na caixa de diálogo Carregar Opções de Trabalho, selecione **[!UICONTROL Crop Options]**. Na lista suspensa **[!UICONTROL Crop]**, escolha **[!UICONTROL Trim]**. Em seguida, escolha estas opções:

* **[!UICONTROL Trim Away Based On]**: Nessa lista suspensa, escolha se deseja cortar com base na cor ou na transparência:

   * **[!UICONTROL Color]**: Escolha a opção **[!UICONTROL Color]**. Em seguida, na lista suspensa **[!UICONTROL Corner]**, selecione o canto da imagem com a cor que melhor representa a cor do espaço em branco que você deseja cortar.

   * **[!UICONTROL Transparency]**: Escolha a opção Transparência.

* **[!UICONTROL Tolerance]**: arraste o controle deslizante para especificar uma tolerância de 0 a 1:

   * **Corte com base na cor**: especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto da imagem. Números próximos a 1 permitem mais diferença de cor.

   * **Corte com base na transparência**: especifique 0 para cortar pixels somente se eles forem transparentes; números mais próximos a 1 permitem mais transparência.

## Recortar manualmente nas laterais das imagens

Para recortar manualmente das laterais de uma imagem, selecione o menu Recortar e escolha Manual. Em seguida, insira o número de pixels a serem cortados de qualquer lado ou de cada lado da imagem. O quanto da imagem é cortada depende da configuração ppi (pixels por polegada) no arquivo de imagem. Por exemplo, suponha que a imagem exiba 150 ppi. Em seguida, digite 75 nas caixas de texto Superior, Direito, Inferior e Esquerdo. Neste ponto, cada lado é cortado 0,5 polegada.

## Escolha um perfil de cores

Para selecionar um espaço de cores para a imagem, escolha uma opção de Perfil de Cores:

* **[!UICONTROL Convert To sRGB]**: Converte para sRGB (Vermelho Verde Azul Padrão). sRGB é o espaço de cores recomendado para exibir imagens em páginas da Web.

* **[!UICONTROL Keep Original Color Space]**: retém o espaço de cores original.

* **[!UICONTROL Custom From]** > **[!UICONTROL To]**: abre menus para que você possa escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores padrão do Photoshop ou um espaço de cores carregado no Adobe Dynamic Media Classic.

Consulte [perfis ICC](icc-profiles.md#icc_profiles).

## Criação de uma máscara a partir de um traçado de recorte

Para criar uma máscara para a imagem com base nas informações do caminho de recorte, selecione **[!UICONTROL Create Mask From Clipping Path]**. Essa opção se aplica a imagens criadas com aplicativos de edição de imagens nos quais um traçado de recorte foi criado.

## Nitidez de uma imagem usando Tirar nitidez da máscara

Esse filtro permite ajustar um efeito de filtro de nitidez na imagem final com resolução reduzida. Ela ajuda a controlar a intensidade do efeito, o raio do efeito (medido em pixels) e um limite de contraste ignorado.

Esse efeito usa as mesmas opções do filtro Tirar nitidez da máscara do Photoshop. Ao contrário do que o nome sugere, Unsharp Mask é um filtro de nitidez.

Em Tirar nitidez da máscara, defina as opções desejadas. As opções de configuração são descritas na tabela a seguir:

| Opções de Tirar nitidez da máscara | Descrição |
| --- | --- |
| Quantidade | A quantidade controla a quantidade de contraste aplicada aos pixels de borda.<br><br>Pense nisso como a intensidade do efeito. Há uma diferença entre os valores de quantidade de Tirar nitidez da máscara no Dynamic Media Classic e no Adobe Photoshop. A principal diferença é que o Photoshop tem um intervalo de valores de 1% a 500%. Enquanto no Adobe Dynamic Media Classic, o intervalo de valores é de 0,0 a 5,0. Um valor de 5,0 no Adobe Dynamic Media Classic é o equivalente aproximado de 500% no Photoshop; um valor de 0,9 é o equivalente de 90% e assim por diante. |
| Raio | Controla o raio do efeito. <br><br>O intervalo de valores é de 0 a 250. O efeito é executado em todos os pixels em uma imagem e irradia de todos os pixels em todas as direções. O raio é medido em pixels. Por exemplo, para obter um efeito de nitidez semelhante para uma imagem de 2000 × 2000 pixels e uma imagem de 500 × 500 pixels, você definiria um raio de dois pixels na imagem de 2000 × 2000 pixels. Em seguida, defina um valor de raio de um pixel na imagem de 500 × 500 pixels. Um valor maior é usado para uma imagem com mais pixels. |
| Limite | O limite é um intervalo de contraste ignorado quando o filtro Tirar nitidez da máscara é aplicado. Esse efeito é importante para que nenhum &quot;ruído&quot; seja introduzido em uma imagem quando esse filtro for usado. O intervalo de valores é de 0 a 255, que é o número de etapas de brilho em uma imagem em tons de cinza. 0=preto, 128=50% cinza e 255=branco.<br><br>Por exemplo, um valor limite de 12 ignora pequenas variações no brilho do tom da pele para evitar a adição de ruído, mas ainda adiciona o contraste da borda a áreas contrastadas, como onde as pálpebras tocam a pele.<br><br>Por exemplo, se você tiver uma foto do rosto de alguém, a Máscara de Nitidez afetará as partes contrastadas da imagem. Por exemplo, onde pestanas e pele se encontram para criar uma área óbvia de contraste e a própria pele lisa. Mesmo a pele mais suave exibe alterações sutis nos valores de brilho. Se você não usar um valor de limite, o filtro acentua essas alterações sutis nos pixels de capa. Por sua vez, um efeito ruidoso e indesejável é criado enquanto o contraste das pálpebras é aumentado, aumentando a nitidez.<br><br>Para evitar esse problema, é introduzido um valor limite que informa ao filtro para ignorar os pixels que não alteram drasticamente o contraste, como a capa lisa. <br><br>No gráfico de zíper mostrado anteriormente, observe a textura ao lado dos zíperes. O ruído da imagem é exibido porque os valores de limite são muito baixos para suprimir o ruído. |
| Monocromático | Selecione para desfazer a nitidez da imagem de brilho (intensidade).<br><br>Desmarque para remover a nitidez de cada componente de cor separadamente. |

Consulte também [Nitidez de uma imagem](sharpening-image.md#sharpening_an_image).

Consulte também [Nitidez de imagens no Adobe Dynamic Media e no Servidor de imagens](/help/using/assets/s7_sharpening_images.pdf).

## Plano de fundo de separação

Use o Plano de fundo de separação para remover automaticamente o plano de fundo de uma imagem ao carregá-la. Essa técnica é útil para chamar a atenção para um objeto específico e destacá-lo de um plano de fundo ocupado.

| Opções de plano de fundo de separação | Descrição |
| --- | --- |
| Plano de fundo de separação | Selecione para ativar ou &quot;ativar&quot; o recurso e as opções de Plano de fundo de separação. |
| Canto | Obrigatório.<br>O canto da imagem usado para definir a cor do plano de fundo a ser vazada.<br>Você pode escolher entre <b>Superior Esquerdo, Inferior Esquerdo, Superior Direito ou Inferior Direito</b>. |
| Método de preenchimento | Obrigatório. <br>Controla a transparência de pixels do local do Canto definido.<br>Você pode escolher entre os seguintes métodos de preenchimento:<br>· <b>Preenchimento do Flood</b>: transforma todos os pixels transparentes que correspondem ao Canto que você especificou e que estão conectados a ele.<br>· <b>Pixel de correspondência</b>: torna transparentes todos os pixels correspondentes, independentemente de sua localização na imagem. |
| Tolerância | Opcional.<br>Controla a quantidade permitida de variação na correspondência de cores de pixels com base no local do Canto definido.<br>Use um valor de 0,0 para corresponder exatamente às cores do pixel. Ou use um valor de 1,0 para permitir a maior variação. |

>[!MORELIKETHIS]
>
>* [Cortar uma imagem](cropping-image.md#cropping_an_image)
