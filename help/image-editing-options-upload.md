---
title: Opções de edição de imagem no upload
seo-title: Opções de edição de imagem no upload
description: nulo
seo-description: Saiba mais sobre as opções de edição de imagens disponíveis no momento do upload.
uuid: 0912ae6f-41c9-41b5-94d1-e266face782e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: d3f21cdf-2cb3-46e8-955a-b8daf0b233bc
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 0%

---


# Opções de edição de imagem no upload{#image-editing-options-at-upload}

Ao carregar arquivos de imagem, incluindo arquivos AI, EPS e PSD, você pode realizar as seguintes ações de edição na caixa de diálogo Carregar opções de trabalho:

* Recorte o espaço em branco da borda das imagens.
* Recorte manualmente dos lados das imagens.
* Escolha um perfil colorido.
* Crie uma máscara a partir de um caminho de recorte.
* Nitidez de imagens com opções de máscara nítida
* Plano de fundo de separação

Essas opções estão localizadas na tela Carregar em Opções de edição de imagem.

**Recortar espaço em branco de imagens**

Para recortar automaticamente pixels de espaço em branco de uma imagem, selecione o menu Recortar e escolha Aparar. Em seguida, escolha estas opções:

* **Aparar para longe com base em** Escolha se deseja cortar com base na cor ou na transparência:

* **Cor** Escolha a opção Cor. Em seguida, na lista suspensa Canto, selecione o canto da imagem com a cor que melhor representa a cor do espaço em branco que você deseja cortar.

* **Transparência** Escolha a opção Transparência.

* **Tolerância** Arraste o controle deslizante para especificar uma tolerância de 0 a 1:

* **Aparar com base na cor** Especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto da imagem. Números próximos a 1 permitem mais diferenças de cor.

* **Aparar com base na transparência** Especifique 0 para cortar pixels somente se eles forem totalmente transparentes. números mais próximos de 1 permitem mais transparência.

**Recortar manualmente dos lados das imagens**

Para recortar manualmente das laterais de uma imagem, selecione o menu Recortar e escolha Manual. Em seguida, insira o número de pixels a serem cortados de qualquer lado ou de cada lado da imagem. A quantidade de imagens cortadas depende da configuração ppi (pixels por polegada) no arquivo de imagem. Por exemplo, se a imagem exibir 150 ppi e você digitar 75 nas caixas de texto Superior, Direita, Inferior e Esquerda, meia polegada será cortada de cada lado.

**Como escolher um perfil colorido**

Escolha uma opção Perfil de cor para selecionar um espaço de cor para a imagem:

* **Converter em sRGB** converte em sRGB (Padrão Vermelho Verde Azul). O sRGB é o espaço de cores recomendado para exibir imagens em páginas da Web.

* **Manter espaço** de cor original Retém o espaço de cor original.

* **Menus Personalizado de > Para** abrir para que você possa escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores padrão do Photoshop ou um espaço de cores carregado no Dynamic Media Classic.

Consulte perfis [](icc-profiles.md#icc_profiles)ICC.

**Criação de uma máscara a partir de um caminho de recorte**

Selecione **Criar máscara a partir do caminho** de recorte para criar uma máscara para a imagem com base nas informações do caminho de recorte. Essa opção se aplica a imagens criadas com aplicativos de edição de imagens nas quais um caminho de recorte foi criado.

**Nitidez de uma imagem usando a Máscara de nitidez**

Esse filtro permite ajustar um efeito de filtro de nitidez na imagem final com resolução reduzida, controlando a intensidade do efeito, o raio do efeito (conforme medido em pixels) e um limite de contraste que é ignorado.

Esse efeito usa as mesmas opções do filtro Máscara de nitidez do Photoshop. Ao contrário do que o nome sugere, a Máscara de nitidez é um filtro de nitidez.

Em Mascaramento de nitidez, defina as opções desejadas. As opções de configuração são descritas na tabela a seguir:

| Opções de máscara de nitidez | Descrição |
|--- |--- |
| Valor | Controla a quantidade de contraste que é aplicada aos pixels da borda.<br><br>Pense nisso como a intensidade do efeito. A principal diferença entre os valores de quantidade de máscara de nitidez no Dynamic Media Classic e os valores de quantidade no Adobe Photoshop é que o Photoshop tem um intervalo de quantidade de 1% a 500%. Enquanto que, no Dynamic Media Classic, o intervalo de valores é de 0,0 a 5,0. Um valor de 5,0 no Dynamic Media Classic é o equivalente bruto de 500% no Photoshop; um valor de 0,9 é o equivalente a 90%, e assim por diante. |
| Raio | Controla o raio do efeito. <br><br>O intervalo de valores é de 0 a 250. O efeito é executado em todos os pixels em uma imagem e irradia de todos os pixels em todas as direções. O raio é medido em pixels. Por exemplo, para obter um efeito de nitidez semelhante para uma imagem de 2000 x 2000 pixels e 500 x 500 pixels, você definiria um raio de dois pixels na imagem de 2000 x 2000 pixels e um valor de raio de um pixel na imagem de 500 x 500 pixels. Um valor maior é usado para uma imagem que tem mais pixels. |
| Limiar | O limite é um intervalo de contraste que é ignorado quando o filtro Máscara de nitidez é aplicado. Isso é importante para que nenhum &quot;ruído&quot; seja introduzido em uma imagem quando esse filtro for usado. O intervalo de valores é de 0 a 255, que é o número de etapas de brilho em uma imagem em tons de cinza. 0=preto, 128=50% cinza e 255=branco.<br><br>Por exemplo, um valor limite de 12 ignora pequenas variações é o brilho do tom de pele para evitar a adição de ruído, mas ainda adiciona contraste de borda a áreas contrastantes, como onde as pestanas encontram a pele.<br><br>Por exemplo, se você tiver uma foto do rosto de alguém, a Máscara de Nitidez afeta as partes contrastantes da imagem, como onde as pestanas e a pele se encontram para criar uma área de contraste óbvia, e a própria pele lisa. Mesmo a pele mais suave exibe alterações sutis nos valores de brilho. Se você não usar um valor limite, o filtro acentuará essas alterações sutis em pixels de pele. Por sua vez, cria-se um efeito ruidoso e indesejável enquanto o contraste nas pestanas aumenta, aumentando a nitidez.<br><br>Para evitar esse problema, é introduzido um valor limite que informa ao filtro que ignore os pixels que não alteram o contraste drasticamente, como pele lisa. <br><br>No gráfico de zipper mostrado anteriormente, observe a textura ao lado dos zippers. O ruído da imagem é exibido porque os valores de limite eram muito baixos para suprimir o ruído. |
| Monocromático | Selecione para desmarcar o brilho da imagem da máscara de nitidez (intensidade).<br><br>Desmarque para desmarcar a máscara de nitidez de cada componente de cor separadamente. |

Consulte também [Nitidez de uma imagem](sharpening-image.md#sharpening_an_image).

Consulte também [Compartilhamento de imagens no Scene7 Publishing System e no Image Server](/help/assets/s7_sharpening_images.pdf).

**Plano de fundo de separação**

Você pode usar o Plano de fundo de separação para remover automaticamente o plano de fundo de uma imagem ao carregá-la. Essa técnica é útil para chamar a atenção para um objeto específico e destacá-lo de um fundo ocupado.

| Opções de plano de fundo do menu suspenso | Descrição |
|:--- |:--- |
| Plano de fundo de separação | Selecione para ativar ou &quot;ativar&quot; o recurso e as opções de Plano de fundo de separação. |
| Canto | Obrigatório.<br><br>O canto da imagem que é usado para definir a cor do plano de fundo para separação.<br><br>Você pode escolher entre <b>Superior Esquerda, Inferior Esquerda, Superior Direita ou Inferior Direita</b>. |
| Método de preenchimento | Obrigatório. <br><br>Controla a transparência de pixels a partir do local Canto que você definiu.<br><br>Você pode escolher entre os seguintes métodos de preenchimento: <ul><li><b>Preenchimento</b> de Flood - torna todos os pixels transparentes que correspondem ao Canto especificado e conectado a ele.</li><li><b>Corresponder pixel</b> - torna todos os pixels correspondentes transparentes, independentemente de sua localização na imagem.</li></ul> |
| Tolerância | Opcional.<br><br>Controla a quantidade permitida de variação na correspondência de cores de pixels com base no local Canto que você definiu.<br><br>Use um valor de 0,0 para corresponder exatamente às cores dos pixels ou use um valor de 1,0 para permitir a maior variação. |

>[!MORELIKETHIS]
>
>* [Recortar uma imagem](cropping-image.md#cropping_an_image)

