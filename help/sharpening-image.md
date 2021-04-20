---
title: Nitidez de uma imagem
description: Saiba como ajustar a nitidez de uma imagem.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '2162'
ht-degree: 0%

---


# Nitidez de uma imagem {#sharpening-an-image}

A nitidez é uma técnica de manipulação de imagem para tornar os contornos de uma imagem digital mais distintos. A nitidez aumenta o contraste entre pixels de borda e enfatiza a transição entre áreas escuras e claras. A nitidez aumenta o contraste local e traz detalhes. Não há fórmula estrita para ajustar a nitidez correta de todas as imagens. Muito pouca nitidez pode fazer com uma imagem suave, mas a nitidez excessiva adiciona halos, artefatos e ruídos.

O Dynamic Media Classic recomenda usar Predefinições de imagem para todas as imagens. Isso garante um tamanho uniforme, e a nitidez é aplicada em qualquer imagem chamada com uma predefinição de imagem. Além disso, você pode editar e alterar facilmente os parâmetros de nitidez de uma predefinição de imagem. Na próxima vez que você publicar, todas as imagens chamadas com essa predefinição receberão os novos valores.

O Dynamic Media Classic também recomenda adicionar nitidez às Predefinições do visualizador e, em seguida, chamar um visualizador com essa predefinição. Isso garante que as imagens em seus visualizadores sejam nítidas e atraentes.

No entanto, se você usar Predefinições de imagem e Predefinições do visualizador ou algum método alternativo de nitidez, a conclusão é que você deve tornar suas imagens mais nítidas. Caso contrário, suas imagens (e seu site) podem parecer suaves e difusas.

>[!NOTE]
>
>Os comandos Nitidez substituem as configurações da Predefinição de imagem, incluindo seus efeitos de nitidez. Uma predefinição de imagem governa o tamanho e a formatação com que as imagens são entregues dos servidores de imagem da Dynamic Media. O Dynamic Media Classic recomenda o uso de predefinições de imagens para fornecer todas as imagens, para garantir que elas sejam entregues em um tamanho e nitidez uniformes. Depois que as configurações de nitidez de uma imagem individual forem alteradas, no entanto, as configurações de nitidez da Predefinição de imagem não se aplicarão mais à imagem. Ele é entregue sem as configurações de nitidez da predefinição de imagem.

Geralmente é necessário ajustar a nitidez das imagens. Os Servidores Dynamic Media Classic e Image oferecem várias opções de nitidez. É importante entender o que a nitidez faz em uma imagem e a nitidez necessária. A maioria das imagens precisa de alguma nitidez, mas a quantidade necessária depende da imagem.

A nitidez da imagem aumenta o contraste dos pixels para criar o efeito de acentuar as bordas. Os seres humanos percebem este contraste de borda melhorado como nitidez. Embora seja fácil aprimorar uma imagem executando filtros de nitidez em uma imagem, também é fácil tornar uma imagem mais nítida.

Acima da nitidez de uma imagem cria um efeito de halo ou faixas das linhas da borda.

Há práticas recomendadas que você pode seguir para otimizar a nitidez de suas imagens no Dynamic Media Classic e no Dynamic Media Image Server.

Consulte [Práticas recomendadas para nitidez de imagens no Dynamic Media Classic e no Dynamic Media Image Server](/help/assets/s7_sharpening_images.pdf).

**Para ajustar a nitidez de uma imagem**

Para ajustar a nitidez de uma imagem, clique no botão **Editar** e escolha Nitidez ou abra-a no Painel de navegação na exibição Detalhes e, em seguida, clique em **Nitidez**. A tela Editor de nitidez é aberta com comandos de nitidez. Escolha comandos e clique em **Save**.

>[!NOTE]
>
>Antes de ajustar a nitidez de uma imagem, selecione o menu Aplicar predefinição e escolha uma predefinição de imagem para ver quais são os seus efeitos de nitidez. Os efeitos de nitidez de uma predefinição de imagem podem ser adequados para a sua imagem. O menu Aplicar predefinição está localizado na parte inferior da tela Editor de nitidez.

**Opções de nitidez**

A tabela a seguir mostra as opções de nitidez do Servidor de imagem.

| Nome | Protocolo de URL | Valores | Exemplo |
|--- |--- |--- |--- |
| Nitidez simples | op_sharpen | `0 | 1` | op_sharpen=1 |
| Modo de reamostra | resMode | `bilin | bicub | sharp2 | trilin`<br><br>bilino: Seleciona a interpolação bi-linear padrão. Método de reamostragem mais rápido; alguns artefatos de aliasing podem ser perceptíveis.<br>bicub: Seleciona a interpolação bicúbica. Mais uso de CPU do que bilin, mas produz imagens mais nítidas com artefatos de aliasing menos perceptíveis.<br><br>afiado2: Seleciona uma função modificada da Janela Lanczos como um algoritmo de interpolação. Pode produzir resultados ligeiramente mais nítidos do que bi-cúbicos a um custo de CPU mais alto.<br><br>trilho: Seleciona uma interpolação trilinear modificada, que usa resoluções mais altas e mais baixas, se disponível. Recomendado somente quando a aliasing é um problema. Reduz os tamanhos de JPEG devido à redução dos dados de alta frequência. | resMode=shark2 |
| Tirar nitidez da máscara | op_usm | quantidade, raio, limite, monocromático<br><br>quantia: fator de força do filtro (real 0...5)<br><br>raio: raio do kernel do filtro em pixels (real 0...250) <br><br>limite: nível de limite de filtro (int 0...255)<br><br>monocromático: defina para 0 para desfazer a nitidez da máscara de cada componente de cor separadamente, defina para 1 para desfazer a nitidez da imagem da máscara de nitidez (intensidade) | op_usm=1,1,10,0 |

Selecione o menu Nitidez e escolha uma opção:

**** NoneDesativa a nitidez.

**** NitidezExecuta uma simples passagem de nitidez no arquivo depois de ser redimensionado. É semelhante ao filtro &quot;Nitidez&quot; no Photoshop e suporta qualquer parâmetro de usuário. Normalmente, você usaria esse filtro ou Tirar nitidez da máscara, mas não ambos. Como prática recomendada, esse método não é recomendado, mas pode ajudar a compensar a indefinição. (URL: op_sharpen)

**Tirar nitidez da** máscaraPermite ajustar um efeito de filtro de nitidez na imagem final com resolução reduzida. Você pode controlar a intensidade do efeito, o raio do efeito (medido em pixels) e um limite de contraste que será ignorado. Esse efeito usa as mesmas opções do filtro &quot;Tirar nitidez da máscara&quot; do Photoshop. (URL: op_usm)

Escolha estas opções para ajustar a nitidez com Tirar nitidez da máscara:

**** AmountControla a quantidade de contraste aplicado aos pixels da borda. O padrão é 0,0. Para imagens de alta resolução, você pode aumentá-lo até 5,0. Considere Quantia como uma medida de intensidade de filtro. Esteja ciente de que a configuração Valor no Dynamic Media Classic não é a mesma que a configuração Valor no Photoshop. O Photoshop usa uma quantidade no intervalo de 1% a 500%, enquanto o Dynamic Media Classic é dimensionado de 0,0 para 5,0. (5.0 equivale aproximadamente a 500% no Photoshop, 0.9 é semelhante a 90% e assim por diante.)

**** RaioDetermina o número de pixels ao redor dos pixels da borda que afetam a nitidez. O efeito é executado em todos os pixels na imagem e irradia em todas as direções.

O melhor valor de raio depende do tamanho da imagem. Um valor baixo ajuste a nitidez apenas dos pixels da borda. Um valor alto ajuste a nitidez de uma faixa maior de pixels.

Por exemplo, para obter um efeito de nitidez semelhante para uma imagem de 2000 x 2000 pixels e imagem de 500x 500 pixels, você pode definir um valor de raio de dois pixels na imagem de 2000 x 2000 pixels. Em seguida, defina um valor de raio de um pixel na imagem de 500 x 500 pixels (um valor maior para uma imagem com mais pixels).

**** LimiteDetermina o intervalo de contraste a ser ignorado quando o filtro de máscara de nitidez for aplicado. Essa opção determina como deve ser a diferença dos pixels com nitidez em relação à área ao redor antes de serem considerados pixels de borda e terem nitidez.

O limite usa um valor de 0 a 255, que é o número de etapas de brilho em uma imagem em tons de cinza. 0=preto, 128=50% cinza e 255=branco. Por exemplo, um valor limite de 12 ignora pequenas variações é o brilho do tom da pele, para não adicionar ruído, enquanto ainda adiciona o contraste da borda a áreas contrastantes, como onde as pálpebras tocam a pele.

Por exemplo, suponha que você tenha uma foto do rosto de alguém. A Tirar nitidez da máscara afeta as partes da imagem com mais contraste e a própria pele lisa. Mesmo a pele mais suave apresenta alterações sutis nos valores de brilho. Se você não usar um valor de limite, o filtro acentua essas sutis alterações em pixels da pele, criando um efeito ruidoso (provavelmente indesejável), além de aumentar o contraste nas pálpebras, melhorando a nitidez (provavelmente desejável). Para evitar esse problema, use um valor de limite que instrua o filtro a ignorar os pixels que não alteram o contraste drasticamente, como pele lisa. Para evitar a introdução de ruído ou posterização, em imagens com tons de carne, por exemplo, tente experimentar com os valores de Limite entre 2 e 20. O valor padrão de Limite de 0 ajuste a nitidez de todos os pixels na imagem.

**Aplicar** aEscolha de cada cor para aplicar a nitidez separadamente a cada componente de cor; escolha Brightness (Brilho) para aplicar a nitidez às áreas de brilho da imagem.

**Reamostragem**

Selecione o menu Reamostragem e escolha uma opção. Essas opções aprimoram a imagem quando ela é reduzida:

**** NoneDesativa a redefinição de amostra.

**** BilinearO método de reamostragem mais rápido; alguns artefatos de aliasing são perceptíveis.

**** Bicicleta Aumenta o uso da CPU no Servidor de Imagem, mas produz imagens mais nítidas com artefatos de aliasing menos perceptíveis.

**O Sharpen2** pode produzir resultados ligeiramente mais nítidos do que a opção Bicúbica, mas a um custo de CPU ainda maior no Servidor de imagem.

**** TrilinearUsa resoluções mais altas e mais baixas, se disponível; recomendado somente quando aliasing for um problema. Este método reduz o tamanho do JPEG devido à redução dos dados de alta frequência.

**Nitidez e predefinições de imagens**

Você pode combinar os três efeitos de nitidez para obter o resultado final. No entanto, isso não é recomendado. O Dynamic Media Classic recomenda que você salve seus efeitos de nitidez como parte de uma predefinição de imagem. As predefinições de imagem permitem agrupar os modificadores de imagem usados com mais frequência para criar uma imagem dinamicamente redimensionada em uma pequena string de texto. Uma predefinição de imagem contém valores para o formato de arquivo (geralmente JPEG para a Web), contagem de pixels e nitidez da imagem. Em vez de anexar o URL a cada modificador de imagem necessário para criar um tipo específico de tamanho de imagem, crie uma Predefinição de imagem chamada, como &quot;miniatura&quot;, configure a Predefinição de imagem em miniatura com o tamanho, o formato de arquivo e as opções de nitidez apropriados e chame a imagem usando o nome da Predefinição de imagem. As predefinições de imagem reduzem o comprimento do URL geral. Esses dois URLs produzem a mesma imagem JPEG 350x350 com nitidez:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

As predefinições da imagem podem ser alteradas e atualizadas a qualquer momento. Você verá os resultados de uma alteração em uma predefinição de imagem depois de publicar e depois que o cache do URL limpar.

Se você usar uma predefinição para cada imagem em uma categoria de tamanho, qualquer Administrador da empresa poderá atualizar a definição dessa Predefinição de imagem, republicar e afetar todas as imagens usando esse formato, sem alterar nenhum código da Web. Como prática recomendada, use uma Predefinição de imagem por tamanho exclusivo em seu site. Para adicionar uma predefinição de imagem, vá para Configuração > Configurações do aplicativo > Predefinições de imagem. Em seguida, Adicione ou edite uma predefinição existente. O único campo obrigatório é o nome da própria predefinição. No entanto, você deve incluir algum nível de nitidez em cada predefinição.

**Qualidade JPG**

As opções de Qualidade JPG controlam o nível de compactação JPG:

**Qualidade** JPGSelecione essa opção se quiser controlar níveis de compactação e redução da amostragem de crominância.

**** Controle deslizanteDetermina o nível de compactação JPG. Essa configuração afeta o tamanho do arquivo e a qualidade da imagem. A escala de qualidade JPG é de 1 a 100.

**Ativar** Redução do Chrominance JPGComo o olho é menos sensível às informações de cores de alta frequência do que à luminância de alta frequência, as imagens JPEG dividem as informações da imagem em elementos de luminância e cor. Quando uma imagem JPEG é compactada, o componente de luminância é deixado em resolução completa, enquanto os componentes de cor são reduzidos pela média de grupos de pixels. A redução da amostragem reduz o volume de dados em um terço ou metade, quase sem impacto na qualidade percebida. A redução da amostragem não é aplicável a imagens em tons de cinza. Essa técnica reduz a quantidade de compactação útil para imagens com alto contraste (por exemplo, imagens com texto sobreposto).

**Configuração das opções de nitidez em toda a empresa**

Se você não usar uma Predefinição de imagem ou transmitir protocolos de nitidez específicos do Servidor de imagem ao longo da string de URL, a imagem não será dimensionada com nitidez quando for reduzida. No entanto, você pode definir valores de nitidez padrão se isso ocorrer e qualquer imagem sempre terá alguma nitidez.

Para definir as opções de nitidez padrão da sua empresa, vá até Configuração > Configuração do aplicativo > Configuração de publicação > Servidor de imagem. Se você definir o Modo de amostragem padrão como Sharp2, ele sempre aprimorará a imagem durante a resolução.

**Adição de nitidez às predefinições do visualizador**

A menos que você adicione modificadores de imagem de nitidez à predefinição, a pequena imagem de carregamento inicial pode parecer suave, pois a resolução é reduzida para caber na janela do visualizador sem ser nitidez.

No Dynamic Media Classic, as Predefinições do visualizador (como Predefinições de imagem) permitem centralizar várias opções em um local, incluindo opções de capa e do visualizador (como incluir um botão Imprimir ou controlar a velocidade da animação de zoom). As Predefinições do visualizador são encontradas na mesma seção que as Predefinições de imagem, em Configurar > Configurações do aplicativo > Predefinições do visualizador.

A opção Modificadores é encontrada na seção Configurações principais de todas as predefinições do eCatalog, rotação e do visualizador de zoom personalizado. Ao adicionar os comandos de nitidez do URL à caixa Modificadores, adicione a nitidez sempre que o visualizador for chamado com essa predefinição do visualizador.

Para chamar a Predefinição do visualizador, use o comando config= no URL do visualizador. Este é um exemplo de chamada de um Conjunto de imagens (sapatos) com uma Predefinição do visualizador (FantasticoZoom2009):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2009`

A predefinição aqui ajuste a nitidez e altera a pele padrão do visualizador.

**Criação de substituições específicas da imagem**

O último método de nitidez, e o menos recomendado, é criar substituições de nitidez em uma base imagem por imagem. Isso substitui a nitidez em uma predefinição de imagem com seus próprios valores específicos. No entanto, isso substitui todos os outros métodos de nitidez em qualquer tamanho. O melhor caso de uso para esse método é se algumas de suas imagens não tiverem alta resolução e os valores nas Predefinições de imagem forem altos demais para essas imagens pequenas. Nesse caso, pode ser necessário aumentar a nitidez por imagem.

No Dynamic Media Classic, selecione qualquer imagem, vá para a Exibição de detalhes (clicando duas vezes ou pressionando o botão Exibição de detalhes) e clique em Nitidez. Altere qualquer parâmetro e clique em Salvar. Isso instrui o Servidor de imagem a usar esses parâmetros de nitidez em vez de qualquer comando que você chamar no URL, como um modificador de nitidez ou Predefinição de imagem. Você deve publicar para ver as alterações entrarem em vigor.
