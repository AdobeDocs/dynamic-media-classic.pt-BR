---
title: Manipulação de DOM
seo-title: Manipulação de DOM
description: 'null'
seo-description: Saiba mais sobre a manipulação de DOM.
uuid: 275 cd 49 d -2 a 55-41 f 9-80 b 0-e 147 d 0 cd 2907
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/modelo-publishing
discoiquuid: 890 ca 93 e -3146-4347-864 b-bd 5 e 94037038
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Manipulação de DOM{#dom-manipulation}

A manipulação DOM (modelo de objeto de documento) é uma técnica para editar um arquivo de design manipulando diretamente seu código XML. A manipulação de DOM oferece mais controle sobre elementos de design variáveis, incluindo alterar seu conteúdo e aparência; você pode até mesmo criar novos elementos, conforme necessário.

O Dynamic Media Classic permite manipular o DOM de um modelo FXG clássico do Dynamic Media por meio de comandos de URL após a publicação do modelo. Os elementos de design no modelo FXG são manipulados ao passar comandos por meio do URL. Dessa forma, você pode manipular e adicionar dinamicamente atributos a gráficos.

Para usar a manipulação de DOM, você cria s 7: Elementids no arquivo do Illustrator antes de convertê-lo em um arquivo FXG clássico do Dynamic Media e carregá-lo no SPS.

>[!NOTE]
>
>Ao usar comandos de manipulação de DOM, todos os valores transmitidos devem ser codificados por URL.

>[!NOTE]
>
>O plug-in do Illustrator para Web-to-Print (para conversão de arquivos do Illustrator) é convertido em FXG 2.0. Para obter informações sobre essa especificação, consulte [www.adobe.com/go/learn_s7_fxg2_en](https://www.adobe.com/go/learn_s7_fxg2_en).

## Criando s 7: Elementids em arquivos do Illustrator {#creating-s-elementids-in-illustrator-files}

Para usar a manipulação de DOM com um design criado no Illustrator, crie s 7: Elementids em seu design do Illustrator. Criando s 7: Os elementids permitem que os elementos de design sejam modificados com comandos de URL após a publicação do modelo.

### Criando s 7: Elementids para manipulação de texto com DOM {#creating-s-elementids-for-dom-manipulation-of-text}

Para criar um s 7: Elementid para manipulação de DOM de um objeto de texto, abra o painel Camadas no Illustrator. Em seguida, na camada de texto que contém o texto da variável, nomeie a camada com s 7: Elementid. Para fazer isso, insira as letras `id` (para identificação), um dois pontos ( `:`) e um nome. Veja exemplos de s 7: Nomes de camadas de texto elementid:

`id:BirthdayBoyName`

`id:DateofBirth`

`id:EnterFirstNameHer`

### Criando s 7: Elementids para manipulação de objetos com DOM {#creating-s-elementids-for-dom-manipulation-of-objects}

Criar s 7: Elementids para objetos quando você deseja que os usuários finais possam alterar os atributos de objetos. Os objetos podem formar quadros de texto inteiros, gráficos e imagens. Um fundo colorido é um exemplo de uma ID de elemento de objeto. À medida que as estações mudam, o usuário final pode trocar a cor de fundo de um pôster para tornar o pôster apropriado para a temporada.

Antes de criar um s 7: ID de elemento para um objeto no Illustrator, crie uma camada separada para o objeto.

Siga estas etapas para criar um s 7: Elementid para um objeto no Illustrator:

1. Selecione o objeto.
1. Clique **em Janelas** &gt; **Camadas**.
1. No painel Camadas, nomeie a camada de objeto com s 7: Elementid. Para fazer isso, insira as letras `id` (para identificação), um dois pontos ( `:`) e uma descrição para identificar o elemento. Veja exemplos de s 7: Nomes de camada de objeto elementid:

   `id:BackgroundColor`

   `id:RotationPercentage`

   `id:JacketJPG`

## Publicar modelos FXG {#publish-fxg-templates}

Publicar seu modelo FXG a coloca nos servidores do Dynamic Media Classic, onde está disponível para seu site e aplicativo. Durante o processo de publicação, o Sistema de publicação Scene 7 ativa os urls necessários para seu site ou aplicativo.

>[!NOTE]
>
>Para usar o modelo FXG, publique todo o conteúdo que entrou na criação, incluindo fontes e imagens. Se você não incluir todos os arquivos necessários, será exibida uma mensagem de erro ao publicar.

### Marcar modelos FXG para publicação {#mark-fxg-templates-for-publish}

Os modelos e todos os arquivos de suporte devem ser marcados para publicação para que sejam colocados em servidores de imagem do Dynamic Media.

1. No Painel Procurar, selecione o modelo FXG junto com quaisquer gráficos, imagens e fontes usadas.
1. Clique **em Marcar para publicar**.

### Publicar seu modelo FXG {#publish-your-fxg-template}

1. Na barra de Navegação global, clique **em Publicar**.
1. Selecione a opção Quando e, opcionalmente, insira um nome para o trabalho de publicação.
1. Clique **em Iniciar publicação**.

### Exibição do indicador de sobrefluxo de texto {#text-overflow-indicator-display}

Um *indicador de sobrefluxo de texto* mostra quando o texto excede o espaço alocado para ele em um quadro de texto (ou no último quadro de texto no caso de texto encadeado). O indicador é uma caixa vermelha com um sinal de mais. Os indicadores de sobrefluxo de texto no SPS sempre estão ativados.

Os indicadores de sobrefluxo de texto são controlados com o `markOverflowingTextFrame` modificador. Use o modificador da seguinte maneira:

| Modificador/Valores | Descrição |
|--- |--- |
| Markoverflowingtextframe = 0,1 | O valor 1 torna os indicadores de fluxo de texto exibidos. O padrão é 0. (Embora o padrão seja 0, os indicadores de sobrefluxo de texto no SPS sempre estão ativados.) Observe que o modificador markoverflowingtextframe diferencia maiúsculas de minúsculas. |

>[!MORELIKETHIS]
>
>* [Definindo a variabilidade: Manipulação de parâmetros versus manipulação de DOM](defining-variability-parameterization-versus-dom.md#defining_variability_parameterization_versus_dom_manipulation)
>* [Publicação](publishing-files.md#publishing_files)

