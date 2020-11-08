---
title: Criação de mapas de imagem
seo-title: Criação de mapas de imagem
description: nulo
seo-description: Saiba como criar mapas de imagem.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '2444'
ht-degree: 0%

---


# Criação de mapas de imagem{#creating-image-maps}

Um Mapa de imagem é uma região em uma imagem, uma página eCatalog ou uma imagem em um SpinSet, que exibe um painel de sobreposição com texto. Quando o usuário clica em um Mapa de imagem, uma ação de algum tipo é acionada. Por exemplo, uma página da Web é aberta para que o usuário possa saber mais sobre um produto. Para chamar a atenção para os Mapas de imagem, um contorno é exibido ao redor de um Mapa de imagem quando o usuário move o ponteiro sobre ele.

Além da capacidade de criar um mapa de imagem no Dynamic Media Classic, ou você também pode criar mapas de imagem ao projetar um catálogo no Adobe Acrobat ou Adobe InDesign.

Ao criar Mapas de imagem, você pode fazer o seguinte:

* Insira o texto de sobreposição.
* Insira JavaScript e URLs para iniciar páginas da Web.
* Criar modelos de URL para mapas de imagem.
* Copie os mapas de imagem para outras imagens, páginas de eCatalog ou SpinSets.
* Exportar mapas de imagem para CSV ou para XML.
* Importe metadados de imagem de um arquivo delimitado por tabulação ou de um arquivo XML.
* Defina outras ações, conforme determinado pelo World Wide Web Consortium.
* Mapas de imagem de pré-visualização.

## Desenho e ajuste de um Mapa de imagem {#drawing-and-adjusting-an-image-map}

1. Execute um dos procedimentos a seguir:

   * Se você estiver trabalhando com uma imagem na Visualização de grade ou na Visualização de Lista, na lista suspensa Editar, clique em **Mapa** de imagem. Ou abra-o em Visualização de detalhes e clique em Mapa **de** imagem acima da imagem.
   * Se você estiver trabalhando com um SpinSet na Visualização de grade ou na Visualização de Lista, clique em **Editar**. Ou abra-o em Visualização de detalhes e clique em **Editar**. Selecione um ativo de imagem e clique em Mapa de **imagem**.
   * Se você estiver trabalhando com um eCatalog, na Visualização de grade, na Visualização de Lista, na Visualização de detalhes, clique em **Editar**. Clique na guia **Mapear páginas** .

   ![](assets/ma_image_map.png)

1. Desenhe um Mapa de imagem retangular ou poligonal (de muitos lados):

   **Mapa** retangular Selecione a ferramenta Mapa de imagem de retângulo e arraste na página para criar o retângulo. Para adicionar um ponto a um mapa retangular (alterando-o, portanto, para um mapa de polígono), pressione Ctrl, depois insira a ferramenta de inserção no local desejado e clique.

   **Mapa** poligonal Selecione a ferramenta Mapa de imagem de polígono e clique nos pontos no perímetro da área da imagem que você deseja incluir. Use o controle deslizante de densidade do polígono para variar a densidade do ponto no polígono. A densidade original será lembrada se você selecionar outros mapas. Se algum ponto for adicionado, excluído ou movido no polígono, a densidade original será perdida e o controle deslizante será redefinido para seu valor máximo.

1. Digite um nome para o Mapa de imagem, se desejado, na lista do Mapa de imagem. Depois de desenhar um Mapa de imagem, o Dynamic Media Classic atribui um nome a ele.

   Para criar o nome, o Dynamic Media Classic anexa um número sequencial ao nome da imagem ou da página do eCatalog com a qual você está trabalhando. Você pode inserir um nome de sua escolha.

1. Se você quiser que os usuários abram uma nova página da Web quando clicarem no Mapa de imagem, insira o URL na lista do Mapa de imagem.

   Consulte [para inserir JavaScript e URLs](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Para exibir o texto de sobreposição quando os usuários movem o ponteiro sobre o Mapa de imagem, insira o texto na lista do Mapa de imagem. Na lista do Mapa de imagem, selecione o menu Mostrar e escolha Texto de sobreposição. Em seguida, insira o texto que deseja que os usuários vejam na tela. Você pode gravar o texto em um processador de texto e copiá-lo no campo de texto Sobreposição.
1. Se você quiser que outro efeito de ação ocorra quando os usuários moverem o mouse sobre um Mapa de imagem, defina a ação. Na lista suspensa Exibir, clique em Outras ações. Informe os atributos da ação. (Clique em Mostrar > Ambos para criar um texto de sobreposição e uma ação para um Mapa de imagem.)

   Consulte [Definição de outras ações para Mapas](creating-image-maps.md#defining_other_actions_for_image_maps)de imagens.

1. (Opcional) Execute um dos procedimentos a seguir:

   * Clique em Pré-visualização para pré-visualização de mapas de imagem.
   * Para excluir um Mapa de imagem ou um vértice de polígono, selecione uma forma na imagem e clique em Excluir. Ou, para um eCatalog, na guia Order Pages (Solicitar páginas), clique em Clear Maps (Limpar mapas) para remover os Image Maps (Mapas de imagem) de todas as páginas.
   * Para remover temporariamente um Mapa de imagem de uma imagem, uma imagem em um SpinSet ou uma página eCatalog, sem excluí-lo, desmarque a opção Ativado apropriada na lista do Mapa de imagem.

1. Clique em Salvar.

### Ajustar a posição, a forma e o tamanho dos mapas de imagem {#adjusting-the-position-shape-and-size-of-image-maps}

Para alterar a posição, a forma e o tamanho de um Mapa de imagem, selecione o botão Mapa de imagem. Em seguida, selecione a ferramenta Deslocamento e siga estas instruções:

**Alteração da posição** Mova o ponteiro para perto, mas não acima, da borda do Mapa de imagem. Quando você vir o ícone de seta de quatro pontas, arraste o mapa até um novo local.

**Alteração do tamanho e da forma** Como você altera a forma e o tamanho de um Mapa de imagem depende se você está trabalhando com um Mapa de imagem retangular ou poligonal:

***Dica **: Você pode arrastar o controle deslizante Tamanho na parte inferior da tela para alterar as visualizações e obter uma melhor visualização do Mapa de imagem.*

**Mapa** de imagem retangularMove o ponteiro sobre um lado ou canto do Mapa de imagem. Quando você vê o ícone de seta com cabeça de duplo, o start arrasta. Mantenha pressionada a tecla Shift enquanto arrasta para alterar o tamanho, mas mantém a proporção (a forma).

**Mapa** de imagem poligonal Arraste uma alça de seleção quadrada. Para criar uma alça de seleção, clique na borda do Mapa de imagem e arraste do start.

### Manuseio de mapas de imagem sobrepostos {#handling-overlapping-image-maps}

Se a sua imagem ou página de eCatalog incluir mais de um Mapa de imagem e os mapas se sobrepuserem, você poderá determinar como os mapas se sobrepõem. Para fazer isso, altere a ordem dos mapas na lista do Mapa de imagem. Arraste seus nomes para cima ou para baixo na lista. A altura de um nome na lista determina se o Mapa de imagem sobrepõe outros Mapas de imagem.

### Importação de dados do Mapa de imagem {#importing-image-map-data}

Em vez de inserir dados do Mapa de imagem em cada página, você pode importar os dados da imagem, do Conjunto de rotação ou do eCatalog para a tela Resumo do mapa. É possível importar os dados do Mapa de imagem na forma de um arquivo delimitado por tabulação ou XML DTD. Os campos no arquivo devem estar na ordem mostrada na tela Resumo do mapa: Nome, Rótulos de sumário, Mapas, URLs, Texto de sobreposição, Outras ações e Strings de pesquisa. A importação de dados do Mapa de imagem salva o problema de inserir os dados na Lista do Mapa de imagem à medida que você cria cada Mapa de imagem.

**Para importar dados do Mapa de imagem**

1. Vá para a página do editor do Mapa de imagem (para imagens ou em SpinSets) ou para a guia Páginas de mapa da tela de edição do eCatalog.
1. Clique em Importar metadados.
1. Na caixa de diálogo Carregar metadados, clique em Imagem ou Mapa de imagem para fazer upload dos metadados do tipo de propriedade do ativo desejado.
1. Na lista suspensa Gerar arquivo, selecione o tipo de arquivo que deseja criar.
1. (Opcional) Clique em Gerar para pré-visualização dos dados resultantes com base no tipo de arquivo que você deseja criar. Clique em Fechar para retornar à caixa de diálogo Carregar metadados.
1. Navegue até o arquivo que deseja carregar. No campo de texto Nome do arquivo, especifique o nome do arquivo gerado.
1. (Opcional) No campo Nome do trabalho, especifique um nome para o trabalho de upload de metadados.
1. Clique em Carregar.

### Copiando mapas de imagem {#copying-image-maps}

É possível copiar mapas de imagem de uma imagem ou página de eCatalog para outra. Use Copiar mapa de imagem para obter um start principal que os crie. Também é possível copiar Mapas de imagem para recriá-los em imagens ou páginas que compartilham o mesmo layout ou estrutura de mapeamento.

Por exemplo, copiar mapas de imagem em um eCatalog é uma maneira conveniente de copiar todos os mapas de imagem entre versões em idioma estrangeiro do mesmo eCatalog. Para obter melhores resultados, a cópia será mais bem-sucedida se você copiar entre eCatalogs com o mesmo número de páginas e as mesmas imagens. Se o eCatalog ao qual você copia já contiver mapas de imagem, lembre-se de que esses mapas de imagem são excluídos quando a cópia é feita.

**Para copiar mapas de imagem**

1. Vá para a página do editor do Mapa de imagem (para imagens ou em SpinSets) ou para a guia Páginas de mapa da tela de edição do eCatalog.
1. Clique em Copiar mapas para.
1. Execute um dos procedimentos a seguir, caso esteja copiando mapas de imagem de imagens ou copiando mapas de imagem de um eCatalog:

   * (Imagens) Na tela Selecionar imagens, selecione as imagens para as quais deseja copiar os Mapas de imagens.
   * (eCatalog) Na tela Selecionar ativo, selecione as imagens ou as páginas do eCatalog para as quais deseja copiar os mapas de imagem.

1. Clique em Selecionar.

## Usar um modelo para inserir JavaScript e URLs {#using-a-template-to-enter-javascript-and-urls}

Você pode definir um modelo de URL (também conhecido como modelo Href) para facilitar e tornar mais eficiente a inserção de URLs de mapa de imagem. Defina um modelo de URL se a maioria dos URLs do Mapa de imagem compartilharem um formato comum e fixo. Ao inserir a parte do URL que é fixa como modelo de URL, não é necessário inserir essa parte do URL sempre que criar um Mapa de imagem. Seu modelo de URL também pode conter comandos, nomes de caminho e parâmetros JavaScript. Por padrão, o modelo de URL contém um manipulador JavaScript proprietário do Dynamic Media Classic, chamado de `loadProduct` que abre a imagem em uma nova janela.

>[!NOTE]
>
>Lembre-se de que quando você adiciona o código Javascript ao atributo HREF do mapa de imagem, o código é executado no computador do cliente. Portanto, verifique se o código Javascript está seguro.

### Sobre modelos de URL {#about-url-templates}

O modelo de URL funciona substituindo o conteúdo da coluna URL na lista do Mapa de imagem pelos sinais em dólar de duplo (‘$$’) no modelo:

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Você coloca todos os valores que não são alterados entre os Mapas de imagem no modelo de URL. Adicione somente os valores que mudam na coluna URL na lista do Mapa de imagem. Por exemplo:

* Modelo de URL: j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* Valor do URL: `product.htm`
* URL real gerado: `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

Por padrão, o modelo de URL inclui um manipulador JavaScript proprietário do Dynamic Media Classic, chamado `loadProduct` que abre uma nova janela com o destino do URL. No entanto, você pode usar qualquer código JavaScript para substituir esse manipulador JavaScript ou usar um dos seguintes manipuladores do Dynamic Media Classic:

* `loadProductCW`

   Exibe o público alvo de URL especificado na coluna URL na janela atual. Esse manipulador é principalmente para eCatalogs integrados em uma página dentro de um site.

* `loadProductPW`

   Exibe o público alvo de URL especificado na coluna URL na janela pai (a página que abriu a atual). A janela atual permanece aberta, mas a janela pai é alterada para exibir o público alvo de URL.

   ***observação **: O manipulador `loadProductPW` não suporta visualizadores DHTML e HTML5.*

### Creating a URL template {#creating-a-url-template}

Para criar um modelo de URL:

1. Na tela do Editor de mapa (imagens ou Conjuntos de rotação) ou na guia Páginas de mapa da tela eCatalog (eCatalogs), selecione Editar ao lado da opção Modelo de URL. A caixa de diálogo Editar modelo de mapa é aberta.
1. Insira o código JavaScript e o URL completo (com a parte variável substituída por dólar sign [$$]). Você pode colar o código clicando com o botão direito do mouse e escolhendo Colar.
1. Selecione o botão Salvar.

### Manuseio de modelos de URL {#handling-url-templates}

As páginas do Editor de mapa (imagens e Conjuntos de rotação) e a guia Páginas de mapa da tela eCatalog (eCatalogs) oferta estes comandos para manipular modelos de URL:

**Opção** Modelo de URL Selecione a opção Modelo de URL para aplicar seu modelo de URL a todos os Mapas de imagem em uma página de imagem ou eCatalog.

**Opção** Modelo Desmarque uma opção Modelo na lista Mapa de imagem do URL se não quiser que um Mapa de imagem individual use o modelo de URL.

## Definição de outras ações para Mapas de imagem {#defining-other-actions-for-image-maps}

Você pode selecionar o menu Mostrar e escolher Outras ações para acionar ações diferentes de texto de sobreposição e inicializações de página da Web. Quando o usuário move o ponteiro sobre um Mapa de imagem, você pode iniciar uma ação. Essas ações são atributos definidos para mapas de imagem do lado do cliente pelas especificações HTML do World Wide Web Consortium. Eles incluem:

**a tecla de ACESSO** Aciona uma ação quando o usuário pressiona uma tecla designada no teclado.

**onfocus** Aciona um evento quando o Mapa de imagem recebe foco — pelo cursor, tabulação ou pressionando uma tecla de acesso. Por exemplo, você pode iniciar uma página da Web quando o Mapa de imagem receber foco e fechá-lo quando o Mapa de imagem perder foco.

**o Desfoque** Aciona um evento quando o Mapa de imagem perde o foco, seja pelo cursor ou por tabulação.

**Definição de outras ações para Mapas de imagens**

1. Na tela do Editor de mapa (imagens e Conjuntos de rotação) ou na guia Páginas de mapa da tela eCatalog (eCatalogs), selecione o menu Mostrar e escolha Outras ações.
1. Usando a sintaxe especificada pelas especificações HTML do World Wide Web Consortium, adicione os atributos suportados na coluna Outras ações da lista do Mapa de imagem.
1. Clique em **Salvar**.

Selecione o menu Mostrar e escolha Ambos se quiser que um Mapa de imagem tenha um texto de sobreposição, bem como uma ação.

## Criação de mapas de imagem no Adobe Acrobat ou Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Você pode criar mapas de imagem ao projetar seu eCatalog no Adobe Acrobat ou Adobe InDesign.

No Acrobat ou InDesign, crie referências de hiperlink onde deseja que os Mapas de imagem apareçam e especifique os locais de URL para o mapa de imagem. A seleção da opção Extrair links ao carregar o arquivo PDF no Dynamic Media Classic converte automaticamente os links para Mapas de imagens.

Para obter mais informações, consulte Ajuda do InDesign ou Ajuda do Acrobat.

### Para criar mapas de imagem no Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. No InDesign, clique em Janela > Interativo > Hiperlinks para abrir o painel Hiperlinks.
1. Selecione o texto, quadro ou gráfico que deseja transformar em um Mapa de imagem.
1. No painel Hiperlinks, clique em Novo hiperlink no menu do painel.
1. Na caixa de diálogo Novo hiperlink, escolha URL no menu Vincular a.
1. Digite ou cole a ID do produto na caixa URL e clique em OK. (O Dynamic Media Classic conclui o URL usando o modelo de URL do Mapa de imagem.)

   >[!NOTE]
   >
   >Não é necessário definir opções de aparência no InDesign. Você pode especificar a aparência no Dynamic Media Classic.

1. Repita as etapas de 2 a 5 para todos os Mapas de imagem que deseja criar.
1. Exporte o arquivo como um PDF.
1. Carregue o PDF no Dynamic Media Classic e selecione Extrair links nas Opções do PDF.

### Para criar mapas de imagem no Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. No Acrobat, escolha Ferramentas > Edição avançada > Ferramenta de link.
1. Arraste para criar o Mapa de imagem. A caixa Criar link é aberta.
1. Selecione Link personalizado e clique em Avançar.

   ***observação **: Não é necessário definir opções de aparência no Acrobat. Você pode especificar a aparência no Dynamic Media Classic.*

1. Na caixa Propriedades do link, clique em Ações.
1. Selecione Abrir um link da Web no menu Selecionar ação e clique em Adicionar.
1. Digite a ID do produto para o Mapa de imagem na caixa Editar URL e clique em OK. (O Dynamic Media Classic conclui o URL usando o modelo de URL do mapa de imagem.)
1. Repita as etapas de 1 a 7 para todos os Mapas de imagem que deseja criar.
1. Salve o arquivo.
1. Carregue o PDF no Dynamic Media Classic e selecione Extrair links nas Opções do PDF.

