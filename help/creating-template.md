---
title: Criação de um modelo
seo-title: Criação de um modelo
description: 'null'
seo-description: Saiba como criar um modelo no Dynamic Media Classic.
uuid: c 762224 b -7 c 6 c -4434-bada-c 26570079645
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/template_ basics
discoiquuid: 8 f 7093 da-d 215-4337-ac 95-69 f 0 a 5 bf 8648
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Criação de um modelo {#creating-a-template}

Para criar um modelo, clique em Build &gt; Noções básicas do modelo. Selecione Designer ou Desenvolvedor. Nessa página, é possível adicionar camadas de texto e imagem. Também é possível reordenar camadas, alterar o tamanho e a posição das camadas e aplicar efeitos de sombra e brilho a imagens e texto.

>[!NOTE]
>
>Se você editar um modelo criado em uma versão anterior do Scene 7 Publishing System, poderá receber o prompt ao salvar perguntando "Deseja adicionar uma camada de tela? » Escolha Não para evitar adicionar uma nova camada base. Se você escolher acidentalmente Sim, exclua os modificadores «&amp; allowcanvasprompt» e «&amp; layer = 0» no URL e pressione Enter ou Return.

## Criação do modelo inicial {#creating-the-initial-template}

Quando você cria um conjunto de modelo, **a opção Publicar depois de salvar** afeta o conjunto e os membros definidos das seguintes maneiras:

| A opção «Publicar após salvar» selecionada antes de salvar? | Estado de conjunto após salvar | Estado dos membros definidos após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros podem reter seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

Você pode criar um modelo a partir de um modelo existente. Abra o modelo, clique **em Salvar como** e insira um novo nome na caixa de diálogo Salvar como.

**Para criar o conjunto Temple inicial**

1. Para criar seu modelo, use um dos seguintes métodos:

   **Selecione o PSD ou as imagens primeiro** no Painel Procurar, selecione o arquivo PSD ou imagens que deseja para o modelo, clique em Criar &gt; Noções básicas do modelo.

   **Comece na tela Modelo** clique em Build &gt; Noções básicas do modelo. Selecione Designer ou Desenvolvedor.

1. Na caixa de diálogo Digitar tamanho de tela, insira medidas de largura e altura para o seu modelo.
1. Selecione uma pasta na Biblioteca de ativos e arraste o arquivo PSD ou as imagens que deseja para o modelo na tela Modelo.
1. Quando terminar, próximo ao canto inferior direito da página, certifique-se de **que Publicar depois de salvar** esteja selecionado (padrão).
1. Clique **em Salvar**.
1. Selecione uma pasta para armazenar seu modelo, insira um nome para o modelo e clique **em Enviar**.

   O Dynamic Media Classic reduz as imagens, se necessário para se ajustá-las na tela, a área na tela Modelo para definir o modelo.

## Editar um conjunto de modelos {#editing-a-template-set}

Dependendo se você editar um conjunto publicado ou um modelo não publicado, **a opção Publicar depois de salvar** afeta o conjunto e os membros definidos das seguintes maneiras:

| Já foi publicado? | A opção «Publicar após salvar» selecionada antes de salvar sua edição? | Estado de conjunto após salvar | Estado dos membros definidos após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros definidos existentes mantêm seu estado publicado. Todos os novos membros definidos durante a edição mantêm seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros definidos e todos os novos membros definidos durante a edição mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um Conjunto de modelos**

1. No modo de exibição de Grade, navegue até um Conjunto de modelos e abaixo da imagem, clique **em Editar**.
1. Faça alterações no modelo conforme necessário.
1. Quando terminar de editar, próximo ao canto inferior direito da página, certifique-se de **que Publicar depois de salvar** esteja selecionado (padrão).
1. Clique **em Salvar**, selecione uma pasta de armazenamento, digite um nome para o conjunto e clique **em Salvar**.

## Excluindo um Modelo {#deleting-a-template}

Quando um conjunto de modelo é excluído, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou «filhos») dentro desse conjunto não serão afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um modelo**

1. Na Exibição de grade, Exibição de lista ou Exibição de detalhes, selecione um ou mais Modelos.
1. Na barra de navegação global, clique **em Arquivo** &gt; **Excluir** &gt; **Excluir**.

## Compreensão da tela Modelo {#understanding-the-template-screen}

A tela Modelo oferece ferramentas para manipular e modelar camadas.

Use essas ferramentas na tela Modelo para criar modelos:

**Ferramenta** de deslocamento Permite selecionar camadas, movê-las ao redor da tela, redimensioná-las ou gestá-las.

**Ferramenta** de texto Cria uma camada de texto. Arraste a tela para criar uma camada de texto e insira o texto na camada. Consulte Criar uma camada de texto.

**O botão Visualizar** abre a tela Visualizar e mostra o modelo em um Visualizador de zoom. Você verá como o modelo é semelhante aos usuários em seu site ou aplicativo.

**Botão Resumo do parâmetro** Abre a tela Resumo do parâmetro. É possível visualizar o nome de cada camada em um modelo e, em cada camada, os nomes dos parâmetros que foram ativados.

**Editor de texto v 4.3 e Editor de texto v 4.2** Você pode escolher usar o editor de texto mais recente e completamente em destaque, o Editor de texto v 4.3 ou o editor de texto anterior, Editor de texto v 4.2. Ao criar novos modelos, o Editor de texto v 4.3 é selecionado por padrão. Ao editar modelos mais antigos, o Editor de texto v 4.2 é selecionado por padrão. No momento, o Editor de texto v 4.3 não suporta quebra automática de palavras, portanto, ao editar modelos antigos que usam quebra automática de palavras, use o Editor de texto v 4.2 para manter a fidelidade do modelo totalmente intacta. Se o modelo mais antigo não usar quebra automática, você poderá escolher o Editor de texto v 4.3 para aproveitar os diversos novos recursos que ela oferecer, como Aumentar margens, Diminuir margens, Definir texto em todas as maiúsculas e Copiar texto.

***observação**: O Editor de texto v 4.2 será removido como uma opção no Dynamic Media Classic, portanto, recomenda-se usar o Editor de texto 4.3 quando possível. A opção Quebra automática de palavras será incorporada em uma versão futura do Editor de texto.*

**Designer e desenvolvedor** Selecione a opção que melhor descreve sua função.

**Tela** Define a área total disponível, em pixels, para a definição do modelo. O tamanho padrão é de 300 x 300 pixels. As camadas são colocadas na tela.

**Lista de camadas** Lista o nome das camadas no modelo. Para selecionar uma camada, selecione o nome na lista Camadas. A lista de camadas oferece ferramentas para adicionar efeitos a camadas, excluir camadas, reordenar camadas e camadas de parâmetros. Consulte Trabalhar com camadas.

**Área de propriedades de camada** As ferramentas Oferecem ferramentas para alterar a cor do plano de fundo, a opacidade, o tamanho e a posição de uma camada, bem como a cor do plano de fundo, a opacidade e o tamanho da tela. Também é possível ajustar os efeitos de sombra e brilho. Consulte Trabalhar com camadas.

## Criar camadas de imagens {#creating-image-layers}

1. Arraste a imagem da Biblioteca de ativos para a tela.

   O nome da ID da imagem aparece na lista Camadas.

>[!NOTE]
>
>Se necessário, o Dynamic Media Classic reduz as imagens para que caibam na tela quando você criar uma camada de imagem.

## Criação de uma camada de texto {#creating-a-text-layer}

1. Clique na ferramenta Texto.
1. Arraste para criar uma caixa de texto na tela ou em uma imagem.
1. Na tela Texto que é aberto, adicione texto executando qualquer um dos seguintes procedimentos na guia Visualizar:

   * Digite o texto na caixa de texto. Escolha Copiar ajustar texto para ajustar o texto à caixa de texto.
   * Cole o texto da área de transferência na caixa de texto.

1. Clique em Aplicar e feche a tela Texto.

### Formatar texto {#format-text}

Siga estas etapas para formatar o texto em uma camada de texto:

1. Na lista Camadas, clique duas vezes no nome da caixa de texto com texto que você deseja editar. O Editor de texto é aberto.
1. Na caixa de texto, selecione o texto que deseja formatar. Você pode selecionar todo o texto, partes do texto e caracteres individuais.
1. Especifique qualquer uma dessas opções de formatação e clique em Aplicar.

   **Fonte** Escolha uma fonte no menu Fonte. Se uma fonte desejada não aparecer no menu, você poderá carregá-la no Sistema de publicação Scene 7. Consulte Fontes.

   **Tamanho** da fonte Escolha um tamanho de fonte no menu, digite um tamanho específico na caixa ou clique nas setas para cima ou para baixo para aumentar ou diminuir o tamanho em dois pontos.

   **Clique em Cor** para escolher uma cor para o texto.

   **Negrito, Itálico ou Sublinhado** Selecione o texto e clique no ícone para o tipo de formatação que deseja aplicar ao texto.

   **Todos os maiúsculas, Sobrescrito ou Subscrito** Selecione o texto e clique no ícone para o tipo de formatação que deseja aplicar ao texto.

   **Alinhamento** Escolha um botão Alinhamento para alinhar à esquerda, centralizar ou alinhar à direita o texto na camada de texto.

   **Tipo de rastreamento** ou selecione um valor numérico com o qual ajustar a quantidade de espaço entre palavras.

   **Tipo de ajuste** de espaço ou selecione um valor numérico com o qual ajustar a quantidade de espaço entre os caracteres.

   **Espaçamento** entre linhas ou selecione um valor numérico com o qual ajustar a quantidade de espaço entre as linhas.

   **Tipo de deslocamento** da linha de base ou selecione um valor numérico com o qual mover um caractere selecionado para cima ou para baixo relativo à linha de base do texto circundante. Essa opção é especialmente útil quando você define frações ou ajusta a posição de gráficos em linha.

>[!NOTE]
>
>Clique em Desfazer para inverter sua última ação. Clique em Refazer se mudar de ideia sobre a ação de reverter uma ação depois de clicar em Desfazer.

### Formatar parágrafos {#format-paragraphs}

1. Na lista Camadas, clique duas vezes no nome da caixa de texto com texto que você deseja editar. O Editor de texto é aberto.
1. Selecione o parágrafo que deseja formatar.
1. Especifique qualquer uma dessas opções de formatação e clique em Aplicar.

   **Alinhamento** Clique para especificar o tipo de alinhamento: alinhar à esquerda, alinhar centralizar, alinhar à direita ou justificar.

   **Fim da justificação do parágrafo** clique para especificar o tipo de justificação da última linha no parágrafo: a última linha se alinha; a última linha alinha o centro; e a última linha alinha à direita.

   **Espaçamento** entre linhas ou seleciona um valor numérico com o qual ajustar a quantidade de espaço entre todas as linhas no parágrafo.

   **Recuar Todos** os clique para aumentar a quantidade que o texto é recuado.

   **Remover recuo** Clique para diminuir a quantidade que o texto é recuado.

   **Recuar primeira linha** Especifique a quantidade pela qual você deseja recuar a primeira linha de texto.

   **Espaço antes do parágrafo** Especifique a quantidade de espaço que deseja exibir acima da primeira linha de texto no parágrafo.

   **Espaço depois do parágrafo** Especifique a quantidade de espaço que deseja exibir abaixo da última linha de texto no parágrafo.

   **Alinhamento** vertical Selecione onde deseja que o texto apareça verticalmente na caixa de texto: Parte superior, Meio, Inferior.

   **Direção do texto** Selecione a direção na qual deseja que o texto seja exibido: Da direita para a esquerda ou da esquerda para a direita.

### Ajustar propriedades da camada de texto {#adjust-text-layer-properties}

1. Na tela Informações básicas sobre modelos, selecione a caixa de texto que deseja ajustar.
1. No painel Propriedades da camada, selecione um dos seguintes:

   **Reduzir texto (Somente editor de texto v 4.2)** Selecione para reduzir o texto para ajustá-lo à caixa de texto.

   **Quebra de palavras (Somente editor de texto v 4.2)** Selecione uma opção de quebra automática para especificar se ou como o texto envolve:

   **Encapsule** o texto para ajustar em uma caixa de texto que é pequena demais horizontalmente.

   **Nenhuma quebra não** vincula o texto quando a caixa de texto é pequena demais e, em vez disso, recorta uma parte do texto.

   **NB Vinculação** (quebra automática de linha) Quebra o texto para se ajustar a uma caixa de texto e não quebra palavras.

   **Posição** Especifica o local da caixa de texto na tela.

   **O preenchimento** adiciona margens ou corta o retângulo da camada. Especifique o número de pixels para adicionar ou remover para esquerda, superior, inferior e direita. Digite números positivos para adicionar uma margem; inserir números negativos para cortar.

### Exibir e editar o código fonte de texto {#view-and-edit-text-source-code}

As informações fornecidas na guia Origem do Editor de texto são para a sua referência. Edite o texto somente se você estiver familiarizado com a edição do código-fonte.

1. Na lista Camadas, clique duas vezes no nome da caixa de texto com texto que você deseja editar. O Editor de texto é aberto.
1. Clique na guia Origem do Editor de texto para revelar o código-fonte do texto.
1. Exiba ou edite o texto conforme desejado.

   As alterações permanecerão intactas se você alternar entre a visualização de Visualização e Fonte.

1. Clique em Aplicar para renderizar as edições.

## Trabalho com camadas {#working-with-layers}

Use a lista de camadas e a área Propriedades da camada para trabalhar com camadas. É possível reordenar camadas, alterar seu tamanho e posição, girar camadas e determinar a cor do plano de fundo, a cor em primeiro plano, a opacidade e o modo de mesclagem de uma camada.

Também é possível alterar o tamanho da tela, escolher a cor do plano de fundo e alterar a configuração de opacidade.

### Reordenamento de camadas {#reordering-layers}

A alteração da ordem de camadas pode afetar a aparência, especialmente quando a transparência ou a superimposição está envolvida. Certifique-se de visualizar o resultado antes de confirmar suas alterações.

1. Use uma destas técnicas para reorganizar as camadas em um modelo:

   * Selecione uma camada na lista Camadas. Em seguida, clique no botão Para cima ou para baixo quantas vezes forem necessárias para colocá-lo na posição correta na lista.
   * Arraste uma camada para cima ou para baixo na lista Camadas.

### Alteração do tamanho e da posição das camadas e da tela {#changing-the-size-and-position-of-layers-and-the-canvas}

As camadas devem ser pequenas o suficiente para se ajustarem à tela. É possível alterar o tamanho de uma camada ou da tela manualmente ou inserindo medidas de tamanho. É possível alterar a posição de uma camada manualmente ou inserindo medidas de deslocamento. Também é possível girar uma camada.

>[!NOTE]
>
>O Dynamic Media Classic recomenda criar uma predefinição de imagem que é o tamanho exato do seu modelo. A correspondência do tamanho Predefinido de imagem para o tamanho do modelo garante que as opções de tamanho final e de nitidez do modelo sejam definidas corretamente. Depois de criar essa Predefinição de imagem, você pode escolhê-la no menu Aplicar predefinição na tela Visualização do modelo. A tela mostra a aparência da imagem quando ela é entregue pelo servidor. Consulte [Configuração de predefinições de imagens](setting-image-presets.md#setting_up_image_presets).

**Alteração do tamanho de uma camada**

Para alterar o tamanho de uma camada ou tela, selecione a camada ou tela na lista Camadas e use uma destas técnicas:

**Alterar manualmente o tamanho** Selecione e arraste um canto da camada ou tela. Com camadas de texto, também é possível arrastar um lado da camada. Mantenha a tecla Shift pressionada enquanto arrasta para alterar o tamanho, mas mantenha a proporção (a forma).

**Inserir medições de tamanho de camada** Insira medições de pixel nas caixas de texto W (Largura) e H (Altura) na área Propriedades da camada.

Ao lado de alterar o tamanho de uma camada, você pode preenchê-lo. Para isso, insira uma medida de Preenchimento na caixa Esquerda, Direita, Superior e Inferior da área Propriedades da camada. O preenchimento adiciona uma margem à camada atual para deslocá-la a partir do perímetro de sua camada base. O preenchimento é útil se você adicionar um efeito de sombra projetada ou brilho externo, e quiser tornar o efeito mais visível. O preenchimento aumenta o tamanho de uma camada e exibe a cor de plano de fundo na área estendida e preenchida. A camada base é reposicionada em relação ao novo tamanho da camada. Por exemplo, se a camada atual estiver centralizada na camada base, estender o lado esquerdo da camada o move mais para a direita da camada base.

**Alteração da posição de uma camada**

Para alterar a posição de uma camada na tela, selecione o seu nome na lista Camadas e use uma destas técnicas:

**Alteração manual
da posição** Mova o ponteiro próximo, mas não sobre um limite de camada, e quando você visualizar o cursor de seta de quatro pontas, clique em e comece a arrastar.

**Inserção de medidas de deslocamento de posição** Insira medições de deslocamento X e Y nas caixas de texto X e Y. Essas medições representam o deslocamento x e y do ponto de ancoragem em pixels.

**Girar uma camada**

A caixa Girar lista o ângulo ao qual a camada foi girada. Para girar uma camada, selecione o seu nome na lista Camadas e use uma destas técnicas:

**Girar** manualmente Mover o cursor próximo, mas não sobre um canto da camada. Ao visualizar o cursor de rotação, arraste o canto da camada. Mantenha a tecla Shift pressionada enquanto arrasta para girar incrementos de 15 graus.

**Inserir uma medida de grau** Digite o número de graus para girar a camada. A rotação é no sentido horário; para girar no sentido anti-horário, insira um número negativo.

**Ocultar uma camada ou um efeito de camada**

É possível ocultar uma camada ou efeito de camada clicando no ícone de olho ao lado de um nome de camada ou nome de efeito. Camadas ocultas não aparecem em visualizações ou saída. As informações da camada não são excluídas do URL. Em vez disso, «hide = 1» é adicionado ao URL para observar que a camada está atualmente oculta da exibição. Por exemplo:

layer = 5 &amp; src = is {portalco/title} &amp; pos = 274,192 &amp; effect = -1 &amp;. effect = -1 &amp;. effect

layer = 5 &amp; src = is {portalco/title} &amp; pos = 274,192 &amp; hide = 1 &amp; effect = -1 &amp;. effect = drop Shadow &amp; blendmode

### Determinação da cor do plano de fundo, opacidade e modo de mesclagem {#determining-the-background-color-opacity-and-blend-mode}

Para escolher uma cor de plano de fundo, opacidade e modo de mesclagem para uma camada ou tela, selecione a camada ou tela e use essas técnicas:

**Cor do primeiro plano** Clique no botão Cor do primeiro plano e escolha uma amostra de cor para alterar a cor da sombra ou brilho. Também é possível inserir um parâmetro de valor de cor na caixa. A cor de fundo se aplica somente às camadas que usam transparência. Por exemplo, ela se aplica a uma camada parcialmente transparente em uma tag de preço ou ao plano de fundo de um campo de texto. As camadas que consistem em uma imagem PSD, TIFF ou PNG com transparência ativada podem ter fundos transparentes.

**Cor do plano de fundo** Clique no botão Cor do plano de fundo e escolha uma amostra de cores para alterar a cor das áreas padas.

**Opacidade** Arraste o controle deslizante de Opacidade para tornar qualquer camada translúcida para que a parte da imagem subjacente seja exibida. A configuração de 100 % é completamente opaca; a configuração 0 é transparente.

**Modo de Mesclar** uma opção para simular um dos modos de mesclagem disponíveis no Photoshop. As opções são Normal, Dissolver, Lighdez, Escurecer, Multiplicar e Tela. Essas opções estão disponíveis para camadas, não para a tela.

## Uso de efeitos de sombra e brilho em camadas {#using-shadow-and-glow-effects-on-layers}

É possível aplicar uma sombra ou brilho a uma camada. A sombra ou brilho é aplicada ao perímetro da camada e estende-se para fora ou para fora, dependendo da opção de sombra ou brilho escolhida. Se o modelo tiver sido originado com um arquivo PSD com efeitos de sombra e brilho, você pode ajustar esses efeitos no Sistema de publicação Scene 7.

Depois de aplicar um efeito de sombra ou brilho, você pode ajustar seu tamanho, cor, opacidade e posição na área Propriedades da camada da tela Modelo.

### Aplicar um efeito de sombra ou brilho a uma camada {#applying-a-shadow-or-glow-effect-to-a-layer}

Para aplicar um efeito de sombra ou brilho:

1. Selecione uma camada na lista Camadas.
1. Selecione o menu Adicionar efeito e escolha uma opção:

   **Sombra** Aplica uma sombra à parte inferior e à lateral direita da camada.

   **Sombra interna** Aplica um efeito de sombra em todas as bordas da camada.

   **Brilho externo** aplica um efeito de brilho em todas as bordas da camada.

   **Brilho interno** aplica um efeito de brilho em todas as bordas da camada.

Um nome de efeito aparece na lista Camadas depois de aplicar um efeito. Para excluir um efeito, selecione seu nome na lista Camadas e selecione o botão Excluir.

>[!NOTE]
>
>Às vezes, não é possível ver o efeito de uma sombra projetada ou um brilho externo se a camada subjacente não for grande o suficiente para exibi-la. Se não conseguir ver a sombra ou o brilho, considere adicionar valores de preenchimento à camada ou reordenar a camada. Consulte [Alterar o tamanho e a posição das camadas e as camadas de canetas e](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas)[reordenação](creating-template.md#reordering_layers).

### Como ajustar um efeito de sombra ou brilho {#adjusting-a-shadow-or-glow-effect}

Para ajustar um efeito de sombra ou brilho, comece selecionando seu nome na lista Camadas. Em seguida, altere suas configurações na área Propriedades da camada da tela Modelo:

**Cor** Selecione o botão Cor e escolha uma amostra de cor para alterar a cor da sombra ou brilho. Também é possível inserir um parâmetro de valor de cor na caixa.

**Opacidade** Arraste o controle deslizante para determinar a intensidade do efeito. Os efeitos opacos são mais transparentes.

**Modo de mesclagem** Escolha uma opção para simular um dos modos de mesclagem disponíveis no Photoshop. As opções são Normal, Dissolver, Lighdez, Escurecer, Multiplicar e Tela.

**Tamanhoinsira** medidas na caixa X e Y para ampliar ou reduzir o efeito de sombra. As opções de tamanho estão disponíveis apenas para sombras internas e sombras projetadas.

**Aumentar** arrastar o controle deslizante para estender o efeito em cima ou para fora.

**Desfoque** Arraste o controle deslizante para controlar a difusão nas bordas do efeito. Os efeitos com mais desfoque são mais difusos.

## Mascarar camadas {#masking-layers}

A lista Camadas oferece um botão Máscara que especifica como a máscara ou o canal alfa de uma camada é usado. Usando o botão Máscara, é possível aplicar o efeito de uma camada de plano de fundo a uma camada específica ou a toda a camada pai no seu modelo. Selecione uma camada na lista Camadas e selecione o botão Máscara para percorrer estes estados:

* O plano de fundo da camada é opaco.
* O conteúdo da camada é invertido e o plano de fundo da camada é preenchido com preto sólido.
* O plano de fundo da camada é preenchido com preto sólido.

