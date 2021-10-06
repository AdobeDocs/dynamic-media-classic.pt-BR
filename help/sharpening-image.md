---
title: Nitidez de uma imagem
description: Saiba como ajustar a nitidez de uma imagem no Adobe Dynamic Media Classic.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '2230'
ht-degree: 0%

---

# Nitidez de uma imagem {#sharpening-an-image}

A nitidez é uma técnica de manipulação de imagem para tornar os contornos de uma imagem digital mais distintos. A nitidez aumenta o contraste entre pixels de borda e enfatiza a transição entre áreas escuras e claras. A nitidez aumenta o contraste local e traz detalhes. Não há fórmula estrita para ajustar a nitidez correta de todas as imagens. Muito pouca nitidez pode fazer com uma imagem suave, mas a nitidez excessiva adiciona halos, artefatos e ruídos.

A Adobe Dynamic Media Classic recomenda usar as Predefinições de imagem para todas as imagens. Eles garantem um tamanho uniforme, e a nitidez é aplicada em qualquer imagem chamada com uma predefinição de imagem. Além disso, você pode editar e alterar facilmente os parâmetros de nitidez de uma predefinição de imagem. Na próxima vez que você publicar, todas as imagens chamadas com essa predefinição receberão os novos valores.

A Adobe Dynamic Media Classic também recomenda adicionar nitidez às Predefinições do visualizador e, em seguida, chamar um visualizador com essa predefinição. Isso garante que as imagens em seus visualizadores sejam nítidas e atraentes.

No entanto, se você usar Predefinições de imagem e Predefinições do visualizador ou algum método alternativo de nitidez, a conclusão é que você deve tornar suas imagens mais nítidas. Caso contrário, suas imagens (e seu site) podem parecer suaves e difusas.

>[!NOTE]
>
>Os comandos Nitidez substituem as configurações da Predefinição de imagem, incluindo seus efeitos de nitidez. Uma predefinição de imagem governa o tamanho e a formatação com que as imagens são entregues dos servidores de imagem da Dynamic Media. A Adobe Dynamic Media Classic recomenda usar as Predefinições de imagem para fornecer todas as imagens e garantir que elas sejam entregues em um tamanho e nitidez uniformes. Depois que as configurações de nitidez de uma imagem individual forem alteradas, no entanto, as configurações de nitidez da Predefinição de imagem não se aplicarão mais à imagem. Ele é entregue sem as configurações de nitidez da predefinição de imagem.

Geralmente é necessário ajustar a nitidez das imagens. Adobe Dynamic Media Classic e Servidores de Imagem oferecem várias opções de nitidez. É importante entender o que a nitidez faz em uma imagem e a nitidez necessária. A maioria das imagens precisa de alguma nitidez, mas a quantidade necessária depende da imagem.

A nitidez da imagem aumenta o contraste dos pixels para criar o efeito de acentuar as bordas. Os seres humanos percebem este contraste de borda melhorado como nitidez. Embora seja fácil aprimorar uma imagem executando filtros de nitidez em uma imagem, também é fácil tornar uma imagem mais nítida.

Acima da nitidez de uma imagem cria um efeito de halo ou faixas das linhas da borda.

Você pode seguir as práticas recomendadas para otimizar a nitidez de suas imagens no Adobe Dynamic Media Classic e no Dynamic Media Image Server.

Consulte [Práticas recomendadas para nitidez de imagens no Adobe Dynamic Media Classic e no Dynamic Media Image Server](/help/assets/s7_sharpening_images.pdf).

Consulte também [Nitidez](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) vídeo de treinamento.

**Para ajustar a nitidez de uma imagem:**

Para ajustar a nitidez de uma imagem, selecione o botão de sobreposição **[!UICONTROL Edit]** e escolha **[!UICONTROL Sharpen]**, ou abra-o no Painel de navegação na Exibição de detalhes e selecione **[!UICONTROL Sharpen]**. A página Editor de nitidez é aberta com comandos de nitidez. Escolha comandos e selecione **[!UICONTROL Save]**.

>[!NOTE]
>
>Antes de ajustar a nitidez de uma imagem, selecione o menu Aplicar predefinição e escolha uma predefinição de imagem para ver quais são os seus efeitos de nitidez. Os efeitos de nitidez de uma predefinição de imagem são adequados para a sua imagem. O menu **[!UICONTROL Apply Preset]** está na parte inferior da página Editor de nitidez.

**Opções de nitidez**

A tabela a seguir mostra as opções de nitidez do Servidor de imagem.

| Nome | Protocolo de URL | Valores | Exemplo |
| --- | --- | --- | --- |
| Nitidez simples | `op_sharpen` | `0` ou  `1` | `op_sharpen=1` |
| Modo de reamostra | `resMode` | `bilin`,  `bicub`,  `sharp2`,  `trilin`<br><br>`bilin`: Seleciona a interpolação bi-linear padrão. Método de reamostragem mais rápido; alguns artefatos de aliasing geralmente são perceptíveis.<br>`bicub`: Seleciona a interpolação bicúbica. Mais uso de CPU do que bilin, mas produz imagens mais nítidas com artefatos de aliasing menos perceptíveis.<br><br>`sharp2`: Seleciona uma função do Lanczos Windows® modificada como um algoritmo de interpolação. Pode produzir resultados ligeiramente mais nítidos do que bi-cúbicos a um custo de CPU mais alto.<br><br>`trilin`: Seleciona uma interpolação trilinear modificada, que usa resoluções mais altas e mais baixas, se disponível. Recomendado somente quando a aliasing é um problema. Reduz os tamanhos dos JPEG devido à redução dos dados de alta frequência. | `resMode=sharp2` |
| Tirar nitidez da máscara | `op_usm` | `amount`,  `radius`,  `threshold`,  `monochrome`<br><br>`amount`: fator de força do filtro (real 0...5)<br><br>`radius`: raio do kernel do filtro em pixels (real 0...250)  <br><br>`threshold`: nível do limite do filtro (int 0...255)<br><br>`monochrome`: definido  `0` para desfazer a nitidez da máscara de cada componente de cor separadamente, definido  `1` para desfazer nitidez do brilho da imagem da máscara de nitidez (intensidade) | `op_usm=1,1,10,0` |

Selecione o menu **[!UICONTROL Sharpening]** e escolha uma opção:

* **None**  - Desativa a nitidez.

* **Nitidez**  - Executa uma passagem de nitidez simples no arquivo depois de ser redimensionado. É semelhante ao filtro &quot;Nitidez&quot; no Adobe Photoshop e suporta qualquer parâmetro de usuário. Normalmente, você usaria esse filtro ou **[!UICONTROL Unsharp Mask]**, mas não ambos. Como prática recomendada, esse método não é recomendado, mas pode ajudar a compensar a indefinição. (URL: `op_sharpen`)

* **Tirar nitidez da máscara**  - Permite ajustar um efeito de filtro de nitidez na imagem final com resolução reduzida. Você pode controlar a intensidade do efeito, o raio do efeito (medido em pixels) e um limite de contraste que é ignorado. Esse efeito usa as mesmas opções do filtro &quot;Tirar nitidez da máscara&quot; do Photoshop. (URL: `op_usm`)

Escolha essas opções para ajustar a nitidez com Tirar nitidez da máscara:

* **Quantia**  - Controla a quantidade de contraste aplicado aos pixels da borda. O padrão é 0,0. Para imagens de alta resolução, você pode aumentá-lo até 5,0. Considere Quantia como uma medida de intensidade de filtro. A configuração **[!UICONTROL Amount]** no Adobe Dynamic Media Classic não é igual à configuração Valor no Adobe Photoshop. O Adobe Photoshop usa uma quantidade no intervalo de 1% a 500%, enquanto o Adobe Dynamic Media Classic é dimensionado de 0,0 para 5,0. (5.0 equivale aproximadamente a 500% no Photoshop, 0.9 é semelhante a 90% e assim por diante.)

* **Raio**  - Determina o número de pixels ao redor dos pixels da borda que afetam a nitidez. O efeito é executado em todos os pixels na imagem e irradia em todas as direções.

O melhor valor de raio depende do tamanho da imagem. Um valor baixo ajuste a nitidez apenas dos pixels da borda. Um valor alto ajuste a nitidez de uma faixa maior de pixels.

Por exemplo, para obter um efeito de nitidez semelhante para uma imagem de 2000 x 2000 pixels e imagem de 500x 500 pixels, você pode definir um valor de raio de dois pixels na imagem de 2000 x 2000 pixels. Em seguida, defina um valor de raio de um pixel na imagem de 500 x 500 pixels (um valor maior para uma imagem com mais pixels).

* **Limite**  - Determina o intervalo de contraste a ser ignorado quando o filtro de máscara de nitidez for aplicado. Essa opção determina como deve ser a diferença dos pixels com nitidez em relação à área ao redor antes de serem considerados pixels de borda e terem nitidez.

O limite usa um valor de 0 a 255, que é o número de etapas de brilho em uma imagem em tons de cinza. 0=preto, 128=50% cinza e 255=branco. Por exemplo, um valor limite de 12 ignora pequenas variações é o brilho do tom da pele, para não adicionar ruído, enquanto ainda adiciona o contraste da borda a áreas contrastantes, como onde as pálpebras tocam a pele.

Por exemplo, suponha que você tenha uma foto do rosto de alguém. A Tirar nitidez da máscara afeta as partes da imagem com mais contraste e a própria pele lisa. Mesmo a pele mais suave apresenta alterações sutis nos valores de brilho. Se você não usar um valor de limite, o filtro acentua essas sutis alterações em pixels da pele, criando um efeito ruidoso (provavelmente indesejável), além de aumentar o contraste nas pálpebras, melhorando a nitidez (provavelmente desejável). Para evitar esse problema, use um valor de limite que instrua o filtro a ignorar os pixels que não alteram o contraste drasticamente, como pele lisa. Para evitar a introdução de ruídos ou imagens de posterização com tons de carne, por exemplo, tente experimentar com **[!UICONTROL Threshold]** valores dois a 20. O valor padrão **[!UICONTROL Threshold]** de 0 ajuste a nitidez de todos os pixels na imagem.

* **Aplicar a**  - Escolha  **[!UICONTROL Each Color]** se deseja aplicar a nitidez separadamente a cada componente de cor; escolha  **[!UICONTROL Brightness]** se deseja aplicar a nitidez às áreas de brilho da imagem.

**Reamostragem**

Selecione o menu **[!UICONTROL Resampling]** e escolha uma opção. Essas opções aprimoram a imagem quando ela é reduzida:

* **[!UICONTROL None]** - Desativa a reamostragem.

* **[!UICONTROL Bilinear]** - o método de reamostragem mais rápido; alguns artefatos de aliasing são perceptíveis.

* **[!UICONTROL Bicubic]** - Aumenta o uso da CPU no Servidor de imagem, mas gera imagens mais nítidas com artefatos de aliasing menos perceptíveis.

* **[!UICONTROL Sharpen2]** - Produz resultados ligeiramente mais nítidos do que  **[!UICONTROL Bicubic]**, mas com um custo de CPU ainda maior no servidor de imagem.

* **[!UICONTROL Trilinear]** - Utiliza resoluções mais altas e mais baixas, se disponíveis; recomendado somente quando aliasing for um problema. Este método reduz o tamanho do JPEG devido à redução dos dados de alta frequência.

**Predefinições de nitidez e imagem**

Você pode incorporar todos os três efeitos de nitidez para obter o resultado final. No entanto, esse método não é recomendado. A Adobe Dynamic Media Classic recomenda salvar seus efeitos de nitidez como parte de uma Predefinição de imagem. As Predefinições de imagem permitem agrupar os modificadores de imagem usados com mais frequência para criar uma imagem redimensionada dinamicamente em uma pequena string de texto. Uma predefinição de imagem contém valores para o formato de arquivo (geralmente JPEG para a Web), contagem de pixels e nitidez da imagem. Em vez de anexar o URL a cada modificador de imagem que deve ser usado para criar um tipo específico de tamanho de imagem, crie uma Predefinição de imagem chamada, como &quot;miniatura&quot;. Em seguida, configure a predefinição de imagem em miniatura com o tamanho, formato de arquivo e opções de nitidez apropriados. Chame a imagem usando o nome Predefinição de imagem. As predefinições de imagem reduzem o comprimento do URL geral. Esses dois URLs produzem a mesma imagem de JPEG 350x350 com nitidez:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

As predefinições da imagem podem ser alteradas e atualizadas a qualquer momento. Você verá os resultados de uma alteração em uma predefinição de imagem depois de publicar e depois que o cache do URL for limpo.

Se você usar uma predefinição para cada imagem em uma categoria de tamanho, qualquer Administrador da empresa poderá atualizar a definição dessa Predefinição de imagem, republicar e afetar todas as imagens usando esse formato, sem alterar nenhum código da Web. Como prática recomendada, use uma Predefinição de imagem por tamanho exclusivo em seu site. Para adicionar uma predefinição de imagem, na barra Navegação global, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Settings]** > **[!UICONTROL Image Presets]**. Em seguida, selecione **[!UICONTROL Add]** ou **[!UICONTROL Edit]** para alterar uma predefinição existente. O único campo obrigatório é o nome da própria predefinição. No entanto, é melhor incluir algum nível de nitidez em cada predefinição.

**Qualidade JPG**

As opções de Qualidade JPG controlam o nível de compactação JPG:

* **Qualidade do JPG**  - Selecione essa opção se desejar controlar os níveis de compactação e a redução da amostragem de crominância.

* **Controle deslizante**  - Determina o nível de compactação de JPG. Essa configuração afeta o tamanho do arquivo e a qualidade da imagem. A escala de qualidade do JPG é de 1 a 100.

* **Ativar a redução da frequência do JPG Chrominance**  - Como o olho é menos sensível às informações de cores de alta frequência do que à luminância de alta frequência, as imagens de JPEG dividem as informações da imagem em luminância e componentes de cores. Quando uma imagem de JPEG é compactada, o componente de luminância é deixado em resolução completa, enquanto os componentes de cor são reduzidos pela média de grupos de pixels. A redução da amostragem reduz o volume de dados em um terço ou metade, quase sem impacto na qualidade percebida. A redução da amostragem não é aplicável a imagens em tons de cinza. Essa técnica reduz a quantidade de compactação útil para imagens com alto contraste (por exemplo, imagens com texto sobreposto).

**Definir opções de nitidez em toda a empresa**

Se você não usar uma Predefinição de imagem ou transmitir protocolos de nitidez específicos do Servidor de imagem ao longo da string de URL, a imagem não será dimensionada com nitidez quando for reduzida. No entanto, se essa falta de nitidez ocorrer, você poderá definir valores de nitidez padrão e, em seguida, qualquer imagem sempre terá alguma nitidez.

Para definir as opções de nitidez padrão da sua empresa, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]**. Se você definir o Modo de amostragem padrão como **[!UICONTROL Sharp2]**, ele sempre ajuste a nitidez da imagem ao fazer a resolução.

**Adicionar nitidez às predefinições do visualizador**

A menos que você adicione modificadores de imagem de nitidez à predefinição, a pequena imagem de carregamento inicial pode parecer suave, pois a resolução é reduzida para caber na janela do visualizador sem ser nitidez.

As Predefinições do visualizador (como as Predefinições de imagem) permitem centralizar várias opções em um único local, incluindo opções de capa e do visualizador (como incluir um botão Imprimir ou controlar a velocidade da animação de zoom). As Predefinições do visualizador são encontradas na mesma seção que as Predefinições de imagem, em **[!UICONTROL Setup]** > **[!UICONTROL Application Settings]** > **[!UICONTROL Viewer Presets]**.

Consulte [Vídeo de treinamento de predefinições do visualizador](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS).

A opção Modificadores é encontrada na seção Configurações principais de todas as predefinições do eCatalog, rotação e do visualizador de zoom personalizado. Ao adicionar os comandos de nitidez do URL à caixa Modificadores, adicione a nitidez sempre que o visualizador for chamado com essa predefinição do visualizador.

Para chamar a Predefinição do visualizador, use o comando `config=` no URL do visualizador. Veja um exemplo de como chamar um Conjunto de imagens (sapatos) com uma Predefinição do visualizador (`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

A predefinição aqui ajuste a nitidez e altera a pele padrão do visualizador.

**Criar substituições específicas por imagem**

O último método de nitidez, e o menos recomendado, é criar substituições de nitidez em uma base imagem por imagem. Esse método substitui a nitidez em uma predefinição de imagem por seus próprios valores específicos. No entanto, esse método também substitui todos os outros métodos de nitidez em qualquer tamanho. O melhor caso de uso para esse método é se algumas de suas imagens não tiverem alta resolução e os valores nas Predefinições de imagem forem altos demais para essas imagens pequenas. Nesse caso, é possível que seja necessária alguma nitidez por imagem.

No Adobe Dynamic Media Classic, selecione qualquer imagem, vá para a Exibição de detalhes (clicando duas vezes ou pressionando o botão **[!UICONTROL Detail View]**) e selecione **[!UICONTROL Sharpen]**. Altere qualquer parâmetro e selecione **[!UICONTROL Save]**. Esse processo instrui o Servidor de imagem a usar esses parâmetros de nitidez em vez de qualquer comando que você chamar no URL, como um modificador de nitidez ou Predefinição de imagem. Certifique-se de publicar para ver se as alterações entrarão em vigor.
