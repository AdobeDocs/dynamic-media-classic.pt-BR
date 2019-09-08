---
title: Opções de edição de imagens no upload
seo-title: Opções de edição de imagens no upload
description: 'null'
seo-description: Saiba mais sobre as opções de edição de imagens disponíveis no momento do upload.
uuid: 0912 ae 6 f -41 c 9-41 b 5-94 d 1-e 266 face 782 e
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/master_ files
discoiquuid: d 3 f 21 cdf -2 cb 3-46 e 8-955 a-b 8 daf 0 b 233 bc
translation-type: tm+mt
source-git-commit: 0f6c8e6ac69e29aab7a48425aab76c10170d9ddf

---


# Opções de edição de imagens no upload{#image-editing-options-at-upload}

Ao carregar arquivos de imagem, incluindo arquivos AI, EPS e PSD, você pode realizar as seguintes ações de edição na caixa de diálogo Carregar opções de trabalho:

* Recorte o espaço em branco da borda das imagens.
* Cortar manualmente das laterais das imagens.
* Escolha um perfil de cor.
* Crie uma máscara de um caminho de corte.
* Nitidez de imagens com opções de máscara unificadas
* Plano de fundo de separação

Essas opções estão localizadas na tela Upload em Opções de edição de imagens.

**Recortar o espaço em branco das imagens**

Para cortar automaticamente pixels de espaço em branco de uma imagem, selecione o menu Cortar e escolha Aparar. Em seguida, escolha estas opções:

**Aparar
com base em** Escolher se deseja cortar com base em cor ou transparência:

**Cor** Escolha a opção Cor. Em seguida, na lista suspensa Canto, selecione o canto da imagem com a cor que representa melhor a cor de espaço em branco que você deseja cortar.

**Opção Transparência** escolha a opção Transparência.

**Tolerância** Arraste o controle deslizante para especificar uma tolerância de 0 a 1:

**Aparar com base na cor** especificada 0 Para cortar os pixels apenas se eles corresponderem exatamente à cor selecionada no canto da imagem. Números mais próximos a 1 permitem mais diferença de cor.

**Aparar com base na transparência** especificada 0 para cortar pixels apenas se eles forem totalmente transparentes; os números mais próximos a 1 permitem mais transparência.

**Recortar manualmente dos lados das imagens**

Para cortar manualmente dos lados de uma imagem, selecione o menu Cortar e escolha Manual. Em seguida, insira o número de pixels para cortar de qualquer lado ou cada lado da imagem. A quantidade de cortes da imagem depende da configuração de ppi (pixels por polegada) no arquivo de imagem. Por exemplo, se a imagem exibir 150 ppi e você inserir 75 nas caixas de texto Superior, Direito, Inferior e Esquerda, uma meia polegada será recortada de cada lado.

**Escolha de um perfil de cor**

Escolha uma opção Perfil de cor para selecionar um espaço de cor para a imagem:

**Converter em srgb** converte para srgb (Azul vermelho padrão). O srgb é o espaço de cores recomendado para exibir imagens em páginas da Web.

**Manter Espaço original de cor** retém o espaço de cores original.

**Personalizado de &gt; Para** abrir menus para que você possa escolher um espaço de cores Converter de e Converter para. É possível escolher um espaço de cor padrão do Photoshop ou um espaço de cores carregado no SPS.

Consulte [Perfis ICC](icc-profiles.md#icc_profiles).

**Criar uma máscara a partir de um caminho de corte**

Selecione **Criar máscara a partir do traçado** de recorte para criar uma máscara para a imagem com base nas informações do caminho de recorte. Essa opção se aplica a imagens criadas com aplicativos de edição de imagens nos quais um caminho de corte foi criado.

**Tornar uma imagem nítida usando Máscara de nitidez**

Esse filtro permite ajustar um efeito de filtro de nitidez na imagem final de resolução reduzida, controlar a intensidade do efeito, o raio do efeito (como medido em pixels) e um limite de contraste ignorado.

Esse efeito usa as mesmas opções do filtro Máscara de nitidez do Photoshop. Ao contrário do que o nome sugere, Máscara de nitidez é um filtro de nitidez.

Em Tirar nitidez, defina as opções desejadas. As opções de configuração são descritas na tabela a seguir:

| Opções de máscara de nitidez | Descrição |
|--- |--- |
| Quantia | Controla a quantidade de contraste aplicada aos pixels da borda.<br><br>Pense nisso como a intensidade do efeito. A principal diferença entre os valores de quantidade de Máscara de nitidez no SPS e os valores de quantidade no Adobe Photoshop é que o Photoshop tem um intervalo de valor de 1% a 500%. Enquanto no SPS, o intervalo de valor é de 0.0 a 5.0. Um valor de 5.0 no SPS é o equivalente aproximado de 500% no Photoshop; um valor de 0.9 equivale a 90%, e assim por diante. |
| Raio | Controla o raio do efeito. <br><br>O intervalo de valor é 0-250. O efeito é executado em todos os pixels de uma imagem e é radiado em todos os pixels em todas as direções. O raio é medido em pixels. Por exemplo, para obter um efeito de nitidez semelhante para uma imagem de 2000 x 2000 pixels e imagens de 500 x 500 pixels, você deve definir um raio de dois pixels na imagem de 2000 x 2000 pixels e um valor radius de um pixel na imagem de 500 x 500 pixels. Um valor maior é usado para uma imagem com mais pixels. |
| Limite | O limite é uma faixa de contraste ignorada quando o filtro Máscara de nitidez é aplicado. Isso é importante para que nenhum «barulho» seja inserido em uma imagem quando esse filtro for usado. O intervalo de valor é de 0-255, que é o número de etapas de brilho em uma imagem em tons de cinza. 0 = preto, 128 = 50% cinza e 255 = branco.<br><br>Por exemplo, um valor limite de 12 ignora pequenas variações que são brilho de tom de pele para evitar adicionar ruído, mas ainda adiciona contraste borda a áreas contrastantes, como onde as barras atingem a capa.<br><br>Por exemplo, se houver uma foto de face de alguém, a Máscara de nitidez afeta as partes contrastantes da imagem, como em que eamarelos e pele se encontram para criar uma área óbvia do contraste, e a própria pele suave. Até mesmo a capa mais sutil exibe alterações sutis nos valores de brilho. Se um valor de limite não for usado, o filtro acentuará essas alterações sutis em pixels de pele. Por sua vez, um efeito barulhento e indesejado é criado enquanto o contraste com as marcas de formatação aumenta, melhorando a nitidez.<br><br>Para evitar esse problema, é apresentado um valor de limite que informa ao filtro ignorar pixels que não mudam o contraste dramaticamente, como uma capa suave. <br><br>No gráfico zipper mostrado anteriormente, observe a textura ao lado dos zippers. O ruído da imagem é exibido porque os valores de limite eram muito baixos para suprimir o ruído. |
| Monocromático | Selecione para desvincular o brilho da imagem (intensidade).<br><br>Desmarque para desfazer a nitidez de cada componente de cor separadamente. |

Consulte [também Nitidez de uma imagem](sharpening-image.md#sharpening_an_image).

Consulte também [Como nitidez de imagens no Scene 7 Publishing System e no Servidor de imagens](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

**Plano de fundo de separação**

É possível usar o Plano de fundo de Separação para remover automaticamente o plano de fundo de uma imagem ao carregá-lo. Essa técnica é útil para chamar a atenção para um objeto específico e destacar a partir de um plano de fundo ocupado.

| Opções de plano de fundo knockout | Descrição |
|:--- |:--- |
| Plano de fundo de separação | Selecione para ativar ou «ativar» o recurso e as opções em segundo plano. |
| Canto | Obrigatório.<br><br>O canto da imagem usada para definir a cor do plano de fundo para separação.<br><br>Você pode escolher entre <b>Esquerda superior, Inferior esquerdo, Superior à direita ou Inferior à direita</b>. |
| Método de preenchimento | Obrigatório. <br><br>Controla a transparência de pixels a partir do local de canto definido.<br><br>É possível escolher entre os seguintes métodos de preenchimento: <ul><li><b>Preenchimento</b> de cheias - transforma todos os pixels transparentes que correspondem ao canto especificado e estão conectados a ele.</li><li><b>Corresponder pixel</b> - transforma todos os pixels correspondentes transparentes, independentemente da localização na imagem.</li></ul> |
| Tolerância | Opcional.<br><br>Controla a quantidade permitida de variação na correspondência de cores de pixels com base no local de canto definido.<br><br>Use um valor de 0.0 para corresponder a cores de pixel exatamente ou, use um valor de 1.0 para permitir a maior variação. |

>[!MORELIKETHIS]
>
>* [Recortar uma imagem](cropping-image.md#cropping_an_image)

