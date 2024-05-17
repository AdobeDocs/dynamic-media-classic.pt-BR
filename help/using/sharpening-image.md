---
title: Nitidez de uma imagem
description: Saiba como ajustar a nitidez de uma imagem no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '2163'
ht-degree: 0%

---

# Nitidez de uma imagem {#sharpening-an-image}

A nitidez é uma técnica de manipulação de imagem usada para tornar os contornos de uma imagem digital mais distintos. A nitidez aumenta o contraste entre os pixels da borda e enfatiza a transição entre áreas escuras e claras. A nitidez aumenta o contraste local e realça detalhes refinados. Não há nenhuma fórmula rígida para a nitidez correta de todas as imagens. A nitidez muito pequena pode gerar uma imagem suave, mas a nitidez excessiva adiciona halos, artefatos e ruídos.

A Adobe Dynamic Media Classic recomenda usar Predefinições de imagem para todas as imagens. Elas garantem um tamanho uniforme e a nitidez é aplicada em qualquer imagem chamada com uma Predefinição de imagem. Além disso, é possível editar e alterar facilmente os parâmetros de nitidez de uma Predefinição de imagem. Na próxima vez que você publicar, todas as imagens chamadas com essa predefinição receberão os novos valores.

A Adobe Dynamic Media Classic também recomenda adicionar nitidez às Predefinições do visualizador e, em seguida, chamar um visualizador com essa predefinição. Isso garante que as imagens dos visualizadores sejam nítidas e atraentes.

No entanto, se você usar Predefinições de imagem e Predefinições do visualizador ou algum método de nitidez, o resultado final é que você deve tornar as imagens mais nítidas. Caso contrário, suas imagens (e site) podem parecer suaves e difusas.

>[!NOTE]
>
>Os comandos Nitidez substituem as configurações de Predefinição de imagem, incluindo seus efeitos de nitidez. Uma Predefinição de imagem controla o tamanho e a formatação com que as imagens são entregues dos Servidores de imagem da Dynamic Media. A Adobe Dynamic Media Classic recomenda o uso de Predefinições de imagem para fornecer todas as imagens, garantindo que elas sejam entregues com tamanho e nitidez uniformes. Depois que as configurações de nitidez de uma imagem individual forem alteradas, as configurações de nitidez da Predefinição de imagem não serão mais aplicadas à imagem. Ele é fornecido sem as configurações de nitidez da Predefinição de imagem.

Muitas vezes, é necessário ajustar a nitidez das imagens. O Adobe Dynamic Media Classic e os servidores de imagem oferecem várias opções de nitidez. É importante entender o que a nitidez faz em uma imagem e a intensidade de nitidez necessária. A maioria das imagens precisa de nitidez, mas a quantidade necessária depende da imagem.

A nitidez da imagem aumenta o contraste dos pixels para criar o efeito de bordas acentuadas. Os seres humanos percebem esse contraste avançado de bordas como nitidez. Embora seja fácil aprimorar uma imagem executando filtros de nitidez em uma imagem, também é fácil aumentar a nitidez de uma imagem.

A nitidez excessiva de uma imagem cria um efeito de halo ou banda das linhas da borda.

Há práticas recomendadas que você pode seguir para otimizar a nitidez das imagens no Adobe Dynamic Media Classic e no Dynamic Media Image Server.

Consulte [Práticas recomendadas para nitidez de imagens no Adobe Dynamic Media Classic e no Dynamic Media Image Server](/help/using/assets/s7_sharpening_images.pdf).

Consulte também [Nitidez](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) vídeo de treinamento.

**Para ajustar a nitidez de uma imagem:**

Para ajustar a nitidez de uma imagem, selecione sua sobreposição **[!UICONTROL Edit]** e escolha **[!UICONTROL Sharpen]**, ou abra-o no painel Procurar na Exibição de detalhes e, em seguida, selecione **[!UICONTROL Sharpen]**. A página Editor de nitidez é aberta com comandos de nitidez. Escolha os comandos desejados e clique em **[!UICONTROL Save]**.

>[!NOTE]
>
>Antes de ajustar a nitidez de uma imagem, selecione o menu Aplicar predefinição e escolha uma Predefinição de imagem para ver quais são seus efeitos de nitidez. Os efeitos de nitidez de uma Predefinição de imagem são adequados para a sua imagem. A variável **[!UICONTROL Apply Preset]** está na parte inferior da página do Editor de nitidez.

**Opções de nitidez**

A tabela a seguir mostra as opções de nitidez do Servidor de imagens.

| Nome | Protocolo de URL | Valores | Exemplo |
| --- | --- | --- | --- |
| Nitidez simples | `op_sharpen` | `0` ou `1` | `op_sharpen=1` |
| Modo de reamostragem | `resMode` | `bilin`, `bicub`, `sharp2`, `trilin`<br><br>`bilin`: seleciona a interpolação bilinear padrão. Método de reamostragem mais rápido; alguns artefatos de suavização são geralmente visíveis.<br>`bicub`: seleciona a interpolação bi-cúbica. Maior uso intenso da CPU do que `bilin`, mas produz imagens mais nítidas com menos artefatos de suavização visíveis.<br><br>`sharp2`: seleciona uma função do Windows® Lanczos modificada como um algoritmo de interpolação. Ele pode produzir resultados ligeiramente mais nítidos do que o bi-cúbico a um custo de CPU mais alto.<br><br>`trilin`: seleciona uma interpolação trilinear modificada, que usa resoluções mais altas e mais baixas, se disponíveis. Recomendado somente quando o alias for um problema. Reduz os tamanhos de JPEG devido à redução dos dados de alta frequência. | `resMode=sharp2` |
| Tirar nitidez da máscara | `op_usm` | `amount`, `radius`, `threshold`, `monochrome`<br><br>`amount`: fator de resistência do filtro (real 0 a 5)<br><br>`radius`: raio do kernel do filtro em pixels (0 a 250 reais) <br><br>`threshold`: nível limite do filtro (int 0...255)<br><br>`monochrome`: defina como `0` para tornar cada componente de cor menos nítido, defina como `1` para aumentar a nitidez da imagem (intensidade) | `op_usm=1,1,10,0` |

Selecione o **[!UICONTROL Sharpening]** e escolha uma opção:

* **Nenhum**: desativa a nitidez.

* **Nitidez**: executa uma passagem de nitidez simples no arquivo após seu redimensionamento. É semelhante ao filtro &quot;Nitidez&quot; no Adobe Photoshop e oferece suporte a quaisquer parâmetros do usuário. Normalmente, você usaria esse filtro ou **[!UICONTROL Unsharp Mask]**, mas não ambos. Como prática recomendada, esse método não é recomendado, mas pode ajudar a compensar o desfoque. (URL: `op_sharpen`)

* **Tirar nitidez da máscara**: permite ajustar um efeito de filtro de nitidez na imagem final com resolução reduzida. É possível controlar a intensidade do efeito, o raio do efeito (medido em pixels) e um limite de contraste que é ignorado. Esse efeito usa as mesmas opções do filtro &quot;Tirar nitidez da máscara&quot; do Photoshop. (URL: `op_usm`)

Escolha estas opções para poder ajustar a nitidez com a opção Tirar nitidez da máscara:

* **Quantidade**: controla a quantidade de contraste aplicada aos pixels de borda. O padrão é 0,0. Para imagens de alta resolução, é possível aumentá-las para até 5,0. Pense na Quantidade como uma medida da intensidade do filtro. A variável **[!UICONTROL Amount]** no Adobe Dynamic Media Classic não é a mesma configuração de Quantidade no Adobe Photoshop. O Adobe Photoshop usa uma quantidade no intervalo de 1% a 500%, enquanto o Adobe Dynamic Media Classic pode ser dimensionado de 0,0 a 5,0. (5,0 equivale aproximadamente a 500% no Photoshop, 0,9 é semelhante a 90% e assim por diante.)

* **Raio**: determina o número de pixels em torno dos pixels de borda que afetam a nitidez. O efeito é executado em todos os pixels da imagem e irradia em todas as direções.

O melhor valor de raio depende do tamanho da imagem. Um valor baixo aplica nitidez apenas aos pixels da borda. Um valor alto aplica nitidez a uma faixa mais ampla de pixels.

Por exemplo, para obter um efeito de nitidez semelhante para uma imagem de 2000 × 2000 pixels e uma imagem de 500 × 500 pixels, você pode definir um valor de raio de dois pixels na imagem de 2000 × 2000 pixels. Em seguida, defina um valor de raio de um pixel na imagem de 500 × 500 pixels (um valor maior para uma imagem com mais pixels).

* **Limite**: determina o intervalo de contraste que deve ser ignorado quando o filtro Tirar nitidez da máscara é aplicado. Essa opção determina como deve ser a diferença dos pixels com nitidez em relação à área ao redor antes da nitidez dos pixels de borda.

O limite usa um valor de 0 a 255, que é o número de etapas de brilho em uma imagem em tons de cinza. 0=preto, 128=50% cinza e 255=branco. Por exemplo, um valor limite de 12 ignora pequenas variações no brilho do tom da pele. Ao fazer isso, não acrescenta ruído, enquanto ainda adiciona contraste de borda a áreas contrastadas, como onde as pálpebras encontram a pele.

Por exemplo, suponha que você tenha uma foto do rosto de alguém. A Tirar nitidez da máscara afeta as partes da imagem com mais contraste e a própria pele lisa. Mesmo a pele mais suave exibe alterações sutis nos valores de brilho. Se você não usar um valor limite, o filtro acentua essas alterações sutis nos pixels da pele, criando um efeito ruidoso (provavelmente indesejável) e, ao mesmo tempo, aumentando o contraste das pálpebras, aumentando a nitidez (provavelmente desejável). Para evitar esse problema, use um valor limite que informe ao filtro para ignorar pixels que não alteram drasticamente o contraste, como a capa lisa. Para evitar a introdução de ruídos ou imagens de posterização com tons de carne, por exemplo, experimente **[!UICONTROL Threshold]** valores dois a 20. O padrão **[!UICONTROL Threshold]** valor 0 aplica nitidez a todos os pixels da imagem.

* **Aplicar a**: Escolher **[!UICONTROL Each Color]** se quiser aplicar nitidez separadamente a cada componente de cor, escolha **[!UICONTROL Brightness]** se quiser aplicar nitidez às áreas de brilho da imagem.

**Reamostragem**

Selecione o **[!UICONTROL Resampling]** e escolha uma opção. Essas opções deixam a imagem mais nítida quando a resolução é reduzida:

* **[!UICONTROL None]**: desativa a reamostragem.

* **[!UICONTROL Bilinear]**: o método de reamostragem mais rápido; alguns artefatos de suavização são visíveis.

* **[!UICONTROL Bicubic]**: aumenta o uso da CPU no servidor de imagens, mas produz imagens mais nítidas com menos artefatos de suavização visíveis.

* **[!UICONTROL `Sharpen 2`]**: produz resultados ligeiramente mais nítidos do que **[!UICONTROL Bicubic]**, mas com um custo de CPU ainda maior no Servidor de imagens.

* **[!UICONTROL Trilinear]**: usa resoluções mais altas e mais baixas, se disponíveis; recomendado somente quando a suavização for um problema. Este método reduz o tamanho do JPEG devido à redução dos dados de alta frequência.

**Predefinições e nitidez da imagem**

Você pode incorporar todos os três efeitos de nitidez para alcançar o resultado final. No entanto, esse método não é recomendado. A Adobe Dynamic Media Classic recomenda salvar os efeitos de nitidez como parte de uma Predefinição de imagem. As Predefinições de imagem permitem empacotar os modificadores de imagem usados com mais frequência para criar uma imagem redimensionada dinamicamente em uma pequena cadeia de texto. Uma Predefinição de imagem contém valores para o formato de arquivo (geralmente JPEG para a Web), contagem de pixels e nitidez da imagem. Em vez de anexar o URL a cada modificador de imagem que você deve usar para criar um tipo específico de tamanho de imagem, crie uma Predefinição de imagem nomeada, como &quot;miniatura&quot;. Em seguida, configure a Predefinição de imagem em miniatura com as opções apropriadas de tamanho, formato de arquivo e nitidez. Chame a imagem usando o nome da Predefinição de imagem. As predefinições de imagem encurtam o comprimento do URL geral. Esses dois URLs produzem a mesma imagem de JPEG 350x350 com nitidez:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

As predefinições de imagem podem ser alteradas e atualizadas a qualquer momento. Você verá os resultados de uma alteração em uma Predefinição de imagem após a publicação e depois que o cache do URL for limpo.

Se você usar uma predefinição para cada imagem em uma categoria de tamanho, qualquer Administrador da empresa poderá atualizar a definição dessa Predefinição de imagem. Em seguida, eles podem republicar e afetar cada imagem usando esse formato. Tudo isso sem alterar nenhum código da Web. Como prática recomendada, use uma Predefinição de imagem por tamanho exclusivo no site. Para adicionar uma predefinição de imagem, na barra Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Application Settings]** > **[!UICONTROL Image Presets]**. Em seguida, selecione **[!UICONTROL Add]** ou selecione **[!UICONTROL Edit]** para alterar uma predefinição existente. O único campo obrigatório é o nome da própria predefinição. No entanto, é melhor incluir algum nível de nitidez em cada predefinição.

**Qualidade do JPG**

As opções de Qualidade de JPG controlam o nível de compactação de JPG:

* **Qualidade do JPG**: selecione essa opção se desejar controlar os níveis de compactação e a redução da resolução de crominância.

* **Controle deslizante**: determina o nível de compactação JPG. Essa configuração afeta o tamanho do arquivo e a qualidade da imagem. A escala de qualidade do JPG é de 1 a 100.

* **Ativar redução de resolução de crominância de JPG**: como o olho é menos sensível a informações de cores de alta frequência do que a luminosidade de alta frequência, as imagens de JPEG dividem as informações da imagem em componentes de luminosidade e cor. Quando uma imagem de JPEG é compactada, o componente de luminosidade fica com a resolução total, enquanto os componentes de cor ficam com uma resolução mais baixa para calcular a média de grupos de pixels. A redução da resolução reduz o volume de dados pela metade ou em um terço com quase nenhum impacto na qualidade aparente. A redução da resolução não é aplicável a imagens em tons de cinza. Essa técnica reduz a quantidade de compactação útil para imagens com alto contraste (por exemplo, imagens com texto sobreposto).

**Definir opções de nitidez em toda a empresa**

Se você não usou uma Predefinição de imagem ou transmitiu protocolos de nitidez específicos do Servidor de imagens ao longo da string do URL, a nitidez da imagem não ocorrerá quando a resolução for reduzida. No entanto, se essa falta de nitidez ocorrer, será possível definir os valores de nitidez padrão para garantir que qualquer imagem sempre tenha alguma nitidez.

Para definir as opções de nitidez padrão da sua empresa, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]**. Se você definir o Modo de reamostragem padrão como **`Sharp2`**, ela sempre aplica nitidez à imagem ao diminuir a resolução.

**Adicionar nitidez às Predefinições do visualizador**

A menos que você tenha adicionado modificadores de nitidez de imagem à predefinição, a imagem de carregamento inicial pequena pode parecer suave porque tem uma resolução reduzida para caber na janela do visualizador sem ter nitidez.

As Predefinições do visualizador (como Predefinições de imagem) permitem centralizar muitas opções em um único local, incluindo a escolha de opções de capa e do visualizador (como incluir um botão Imprimir ou controlar a velocidade da animação de zoom). As Predefinições do visualizador são encontradas na mesma seção que Predefinições da imagem, em **[!UICONTROL Setup]** > **[!UICONTROL Application Settings]** > **[!UICONTROL Viewer Presets]**.

Consulte [Predefinições do visualizador](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) vídeo de treinamento.

A opção Modificadores é encontrada na seção Configurações principais de todas as predefinições do visualizador de eCatalog, Rotação e Zoom personalizado. Ao adicionar os comandos de nitidez do URL à caixa Modificadores, você adiciona nitidez sempre que o visualizador é chamado com essa Predefinição do visualizador.

Para chamar a Predefinição do visualizador, use o `config=` no URL do visualizador. Este é um exemplo de chamada de um Conjunto de imagens (sapatos) com uma Predefinição do visualizador (`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

A predefinição aqui aplica nitidez e altera a capa padrão do visualizador.

**Criar substituições específicas de imagem**

O último método, e menos recomendado, de nitidez é criar substituições de nitidez imagem por imagem. Esse método substitui a nitidez em uma predefinição de imagem por seus próprios valores específicos. No entanto, esse método também substitui todos os outros métodos de nitidez de qualquer tamanho. O melhor caso de uso para esse método é se algumas das imagens não estiverem em alta resolução e os valores nas Predefinições de imagem estiverem muito altos para essas imagens pequenas. Nesse caso, possivelmente será necessário aplicar nitidez a cada imagem.

No Adobe Dynamic Media Classic, selecione qualquer imagem, vá para a Exibição de detalhes (clicando duas vezes ou pressionando o botão **[!UICONTROL Detail View]** ) e selecione **[!UICONTROL Sharpen]**. Altere qualquer parâmetro e selecione **[!UICONTROL Save]**. Esse processo instrui o Servidor de imagens a usar esses parâmetros de nitidez em vez de qualquer comando chamado no URL, como um modificador de nitidez ou uma Predefinição de imagem. Certifique-se de publicar para ver se as alterações entram em vigor.
