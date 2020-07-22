---
title: Como tornar uma imagem nítida
seo-title: Como tornar uma imagem nítida
description: nulo
seo-description: Saiba como aumentar a nitidez de uma imagem.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '2159'
ht-degree: 0%

---


# Como tornar uma imagem nítida {#sharpening-an-image}

O ajuste de nitidez é uma técnica de manipulação de imagens para tornar os contornos de uma imagem digital mais distintos. O ajuste de nitidez aumenta o contraste entre os pixels da borda e enfatiza a transição entre áreas escuras e claras. O ajuste de nitidez aumenta o contraste local e traz detalhes finos. Não há fórmula rigorosa para ajustar a nitidez de todas as imagens corretamente. Pouca nitidez pode ser suficiente para uma imagem suave, mas a nitidez excessiva adiciona halos, artefatos e ruídos.

O Dynamic Media Classic recomenda o uso de predefinições de imagens para todas as imagens. Isso garante um tamanho uniforme, e a nitidez é aplicada em qualquer imagem chamada com uma predefinição de imagem. Além disso, é possível editar e alterar os parâmetros de nitidez de uma predefinição de imagem com facilidade. Na próxima vez que você publicar, todas as imagens chamadas com essa predefinição receberão os novos valores.

O Dynamic Media Classic também recomenda adicionar nitidez às predefinições do visualizador e, em seguida, chamar um visualizador com essa predefinição. Isso garante que as imagens em seus visualizadores sejam nítidas e atraentes.

No entanto, se você usar as predefinições de imagens e as predefinições do visualizador ou algum método alternativo de nitidez, o resultado final é que você deve aumentar a nitidez das imagens. Caso contrário, suas imagens (e site) podem parecer suaves e indistintas.

>[!NOTE]
>
>Os comandos Nitidez substituem as configurações de Predefinição de imagem, incluindo seus efeitos de nitidez. Uma predefinição de imagem governa o tamanho e a formatação com os quais as imagens são entregues pelos servidores de imagem Dynamic Media. O Dynamic Media Classic recomenda usar as predefinições de imagens para fornecer todas as imagens, a fim de garantir que elas sejam entregues em tamanho e nitidez uniformes. Após as configurações de nitidez de uma imagem individual terem sido alteradas, no entanto, as configurações de nitidez da Predefinição de imagem não se aplicam mais à imagem. É entregue sem as configurações de nitidez da predefinição de imagem.

Muitas vezes, é necessário aumentar a nitidez das imagens. Servidores Dynamic Media Classic e Image ofertas várias opções de nitidez. É importante entender o que a nitidez faz a uma imagem e a intensidade de nitidez que você precisa. A maioria das imagens precisa de alguma nitidez, mas a quantidade necessária depende da imagem.

O ajuste da nitidez da imagem aumenta o contraste dos pixels para criar o efeito de bordas acentuadas. Os humanos percebem este contraste avançado de borda como nitidez. Embora seja fácil aprimorar uma imagem ao executar filtros de nitidez em uma imagem, também é fácil aumentar a nitidez de uma imagem.

A nitidez excessiva de uma imagem cria um efeito de halo ou uma faixa das linhas da borda.

Existem práticas recomendadas que você pode seguir para otimizar a nitidez de suas imagens no Dynamic Media Classic e no Dynamic Media Image Server.

Consulte Práticas [recomendadas para aumentar a nitidez de imagens no Dynamic Media Classic e no Dynamic Media Image Server](/help/assets/s7_sharpening_images.pdf).

**Para ajustar a nitidez de uma imagem**

Para ajustar a nitidez de uma imagem, clique no botão **Editar** de sobreposição e escolha Nitidez ou abra-a no Painel de navegação em visualização de detalhes e clique em **Nitidez**. A tela Editor de nitidez é aberta com comandos de nitidez. Escolha os comandos e clique em **Salvar**.

>[!NOTE]
>
>Antes de ajustar a nitidez de uma imagem, selecione o menu Aplicar predefinição e escolha uma predefinição de imagem para ver quais são os seus efeitos de nitidez. Os efeitos de nitidez de uma predefinição de imagem podem ser adequados para a sua imagem. O menu Aplicar predefinição está localizado na parte inferior da tela Editor de nitidez.

**Opções de nitidez**

A tabela a seguir mostra as opções de nitidez do Servidor de imagens.

| Nome | Protocolo de URL | Valores | Exemplo |
|--- |--- |--- |--- |
| Nitidez simples | op_sharpen | `0 | 1` | op_sharpen=1 |
| Modo de nova amostra | resMode | `bilin | bicub | sharp2 | trilin`<br><br>bilino: Seleciona a interpolação bi-linear padrão. Método de reamostragem mais rápido; alguns artefatos de aliasing podem ser perceptíveis.<br>bicub: Seleciona a interpolação bicúbica. Mais uso intenso da CPU do que o bilin, mas produz imagens mais nítidas com artefatos de aliasing menos visíveis.<br><br>afiado2: Seleciona uma função Lanczos Window modificada como um algoritmo de interpolação. Pode produzir resultados ligeiramente mais nítidos do que bi-cúbicos a um custo de CPU mais alto.<br><br>trilho: Seleciona uma interpolação trilinear modificada, que usa resoluções mais altas e mais baixas, se disponível. Recomendado somente quando a suavização de borda for um problema. Reduz os tamanhos de JPEG devido à redução dos dados de alta frequência. | resMode=shark2 |
| Tirar nitidez da máscara | op_usm | quantidade, raio, limiar,<br><br>monocromática: raio do fator de força do filtro (real 0.5.5)<br><br>Raio: raio do kernel do filtro em pixels (real 0...250) <br><br>limite: nível limiar de filtragem (int 0...255)<br><br>monocromático: definido como 0 para desfazer a máscara de nitidez de cada componente colorido separadamente, definido como 1 para desfazer o brilho da imagem da máscara de nitidez (intensidade) | op_usm=1,1,10,0 |

Selecione o menu Nitidez e escolha uma opção:

**Nenhum** Desativa a nitidez.

**Nitidez** Executa uma simples passagem de nitidez no arquivo depois que ele é redimensionado. Isso é semelhante ao filtro &quot;Nitidez&quot; no Photoshop e suporta qualquer parâmetro do usuário. Normalmente, você usaria esse filtro ou a Máscara de nitidez, mas não ambos. Como prática recomendada, esse método não é recomendado, mas pode ajudar a compensar o desfocamento. (URL: op_sharpen)

**Máscara** de nitidezPermite ajustar um efeito de filtro de nitidez na imagem final com resolução reduzida. É possível controlar a intensidade do efeito, o raio do efeito (medido em pixels) e um limite de contraste que será ignorado. Esse efeito usa as mesmas opções do filtro &quot;Tirar nitidez da máscara&quot; do Photoshop. (URL: op_usm)

Escolha estas opções para ajustar a nitidez com a máscara de nitidez:

**Quantidade** Controla a quantidade de contraste aplicada aos pixels da borda. O padrão é 0.0. Para imagens de alta resolução, é possível aumentá-las para até 5.0. Pense em Amount como uma medida da intensidade do filtro. Observe que a configuração Quantia no Dynamic Media Classic não é igual à configuração Quantia no Photoshop. O Photoshop usa uma quantidade no intervalo de 1% a 500%, enquanto o Dynamic Media Classic é dimensionado de 0,0 a 5,0. (5,0 equivale aproximadamente a 500% no Photoshop, 0,9 é semelhante a 90% e assim por diante).

**Raio** Determina o número de pixels em torno dos pixels da borda que afetam a nitidez. O efeito é executado em todos os pixels na imagem e irradia em todas as direções.

O melhor valor de raio depende do tamanho da imagem. Um valor baixo aplica nitidez somente aos pixels da borda. Um valor alto aumenta a nitidez de uma faixa maior de pixels.

Por exemplo, para obter um efeito de nitidez semelhante para uma imagem de 2000 x 2000 pixels e 500 x 500 pixels, você pode definir um valor de raio de dois pixels na imagem de 2000 x 2000 pixels. Em seguida, defina um valor de raio de um pixel na imagem de 500 x 500 pixels (um valor maior para uma imagem com mais pixels).

**Limiar** Determina o intervalo de contraste a ser ignorado quando o filtro de máscara de nitidez for aplicado. Essa opção determina o quão diferentes os pixels com nitidez devem ser da área ao redor antes que sejam considerados pixels de borda e sejam apontados.

O limite usa um valor de 0 a 255, que é o número de etapas de brilho em uma imagem em tons de cinza. 0=preto, 128=50% cinza e 255=branco. Por exemplo, um valor limite de 12 ignora variações leves é o brilho do tom de pele, para não adicionar ruído, enquanto adiciona o contraste da borda a áreas contrastantes, como onde as pestanas encontram a pele.

Por exemplo, suponha que você tenha uma foto do rosto de alguém. A Máscara de nitidez afeta as partes da imagem com mais contraste e a própria pele suave. Mesmo a pele mais suave exibe alterações sutis nos valores de brilho. Se você não usar um valor limite, o filtro acentua essas alterações sutis nos pixels da pele, criando um efeito ruidoso (provavelmente indesejável) e aumentando o contraste nas pestanas, aumentando a nitidez (provavelmente desejável). Para evitar esse problema, use um valor de limite que instrua o filtro a ignorar os pixels que não alteram o contraste drasticamente, como pele suave. Para evitar a introdução de ruído ou posterização — em imagens com tons de carne, por exemplo — tente experimentar com valores de Limite entre 2 e 20. O valor padrão de Limite de 0 aumenta a nitidez de todos os pixels na imagem.

**Aplicar para** escolher cada cor para aplicar a nitidez separadamente a cada componente de cor; escolha Brilho para aplicar à nitidez às áreas de brilho da imagem.

**Reamostragem**

Selecione o menu Reamostragem e escolha uma opção. Essas opções tornam a imagem nítida quando tem resolução reduzida:

**Nenhum** Desativa a reamostragem.

**Bilinear** O método de reamostragem mais rápido; alguns artefatos de aliasing são perceptíveis.

**Bicúbica** aumenta o uso da CPU no Servidor de imagens, mas produz imagens mais nítidas com artefatos de aliasing menos visíveis.

**O Sharpen2** pode produzir resultados ligeiramente mais nítidos do que a opção Bicúbica, mas a um custo de CPU ainda maior no Servidor de imagens.

**Trilinear** Usa resoluções mais altas e mais baixas, se disponíveis; recomendado somente quando a suavização de borda for um problema. Este método reduz o tamanho do JPEG devido à redução dos dados de alta frequência.

**Predefinições de nitidez e imagem**

Você pode combinar os três efeitos de nitidez para obter o resultado final. No entanto, isso não é recomendado. O Dynamic Media Classic recomenda que você salve seus efeitos de nitidez como parte de uma predefinição de imagem.As predefinições de imagem permitem que você empacote os modificadores de imagem usados com mais frequência para criar uma imagem dinamicamente redimensionada em uma pequena string de texto. Uma predefinição de imagem contém valores para o formato de arquivo (geralmente JPEG para a Web), contagem de pixels e nitidez da imagem. Em vez de anexar o URL a cada modificador de imagem necessário para criar um tipo específico de tamanho de imagem, crie uma predefinição de imagem nomeada, como &quot;miniatura&quot;, configure a predefinição de imagem em miniatura com o tamanho, o formato de arquivo e as opções de nitidez apropriados, e chame a imagem usando o nome Predefinição de imagem. As predefinições de imagem reduzem o comprimento do URL geral.Esses dois URLs produzem a mesma imagem JPEG 350x350 com nitidez:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

As predefinições de imagens podem ser alteradas e atualizadas a qualquer momento. Você verá os resultados de uma alteração em uma predefinição de imagem depois de publicar e depois que o cache do URL for limpo.

Se você usar uma predefinição para cada imagem em uma categoria de tamanho, qualquer administrador de Empresa poderá atualizar a definição dessa predefinição de imagem, republicar e afetar todas as imagens usando esse formato, sem alterar nenhum código da Web. Como prática recomendada, use uma predefinição de imagem por tamanho exclusivo no site. Para adicionar uma predefinição de imagem, vá até Configuração > Configurações do aplicativo > Predefinições de imagem. Em seguida, adicione ou edite uma predefinição existente. O único campo obrigatório é o nome da própria predefinição. No entanto, você deve incluir algum nível de nitidez em cada predefinição.

**Qualidade JPG**

As opções de Qualidade JPG controlam o nível de compactação JPG:

**Qualidade** JPG Selecione essa opção se quiser controlar os níveis de compactação e a redução da resolução de crominância.

**Controle deslizante** Determina o nível de compactação JPG. Essa configuração afeta o tamanho do arquivo e a qualidade da imagem. A escala de qualidade do JPG é 1-100.

**Ativar a Redução da resolução** do crominância JPG Devido ao olho ser menos sensível às informações de cores de alta frequência do que à luminância de alta frequência, as imagens JPEG dividem as informações da imagem em luminância e componentes de cor. Quando uma imagem JPEG é compactada, o componente de luminância é deixado em resolução completa, enquanto os componentes de cor têm resolução reduzida, fazendo a média em grupos de pixels. A diminuição da resolução reduz o volume de dados em metade ou um terço, com quase nenhum impacto na qualidade percebida. A redução da resolução não se aplica a imagens em tons de cinza. Essa técnica reduz a quantidade de compactação útil para imagens com alto contraste (por exemplo, imagens com texto sobreposto).

**Definição de opções de nitidez em toda a empresa**

Se você não usar uma predefinição de imagem ou aprovar protocolos específicos de nitidez do Servidor de imagens ao longo da string de URL, a imagem não será ajustada quando for reduzida. No entanto, você pode definir valores de nitidez padrão se isso ocorrer e, em seguida, qualquer imagem sempre terá alguma nitidez.

Para definir as opções de nitidez padrão da sua empresa, vá até Configuração > Configuração do aplicativo > Configuração de publicação > Servidor de imagens. Se você definir o Modo de reamostragem padrão como Sharp2, ele sempre apontará a imagem para nitidez ao diminuir a resolução.

**Adicionar nitidez às predefinições do visualizador**

A menos que você adicione modificadores de imagem de nitidez à predefinição, a pequena imagem de carregamento inicial pode parecer suave, pois a resolução é reduzida para caber na janela do visualizador sem ser ajustada.

No Dynamic Media Classic, as predefinições do visualizador (como as predefinições de imagem) permitem centralizar várias opções em um local, incluindo opções de capa e visualizador (como incluir um botão Imprimir ou controlar a velocidade da animação de zoom). As predefinições do visualizador são encontradas na mesma seção que as predefinições de imagem, em Configuração > Configurações do aplicativo > Predefinições do visualizador.

A opção Modificadores é encontrada na seção Principais configurações de todas as predefinições de eCatalog, Spin e Custom Zoom Viewer. Ao adicionar os comandos de ajuste de nitidez do URL à caixa Modificadores, adicione a nitidez sempre que o visualizador for chamado com essa predefinição do visualizador.

Para chamar a predefinição do visualizador, use o comando config= no URL do visualizador. Este é um exemplo de como chamar um conjunto de imagens (sapatos) com uma predefinição de visualizador (FantasticoZoom2009):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2009`

A predefinição aqui acentua e altera a capa padrão do visualizador.

**Criação de substituições específicas à imagem**

O último método de nitidez, e o menos recomendado, é criar substituições de nitidez com base em imagem por imagem. Isso substitui a nitidez em uma predefinição de imagem com seus próprios valores específicos. No entanto, isso substitui todos os outros métodos de nitidez em qualquer tamanho. O melhor caso de uso para esse método é se algumas de suas imagens não tiverem alta resolução e os valores nas Predefinições de imagem forem muito altos para essas pequenas imagens. Nesse caso, pode ser necessário ajustar a nitidez por imagem.

No Dynamic Media Classic, selecione qualquer imagem, vá para a Visualização Detalhe (clicando no duplo ou pressionando o botão Visualização Detalhe) e clique em Nitidez. Altere qualquer parâmetro e clique em Salvar. Isso instrui o Servidor de imagens a usar esses parâmetros de nitidez em vez de qualquer comando que você chamar no URL, como um modificador de nitidez ou uma predefinição de imagem. É necessário publicar para que as alterações entrem em vigor.
