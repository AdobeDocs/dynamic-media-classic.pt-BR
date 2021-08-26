---
title: Opções de ajuste de imagem no upload
description: Saiba mais sobre as opções de ajuste fino de imagem disponíveis no momento do upload no Adobe Dynamic Media Classic.
uuid: 0912ae6f-41c9-41b5-94d1-e266face782e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: d3f21cdf-2cb3-46e8-955a-b8daf0b233bc
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# Opções de ajuste de imagem no upload{#image-editing-options-at-upload}

Ao carregar arquivos de imagem, incluindo arquivos AI, EPS e PSD, você pode realizar as seguintes ações de edição na caixa de diálogo Upload Job Options :

* Recorte o espaço em branco da borda das imagens.
* Recorte manualmente das laterais das imagens.
* Escolha um perfil de cor.
* Crie uma máscara a partir de um traçado de recorte.
* Afiar imagens com opções de máscara nítidas
* Plano de Fundo de Vazamento

Essas opções estão na página Upload sob o cabeçalho **[!UICONTROL Imaging Edit Options]**.

## Recortar espaço em branco de imagens

Para cortar automaticamente pixels de espaço em branco de uma imagem, na caixa de diálogo Upload Job Options , selecione **[!UICONTROL Crop Options]**. Na lista suspensa **[!UICONTROL Crop]**, escolha **[!UICONTROL Trim]**. Em seguida, escolha estas opções:

* **[!UICONTROL Trim Away Based On]** - Nessa lista suspensa, escolha entre cortar com base na cor ou na transparência:

   * **[!UICONTROL Color]** - Escolha a  **[!UICONTROL Color]** opção . Em seguida, na lista suspensa **[!UICONTROL Corner]**, selecione o canto da imagem com a cor que melhor representa a cor do espaço em branco que deseja recortar.

   * **[!UICONTROL Transparency]** - Escolha a opção Transparency .

* **[!UICONTROL Tolerance]** - Arraste o controle deslizante para especificar uma tolerância de 0 a 1:

   * **Aparar com base na cor**  - Especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto da imagem. Os números mais próximos de 1 permitem mais diferenças de cor.

   * **Aparar com base na transparência**  - Especifique 0 para cortar pixels somente se eles forem transparentes; números mais próximos de 1 permitem mais transparência.

## Recortar manualmente das laterais das imagens

Para recortar manualmente das laterais de uma imagem, selecione o menu Recortar e escolha Manual. Em seguida, insira o número de pixels para cortar de qualquer lado ou de cada lado da imagem. A quantidade de imagens cortadas depende da configuração ppi (pixels por polegada) no arquivo de imagem. Por exemplo, se a imagem exibir 150 ppi e você digitar 75 nas caixas de texto Superior, Direito, Inferior e Esquerdo, meia polegada será cortada de cada lado.

## Escolha um perfil de cores

Para selecionar um espaço de cores para a imagem, escolha uma opção de Perfil de cores:

* **[!UICONTROL Convert To sRGB]** - Converte em sRGB (Azul Verde Vermelho Padrão). sRGB é o espaço de cores recomendado para exibir imagens nas páginas da Web.

* **[!UICONTROL Keep Original Color Space]** - Mantém o espaço de cores original.

* **[!UICONTROL Custom From]** >  **[!UICONTROL To]** - Abre menus para que você possa escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores Photoshop padrão ou um espaço de cores carregado no Adobe Dynamic Media Classic.

Consulte [Perfis ICC](icc-profiles.md#icc_profiles).

## Criar uma máscara a partir de um traçado de recorte

Para criar uma máscara para a imagem com base em suas informações de traçado de recorte, selecione **[!UICONTROL Create Mask From Clipping Path]**. Essa opção se aplica a imagens criadas com aplicativos de edição de imagens nas quais um traçado de recorte foi criado.

## Nitidez de uma imagem usando a máscara de ajuste de nitidez

Esse filtro permite ajustar um efeito de filtro de nitidez na imagem final com resolução reduzida. Ajuda a controlar a intensidade do efeito, o raio do efeito (conforme medido em pixels) e um limite de contraste que é ignorado.

Esse efeito usa as mesmas opções do filtro Tirar nitidez da máscara da Photoshop. Ao contrário do que o nome sugere, Tirar nitidez da máscara é um filtro de nitidez.

Em Tirar nitidez da máscara, defina as opções desejadas. As opções de configuração são descritas na tabela a seguir:

| Tirar nitidez das opções de Máscara | Descrição |
| --- | --- |
| Valor | Controla a quantidade de contraste que é aplicada aos pixels da borda.<br><br>Pense nisso como a intensidade do efeito. A principal diferença entre os valores de quantidade de Tirar nitidez da máscara no Adobe Dynamic Media Classic e os valores de quantidade no Adobe Photoshop é que o Photoshop tem um intervalo de quantidade de 1% a 500%. Considerando que no Adobe Dynamic Media Classic, o intervalo de valor é de 0,0 a 5,0. Um valor de 5,0 no Adobe Dynamic Media Classic é o equivalente bruto de 500% no Photoshop; um valor de 0,9 é o equivalente a 90%, e assim por diante. |
| Raio | Controla o raio do efeito. <br><br>O intervalo de valores é de 0 a 250. O efeito é executado em todos os pixels em uma imagem e irradia de todos os pixels em todas as direções. O raio é medido em pixels. Por exemplo, para obter um efeito de nitidez semelhante para uma imagem de 2000 x 2000 pixels e imagem de 500 x 500 pixels, você define um raio de dois pixels na imagem de 2000 x 2000 pixels. Em seguida, defina um valor de raio de um pixel na imagem de 500 x 500 pixels. Um valor maior é usado para uma imagem que tem mais pixels. |
| Limite | O limite é um intervalo de contraste que é ignorado quando o filtro Tirar nitidez da máscara é aplicado. Esse efeito é importante para que nenhum &quot;ruído&quot; seja introduzido em uma imagem quando esse filtro for usado. O intervalo de valores é de 0 a 255, que é o número de etapas de brilho em uma imagem em tons de cinza. 0=preto, 128=50% cinza e 255=branco.<br><br>Por exemplo, um valor limite de 12 ignora pequenas variações é o brilho do tom da pele para evitar a adição de ruído, mas ainda adiciona o contraste da borda a áreas contrastantes, como onde as pálpebras tocam a pele.<br><br>Por exemplo, se você tiver uma foto do rosto de alguém, a Máscara de Nitidez afeta as partes contrastantes da imagem. Por exemplo, onde as pálpebras e a pele se encontram para criar uma área de contraste óbvia e a própria pele lisa. Mesmo a pele mais suave apresenta alterações sutis nos valores de brilho. Se você não usar um valor de limite, o filtro acentuará essas sutis alterações em pixels da pele. Por sua vez, um efeito ruidoso e indesejável é criado enquanto o contraste nas pálpebras aumenta, aumentando a nitidez.<br><br>Para evitar esse problema, é introduzido um valor limite que informa ao filtro para ignorar pixels que não alteram o contraste drasticamente, como pele lisa. <br><br>No gráfico zipper mostrado anteriormente, observe a textura ao lado dos zippers. O ruído da imagem é exibido porque os valores de limite eram muito baixos para suprimir o ruído. |
| Monocromático | Selecione para ativar o brilho (intensidade) da imagem da máscara de nitidez.<br><br>Desmarque para desfazer a nitidez de cada componente de cor separadamente. |

Consulte também [Nitidez uma imagem](sharpening-image.md#sharpening_an_image).

Consulte também [Nitidez de imagens no Adobe Dynamic Media e no Servidor de imagens](/help/assets/s7_sharpening_images.pdf).

## Plano de Fundo de Vazamento

Você pode usar o Plano de fundo de Knockout para remover automaticamente o plano de fundo de uma imagem quando você a faz upload. Essa técnica é útil para chamar a atenção para um objeto específico e destacá-lo a partir de um fundo ocupado.

| Opções de plano de fundo do KnockOut | Descrição |
| --- | --- |
| Plano de Fundo de Vazamento | Selecione para ativar ou &quot;ativar&quot; o recurso e as opções de Plano de Fundo de Knockout. |
| Canto | Obrigatório.<br>O canto da imagem que é usado para definir a cor do plano de fundo para nocautear.<br>Você pode escolher entre  <b>Superior esquerdo, Inferior esquerdo, Superior direito ou Inferior direito</b>. |
| Método de preenchimento | Obrigatório. <br>Controla a transparência de pixels do local Canto que você definiu.<br>Você pode escolher entre os seguintes métodos de preenchimento:<br> ・  <b>Flood Fill</b>  - torna todos os pixels transparentes que correspondem ao Canto especificado e conectado a ele.<br>・  <b>Corresponder pixel</b>  - torna todos os pixels correspondentes transparentes, independentemente de sua localização na imagem. |
| Tolerância | Opcional.<br>Controla a quantidade permitida de variação na correspondência de cores de pixels com base na localização Canto que você definiu.<br>Use um valor de 0,0 para corresponder exatamente às cores dos pixels ou use um valor de 1,0 para permitir a maior variação. |

>[!MORELIKETHIS]
>
>* [Recortar uma imagem](cropping-image.md#cropping_an_image)

