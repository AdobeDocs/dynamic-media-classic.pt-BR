---
title: Criar mapas de imagem
seo-title: Criar mapas de imagem
description: 'null'
seo-description: Saiba como criar mapas de imagem.
uuid: 0 dcc 4956-006 e -4 a 74-9 d 6 a -6 d 4 bb 23790 ce
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/master_ files
discoiquuid: 4 eddf 983-38 cb -4 f 00-b 3 be -85 c 20 bdd 6 f 69
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Criar mapas de imagem{#creating-image-maps}

Um Mapa de imagem é uma região de uma imagem, uma página ecatalog ou uma imagem em um spinset, que exibe um painel de rolagem com texto. Quando o usuário clica em um Mapa de imagem, uma ação de algum tipo é acionada. Por exemplo, uma página da Web é aberta para que o usuário saiba mais sobre um produto. Para chamar a atenção para Mapas de imagem, um contorno aparece em torno de um Mapa de imagem quando o usuário move o ponteiro sobre ele.

Além da capacidade de criar um mapa de imagem no Dynamic Media Classic, ou você também pode criar mapas de imagem ao projetar um catálogo no Adobe Acrobat ou no Adobe indesign.

Ao criar Mapas de imagem, você pode fazer qualquer um dos seguintes:

* Insira texto de sobreposição.
* Insira javascript e urls para iniciar páginas da Web.
* Crie modelos de URL para Mapas de imagem.
* Copie mapas de imagem para outras imagens ou para páginas do ecatalog ou spinsets.
* Exportar mapas de imagem para CSV ou XML.
* Importe metadados de imagem de um arquivo delimitado por tabulação ou de um arquivo XML.
* Defina outras ações como determinadas pelo Consórcio da Web Wide Wide Web.
* Visualizar mapas de imagem.

## Desenho e ajuste de um Mapa de imagem {#drawing-and-adjusting-an-image-map}

1. Execute um dos procedimentos a seguir:

   * Se estiver trabalhando com uma imagem na Exibição de grade ou na Exibição de lista, na lista suspensa Editar, clique em Mapa **de imagem**. Ou abra-o na Exibição de detalhes e clique em Mapa **de imagem** acima da imagem.
   * Se estiver trabalhando com um spinset no modo de exibição de grade ou na exibição de lista, clique **em Editar**. Ou abra-o na Exibição de detalhes e clique **em Editar**. Selecione um ativo de imagem e clique em Mapa **de imagem**.
   * Se estiver trabalhando com um ecatalog, na Exibição de grade, Exibição de lista, Exibição de detalhes, clique **em Editar**. Clique na guia **Mapear páginas** .
   ![](assets/ma_image_map.png)

1. Desenhe um Mapa de imagem retangular ou poligonal (muitas vezes):

   **Mapa retangular** Selecione a ferramenta Mapa de imagem retangular e arraste a página para criar o retângulo. Para adicionar um ponto a um mapa retangular (alterando-o para um mapa de polígono), pressione Ctrl e insira a ferramenta de inserção no local desejado e clique em.

   **Mapa poligonal** Selecione a ferramenta do Mapa de imagem polígono e clique pontos no perímetro da área da imagem que você deseja incluir. Use o controle deslizante da densidade poligonal para variar a densidade do ponto no polígono. A densidade original será lembrada se você selecionar outros mapas. Se algum ponto for adicionado, excluído ou movido no polígono, a densidade original será perdida e o controle deslizante será redefinido para o valor máximo.

1. Digite um nome para o Mapa de imagem, se desejado, na lista Mapa de imagens. Depois de desenhar um Mapa de imagem, o Dynamic Media Classic o atribui.

   Para criar o nome, o Dynamic Media Classic anexa um número sequencial ao nome da página ou página ecatalog com a qual você está trabalhando. Você pode inserir um nome de sua escolha.

1. Se você quiser que os usuários abram uma nova página da Web quando clicarem no Mapa de imagens, digite o URL na lista Mapa de imagens.

   Consulte [Inserir javascript e urls](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Para exibir texto de sobreposição quando os usuários movimentam o ponteiro sobre o Mapa de imagem, insira o texto na lista Mapa de imagens. Na lista Mapa de imagens, selecione o menu Exibir e escolha Texto de sobreposição. Em seguida, digite o texto que deseja que os usuários vejam na tela. Você pode gravar o texto em um processador de texto e copiá-lo no campo de texto Rollover.
1. Se você quiser que outro efeito de ação ocorra quando os usuários movem o mouse sobre um Mapa de imagem, defina a ação. Na lista suspensa Mostrar, clique em Outras ações. Insira os atributos da ação. (Clique em Mostrar &gt; Ambas para criar texto de sobreposição e uma ação para um Mapa de imagem.)

   Consulte [Definição de outras ações para Mapas de imagem](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Opcional) Execute um dos procedimentos a seguir:

   * Clique em Visualizar para visualizar mapas de imagem.
   * Para excluir um Mapa de imagem ou vértice polígono, selecione uma forma na imagem e clique em Excluir. Ou, para um ecatalog, na guia Ordenar páginas, clique em Limpar mapas para remover Mapas de imagem de todas as páginas.
   * Para remover temporariamente um Mapa de imagem de uma imagem, uma imagem em um spinset ou uma página ecatalog, sem excluí-la, desmarque a opção Ativar adequada na lista Mapa de imagens.

1. Clique em Salvar.

### Como ajustar a posição, a forma e o tamanho dos mapas de imagem {#adjusting-the-position-shape-and-size-of-image-maps}

Para alterar a posição, a forma e o tamanho de um Mapa de imagem, selecione o botão Mapa de imagens. Em seguida, selecione a ferramenta Deslocamento e siga estas instruções:

**Alterar posição** Mova o ponteiro próximo, mas não sobre a borda do Mapa de imagem. Ao visualizar o ícone de seta de quatro pontilhados, arraste o mapa para um novo local.

**Alterar o tamanho e a forma** Como a forma e o tamanho de um Mapa de imagem dependem se você está trabalhando com um Mapa de imagem retangular ou poligonal:

***Dica**: Você pode arrastar o controle deslizante de Tamanho na parte inferior da tela para alterar as visualizações e obter uma aparência melhor do Mapa de imagem.*

**Mapa de imagem retangular** Mova o ponteiro sobre um lado ou canto do Mapa de imagem. Ao visualizar o ícone de seta de duas pontas, comece a arrastar. Mantenha a tecla Shift pressionada enquanto arrasta para alterar o tamanho, mas mantenha a proporção (a forma).

**Mapa de imagem poligonal** Arraste uma alça de seleção quadrada. Para criar uma alça de seleção, clique na borda do Mapa de imagem e comece a arrastar.

### Tratamento de mapas de imagem sobrepostos {#handling-overlapping-image-maps}

Se a sua página ou página do ecatalog incluir mais de um Mapa de imagem e os mapas se sobrepor, você pode determinar como os mapas se sobrepõem. Para isso, altere a ordem dos mapas na lista Mapa de imagens. Arraste seus nomes para cima ou para baixo na lista. O nível alto de um nome na lista determina se o Mapa de imagem sobrepõe outros Mapas de imagem.

### Importação de dados do Mapa de imagem {#importing-image-map-data}

Em vez de inserir os dados do Mapa de imagem em cada página, você pode importar os dados para a imagem, o Conjunto de rotação ou o ecatalog na tela Resumo do mapa. Você importa os dados do Mapa de imagem na forma de um arquivo delimitado por tabulação ou DTD XML. Os campos no arquivo devem estar na ordem mostrada na tela Resumo do mapa: Nome, Rótulos de sumário, Mapas, urls, Texto de sobreposição, Outras ações e Strings de pesquisa. Importar os dados do Mapa de imagens poupa o problema de inserir os dados na lista do Mapa de imagens à medida que você cria cada Mapa de imagens.

**Para importar dados do Mapa de imagem**

1. Vá até a página do editor do Mapa de imagens (para imagens ou imagens em spinsets) ou a guia Mapa de páginas da tela de edição do ecatalog.
1. Clique em Importar metadados.
1. Na caixa de diálogo Carregar metadados, clique em Imagem ou Mapa de imagem para carregar os metadados do tipo desejado de propriedade do ativo.
1. Na lista suspensa Gerar arquivo, selecione o tipo de arquivo que deseja criar.
1. (Opcional) Clique em Gerar para visualizar os dados resultantes com base no tipo de arquivo que deseja criar. Clique em Fechar para retornar à caixa de diálogo Carregar metadados.
1. Navegue até o arquivo que deseja carregar. No campo de texto Nome do arquivo, especifique o nome do arquivo gerado.
1. (Opcional) No campo Nome do trabalho, especifique um nome para o trabalho de upload de metadados.
1. Clique em Carregar.

### Copiando mapas de imagem {#copying-image-maps}

É possível copiar Mapas de imagem de uma imagem ou de uma página do ecatalog para outra. Use Copiar mapa de imagem para começar a criá-los. Também é possível copiar Mapas de imagem para recriá-los em imagens ou páginas que compartilham a mesma estrutura de layout ou de mapeamento.

Por exemplo, copiar mapas de imagem em um ecatalog é uma maneira conveniente de copiar todos os mapas de imagem entre as versões de idioma estrangeiro do mesmo ecatalog. Para obter melhores resultados, copiar é mais bem-sucedido se você copiar entre o ecatalogs com o mesmo número de páginas e as mesmas imagens. Se o ecatalog para o qual você copiar já contém Mapas de imagem, esteja ciente de que esses Mapas de imagem são excluídos quando a cópia é feita.

**Para copiar Mapas de imagem**

1. Vá até a página do editor do Mapa de imagens (para imagens ou imagens em spinsets) ou a guia Mapa de páginas da tela de edição do ecatalog.
1. Clique em Copiar mapas para.
1. Execute um dos procedimentos a seguir com base em se você estiver copiando Mapas de imagem a partir de imagens ou copiando Mapas de imagem de um ecatalog:

   * (Imagens) Na tela Selecionar imagens, selecione as imagens para as quais deseja copiar os Mapas de imagem.
   * (Ecatalog) Na tela Selecionar ativo, selecione as páginas ou páginas do ecatalog às quais você deseja copiar os Mapas de imagem.

1. Clique em Selecionar.

## Uso de um modelo para inserir javascript e urls {#using-a-template-to-enter-javascript-and-urls}

Você pode definir um modelo de URL (também conhecido como um modelo Href) para tornar os urls do Mapa de imagem mais fáceis e mais eficientes. Defina um modelo de URL se a maioria dos urls do Mapa de imagens compartilhar um formato fixo e fixo. Ao inserir a parte do URL que é corrigida como modelo de URL, você não precisa inserir essa parte do URL toda vez que criar um Mapa de imagem. O modelo de URL também pode conter comandos de javascript, nomes de caminho e parâmetros. Por padrão, o modelo de URL contém um gerenciador javascript do Dynamic Media Classic proprietário chamado `loadProduct` que abre a imagem em uma nova janela.

>[!NOTE]
>
>Observe que quando você adiciona o código Javascript no atributo HREF do mapa de imagem, o código é executado no computador do cliente. Portanto, certifique-se de que o código Javascript esteja protegido.

### Sobre modelos de URL {#about-url-templates}

O modelo de URL funciona substituindo o conteúdo da coluna URL na lista Mapa de imagens, com os sinais de dólar duplo (' $ $') no modelo:

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Você insere todos os valores que não mudam entre Mapas de imagem no modelo de URL. Adicione apenas os valores que mudam na coluna URL na lista Mapa de imagens. Por exemplo:

* Modelo de URL: j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* Valor do URL: `product.htm`
* URL real gerado: `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

Por padrão, o modelo de URL inclui um manipulador de javascript do Dynamic Media Classic proprietário, chamado `loadProduct` que abre uma nova janela com o destino do URL. No entanto, você pode usar qualquer código javascript para substituir esse manipulador javascript ou usar um dos seguintes manipuladores do Dynamic Media Classic:

* `loadProductCW`

   Exibe o destino do URL especificado na coluna URL na janela atual. Esse manipulador é principalmente para ecatalogs que são integrados a uma página dentro de um site.

* `loadProductPW`

   Exibe o alvo do URL especificado na coluna URL na janela pai (a página que abriu o atual). A janela atual permanece aberta, mas a janela pai muda para exibir o destino do URL.

   ***observação**: O manipulador`loadProductPW`não suporta visualizadores DHTML e HTML 5.*

### Criação de um modelo de URL {#creating-a-url-template}

Para criar um modelo de URL:

1. Na tela do Editor de mapa (imagens ou spinsets) ou na guia Mapa de páginas da tela ecatalog (ecatalogs), selecione Editar ao lado da opção Modelo de URL. A caixa de diálogo Editar modelo do mapa é aberta.
1. Insira o código javascript e o URL completo (com a porção de variável substituída pelo dólar [$ $]). Você pode colar o código clicando com o botão direito do mouse e escolhendo Colar.
1. Selecione o botão Salvar.

### Como lidar com modelos de URL {#handling-url-templates}

A página do Editor de mapa (imagens e spinsets) e a guia Mapa de páginas da tela ecatalog (ecatalogs) oferecem esses comandos para gerenciar modelos de URL:

**Opção Modelo de URL** Selecione a opção Modelo de URL para aplicar seu modelo de URL a todos os Mapas de imagem em uma página ou página do ecatalog.

**Opção de modelo** Desmarque uma opção de Modelo na lista do Mapa de imagem do URL se você não quiser que um Mapa de imagem individual use o modelo de URL.

## Definição de outras ações para Mapas de imagem {#defining-other-actions-for-image-maps}

Você pode selecionar o menu Mostrar e escolher Outras ações para acionar ações que não sejam texto de sobreposição e inicializações de página da Web. Quando o usuário move o ponteiro sobre um Mapa de imagem, você pode iniciar uma ação. Essas ações são atributos definidos para Mapas de imagem do lado do cliente por especificações HTML do Consórcio da Web todo mundo. Eles incluem:

**accesskey** aciona uma ação quando o usuário pressiona uma tecla designada no teclado.

**onfocus** aciona um evento quando o Mapa de imagem recebe foco— pelo cursor, por tabulação ou pressionando uma tecla de acesso. Por exemplo, você pode iniciar uma página da Web quando o Mapa de imagens receber foco e fechá-lo quando o Mapa de imagem perder o foco.

**onblur** Aciona um evento quando o Mapa de imagem perde o foco, seja pelo cursor ou por tabulação.

**Definição de outras ações para Mapas de imagem**

1. Na tela do Editor do mapa (imagens e spinsets) ou no guia Mapear páginas da tela ecatalog (ecatalogs), selecione o menu Exibir e escolha Outras ações.
1. Usando a sintaxe especificada pelas especificações HTML do Consórcio da World Wide Web, adicione os atributos compatíveis na coluna Outras ações da lista Mapa de imagens.
1. Clique **em Salvar**.

Selecione o menu Mostrar e escolha Ambos se desejar que um Mapa de imagem tenha texto de sobreposição e uma ação.

## Criar mapas de imagem no Adobe Acrobat ou no Adobe indesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Você pode criar Mapas de imagem ao criar seu ecatalog no Adobe Acrobat ou Adobe indesign.

No Acrobat ou no indesign, crie referências de hiperlink onde deseja que os Mapas de imagem sejam exibidos e especifique os locais do URL para o mapa de imagem. A seleção da opção Extrair links ao carregar o arquivo PDF no Dynamic Media Classic converte automaticamente os links para Mapas de imagem.

Para obter mais informações, consulte Ajuda do indesign ou Ajuda do Acrobat.

### Criação de mapas de imagem no Adobe indesign {#to-create-image-maps-in-adobe-indesign}

1. No indesign, clique em Janela &gt; Interativo &gt; Hiperlinks para abrir o painel Hiperlinks.
1. Selecione o texto, o quadro ou o gráfico que você deseja transformar em um Mapa de imagem.
1. No painel Hiperlinks, clique em Novo hiperlink no menu do painel.
1. Na caixa de diálogo Novo hiperlink, escolha URL no menu Link para.
1. Digite ou cole a ID de produto na caixa URL e clique em OK. (O Dynamic Media Classic completa o URL usando o modelo URL do Mapa de imagem.)

   >[!NOTE]
   >
   >Não é necessário definir opções de aparência no indesign. Você pode especificar a aparência no Dynamic Media Classic.

1. Repita as etapas de 2 a 5 para todos os Mapas de imagem que deseja criar.
1. Exporte o arquivo como um PDF.
1. Faça upload do PDF para o Dynamic Media Classic e selecione Extrair links das Opções de PDF.

### Para criar Mapas de imagem no Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. No Acrobat, escolha Ferramentas &gt; Edição avançada &gt; Ferramenta Link.
1. Arraste para criar o Mapa de imagem. A caixa Criar link é aberta.
1. Selecione Link personalizado e clique em Avançar.

   ***observação**: Não é necessário definir opções de aparência no Acrobat. Você pode especificar a aparência no Dynamic Media Classic.*

1. Na caixa Propriedades do link, clique em Ações.
1. Selecione Abrir um link da Web no menu Selecionar ação e clique em Adicionar.
1. Digite a ID de produto do Mapa de imagem na caixa Editar URL e clique em OK. (O Dynamic Media Classic completa o URL usando o modelo de URL do mapa de imagem.)
1. Repita as etapas de 1 a 7 para todos os Mapas de imagem que deseja criar.
1. Salve o arquivo.
1. Faça upload do PDF para o Dynamic Media Classic e selecione Extrair links das Opções de PDF.

