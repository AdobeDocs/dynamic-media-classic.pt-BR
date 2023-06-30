---
title: Criar um modelo
description: Saiba como criar um modelo no Adobe Dynamic Media Classic.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
topic: Content Management
level: Experienced
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '3310'
ht-degree: 0%

---

# Criar um modelo {#creating-a-template}

Para criar um template, acesse **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. Selecione Designer ou Desenvolvedor. Nessa página, é possível adicionar camadas de imagem e texto. Também é possível reordenar camadas, alterar o tamanho e a posição das camadas e aplicar efeitos de sombra e brilho a imagens e texto.

Consulte também [Noções básicas de modelo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) vídeo de treinamento.

>[!NOTE]
>
>Se você editar um modelo criado em uma versão anterior do Adobe Dynamic Media Classic, um prompt perguntará ao salvar &quot;Deseja adicionar uma camada da tela de desenho?&quot;. Selecionar **[!UICONTROL No]** para evitar a adição de uma camada base. Se você selecionar **[!UICONTROL Yes]**, exclua o `&allowCanvasPrompt` e `&layer=0` modificadores no URL e pressione **[!UICONTROL Enter]** ou **[!UICONTROL Return]**.

## Criar o modelo inicial {#creating-the-initial-template}

Ao criar um conjunto de modelos, a variável **[!UICONTROL Publish after save]** opção afeta os membros set e set das seguintes maneiras:

| **[!UICONTROL Publish after save]** opção selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos mantêm seu estado publicado ou não publicado. |

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

Você pode criar um template a partir de um template existente. Abra o modelo e selecione **[!UICONTROL Save As]** e digite um novo nome na caixa de diálogo Salvar como.

**Para criar o modelo inicial:**

1. Para criar o template inicial, use um dos seguintes métodos:

   * **Selecione o PSD ou as imagens primeiro** - No painel Procurar, selecione o arquivo de PSD ou as imagens desejadas para o modelo, vá para **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**.

   * **Iniciar na tela Modelo** - Vá para **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. Selecione Designer ou Desenvolvedor.

1. Na caixa de diálogo Inserir Tamanho da Tela de Pintura, insira medidas de largura e altura para o modelo.
1. Selecione uma pasta na Biblioteca de ativos e arraste o arquivo PSD ou as imagens desejadas para o modelo na tela Modelo.
1. Quando terminar, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]**.
1. Selecione uma pasta para armazenar o modelo, digite um nome para o modelo e selecione **[!UICONTROL Submit]**.

   O Adobe Dynamic Media Classic reduz as imagens, se necessário, para ajustá-las à tela, que é a área na tela Modelo para definição do modelo.

## Editar um conjunto de modelos {#editing-a-template-set}

Se você editar um conjunto publicado ou um conjunto de modelos não publicado, a variável **[!UICONTROL Publish after save]** opção afeta os membros set e set das seguintes maneiras:

| Conjunto já publicado? | **[!UICONTROL Publish after save]** opção selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- | --- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existentes mantêm seu estado publicado. Qualquer novo membro do conjunto adicionado durante sua edição manterá seu estado publicado ou não. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existentes e os novos membros do conjunto adicionados durante a edição mantêm seus estados publicado ou não. |

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um conjunto de modelos:**

1. Na Exibição de Grade, navegue até um Conjunto de Modelos e, abaixo da imagem, selecione **[!UICONTROL Edit]**.
1. Altere o template conforme necessário.
1. Ao concluir a edição, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]**, selecione uma pasta de armazenamento, digite um nome para o conjunto e selecione **[!UICONTROL Save]**.

## Excluir um modelo {#deleting-a-template}

Ao excluir um conjunto de modelos, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um modelo:**

1. Na Exibição em Grade, Exibição em Lista ou Exibição de Detalhes, selecione um ou mais Modelos.
1. Na Barra de navegação global, acesse **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.

## Compreender a tela Modelo {#understanding-the-template-screen}

A tela Modelo oferece ferramentas para manipular e parametrizar camadas.

Use estas ferramentas na tela Modelo para criar modelos:

* **[!UICONTROL Pan]** - Permite selecionar camadas, movê-las ao redor da tela de desenho, redimensioná-las ou girá-las.

* **[!UICONTROL Text]** - Cria uma camada de texto. Arraste na tela de desenho para criar uma camada de texto e, em seguida, insira o texto na camada. Consulte [Criação de uma camada de texto](#creating-a-text-layer).

* **[!UICONTROL Preview]** - Abre a tela Visualizar e mostra o modelo em um Visualizador de zoom. Você vê a aparência do modelo para os usuários no seu site ou aplicativo.

* **[!UICONTROL Parameter Summary]** Abre a tela Resumo de Parâmetros. Você pode ver o nome de cada camada em um modelo e, em cada camada, os nomes dos parâmetros que foram ativados.

* **[!UICONTROL Text Editor v4.3 and Text Editor v4.2]** - Você pode optar por usar o editor de texto mais recente e completo, editor de texto v4.3, ou o editor de texto anterior, editor de texto v4.2. Ao criar modelos, o Editor de texto v4.3 é selecionado por padrão. Ao editar modelos mais antigos, o Editor de texto v4.2 é selecionado por padrão. No momento, o Editor de texto v4.3 não é compatível com quebra automática de linha. Portanto, ao editar modelos mais antigos que usam quebra automática de linha, use o Editor de texto v4.2 para manter a fidelidade do modelo totalmente intacta. Se o modelo mais antigo não usar quebra automática de linha, você poderá escolher o Editor de texto v4.3 para aproveitar os vários recursos novos que ele oferece. Por exemplo, Aumentar Margens, Diminuir Margens, Definir Texto em Todas as Maiúsculas e Copiar Ajustar Texto.

  >[!NOTE]
  >
  >Como a remoção do Editor de texto v4.2 está planejada como uma opção no Adobe Dynamic Media Classic, é recomendável usar o Editor de texto 4.3, quando possível. A variável **[!UICONTROL Word Wrap]** será incorporada em uma versão futura do Editor de texto.

* **[!UICONTROL Designer and Developer]** - Selecione a opção que melhor descreva sua função.

* **[!UICONTROL Canvas]** - Define a área total disponível, em pixels, para definir o modelo. O tamanho padrão é 300 x 300 pixels. As camadas são colocadas na tela de desenho.

* **[!UICONTROL Layers list]** - Lista o nome das camadas no modelo. Para selecionar uma camada, selecione seu nome na lista Camadas. A lista Camadas oferece ferramentas para adicionar efeitos a camadas, excluir camadas, reordenar camadas e parametrizar camadas. Consulte [Trabalhar com camadas](#working-with-layers).

* **[!UICONTROL Layer Properties area]** - Oferece ferramentas para alterar a cor, a opacidade, o tamanho e a posição do plano de fundo de uma camada, bem como a cor, a opacidade e o tamanho da tela de desenho. Também é possível ajustar efeitos de sombra e brilho. Consulte [Trabalhar com camadas](#working-with-layers).

## Criar camadas de imagem {#creating-image-layers}

1. Arraste a imagem da Biblioteca de ativos para a tela.

   O nome da ID da imagem aparece na lista Camadas.

   >[!NOTE]
   >
   >Se necessário, o Adobe Dynamic Media Classic reduz as imagens para ajustá-las à tela ao criar uma camada de imagem.

## Criar uma camada de texto {#creating-a-text-layer}

1. Selecione o **[!UICONTROL Text]** ferramenta.
1. Arraste para criar uma caixa de texto na tela ou em uma imagem.
1. Na tela Texto que é aberta, adicione o texto seguindo um destes procedimentos na guia Visualizar:

   * Digite texto na caixa de texto. Escolha &#39;Copiar texto de ajuste&#39; para ajustar o texto à caixa de texto.
   * Cole o texto da Área de Transferência na caixa de texto.

1. Selecionar **[!UICONTROL Apply]** e feche a tela Texto.

### Formatar texto {#format-text}

Para formatar o texto em uma camada de texto, faça o seguinte:

1. Na lista Camadas, clique duas vezes no nome da caixa de texto com o texto que deseja editar. O Editor de texto se abre.
1. Na caixa de texto do Editor de texto, selecione o texto que deseja formatar. Você pode selecionar todo o texto, partes do texto ou caracteres individuais.
1. Especifique qualquer uma das seguintes opções de formatação e selecione **[!UICONTROL Apply]**.

   * **[!UICONTROL Font]** - Escolha uma fonte no menu Fonte. Se uma fonte desejada não for exibida no menu, você poderá carregá-la na Adobe Dynamic Media Classic. Consulte Fontes.

   * **[!UICONTROL Font Size]** - Escolha um tamanho de fonte no menu, digite um tamanho específico na caixa ou selecione o **[!UICONTROL Up]** ou **[!UICONTROL Down]** para aumentar ou diminuir o tamanho em dois pontos.

   * **[!UICONTROL Color]** - Selecione para escolher uma cor para o texto.

   * **[!UICONTROL Bold]**, **[!UICONTROL Italic]** ou **[!UICONTROL Underline]** - Selecione o texto e, em seguida, selecione o ícone do tipo de formatação que deseja aplicar ao texto.

   * **[!UICONTROL All Caps]**, **[!UICONTROL Superscript]** ou **[!UICONTROL Subscript]** - Selecione o texto e, em seguida, selecione o ícone do tipo de formatação que deseja aplicar ao texto.

   * **[!UICONTROL Alignment]** - Escolha um botão Alinhamento para alinhar à esquerda, centralizar ou alinhar à direita o texto na camada de texto.

   * **[!UICONTROL Tracking]** - Digite ou selecione um valor numérico pelo qual ajustar a quantidade de espaço entre palavras.

   * **[!UICONTROL Kerning]** - Digite ou selecione um valor numérico pelo qual ajustar a quantidade de espaço entre caracteres.

   * **[!UICONTROL Line Spacing]** - Digite ou selecione um valor numérico pelo qual ajustar a quantidade de espaço entre linhas.

   * **[!UICONTROL Baseline Shift]** - Digite ou selecione um valor numérico pelo qual mover um caractere selecionado para cima ou para baixo em relação à linha de base do texto ao redor. Essa opção é especialmente útil quando você está ajustando manualmente frações ou ajustando a posição de gráficos incorporados.

>[!NOTE]
>
>Selecionar **[!UICONTROL Undo]** se quiser reverter a última ação. Selecionar **[!UICONTROL Redo]** se você mudar de ideia sobre como reverter uma ação depois de selecionar **[!UICONTROL Undo]**.

### Formatar parágrafos {#format-paragraphs}

1. Na lista Camadas, clique duas vezes no nome da caixa de texto com o texto que deseja editar. O Editor de texto se abre.
1. Selecione o parágrafo que deseja formatar.
1. Especifique qualquer uma das seguintes opções de formatação e selecione **[!UICONTROL Apply]**.

   * **[!UICONTROL Alignment]** - Selecione para especificar o tipo de alinhamento: alinha à esquerda, alinha ao centro, alinha à direita ou justifica.

   * **[!UICONTROL End of Paragraph Justification]** - Selecione para especificar o tipo de justificativa para a última linha do parágrafo: a última linha se alinha à esquerda; a última linha se alinha ao centro; e a última linha se alinha à direita.

   * **[!UICONTROL Line Spacing]** - Digite ou selecione um valor numérico pelo qual ajustar a quantidade de espaço entre todas as linhas no parágrafo.

   * **[!UICONTROL Indent All]** - Selecione para aumentar a quantidade de recuo do texto.

   * **[!UICONTROL Remove Indent]** - Selecione para diminuir a quantidade de recuo do texto.

   * **[!UICONTROL Indent First Line]** - Especifique a quantidade pela qual deseja recuar a primeira linha do texto.

   * **[!UICONTROL Space Before Paragraph]** - Especifique a quantidade de espaço que você deseja exibir acima da primeira linha do texto no parágrafo.

   * **[!UICONTROL Space After Paragraph]** - Especifique a quantidade de espaço que você deseja que apareça abaixo da última linha do texto no parágrafo.

   * **[!UICONTROL Vertical Align]** - Selecione onde deseja que o texto apareça verticalmente na caixa de texto: Superior, Meio, Inferior.

   * **[!UICONTROL Text Direction]** - Selecione a direção na qual deseja que o texto seja exibido: Da Direita para a Esquerda ou Da Esquerda para a Direita.

### Ajustar propriedades da camada de texto {#adjust-text-layer-properties}

1. Na tela Noções básicas do modelo, selecione a caixa de texto que deseja ajustar.
1. No painel Propriedades da camada, selecione qualquer uma das seguintes opções:

   * **[!UICONTROL Shrink Text (Text Editor v4.2 only)]** - Para ajustar na caixa de texto, selecione para reduzir o texto.

   * **[!UICONTROL Word Wrap (Text Editor v4.2 only)]** - Para especificar se ou como o texto é quebrado, selecione uma opção de quebra automática:

   * **[!UICONTROL Wrap]** - Quebra o texto para ajustá-lo em uma caixa de texto muito pequena horizontalmente.

   * **[!UICONTROL No Wrap]** - Não quebra automática de texto quando a caixa de texto é muito pequena horizontalmente e, em vez disso, corta uma parte do texto.

   * **[!UICONTROL Nonbreaking Wrap]** - Quebra o texto para ajustá-lo em uma caixa de texto e não quebra as palavras.

   * **[!UICONTROL Position]** - Especifica o local da caixa de texto na tela de desenho.

   * **[!UICONTROL Padding]** - Adiciona margens ou recorta o retângulo da camada. Especifique o número de pixels que deseja adicionar ou remover para Esquerda, Superior, Inferior e Direito. Insira números positivos se quiser adicionar uma margem ou números negativos ao recorte.

### Exibir e editar o código-fonte do texto {#view-and-edit-text-source-code}

As informações fornecidas na guia Código-fonte do Editor de texto são para sua referência. Edite o texto somente se estiver familiarizado com a edição do código-fonte.

1. Na lista Camadas, clique duas vezes no nome da caixa de texto com o texto que deseja editar. O Editor de texto se abre.
1. No Editor de Texto, para revelar o código-fonte do texto, selecione a **[!UICONTROL Source]** no Editor de texto.
1. Exiba ou edite o texto conforme desejado.

   As alterações permanecerão intactas se você alternar entre a visualização Visualização e Origem.

1. Selecionar **[!UICONTROL Apply]** para renderizar as edições.

## Trabalhar com camadas {#working-with-layers}

Use a lista Camadas e a área Propriedades da camada para trabalhar com camadas. É possível reordenar camadas, alterar seu tamanho e posição, girar camadas e determinar a cor do plano de fundo, a cor do primeiro plano, a opacidade e o modo de mesclagem de uma camada.

Também é possível alterar o tamanho da tela de desenho, escolher sua cor de fundo e alterar sua configuração de opacidade.

### Reordenar camadas {#reordering-layers}

A alteração da ordem das camadas pode afetar a aparência, especialmente quando há envolvimento de transparência ou superimposição. Certifique-se de visualizar o resultado antes de confirmar as alterações.

1. Use uma destas técnicas para reordenar as camadas em um modelo:

   * Selecione uma camada na lista Camadas. Em seguida, selecione **[!UICONTROL Up]** ou **[!UICONTROL Down]** quantas vezes forem necessárias para colocá-lo na posição correta na lista.
   * Arraste uma camada para cima ou para baixo na lista Camadas.

### Alteração do tamanho e da posição das camadas e da tela de desenho {#changing-the-size-and-position-of-layers-and-the-canvas}

As camadas devem ser pequenas o suficiente para caber na tela de desenho. É possível alterar o tamanho de uma camada ou da tela de desenho manualmente ou inserindo medidas de tamanho. É possível alterar a posição de uma camada manualmente ou inserindo medidas de deslocamento. Também é possível girar uma camada.

>[!NOTE]
>
>A Adobe Dynamic Media Classic recomenda criar uma Predefinição de imagem que seja do tamanho exato do modelo. Fazer a correspondência do tamanho da Predefinição de imagem com o tamanho do modelo garante que o tamanho da saída final e as opções de nitidez do modelo sejam definidos corretamente. Depois de criar essa Predefinição de imagem, você pode escolhê-la no menu Aplicar predefinição na tela Visualização de modelo. A tela mostra a aparência da imagem quando entregue pelo servidor. Consulte [Configurar predefinições da imagem](setting-image-presets.md#setting_up_image_presets).

* **Alteração do tamanho de uma camada** - Para alterar o tamanho de uma camada ou tela de desenho, selecione a camada ou tela de desenho na lista Camadas e use uma destas técnicas:

* **Alteração manual do tamanho** - Selecione e arraste um canto da camada ou tela de desenho. Com camadas de texto, também é possível arrastar um lado da camada. Mantenha pressionada a tecla Shift enquanto arrasta para alterar o tamanho, mas mantenha a proporção (a forma).

* **Inserção de medidas de tamanho de camada** - Insira medidas de pixel nas caixas de texto L (Largura) e A (Altura) na área Propriedades da camada.

Além de alterar o tamanho de uma camada, você pode preenchê-la. Para fazer isso, insira uma medida de Preenchimento na caixa Esquerda, Direita, Superior e Inferior da área Propriedades da camada. O preenchimento adiciona uma margem à camada atual para deslocá-la do perímetro de sua camada base. O preenchimento é útil se você adicionar um efeito de sombra projetada ou brilho externo e quiser tornar o efeito mais visível. O preenchimento aumenta o tamanho de uma camada e exibe sua cor de fundo na área estendida e preenchida. A camada base se reposiciona em relação ao novo tamanho da camada. Por exemplo, se a camada atual estiver centralizada na camada base, estender o lado esquerdo da camada a moverá mais para a direita da camada base.

* **Alteração da posição de uma camada** - Para alterar a posição de uma camada na tela de desenho, selecione seu nome na lista Camadas e use uma destas técnicas:

* **Alterando manualmente a posição** - Mova o ponteiro para perto de, mas não acima de um limite de camada e, ao visualizar o cursor de seta de quatro pontas, selecione e comece a arrastar.

* **Inserção de medidas de deslocamento de posição** - Insira medidas de deslocamento X e Y nas caixas de texto X e Y. Essas medidas representam o deslocamento x e y do ponto de ancoragem em pixels.

* **Girar uma camada** - A caixa Girar lista o ângulo em que a camada foi girada. Para girar uma camada, selecione seu nome na lista Camadas e use uma destas técnicas:

* **Rotação manual** - Mover o cursor próximo a, mas não sobre um canto da camada. Ao ver o cursor de rotação, arraste o canto da camada. Mantenha pressionada a tecla Shift enquanto arrasta para girar em incrementos de 15 graus.

* **Informando uma medida de grau** - Insira o número de graus para girar a camada. A rotação é no sentido horário; para girar no sentido anti-horário, insira um número negativo.

**Ocultar uma camada ou um efeito de camada:**

Você pode ocultar uma camada ou um efeito de camada selecionando o ícone de olho ao lado do nome de uma camada ou do nome de um efeito. Camadas ocultas não aparecem em visualizações ou saída. As informações da camada não são excluídas do URL. Em vez disso, `hide=1` é adicionado ao URL para observar que a camada fica oculta da visualização. Por exemplo:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Determine a cor do plano de fundo, a opacidade e o modo de mesclagem {#determining-the-background-color-opacity-and-blend-mode}

Para escolher uma cor de plano de fundo, opacidade e modo de mesclagem para uma camada ou tela de desenho, selecione a camada ou tela de desenho e use estas técnicas:

* **Cor do primeiro plano** - Selecionar **[!UICONTROL Foreground Color]** e escolha uma amostra de cor para alterar a cor da sombra ou do brilho. Você também pode inserir um parâmetro de valor de cor na caixa. A cor do plano de fundo se aplica somente às camadas que usam transparência. Por exemplo, ela se aplica a uma camada parcialmente transparente em uma etiqueta de preço ou ao plano de fundo de um campo de texto. Camadas que consistem em uma imagem PSD, TIFF ou PNG com transparência ativada podem ter planos de fundo transparentes.

* **Cor do plano de fundo** - Selecionar **[!UICONTROL Background Color]** e escolha uma amostra de cor para alterar a cor das áreas preenchidas.

* **Opacidade** - Arraste o controle deslizante de Opacidade para tornar qualquer camada translúcida de forma que parte da imagem subjacente seja exibida. A configuração de 100% é opaca; 0 é transparente.

* **Modo de mesclagem** - Para simular um dos modos de mistura disponíveis no Photoshop, escolha uma opção. As opções são Normal, Dissolver, Clarear, Escurecer, Multiplicar e Tela. Essas opções estão disponíveis para camadas, não para a tela de desenho.

## Usar efeitos de sombra e brilho em camadas {#using-shadow-and-glow-effects-on-layers}

É possível aplicar sombra ou brilho a uma camada. A sombra ou o brilho é aplicado ao perímetro da camada e se estende para dentro ou para fora, dependendo da opção de sombra ou brilho escolhida. Se o modelo tiver sido originado com um arquivo PSD com efeitos de sombra e brilho, é possível ajustar esses efeitos no Adobe Dynamic Media Classic.

Depois de aplicar um efeito de sombra ou brilho, é possível ajustar seu tamanho, cor, opacidade e posição na área Propriedades da camada da tela Modelo.

### Aplicar um efeito de sombra ou brilho a uma camada {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Selecione uma camada na lista Camadas.
1. Selecione o menu Adicionar Efeito e escolha uma opção:

   * **[!UICONTROL Drop Shadow]** - Aplica uma sombra na parte inferior e no lado direito da camada.

   * **[!UICONTROL Inner Shadow]** - Aplica um efeito de sombra dentro de todas as bordas da camada.

   * **[!UICONTROL Outer Glow]** - Aplica um efeito de brilho em todas as bordas da camada.

   * **[!UICONTROL Inner Glow]** - Aplica um efeito de brilho dentro de todas as bordas da camada.

Um nome de efeito é exibido na lista Camadas depois de aplicar um efeito. Para excluir um efeito, selecione seu nome na lista Camadas e selecione **[!UICONTROL Delete]**.

>[!NOTE]
>
>Às vezes, não é possível ver o efeito de sombra projetada ou brilho externo se a camada subjacente não for grande o suficiente para exibi-la. Se não conseguir ver a sombra ou o brilho, considere adicionar valores de Preenchimento à camada ou reordenar a camada. Consulte [Alteração do tamanho e da posição das camadas e da tela de desenho](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) e [Reorganização de camadas](creating-template.md#reordering_layers).

### Ajustar um efeito de sombra ou brilho {#adjusting-a-shadow-or-glow-effect}

Para ajustar um efeito de sombra ou brilho, comece selecionando seu nome na lista Camadas. Em seguida, altere suas configurações na área Propriedades de camada da tela Modelo:

* **[!UICONTROL Color]** - Selecione o botão Cor e escolha uma amostra de cor para alterar a cor da sombra ou do brilho. Você também pode inserir um parâmetro de valor de cor na caixa.

* **[!UICONTROL Opacity]** - Arraste o controle deslizante para determinar a intensidade do efeito. Efeitos menos opacos são mais transparentes.

* **[!UICONTROL Blend Mode]** - Para simular um dos modos de mistura disponíveis no Photoshop, escolha uma opção. As opções são Normal, Dissolver, Clarear, Escurecer, Multiplicar e Tela.

* **[!UICONTROL Size]** - Insira medidas na caixa X e Y para aumentar ou reduzir o efeito de sombra. As opções de tamanho só estão disponíveis para sombras internas e sombras projetadas.

* **[!UICONTROL Grow]** - Arraste o controle deslizante para estender o efeito para dentro ou para fora.

* **[!UICONTROL Blur]** - Arraste o controle deslizante para controlar a difusão nas bordas do efeito. Efeitos com mais desfoque são mais emplumados.

## Mascarar camadas {#masking-layers}

A lista Camadas oferece um botão Máscara que especifica como a máscara ou o canal alfa de uma camada é usado. Usando o botão Máscara, é possível aplicar o efeito de uma camada de plano de fundo a uma camada específica ou a toda a camada pai no modelo. Selecione uma camada na lista Camadas e selecione **[!UICONTROL Mask]** para percorrer esses estados:

* O plano de fundo da camada é opaco.
* O conteúdo da camada é invertido e o plano de fundo da camada é preenchido com preto sólido.
* O plano de fundo da camada é preenchido com preto sólido.
