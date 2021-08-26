---
title: Criar um modelo
description: Saiba como criar um modelo no Adobe Dynamic Media Classic.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '3246'
ht-degree: 0%

---

# Criar um modelo {#creating-a-template}

Para criar um modelo, vá para **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. Selecione Designer ou Desenvolvedor. Nesta página, é possível adicionar camadas de imagem e texto. Também é possível reorganizar camadas, alterar o tamanho e a posição das camadas e aplicar efeitos de sombra e brilho a imagens e texto.

>[!NOTE]
>
>Se você editar um modelo criado em uma versão anterior do Adobe Dynamic Media Classic, um prompt o solicitará ao salvar &quot;Deseja adicionar uma camada de tela?&quot;. Selecione **[!UICONTROL No]** para evitar a adição de uma camada base. Se você selecionar **[!UICONTROL Yes]** acidentalmente, exclua os modificadores `&allowCanvasPrompt` e `&layer=0` no URL e pressione **[!UICONTROL Enter]** ou **[!UICONTROL Return]**.

## Criar o modelo inicial {#creating-the-initial-template}

Ao criar um conjunto de modelos, a opção **[!UICONTROL Publish after save]** afeta o conjunto e os membros do conjunto das seguintes maneiras:

| **[!UICONTROL Publish after save]** opção selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
| --- | --- | --- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros do conjunto mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

Você pode criar um template a partir de um template existente. Abra o modelo, selecione **[!UICONTROL Save As]** e insira um novo nome na caixa de diálogo Salvar como.

**Para criar o template inicial:**

1. Para criar seu template inicial, use um dos seguintes métodos:

   * **Selecione o PSD ou as imagens primeiro**  - No painel Procurar, selecione o arquivo PSD ou as imagens que deseja para o modelo, vá para  **[!UICONTROL Build]** >  **[!UICONTROL Template Basics]**.

   * **Comece na tela**  Modelo - Vá para  **[!UICONTROL Build]** >  **[!UICONTROL Template Basics]**. Selecione Designer ou Desenvolvedor.

1. Na caixa de diálogo Inserir tamanho da tela, insira as medidas de largura e altura do modelo.
1. Selecione uma pasta na Biblioteca de ativos e arraste o arquivo PSD ou as imagens desejadas para o modelo para a tela Modelo.
1. Quando terminar, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionado (padrão).
1. Selecione **[!UICONTROL Save]**.
1. Selecione uma pasta para armazenar o modelo, insira um nome para o modelo e selecione **[!UICONTROL Submit]**.

   O Adobe Dynamic Media Classic encolhe as imagens, se necessário, para ajustá-las à tela, a área na tela Modelo para definir seu modelo.

## Editar um conjunto de modelos {#editing-a-template-set}

Se você editar um conjunto publicado ou um conjunto de modelos não publicados, a opção **[!UICONTROL Publish after save]** afetará o conjunto e definirá membros das seguintes maneiras:

| Definir já publicado? | **[!UICONTROL Publish after save]** opção selecionada antes de salvar a edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
| --- | --- | --- | --- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado. Qualquer novo conjunto de membros adicionado durante a edição manterá o estado publicado ou não. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto adicionados durante a edição mantêm o estado publicado ou não. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um conjunto de modelos:**

1. Na Exibição de grade, navegue até um Conjunto de modelos e, em seguida, abaixo da imagem, selecione **[!UICONTROL Edit]**.
1. Altere o modelo conforme necessário.
1. Quando a edição for concluída, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionado (padrão).
1. Selecione **[!UICONTROL Save]**, selecione uma pasta de armazenamento, insira um nome para o conjunto e selecione **[!UICONTROL Save]**.

## Excluir um modelo {#deleting-a-template}

Ao excluir um conjunto de Modelos, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) desse conjunto não são afetados; em vez disso, cada um mantém seu estado publicado ou não publicado.

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um Modelo:**

1. Na Exibição de Grade, Exibição de Lista ou Exibição de Detalhes, selecione um ou mais Modelos.
1. Na Barra de Navegação Global, vá para **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.

## Entender a tela Modelo {#understanding-the-template-screen}

A tela Modelo oferece ferramentas para manipular e parametrizar camadas.

Use essas ferramentas na tela Modelo para criar modelos:

* **[!UICONTROL Pan]** - Permite selecionar camadas, movê-las ao redor da tela, redimensioná-las ou girá-las.

* **[!UICONTROL Text]** - Cria uma camada de texto. Arraste a tela para criar uma camada de texto e depois insira o texto na camada. Consulte [Criação de uma camada de texto](#creating-a-text-layer).

* **[!UICONTROL Preview]** - Abre a tela Visualização e mostra o modelo em um Visualizador de Zoom. Você verá a aparência do modelo para os usuários em seu site ou aplicativo.

* **[!UICONTROL Parameter Summary]** Abre a tela Resumo dos parâmetros. Você pode ver o nome de cada camada em um modelo e, em cada camada, os nomes dos parâmetros que foram ativados.

* **[!UICONTROL Text Editor v4.3 and Text Editor v4.2]** - Você pode optar por usar o editor de texto mais recente e completo, o Editor de texto v4.3 ou o editor de texto anterior, o Editor de texto v4.2. Ao criar modelos, o Editor de texto v4.3 é selecionado por padrão. Ao editar modelos mais antigos, o Editor de texto v4.2 é selecionado por padrão. No momento, o Editor de texto v4.3 não oferece suporte para quebra automática de texto, portanto, ao editar modelos mais antigos que usam quebra automática de texto, use o Editor de texto v4.2 para manter a fidelidade do modelo totalmente intacta. Se o modelo mais antigo não usar quebra automática de linha, você poderá escolher o Editor de texto v4.3 para aproveitar os vários recursos novos que ele oferece. Por exemplo, Aumentar Margens, Diminuir Margens, Definir Texto em Todas as Legendas e Copiar Ajustar Texto.

   >[!NOTE]
   >
   >O Editor de texto v4.2 está planejado para ser removido como uma opção no Adobe Dynamic Media Classic, portanto, é recomendável usar o Editor de texto 4.3 quando possível. A opção **[!UICONTROL Word Wrap]** será incorporada em uma versão futura do Editor de texto.

* **[!UICONTROL Designer and Developer]** - Selecione a opção que melhor descreve sua função.

* **[!UICONTROL Canvas]** - Define a área total disponível, em pixels, para definir seu modelo. O tamanho padrão é 300 x 300 pixels. As camadas são colocadas na tela.

* **[!UICONTROL Layers list]** - Lista o nome das camadas no modelo. Para selecionar uma camada, selecione seu nome na lista Camadas. A lista de Camadas oferece ferramentas para adicionar efeitos a camadas, excluir camadas, reordenar camadas e parametrizar camadas. Consulte [Trabalhar com camadas](#working-with-layers).

* **[!UICONTROL Layer Properties area]** - Oferece ferramentas para alterar a cor do plano de fundo, a opacidade, o tamanho e a posição de uma camada, bem como a cor do plano de fundo, a opacidade e o tamanho da tela. Também é possível ajustar os efeitos de sombra e brilho. Consulte [Trabalhar com camadas](#working-with-layers).

## Criar camadas de imagem {#creating-image-layers}

1. Arraste a imagem da Biblioteca de ativos para a tela.

   O nome da ID da imagem aparece na lista de Camadas.

   >[!NOTE]
   >
   >Se necessário, o Adobe Dynamic Media Classic encolhe as imagens para ajustá-las à tela ao criar uma camada de imagem.

## Criar uma camada de texto {#creating-a-text-layer}

1. Selecione a ferramenta **[!UICONTROL Text]**.
1. Arraste para criar uma caixa de texto na tela ou em uma imagem.
1. Na tela de texto que é aberta, adicione texto seguindo um destes procedimentos na guia Visualizar :

   * Digite o texto na caixa de texto. Escolha Copiar texto para ajustar o texto na caixa de texto.
   * Cole o texto da Área de transferência na caixa de texto.

1. Selecione **[!UICONTROL Apply]** e feche a tela Texto.

### Formatar texto {#format-text}

Para formatar o texto em uma camada de texto, faça o seguinte:

1. Na lista Camadas, clique duas vezes no nome da caixa de texto com o texto que deseja editar. O Editor de texto é aberto.
1. Na caixa de texto do Editor de texto, selecione o texto que deseja formatar. Você pode selecionar todo o texto, partes do texto ou caracteres individuais.
1. Especifique qualquer uma das opções de formatação a seguir e selecione **[!UICONTROL Apply]**.

   * **[!UICONTROL Font]** - Escolha uma fonte no menu Fonte. Se uma fonte desejada não aparecer no menu, você poderá carregá-la no Adobe Dynamic Media Classic. Consulte Fontes.

   * **[!UICONTROL Font Size]** - Escolha um tamanho de fonte no menu, digite um tamanho específico na caixa ou selecione as  **[!UICONTROL Up]** setas  **[!UICONTROL Down]** ou para aumentar ou diminuir o tamanho em dois pontos.

   * **[!UICONTROL Color]** - Selecione para escolher uma cor para o texto.

   * **[!UICONTROL Bold]**,  **[!UICONTROL Italic]** ou  **[!UICONTROL Underline]** - Selecione o texto e selecione o ícone do tipo de formatação que deseja aplicar ao texto.

   * **[!UICONTROL All Caps]**,  **[!UICONTROL Superscript]** ou  **[!UICONTROL Subscript]** - Selecione o texto e selecione o ícone do tipo de formatação que deseja aplicar ao texto.

   * **[!UICONTROL Alignment]** - Escolha um botão Alinhamento para alinhar o texto à esquerda, ao centro ou ao alinhamento à direita na camada de texto.

   * **[!UICONTROL Tracking]** - Digite ou selecione um valor numérico para ajustar a quantidade de espaço entre palavras.

   * **[!UICONTROL Kerning]** - Digite ou selecione um valor numérico para ajustar a quantidade de espaço entre caracteres.

   * **[!UICONTROL Line Spacing]** - Digite ou selecione um valor numérico para ajustar a quantidade de espaço entre as linhas.

   * **[!UICONTROL Baseline Shift]** - Digite ou selecione um valor numérico para mover um caractere selecionado para cima ou para baixo em relação à linha de base do texto ao redor. Essa opção é especialmente útil quando você está configurando frações manualmente ou ajustando a posição dos gráficos em linha.

>[!NOTE]
>
>Selecione **[!UICONTROL Undo]** se desejar reverter a última ação. Selecione **[!UICONTROL Redo]** se você mudar de ideia sobre a inversão de uma ação depois de selecionar **[!UICONTROL Undo]**.

### Formatar parágrafos {#format-paragraphs}

1. Na lista Camadas, clique duas vezes no nome da caixa de texto com o texto que deseja editar. O Editor de texto é aberto.
1. Selecione o parágrafo que deseja formatar.
1. Especifique qualquer uma das opções de formatação a seguir e selecione **[!UICONTROL Apply]**.

   * **[!UICONTROL Alignment]** - Selecione para especificar o tipo de alinhamento: alinhar à esquerda, alinhar ao centro, alinhar à direita ou justificar.

   * **[!UICONTROL End of Paragraph Justification]** - Selecione para especificar o tipo de justificação para a última linha no parágrafo: alinhamento da última linha à esquerda; centro de alinhamento da última linha; e a última linha se alinha à direita.

   * **[!UICONTROL Line Spacing]** - Digite ou selecione um valor numérico para ajustar a quantidade de espaço entre todas as linhas do parágrafo.

   * **[!UICONTROL Indent All]** - Selecione para aumentar a quantidade de recuo do texto.

   * **[!UICONTROL Remove Indent]** - Selecione para diminuir a quantidade de recuo do texto.

   * **[!UICONTROL Indent First Line]** - Especifique a quantidade pela qual você deseja recuar a primeira linha de texto.

   * **[!UICONTROL Space Before Paragraph]** - Especifique a quantidade de espaço que deseja que apareça acima da primeira linha de texto do parágrafo.

   * **[!UICONTROL Space After Paragraph]** - Especifique a quantidade de espaço que deseja que apareça abaixo da última linha de texto no parágrafo.

   * **[!UICONTROL Vertical Align]** - Selecione onde deseja que o texto apareça verticalmente na caixa de texto: Parte Superior, Meio, Parte Inferior.

   * **[!UICONTROL Text Direction]** - Selecione a direção na qual deseja que o texto seja exibido: Da Direita Para A Esquerda Ou Da Esquerda Para A Direita.

### Ajustar propriedades da camada de texto {#adjust-text-layer-properties}

1. Na tela Noções básicas sobre modelo , selecione a caixa de texto que deseja ajustar.
1. No painel Propriedades da camada , selecione uma das seguintes opções:

   * **[!UICONTROL Shrink Text (Text Editor v4.2 only)]** - Para ajustar na caixa de texto, selecione para reduzir o texto.

   * **[!UICONTROL Word Wrap (Text Editor v4.2 only)]** - Para especificar se ou como o texto será colocado, selecione uma opção de quebra automática:

   * **[!UICONTROL Wrap]** - Quebra o texto para ajustá-lo a uma caixa de texto horizontalmente muito pequena.

   * **[!UICONTROL No Wrap]** - Não envolve o texto quando a caixa de texto é muito pequena horizontalmente e, em vez disso, corta uma parte do texto.

   * **[!UICONTROL Nonbreaking Wrap]** - Quebra o texto para ajustá-lo a uma caixa de texto e não quebra palavras.

   * **[!UICONTROL Position]** - Especifica o local da caixa de texto na tela.

   * **[!UICONTROL Padding]** - Adiciona margens ou corta o retângulo da camada. Especifique o número de pixels que deseja adicionar ou remover para Esquerda, Parte Superior, Parte Inferior e Direita. Insira números positivos se desejar adicionar uma margem ou números negativos para cortar.

### Exibir e editar o código fonte de texto {#view-and-edit-text-source-code}

As informações fornecidas na guia Origem do Editor de texto são para referência. Edite o texto somente se estiver familiarizado com a edição do código-fonte.

1. Na lista Camadas, clique duas vezes no nome da caixa de texto com o texto que deseja editar. O Editor de texto é aberto.
1. No Editor de texto, para revelar o código-fonte do texto, selecione a guia **[!UICONTROL Source]** no Editor de texto.
1. Exiba ou edite o texto conforme desejado.

   As alterações permanecerão intactas se você alternar entre a Visualização e a Visualização de origem.

1. Selecione **[!UICONTROL Apply]** para renderizar as edições.

## Trabalhar com camadas {#working-with-layers}

Use a lista Camadas e a área Propriedades da camada para trabalhar com camadas. É possível reordenar as camadas, alterar seu tamanho e posição, girar as camadas e determinar a cor do plano de fundo, a cor do primeiro plano, a opacidade e o modo de mesclagem de uma camada.

Você também pode alterar o tamanho da tela, escolher a cor de plano de fundo e alterar a configuração de opacidade.

### Reordenar camadas {#reordering-layers}

Alterar a ordem da camada pode afetar a aparência, especialmente quando a transparência ou a impressão excessiva estiver envolvida. Certifique-se de visualizar o resultado antes de confirmar as alterações.

1. Use uma dessas técnicas para reordenar as camadas em um modelo:

   * Selecione uma camada na lista Camadas. Em seguida, selecione **[!UICONTROL Up]** ou **[!UICONTROL Down]** quantas vezes forem necessárias para colocá-lo na posição correta na lista.
   * Arraste uma camada para cima ou para baixo na lista Camadas.

### Alterar o tamanho e a posição das camadas e da tela {#changing-the-size-and-position-of-layers-and-the-canvas}

As camadas devem ser pequenas o suficiente para caber na tela. Você pode alterar o tamanho de uma camada ou da tela manualmente ou inserindo medidas de tamanho. Você pode alterar a posição de uma camada manualmente ou inserindo medidas de deslocamento. Também é possível girar uma camada.

>[!NOTE]
>
>O Adobe Dynamic Media Classic recomenda criar uma predefinição de imagem que tenha o tamanho exato do modelo. A correspondência do tamanho da predefinição de imagem ao tamanho do modelo garante que o tamanho de saída final e as opções de nitidez do modelo sejam definidos corretamente. Depois de criar essa predefinição de imagem, você pode escolhê-la no menu Aplicar predefinição na tela Visualização do modelo. A tela mostra a aparência da imagem quando ela é entregue pelo servidor. Consulte [Configurar predefinições de imagem](setting-image-presets.md#setting_up_image_presets).

* **Alteração do tamanho de uma camada**  - Para alterar o tamanho de uma camada ou da tela, selecione a camada ou a tela na lista Camadas e use uma destas técnicas:

* **Alteração manual do tamanho**  - Selecione e arraste um canto da camada ou da tela. Com camadas de texto, também é possível arrastar um lado da camada. Mantenha pressionada a tecla Shift enquanto arrasta para alterar o tamanho, mas mantém a proporção (a forma).

* **Inserir medidas de tamanho da camada**  - Insira medidas de pixel nas caixas de texto W (Largura) e H (Altura) na área Propriedades da camada.

Além de alterar o tamanho de uma camada, você pode colá-la. Para fazer isso, insira uma medida de Preenchimento nas caixas Esquerda, Direita, Superior e Inferior da área Propriedades da camada. O preenchimento adiciona uma margem à camada atual para deslocá-la do perímetro da camada base. O preenchimento é útil se você adicionar um efeito de sombra ou brilho externo e quiser tornar o efeito mais visível. O preenchimento aumenta o tamanho de uma camada e exibe sua cor de plano de fundo na área estendida e preenchida. A camada base se reposiciona em relação ao novo tamanho da camada. Por exemplo, se a camada atual estiver centralizada na camada base, estender o lado esquerdo da camada a move ainda mais para a direita da camada base.

* **Alteração da posição de uma camada**  - Para alterar a posição de uma camada na tela, selecione seu nome na lista Camadas e use uma destas técnicas:

* **Alteração manual da posição**  - Mova o ponteiro para perto, mas não sobre, um limite de camada e, ao ver o cursor de seta de quatro pontas, selecione e comece a arrastar.

* **Inserindo medidas de deslocamento de posição**  - Insira as medidas de deslocamento X e Y nas caixas de texto X e Y. Essas medidas representam o deslocamento x, y do ponto de ancoragem em pixels.

* **Girar uma camada**  - A caixa Girar lista o ângulo no qual a camada foi girada. Para girar uma camada, selecione seu nome na lista Camadas e use uma destas técnicas:

* **Girar manualmente**  - mova o cursor para perto, mas não sobre, um canto da camada. Ao visualizar o cursor de giro, arraste o canto da camada. Mantenha a tecla Shift pressionada ao arrastar para girar em incrementos de 15 graus.

* **Inserir uma medida de grau**  - Insira o número de graus para girar a camada. A rotação é no sentido dos ponteiros do relógio; para girar no sentido anti-horário, insira um número negativo.

**Ocultar uma camada ou um efeito de camada:**

É possível ocultar uma camada ou um efeito de camada selecionando o ícone de olho ao lado do nome da camada ou do nome do efeito. As camadas ocultas não aparecem em visualizações ou saídas. As informações da camada não são excluídas do URL. Em vez disso, `hide=1` é adicionado ao URL para observar que a camada está oculta da exibição. Por exemplo:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Determine a cor do plano de fundo, a opacidade e o modo de mesclagem {#determining-the-background-color-opacity-and-blend-mode}

Para escolher uma cor de plano de fundo, uma opacidade e um modo de mesclagem para uma camada ou a tela, selecione a camada ou a tela e use estas técnicas:

* **Cor do primeiro plano**  - Selecione  **[!UICONTROL Foreground Color]** e escolha uma amostra de cores para alterar a cor da sombra ou do brilho. Você também pode inserir um parâmetro de valor de cor na caixa . A cor de plano de fundo se aplica somente às camadas que usam transparência. Por exemplo, ela se aplica a uma camada parcialmente transparente em uma tag de preço ou ao plano de fundo de um campo de texto. As camadas que consistem em uma imagem PSD, TIFF ou PNG com transparência ativada podem ter planos de fundo transparentes.

* **Cor do plano de fundo**  - Selecione  **[!UICONTROL Background Color]** e escolha uma amostra de cores para alterar a cor das áreas preenchidas.

* **Opacidade**  - Arraste o controle deslizante Opacidade para tornar qualquer camada translúcida, para que parte da imagem subjacente seja exibida. A configuração de 100% é opaca; 0 é transparente.

* **Modo de mesclagem**  - Para simular um dos modos de mesclagem disponíveis no Photoshop, escolha uma opção. As opções são Normal, Dissolver, Claro, Escuro, Multiplicar e Tela. Essas opções estão disponíveis para camadas, não para a tela.

## Usar efeitos de sombra e brilho em camadas {#using-shadow-and-glow-effects-on-layers}

Você pode aplicar uma sombra ou brilho a uma camada. A sombra ou o brilho é aplicado ao perímetro da camada e se estende para dentro ou para fora, dependendo da opção de sombra ou brilho escolhida. Se o modelo se originou de um arquivo PSD com efeitos de sombra e brilho, você pode ajustar esses efeitos no Adobe Dynamic Media Classic.

Depois de aplicar um efeito de sombra ou brilho, você pode ajustar o tamanho, a cor, a opacidade e a posição na área Propriedades da camada da tela Modelo.

### Aplicar um efeito de sombra ou brilho a uma camada {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Selecione uma camada na lista Camadas.
1. Selecione o menu Adicionar efeito e escolha uma opção:

   * **[!UICONTROL Drop Shadow]** - Aplica uma sombra ao lado inferior e direito da camada.

   * **[!UICONTROL Inner Shadow]** - Aplica um efeito de sombra dentro de todas as bordas da camada.

   * **[!UICONTROL Outer Glow]** - Aplica um efeito de brilho em todas as bordas da camada.

   * **[!UICONTROL Inner Glow]** - Aplica um efeito de brilho dentro de todas as bordas da camada.

Um nome de efeito aparece na lista de Camadas depois de aplicar um efeito. Para excluir um efeito, selecione o nome na lista Camadas e selecione **[!UICONTROL Delete]**.

>[!NOTE]
>
>Às vezes, não é possível ver o efeito de uma sombra ou brilho externo se a camada subjacente não for grande o suficiente para exibi-la. Se você não conseguir ver a sombra ou o brilho, considere adicionar os valores de Preenchimento à camada ou reorganizar a camada. Consulte [Alteração do tamanho e da posição das camadas e da tela](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) e [Reordenação de camadas](creating-template.md#reordering_layers).

### Ajustar um efeito de sombra ou brilho {#adjusting-a-shadow-or-glow-effect}

Para ajustar um efeito de sombra ou brilho, comece selecionando o nome na lista Camadas. Em seguida, altere suas configurações na área Propriedades da camada da tela Modelo :

* **[!UICONTROL Color]** - Selecione o botão Color e escolha uma amostra de cor para alterar a cor da sombra ou do brilho. Você também pode inserir um parâmetro de valor de cor na caixa .

* **[!UICONTROL Opacity]** - Arraste o controle deslizante para determinar a intensidade do efeito. Os efeitos menos opacos são mais transparentes.

* **[!UICONTROL Blend Mode]** - Para simular um dos modos de mesclagem disponíveis no Photoshop, escolha uma opção. As opções são Normal, Dissolver, Claro, Escuro, Multiplicar e Tela.

* **[!UICONTROL Size]** - Insira medidas na caixa X e Y para aumentar ou diminuir o efeito de sombra. As opções de tamanho só estão disponíveis para sombras internas e sombras.

* **[!UICONTROL Grow]** - Arraste o controle deslizante para estender o efeito para dentro ou para fora.

* **[!UICONTROL Blur]** - Arraste o controle deslizante para controlar a captura nas bordas do efeito. Os efeitos com mais desfoque são mais afetados.

## Mascarar camadas {#masking-layers}

A lista de Camadas oferece um botão Máscara que especifica como a máscara ou o canal alfa de uma camada é usado. Usando o botão Máscara, você pode aplicar o efeito de uma camada de plano de fundo a uma camada específica ou a toda a camada pai em seu modelo. Selecione uma camada na lista Camadas e selecione **[!UICONTROL Mask]** para percorrer esses estados:

* O plano de fundo da camada é opaco.
* O conteúdo da camada é invertido e o plano de fundo da camada é preenchido com preto sólido.
* O fundo da camada é preenchido com preto sólido.
