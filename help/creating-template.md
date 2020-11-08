---
title: Criação de um modelo
seo-title: Criação de um modelo
description: nulo
seo-description: Saiba como criar um modelo no Dynamic Media Classic.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '3441'
ht-degree: 0%

---


# Criação de um modelo {#creating-a-template}

Para criar um modelo, clique em Criar > Noções básicas do modelo. Selecione Designer ou Desenvolvedor. Nessa página, é possível adicionar camadas de imagem e texto. Também é possível reordenar camadas, alterar o tamanho e a posição das camadas e aplicar efeitos de sombra e brilho a imagens e texto.

>[!NOTE]
>
>Se você editar um modelo criado em uma versão anterior do Dynamic Media Classic, poderá receber um prompt ao salvar perguntando &quot;Deseja adicionar uma camada de tela?&quot; Escolha Não para evitar a adição de uma nova camada base. Se você acidentalmente escolher Sim, exclua os modificadores &quot;&amp;allowCanvasPrompt&quot; e &quot;&amp;layer=0&quot; no URL e pressione Enter ou Return.

## Criando o modelo inicial {#creating-the-initial-template}

Quando você cria um conjunto de modelos, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| opção &quot;Publicar após salvar&quot; selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos retêm seu estado publicado ou não publicado. |

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually_publishing_assets) a publicação de ativos [](publishing-files.md#manually_unpublishing_assets)manualmente.

Você pode criar um modelo a partir de um modelo existente. Abra o modelo, clique em **Salvar como** e insira um novo nome na caixa de diálogo Salvar como.

**Para criar o Conjunto de templos inicial**

1. Para criar seu modelo, use um dos seguintes métodos:

   **Selecione o PSD ou as imagens primeiro** no painel Procurar, selecione o arquivo PSD ou as imagens que deseja para o modelo e clique em Criar > Noções básicas do modelo.

   **Start da tela** Modelo Clique em Criar > Noções básicas do modelo. Selecione Designer ou Desenvolvedor.

1. Na caixa de diálogo Inserir tamanho da tela de desenho, insira medidas de largura e altura para o modelo.
1. Selecione uma pasta na Biblioteca de ativos e arraste o arquivo PSD ou as imagens desejadas para o seu modelo para a tela Modelo.
1. Quando terminar, próximo ao canto inferior direito da página, verifique se a opção **Publicar após salvar** está selecionada (padrão).
1. Clique em **Salvar**.
1. Selecione uma pasta para armazenar seu modelo, insira um nome para o modelo e clique em **Enviar**.

   O Dynamic Media Classic reduz as imagens, se necessário, para ajustá-las à tela, a área na tela Modelo para definir seu modelo.

## Edição de um conjunto de modelos {#editing-a-template-set}

Dependendo de se você editar um conjunto publicado ou um conjunto de modelos não publicado, a opção **Publicar após salvar** afetará o conjunto e definirá os membros das seguintes maneiras:

| Definir já publicado? | Opção &quot;Publicar após salvar&quot; selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado.Qualquer novo conjunto de membros adicionado durante a edição mantém seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto que você tiver adicionado durante a edição manterão seu estado publicado ou não publicado. |

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually_publishing_assets) a publicação de ativos [](publishing-files.md#manually_unpublishing_assets)manualmente.

**Para editar um conjunto de modelos**

1. Na visualização de grade, navegue até um conjunto de modelos e, abaixo da imagem, clique em **Editar**.
1. Faça alterações no modelo, conforme necessário.
1. Quando terminar a edição, próximo ao canto inferior direito da página, certifique-se de que a opção **Publicar após salvar** esteja selecionada (padrão).
1. Clique em **Salvar**, selecione uma pasta de armazenamento, digite um nome para o conjunto e clique em **Salvar**.

## Excluindo um Modelo {#deleting-a-template}

Quando você exclui um conjunto de modelos, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um deles mantém seu estado publicado ou não publicado.

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually_publishing_assets) a publicação de ativos [](publishing-files.md#manually_unpublishing_assets)manualmente.

**Para excluir um modelo**

1. Na Visualização de grade, Visualização de Lista ou Detalhes, selecione um ou mais modelos.
1. Na barra de navegação global, clique em **Arquivo** > **Excluir** > **Excluir**.

## Como entender a tela Modelo {#understanding-the-template-screen}

A tela Modelo oferta ferramentas para manipular e parametrizar camadas.

Use essas ferramentas na tela Modelo para criar modelos:

**Ferramenta** DeslocamentoPermite selecionar camadas, movê-las ao redor da tela, redimensioná-las ou girá-las.

**Ferramenta** Texto Cria uma camada de texto. Arraste na tela de desenho para criar uma camada de texto e insira o texto na camada. Consulte Criar uma camada de texto.

**Botão** pré-visualização Abre a tela Pré-visualização e mostra o modelo em um Visualizador de zoom. Você verá a aparência do modelo para os usuários em seu site ou aplicativo.

**Botão** Resumo de parâmetros Abre a tela Resumo de parâmetros. É possível ver o nome de cada camada em um modelo e, em cada camada, os nomes dos parâmetros que foram ativados.

**Editor de texto v4.3 e Editor de texto v4.2** Você pode optar por usar o editor de texto mais recente e completo, o Editor de texto v4.3 ou o editor de texto anterior, o Editor de texto v4.2. Ao criar novos modelos, o Editor de texto v4.3 é selecionado por padrão. Ao editar modelos mais antigos, o Editor de texto v4.2 é selecionado por padrão. No momento, o Editor de texto v4.3 não oferece suporte para quebra automática de texto, portanto, ao editar modelos mais antigos que usam quebra automática de texto, use o Editor de texto v4.2 para manter a fidelidade do modelo totalmente intacta. Se o seu modelo mais antigo não usar quebra automática de texto, você poderá escolher o Editor de texto v4.3 para aproveitar os vários recursos novos que ele oferta, como Aumentar margens, Diminuir margens, Definir texto em todas as letras maiúsculas e Copiar ajuste de texto.

***observação **: O Editor de texto v4.2 será eventualmente removido como uma opção no Dynamic Media Classic, portanto, recomenda-se usar o Editor de texto 4.3 quando possível. A opção Quebra automática de texto será incorporada a uma versão futura do Editor de texto.*

**Designer e Desenvolvedor** Selecione a opção que melhor descreve sua função.

**Tela** Define a área total disponível, em pixels, para a definição do modelo. O tamanho padrão é 300 x 300 pixels. As camadas são colocadas na tela.

**A lista** Camadas Lista o nome das camadas no modelo. Para selecionar uma camada, selecione seu nome na lista Camadas. A lista Camadas oferta as ferramentas para adicionar efeitos a camadas, excluir camadas, reordenar camadas e parametrizar camadas. Consulte Trabalhar com camadas.

**Área** Propriedades da camada Oferta ferramentas para alterar a cor, a opacidade, o tamanho e a posição do plano de fundo de uma camada, bem como a cor, a opacidade e o tamanho do plano de fundo da tela. Você também pode ajustar os efeitos de sombra e brilho. Consulte Trabalhar com camadas.

## Criação de camadas de imagem {#creating-image-layers}

1. Arraste a imagem da Biblioteca de ativos para a tela.

   O nome da ID da imagem é exibido na lista Camadas.

>[!NOTE]
>
>Se necessário, o Dynamic Media Classic reduz as imagens para ajustá-las à tela quando você cria uma camada de imagem.

## Criação de uma camada de texto {#creating-a-text-layer}

1. Clique na ferramenta Texto.
1. Arraste para criar uma caixa de texto na tela ou em uma imagem.
1. Na tela de texto que é aberta, adicione texto executando qualquer uma das seguintes ações na guia Pré-visualização:

   * Digite o texto na caixa de texto. Escolha Copiar Ajuste de Texto para ajustar o texto à caixa de texto.
   * Cole o texto da Área de transferência na caixa de texto.

1. Clique em Aplicar e feche a tela Texto.

### Formatar texto {#format-text}

Siga estas etapas para formatar o texto em uma camada de texto:

1. Na lista Camadas, clique com o duplo do mouse no nome da caixa de texto com o texto que deseja editar. O Editor de texto é aberto.
1. Na caixa de texto, selecione o texto que deseja formatar. Você pode selecionar todo o texto, partes do texto, bem como caracteres individuais.
1. Especifique qualquer uma dessas opções de formatação e clique em Aplicar.

   **Fonte** Escolha uma fonte no menu Fonte. Se uma fonte desejada não aparecer no menu, você pode fazer upload dela no Dynamic Media Classic. Consulte Fontes.

   **Tamanho** da fonte Escolha um tamanho de fonte no menu, digite um tamanho específico na caixa ou clique nas setas para cima ou para baixo para aumentar ou diminuir o tamanho em dois pontos.

   **Cor** Clique para escolher uma cor para o texto.

   **Negrito, Itálico ou Sublinhado** Selecione o texto e clique no ícone do tipo de formatação que deseja aplicar ao texto.

   **Todas em maiúsculas, sobrescrito ou subscrito** Selecione o texto e clique no ícone do tipo de formatação que deseja aplicar ao texto.

   **Alinhamento** Escolha um botão Alinhamento para alinhar o texto à esquerda, ao centro ou à direita na camada de texto.

   **Tipo de rastreamento** ou selecione um valor numérico pelo qual ajustar a quantidade de espaço entre as palavras.

   **Tipo de ajuste de espaço** ou selecione um valor numérico pelo qual ajustar a quantidade de espaço entre os caracteres.

   **Tipo de espaçamento** da linha ou selecione um valor numérico pelo qual ajustar a quantidade de espaço entre as linhas.

   **Deslocamento** da linha de baseDigite ou selecione um valor numérico para mover um caractere selecionado para cima ou para baixo em relação à linha de base do texto ao redor. Essa opção é especialmente útil quando você configura frações manualmente ou ajusta a posição de gráficos em linha.

>[!NOTE]
>
>Clique em Desfazer para reverter a última ação. Clique em Refazer se você mudar de ideia sobre reverter uma ação depois de clicar em Desfazer.

### Formatar parágrafos {#format-paragraphs}

1. Na lista Camadas, clique com o duplo do mouse no nome da caixa de texto com o texto que deseja editar. O Editor de texto é aberto.
1. Selecione o parágrafo que deseja formatar.
1. Especifique qualquer uma dessas opções de formatação e clique em Aplicar.

   **Alinhamento** Clique para especificar o tipo de alinhamento: alinhar à esquerda, alinhar ao centro, alinhar à direita ou justificar.

   **Justificação** de fim de parágrafo Clique para especificar o tipo de justificação para a última linha no parágrafo: alinhamento da última linha à esquerda; centro de alinhamento da última linha; e a última linha se alinha à direita.

   **Tipo de espaçamento** de linha ou selecione um valor numérico pelo qual ajustar a quantidade de espaço entre todas as linhas no parágrafo.

   **Recuar todos** os cliques para aumentar a quantidade de recuo do texto.

   **Remover recuo** Clique para diminuir a quantidade de recuo do texto.

   **Recuar primeira linha** Especifique a quantidade pela qual deseja recuar a primeira linha de texto.

   **Espaço antes do parágrafo** Especifique a quantidade de espaço que deseja exibir acima da primeira linha de texto no parágrafo.

   **Espaço após parágrafo** Especifique a quantidade de espaço que deseja exibir abaixo da última linha de texto no parágrafo.

   **Alinhamento** vertical Selecione o local em que deseja que o texto apareça verticalmente na caixa de texto: Parte Superior, Meio, Parte Inferior.

   **Direção** do texto Selecione a direção na qual deseja que o texto seja exibido: Da Direita Para A Esquerda Ou Da Esquerda Para A Direita.

### Ajustar propriedades da camada de texto {#adjust-text-layer-properties}

1. Na tela Informações básicas sobre o modelo, selecione a caixa de texto que deseja ajustar.
1. No painel Propriedades da camada, selecione uma das seguintes opções:

   **Reduzir texto (somente Editor de texto v4.2)** Selecione para reduzir o texto para ajustá-lo à caixa de texto.

   **Quebra automática de linha (somente Editor de texto v4.2)** Selecione uma opção de quebra automática para especificar se o texto envolve ou como:

   **Vincular** Vincula o texto para ajustá-lo a uma caixa de texto que é muito pequena horizontalmente.

   **Sem quebra** não quebra o texto quando a caixa de texto é muito pequena horizontalmente e, em vez disso, corta uma parte do texto.

   **NB Quebrar** (Quebra automática de linha) Quebra o texto para ajustar a uma caixa de texto e não quebra palavras.

   **Posição** Especifica o local da caixa de texto na tela.

   **Preenchimento** Adiciona margens ou corta o retângulo da camada. Especifique o número de pixels a serem adicionados ou removidos para Esquerda, Superior, Inferior e Direita. Insira números positivos para adicionar uma margem; insira números negativos para cortar.

### Visualização e edição do código fonte de texto {#view-and-edit-text-source-code}

As informações fornecidas na guia Origem do Editor de texto são para sua referência. Edite o texto somente se estiver familiarizado com a edição do código-fonte.

1. Na lista Camadas, clique com o duplo do mouse no nome da caixa de texto com o texto que deseja editar. O Editor de texto é aberto.
1. Clique na guia Origem no Editor de texto para revelar o código-fonte do texto.
1. Visualização ou edite o texto conforme desejado.

   As alterações permanecerão intactas se você alternar entre a Pré-visualização e a visualização de origem.

1. Clique em Aplicar para renderizar as edições.

## Trabalhar com camadas {#working-with-layers}

Use a lista Camadas e a área Propriedades da camada para trabalhar com camadas. É possível reordenar as camadas, alterar seu tamanho e posição, girar as camadas e determinar a cor do plano de fundo, a cor do primeiro plano, a opacidade e o modo de mesclagem de uma camada.

Você também pode alterar o tamanho da tela de desenho, escolher sua cor de plano de fundo e alterar sua configuração de opacidade.

### Reorganização de camadas {#reordering-layers}

Alterar a ordem de camadas pode afetar a aparência, especialmente quando a transparência ou a superimposição estiver envolvida. Certifique-se de pré-visualização no resultado antes de confirmar suas alterações.

1. Use uma destas técnicas para reordenar as camadas em um modelo:

   * Selecione uma camada na lista Camadas. Em seguida, clique no botão Para cima ou Para baixo quantas vezes forem necessárias para colocá-lo na posição correta na lista.
   * Arraste uma camada para cima ou para baixo na lista Camadas.

### Alteração do tamanho e da posição das camadas e da tela {#changing-the-size-and-position-of-layers-and-the-canvas}

As camadas devem ser pequenas o suficiente para se ajustarem à tela. É possível alterar o tamanho de uma camada ou da tela manualmente ou inserindo medidas de tamanho. É possível alterar a posição de uma camada manualmente ou inserindo medidas de deslocamento. Também é possível girar uma camada.

>[!NOTE]
>
>O Dynamic Media Classic recomenda a criação de uma predefinição de imagem com o tamanho exato do modelo. A correspondência do tamanho da predefinição de imagem com o tamanho do modelo garante que o tamanho de saída final e as opções de nitidez do modelo sejam definidos corretamente. Depois de criar essa predefinição de imagem, você pode escolhê-la no menu Aplicar predefinição na tela Pré-visualização de modelo. A tela mostra a aparência da imagem quando ela é entregue pelo servidor. Consulte [Configuração de predefinições](setting-image-presets.md#setting_up_image_presets)de imagem.

**Alteração do tamanho de uma camada**

Para alterar o tamanho de uma camada ou da tela, selecione a camada ou a tela na lista Camadas e use uma destas técnicas:

**Alteração manual do tamanho** Selecione e arraste um canto da camada ou da tela. Com camadas de texto, também é possível arrastar um lado da camada. Mantenha pressionada a tecla Shift enquanto arrasta para alterar o tamanho, mas mantém a proporção (a forma).

**Inserir medidas** de tamanho de camada Insira medidas de pixel nas caixas de texto L (Largura) e A (Altura) na área Propriedades de camada.

Além de alterar o tamanho de uma camada, você pode colá-la. Para fazer isso, digite uma medida de Preenchimento na caixa Esquerda, Direita, Superior e Inferior da área Propriedades da camada. O preenchimento adiciona uma margem à camada atual para deslocá-la do perímetro da camada base. O preenchimento é útil se você adicionar um efeito de sombra projetada ou de brilho externo e quiser tornar o efeito mais visível. O preenchimento aumenta o tamanho de uma camada e exibe sua cor de plano de fundo na área estendida e preenchida. A camada base se reposiciona em relação ao novo tamanho da camada. Por exemplo, se a camada atual estiver centralizada na camada base, a extensão do lado esquerdo da camada a moverá para a direita da camada base.

**Alteração da posição de uma camada**

Para alterar a posição de uma camada na tela, selecione seu nome na lista Camadas e use uma destas técnicas:

**Alteração manual da posição** Mova o ponteiro para perto, mas não acima, de um limite de camada e, ao ver o cursor de seta de quatro pontas, clique e arraste do start.

**Informando medidas** de deslocamento de posiçãoInsira medidas de deslocamento X e Y nas caixas de texto X e Y. Essas medidas representam o deslocamento x, y do ponto de ancoragem em pixels.

**Girar uma camada**

A caixa Girar lista o ângulo no qual a camada foi girada. Para girar uma camada, selecione seu nome na lista Camadas e use uma destas técnicas:

**Girar** manualmenteMove o cursor próximo a, mas não sobre, um canto da camada. Quando o cursor de rotação for exibido, arraste o canto da camada. Mantenha pressionada a tecla Shift enquanto arrasta para girar em incrementos de 15 graus.

**Inserindo uma medida** de grauInsira o número de graus para girar a camada. A rotação é no sentido horário; para girar no sentido anti-horário, insira um número negativo.

**Ocultar uma camada ou um efeito de camada**

É possível ocultar uma camada ou um efeito de camada clicando no ícone de olho ao lado do nome da camada ou do efeito. As camadas ocultas não aparecem no pré-visualização ou na saída. As informações da camada não são excluídas do URL. Em vez disso, &quot;hide=1&quot; é adicionado ao URL para observar que a camada está atualmente oculta da visualização. Por exemplo:

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;hide=1&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

### Determinar a cor, a opacidade e o modo de mesclagem do plano de fundo {#determining-the-background-color-opacity-and-blend-mode}

Para escolher uma cor de plano de fundo, opacidade e modo de mesclagem para uma camada ou tela de desenho, selecione a camada ou a tela de desenho e use estas técnicas:

**Cor** do primeiro plano Clique no botão Cor do primeiro plano e escolha uma amostra de cor para alterar a cor da sombra ou do brilho. Também é possível inserir um parâmetro de valor de cor na caixa. A cor de plano de fundo se aplica somente às camadas que usam transparência. Por exemplo, se aplica a uma camada parcialmente transparente em uma tag de preço ou ao plano de fundo de um campo de texto. As camadas que consistem em uma imagem PSD, TIFF ou PNG com transparência ativada podem ter planos de fundo transparentes.

**Cor** do plano de fundo Clique no botão Cor do plano de fundo e escolha uma amostra de cor para alterar a cor das áreas preenchidas.

**Opacidade** Arraste o controle deslizante Opacidade para tornar qualquer camada translúcida, de modo que parte da imagem subjacente seja exibida. A configuração de 100% é completamente opaca. a configuração 0 é transparente.

**Modo** de mesclagem Escolha uma opção para simular um dos modos de mesclagem disponíveis no Photoshop. As opções são Normal, Dissolver, Iluminar, Escuro, Multiplicar e Tela. Essas opções estão disponíveis para camadas, não para a tela de desenho.

## Uso de efeitos de sombra e brilho em camadas {#using-shadow-and-glow-effects-on-layers}

É possível aplicar uma sombra ou um brilho a uma camada. A sombra ou o brilho é aplicado ao perímetro da camada e se estende para dentro ou para fora, dependendo da opção de sombra ou brilho escolhida. Se o modelo tiver se originado de um arquivo PSD com efeitos de sombra e brilho, você poderá ajustar esses efeitos no Dynamic Media Classic.

Depois de aplicar um efeito de sombra ou brilho, é possível ajustar seu tamanho, cor, opacidade e posição na área Propriedades da camada da tela Modelo.

### Aplicar um efeito de sombra ou brilho a uma camada {#applying-a-shadow-or-glow-effect-to-a-layer}

Para aplicar um efeito de sombra ou brilho:

1. Selecione uma camada na lista Camadas.
1. Selecione o menu Adicionar efeito e escolha uma opção:

   **Sombra** projetada Aplica uma sombra ao lado inferior e direito da camada.

   **Sombra** interna Aplica um efeito de sombra dentro de todas as bordas da camada.

   **Brilho** externo Aplica um efeito de brilho em todas as bordas da camada.

   **Brilho** interno Aplica um efeito de brilho dentro de todas as bordas da camada.

Um nome de efeito aparece na lista Camadas depois que você aplica um efeito. Para excluir um efeito, selecione seu nome na lista Camadas e, em seguida, selecione o botão Excluir.

>[!NOTE]
>
>Às vezes, não é possível ver o efeito de uma sombra projetada ou de um brilho externo se a camada subjacente não for grande o suficiente para exibi-la. Se você não conseguir ver a sombra ou o brilho, considere adicionar valores de Preenchimento à camada ou reorganizar a camada. Consulte [Alteração do tamanho e da posição das camadas e da](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas)cobertura e [Reorganização de camadas](creating-template.md#reordering_layers).

### Ajustar um efeito de sombra ou brilho {#adjusting-a-shadow-or-glow-effect}

Para ajustar um efeito de sombra ou brilho, selecione o start selecionando seu nome na lista Camadas. Em seguida, altere suas configurações na área Propriedades da camada da tela Modelo:

**Cor** Selecione o botão Cor e escolha uma amostra de cor para alterar a cor da sombra ou do brilho. Também é possível inserir um parâmetro de valor de cor na caixa.

**Opacidade** Arraste o controle deslizante para determinar a intensidade do efeito. Efeitos menos opacos são mais transparentes.

**Modo** de mesclagem Escolha uma opção para simular um dos modos de mesclagem disponíveis no Photoshop. As opções são Normal, Dissolver, Iluminar, Escuro, Multiplicar e Tela.

**Tamanho** Insira medidas na caixa X e Y para aumentar ou diminuir o efeito de sombra. As opções de tamanho estão disponíveis apenas para sombras internas e sombras projetadas.

**Expandir** Arraste o controle deslizante para estender o efeito para dentro ou para fora.

**Desfoque** Arraste o controle deslizante para controlar a difusão nas bordas do efeito. Os efeitos com mais desfoque são mais afetados.

## Mascaramento de camadas {#masking-layers}

A lista Camadas oferta um botão Máscara que especifica como a máscara ou o canal alfa de uma camada é usado. Usando o botão Máscara, é possível aplicar o efeito de uma camada de plano de fundo a uma camada específica ou a toda a camada pai em seu modelo. Selecione uma camada na lista Camadas e selecione o botão Máscara para percorrer esses estados:

* O plano de fundo da camada é opaco.
* O conteúdo da camada é invertido e o plano de fundo da camada é preenchido com preto sólido.
* O plano de fundo da camada é preenchido com preto sólido.

