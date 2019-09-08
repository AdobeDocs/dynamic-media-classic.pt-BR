---
title: Nitidez de uma imagem
seo-title: Nitidez de uma imagem
description: 'null'
seo-description: Saiba como tornar uma imagem nítida.
uuid: d 86 af 74 a -89 c 5-4 f 2 b -96 ba-f 2 e 7 da 600 bca
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/master_ files
discoiquuid: 11 cd 5362-d 90 a -4 c 1 e-bfbd -46 a 65 a 554409
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Nitidez de uma imagem {#sharpening-an-image}

A nitidez é uma técnica de manipulação de imagens para tornar os contornos de uma imagem digital mais distintos. A nitidez aumenta o contraste entre os pixels da borda e enfatiza a transição entre as áreas escuras e claras. A nitidez aumenta o contraste local e destaca os detalhes. Não há fórmula estrita para ajustar corretamente todas as imagens. Um pouco de nitidez pode ser feito para uma imagem suave, mas o aumento da nitidez adiciona halos, artefatos e ruídos.

O Dynamic Media Classic altamente recomenda o uso de Predefinições de imagens para todas as imagens. Isso garante um tamanho uniforme e a nitidez é imposta em qualquer imagem chamada com uma predefinição de imagem. Além disso, é possível editar e alterar os parâmetros de nitidez de uma predefinição de imagens com facilidade. Na próxima vez que você publicar, todas as imagens chamadas com essa predefinição receberão os novos valores.

O Dynamic Media Classic também recomenda adicionar nitidez às Predefinições do visualizador e, em seguida, chamar um visualizador com essa predefinição. Isso garante que as imagens dentro de seus visualizadores sejam nítidas e atraentes.

No entanto, se você usa Predefinições de imagens e Predefinições do visualizador, ou algum método alternativo de nitidez, a linha inferior é que você deve ajustar as suas imagens. Caso contrário, as imagens (e o site) serão parecidas com o modo de câmera suave e desligado.

>[!NOTE]
>
>Os comandos de Nitidez substituem as configurações de Predefinição de imagem, incluindo seus efeitos de nitidez. Uma predefinição de imagem rege o tamanho e a formatação com as quais as imagens são entregues dos servidores de imagem do Dynamic Media. O Dynamic Media Classic altamente recomenda o uso de predefinições de imagens para entregar todas as imagens para garantir que as imagens sejam entregues em um tamanho uniforme e em uma nitidez. Entretanto, após a alteração das configurações de nitidez de uma imagem individual, as configurações de nitidez Predefinidas de imagens não se aplicam mais à imagem. É entregue sem configurações de nitidez predefinidas de imagem.

Geralmente, é necessário ajustar as imagens. O Dynamic Media Classic SPS e servidores de imagem oferecem várias opções de nitidez. É importante entender o que a nitidez faz a uma imagem e quanta nitidez é necessária. A maioria das imagens precisa de nitidez, mas a quantidade necessária depende da imagem.

A nitidez da imagem aumenta o contraste dos pixels para criar o efeito de acentuar bordas. Os humanos percebem este contraste de borda aprimorado como nitidez. Embora seja fácil melhorar uma imagem ao executar filtros de nitidez em uma imagem, também é fácil aumentar a nitidez de uma imagem.

O aumento de nitidez de uma imagem cria um efeito de auro ou uma marca das linhas da borda.

Há práticas recomendadas que você pode seguir para otimizar a nitidez de suas imagens no Sistema de publicação Scene 7 e no Servidor de imagem do Dynamic Media.

Consulte [Práticas recomendadas para aumentar a nitidez de imagens no Sistema de publicação do Scene 7 e no Servidor de imagem do Dynamic Media](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

**Como tornar uma imagem nítida**

Para tornar uma imagem nítida, clique no botão **Editar** rolagem e escolha Nitidez ou abra-a no painel Procurar na exibição Detalhe e, em seguida, clique **em Nitidez**. A tela Editor de nitidez é aberta com comandos de nitidez. Escolha comandos e clique **em Salvar**.

>[!NOTE]
>
>Antes de ajustar a nitidez de uma imagem, você pode selecionar o menu Aplicar predefinição e escolher uma Predefinição de imagem para ver quais são os efeitos de nitidez. Os efeitos de nitidez de uma predefinição de imagem podem ser adequados para a imagem. O menu Aplicar predefinição está localizado na parte inferior da tela Editor de nitidez.

**Opções de nitidez**

A tabela a seguir mostra as opções de nitidez do Servidor de imagens.

| Nome | Protocolo URL | Valores | Exemplo |
|--- |--- |--- |--- |
| Nitidez simples | op_ sharpen | `0 | 1` | op_ sharpen = 1 |
| Modo de reamostragem | Remode | `bilin | bicub | sharp2 | trilin`<br><br>faturamento: Seleciona a interpolação bi-linear padrão. Método de redefinição mais rápida; alguns artefatos de alfinização podem ser percebidos.<br>bicub: Seleciona a interpolação bi-cuic. Mais CPU com maior consumo de CPU, mas produz imagens mais nítidas com artefatos de alias menos visíveis.<br><br>sharp 2: Seleciona uma função de Janela do Chatzos modificada como um algoritmo de interpolação. Pode produzir resultados ligeiramente mais nítidos do que bi-cuic a um custo maior da CPU.<br><br>trilha: Seleciona uma interpolação trilinear modificada, que utiliza resoluções maiores e mais baixas, se disponível. Recomendado apenas quando a alçăo é um problema. Reduz tamanhos de JPEG devido a dados de alta frequência reduzida. | Remode = sharp 2 |
| Tirar nitidez da máscara | op_ usm | quantidade, raio, limite, monocromequantia<br><br>: fator de força de filtro (real 0… 5)<br><br>: raio do núcleo de núcleo em pixels (real 0… 250) <br><br>: nível de limite de filtro (int 0… 255)<br><br>monocromática: definido como 0 para desfazer a nitidez de cada componente de cor separadamente, definido como 1 para liberar brilho da imagem (intensidade) | op_ usm = 1,1,10,0 |

Selecione o menu de Nitidez e escolha uma opção:

**Nenhum** desativa a nitidez.

**A Nitidez** executa uma passagem de nitidez simples no arquivo depois de ser redimensionada. Isso é semelhante ao filtro «Nitidez» no Photoshop e oferece suporte para quaisquer parâmetros de usuário. Normalmente, você usaria esse filtro ou Tirar nitidez da máscara, mas não ambos. Como prática recomendada, esse método não é recomendado, mas pode ajudar a compensar o desfoque. (URL: op_ sharpen)

**Máscara de Nitidez** Permite ajustar um efeito de filtro de nitidez na imagem final de resolução reduzida. É possível controlar a intensidade do efeito, raio do efeito (medido em pixels) e um limite de contraste que será ignorado. Esse efeito usa as mesmas opções que o filtro «Unsharp Mask» do Photoshop. (URL: op_ usm)

Escolha essas opções para ajustar nitidez com Máscara de nitidez:

**Amount** Controla a quantidade de contraste aplicada aos pixels da borda. O padrão é 0.0. Para imagens de alta resolução, é possível aumentá-la até 5.0. Pense em Amount como uma medida da intensidade do filtro. Observe que a configuração Quantia no Dynamic Media Classic não é igual à configuração Quantia no Photoshop. O Photoshop usa um valor no intervalo de 1% a 500%, enquanto o Dynamic Media Classic escala de 0.0 a 5.0. (5.0 equivale aproximadamente a 500% no Photoshop, 0.9 é semelhante a 90% e assim por diante.)

**Raio** Determina o número de pixels em torno dos pixels da borda que afetam a nitidez. O efeito é executado em todos os pixels da imagem e radiates em todas as direções.

O melhor valor do raio depende do tamanho da imagem. Um valor baixo aplica nitidez apenas aos pixels da borda. Um valor alto comprime uma banda maior de pixels.

Por exemplo, para obter um efeito de nitidez semelhante para uma imagem de 2000 x 2000 pixels e imagens de 500 x 500 pixels, você pode definir um valor de raio de dois pixels na imagem de 2000 x 2000 pixels. Em seguida, defina um valor de raio de um pixel na imagem de 500 x 500 pixels (um valor maior para uma imagem com mais pixels).

**Threshold** Determina o intervalo de contraste a ser ignorado quando o filtro de máscara de nitidez é aplicado. Essa opção determina como os pixels com nitidez devem ser provenientes da área circundante antes que sejam considerados pixels de borda e fiquem nítidos.

O limite usa um valor de 0-255, que é o número de etapas de brilho em uma imagem em tons de cinza. 0 = preto, 128 = 50% cinza e 255 = branco. Por exemplo, um valor limite de 12 ignora pequenas variações que são brilho de tom de pele, a fim de não adicionar ruído, ao mesmo tempo que adiciona contraste de borda a áreas contrastantes, como quando as eamarelações atendem a capa.

Por exemplo, suponha que você tenha uma foto de rosto de alguém. A Máscara de nitidez afeta as partes da imagem com o maior contraste e a própria pele suave. Até mesmo a capa mais sutil exibe alterações sutis nos valores de brilho. Se um valor de limiar não for usado, o filtro acentuará essas alterações sutis em pixels de pele, criando um efeito barulhento (provavelmente indesejável) e aumentando o contraste das marcas de formatação, melhorando a nitidez (provavelmente desejável). Para evitar esse problema, use um valor limite que informe ao filtro ignorar pixels que não mudam o contraste dramaticamente, como uma pele suave. Para evitar a introdução de ruído ou posterização—em imagens com tons granulados, por exemplo—experimente fazer testes com valores limite entre 2 e 20. O valor Limite padrão de 0 compara todos os pixels na imagem.

**Aplicar para** escolher cada cor para aplicar nitidez separadamente a cada componente de cor; escolha Brilho a ser aplicado à nitidez das áreas de brilho de imagem.

**Reamostrando**

Selecione o menu Reamostrando e escolha uma opção. Essas opções tornam a imagem nítida quando ela é reduzida:

**Nenhum** Desativa a redefinição.

**Bilinear** O método de reamostragem mais rápido; alguns artefatos de alfinização são visíveis.

**A bicúbica** aumenta o uso da CPU no Servidor de imagens, mas produz imagens mais nítidas com artefatos de alias menos visíveis.

**A Nitidez 2** pode produzir resultados ligeiramente mais nítidos do que a opção Bicúbica, mas com um custo de CPU ainda maior no Servidor de imagens.

**Trilinear** Usa resoluções tanto maiores quanto mais baixas se disponível; recomendado apenas quando a alçăo é um problema. Esse método reduz o tamanho do JPEG devido a dados reduzidos de alta frequência.

**Predefinições de nitidez e imagens**

Você pode combinar os três efeitos de nitidez para atingir o resultado final. No entanto, isso não é recomendado. O Dynamic Media Classic recomenda salvar seus efeitos de nitidez como parte de uma Predefinição de imagem. As predefinições de imagens permitem disponibilizar os modificadores de imagem usados com mais frequência para criar uma imagem redimensionada dinamicamente em uma pequena string de texto. Uma predefinição de imagem contém valores para o formato de arquivo (geralmente JPEG para a Web), contagem de pixels e nitidez de imagens. Em vez de anexar o URL com cada modificador de imagem necessário para criar um tipo específico de tamanho de imagem, você cria uma Predefinição de imagem nomeada, como «miniatura», configura a predefinição de imagem em miniatura com o tamanho apropriado, o formato do arquivo e as opções de nitidez e, em seguida, chama a imagem usando o nome Predefinido de imagem. As predefinições de imagens reduzem o comprimento do URL geral. Esses dois urls produzem a mesma imagem JPEG de 350 x 350 com nitidez:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

As predefinições de imagens podem ser alteradas e atualizadas a qualquer momento. Você verá os resultados de uma alteração em uma Predefinição de imagem depois de publicar e depois que o cache do URL for limpo.

Se você usar uma predefinição para cada imagem em uma categoria de tamanho, qualquer Administrador de empresa poderá atualizar a definição dessa predefinição de imagem, publicar novamente e afetar cada imagem usando esse formato, sem alterar nenhum código da Web. Como prática recomendada, use uma predefinição de imagem por tamanho exclusivo no site. Para adicionar uma predefinição de imagens, vá até Configuração &gt; Configurações do aplicativo &gt; Predefinições de imagens. Em seguida, adicione ou edite uma predefinição existente. O único campo obrigatório é o nome da predefinição propriamente dita. No entanto, você deve incluir um certo nível de nitidez em cada predefinido.

**Qualidade JPG**

As opções de Qualidade JPG controlam o nível de compactação JPG:

**Qualidade JPG** Selecione essa opção se desejar controlar os níveis de compactação e a redução de crominância.

**Controle deslizante** Determina o nível de compactação JPG. Essa configuração afeta o tamanho do arquivo e a qualidade da imagem. A escala de qualidade JPG é de 1-100.

**Ativar a redução de** crominância JPG, pois o olho é menos sensível às informações de cores de alta frequência do que a luminância de alta frequência, as imagens JPEG dividem informações da imagem em componentes de luminância e cor. Quando uma imagem JPEG é compactada, o componente de luminância é deixado em resolução total, enquanto os componentes de cor são reduzidos pela média de grupos de pixels. A redução da resolução reduz o volume de dados em metade ou um terço sem nenhum impacto sobre a qualidade percebida. A diminuição da resolução não é aplicável a imagens em tons de cinza. Essa técnica reduz a quantidade de compressão útil para imagens com alto contraste (por exemplo, imagens com texto sobreposto).

**Definição de opções de nitidez em toda a empresa**

Se você não usar uma Predefinição de imagem ou passar protocolos de nitidez do Servidor de imagens específicos ao longo da string de URL, a imagem não será nitidez quando for reduzida. No entanto, você pode definir valores de nitidez padrão se isso ocorrer e, em seguida, qualquer imagem sempre terá alguma nitidez.

Para definir as opções de nitidez padrão da empresa, vá para Configuração &gt; Configuração do aplicativo &gt; Configuração de publicação &gt; Servidor de imagens. Se você definir o Modo de reamostragem padrão como Sharp 2, sempre aumentará a nitidez da imagem durante a diminuição da resolução.

**Adicionar nitidez às predefinições do visualizador**

A menos que você adicione modificadores de imagem de nitidez à predefinição, a pequena imagem de carregamento inicial pode parecer suave, pois é reduzida para caber na janela do visualizador sem ser nitidez.

No SPS, Predefinições do visualizador (como Predefinições de imagens) permitem centralizar várias opções em um local, incluindo opções de opções de capa e visualizador (como incluir um botão Imprimir ou controlar a velocidade da animação de zoom). As predefinições do visualizador são encontradas na mesma seção que as Predefinições de imagens, em Configuração &gt; Configurações do aplicativo &gt; Predefinições do visualizador.

A opção Modificadores é encontrada na seção Configurações principais de todas as predefinições do ecatalog, Spin e Custom Zoom Viewer. Ao adicionar os comandos de nitidez de URL na caixa Modificadores, você adiciona nitidez toda vez que o visualizador é chamado com essa predefinição do visualizador.

Para chamar a Predefinição do visualizador, use o comando config = no URL do visualizador. Este é um exemplo de chamada de um Conjunto de imagens (sapatos) com uma Predefinição do visualizador (fantasticozoom 2009):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2009`

A predefinição aqui é compartilhada e altera a capa padrão do visualizador.

**Criar substituições específicas de imagem**

O método de nitidez mais recente e recomendado é criar substituições de nitidez em imagem por imagem. Isso substitui a nitidez em uma predefinição de imagem por seus próprios valores específicos. No entanto, isso substitui todos os outros métodos de nitidez de qualquer tamanho. O melhor caso de uso para este método é se algumas de suas imagens não forem alta resolução, e os valores nas Predefinições de imagens são muito altos para essas pequenas imagens. Nesse caso, alguns ajustes por imagem podem ser necessários.

No SPS, selecione qualquer imagem, vá para a Exibição de detalhes (clicando duas vezes ou pressionando o botão Exibição de detalhes) e clique em Nitidez. Altere qualquer parâmetro e clique em Salvar. Isso instrui o Servidor de imagens a usar esses parâmetros de nitidez em vez de qualquer comando que você chamar no URL, como um modificador de nitidez ou predefinição de imagem. É necessário publicar para ver as alterações aplicadas.
