---
title: Criar mapas de imagem
description: Saiba como criar mapas de imagem no Adobe Dynamic Media Classic.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
source-git-commit: 0e2271924f49edd6ac424bb7cbd56af1e6afd817
workflow-type: tm+mt
source-wordcount: '2349'
ht-degree: 0%

---

# Criar mapas de imagem {#creating-image-maps}

Um Mapa de imagem é uma região em uma imagem, uma página de catálogo eletrônico ou uma imagem em um Conjunto de rotação que exibe um painel de rolagem com texto. Quando o usuário seleciona um Mapa de imagem, uma ação de algum tipo é acionada. Por exemplo, uma página da Web é iniciada para que o usuário possa saber mais sobre um produto. Um contorno é exibido ao redor de um Mapa de imagem quando o usuário move o ponteiro sobre ele.

Além da capacidade de criar mapas de imagem no Adobe Dynamic Media Classic, você também pode criar mapas de imagem ao projetar um catálogo no Adobe Acrobat ou Adobe InDesign.

Ao criar Mapas de imagem, você pode fazer o seguinte:

* Insira o texto de sobreposição.
* Insira JavaScript e URLs para iniciar páginas da Web.
* Criar modelos de URL para mapas de imagem.
* Copiar mapas de imagem para outras imagens, páginas de eCatalog ou SpinSets.
* Exportar mapas de imagem para CSV ou XML.
* Importe metadados de imagem de um arquivo delimitado por tabulação ou de um arquivo XML.
* Defina outras ações conforme determinado pelo World Wide Web Consortium.
* Visualizar mapas de imagem.

## Desenhar e ajustar um mapa de imagem {#drawing-and-adjusting-an-image-map}

1. Siga um destes procedimentos:

   * Se estiver trabalhando com uma imagem na Exibição de grade ou na Exibição de lista, na lista suspensa Editar , selecione **[!UICONTROL Image Map]**. Ou abra-a na Exibição de detalhes e selecione **[!UICONTROL Image Map]** acima da imagem.
   * Se estiver trabalhando com um SpinSet na Exibição de Grade ou na Exibição de Lista, selecione **[!UICONTROL Edit]**. Ou abra-o na Exibição de detalhes e selecione **[!UICONTROL Edit]**. Selecione um ativo de imagem e selecione **[!UICONTROL Image Map]**.
   * Se você estiver trabalhando com um eCatalog, na Exibição de grade, Exibição de lista, Exibição de detalhes, selecione **[!UICONTROL Edit]**. Selecione a guia **[!UICONTROL Map Pages]**.

   ![Imagem do mapa de imagem](assets/ma_image_map.png)

1. Desenhar um mapa de imagem retangular ou polígono (de vários lados):

   * **Mapa retangular**  - Selecione a ferramenta Mapa de imagem do retângulo e arraste na página para criar o retângulo. Para adicionar um ponto a um mapa retangular (alterando-o assim para um mapa de polígono), pressione Ctrl, depois coloque a ferramenta de inserção no local desejado e selecione.

   * **Mapa poligonal**  - Selecione a ferramenta Mapa de imagem de polígono e selecione pontos no perímetro da área da imagem que deseja incluir. Use o controle deslizante de densidade do polígono para variar a densidade do ponto no polígono. A densidade original é lembrada se você selecionar outros mapas. Se qualquer ponto for adicionado, excluído ou movido no polígono, a densidade original será perdida e o controle deslizante será redefinido para seu valor máximo.

1. Insira um nome para o Mapa de imagem, se desejado, na lista Mapa de imagem. Depois de desenhar um Mapa de imagem, o Adobe Dynamic Media Classic atribui um nome a ele.

   Para criar o nome, o Adobe Dynamic Media Classic anexa um número sequencial ao nome da imagem ou página de catálogo eletrônico com a qual você está trabalhando. Você pode inserir um nome de sua escolha.

1. Se desejar que os usuários abram uma nova página da Web ao selecionar o Mapa de imagem, insira o URL na lista Mapa de imagem.

   Consulte [para inserir JavaScript e URLs](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Para exibir o texto de sobreposição quando os usuários moverem o ponteiro sobre o Mapa de imagem, insira o texto na lista Mapa de imagem. Na lista Mapa de imagem, selecione o menu **[!UICONTROL Show]** e selecione **[!UICONTROL Rollover Text]**. Em seguida, insira o texto que deseja que os usuários vejam na tela. Você pode gravar o texto em um processador de texto e copiá-lo no campo de texto Sobreposição .

1. Se desejar que outro efeito de ação ocorra quando os usuários moverem o mouse sobre um Mapa de imagem, defina a ação. Na lista suspensa **[!UICONTROL Show]**, selecione **[!UICONTROL Other Actions]**. Insira os atributos da ação. (Vá para **[!UICONTROL Show]** > **[!UICONTROL Both]** para criar um texto de sobreposição e uma ação para um Mapa de imagem.)

   Consulte [Definir outras ações para Mapas de imagem](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Opcional) Siga um destes procedimentos:

   * Para visualizar mapas de imagem, selecione **[!UICONTROL Preview]**.
   * Para excluir um Mapa de imagem ou vértice de polígono, selecione uma forma na imagem e selecione **[!UICONTROL Delete]**. Ou, para um eCatalog, na guia Páginas do pedido, selecione **[!UICONTROL Clear Maps]** para remover os Mapas de imagem de todas as páginas.
   * Para remover temporariamente um Mapa de imagem de uma imagem, uma imagem em um Conjunto de rotação ou uma página eCatalog, sem excluí-lo, desmarque a opção Ativado apropriada na lista Mapa de imagem.

1. Selecione **[!UICONTROL Save]**.

### Ajustar a posição, a forma e o tamanho dos mapas de imagem {#adjusting-the-position-shape-and-size-of-image-maps}

Para alterar a posição, a forma e o tamanho de um Mapa de imagem, selecione o botão Mapa de imagem . Em seguida, selecione a ferramenta **[!UICONTROL Pan]** e siga estas instruções:

* **Alterar posição**  - Mova o ponteiro para perto, mas não acima, da borda do Mapa de imagem. Ao ver o ícone de seta de quatro pontas, arraste o mapa para um novo local.

* **Alterar o tamanho e a forma**  - A forma como você altera a forma e o tamanho de um Mapa de imagem depende de você estar trabalhando com um Mapa de imagem retangular ou poligonal:

>[!TIP]
>
>Você pode arrastar o controle deslizante Tamanho na parte inferior da tela para alterar as exibições e obter uma visão melhor do Mapa de imagem.

* **Mapa de imagem retangular**  - Mova o ponteiro sobre um lado ou canto do Mapa de imagem. Ao ver o ícone de seta de duas pontas, comece a arrastar. Mantenha pressionada a tecla Shift enquanto arrasta para alterar o tamanho, mas mantém a proporção (a forma).

* **Mapa de imagem poligonal**  - Arraste uma alça de seleção quadrada. Para criar um identificador de seleção, selecione a borda do Mapa de imagem e comece a arrastar.

### Manipular mapas de imagem sobrepostos {#handling-overlapping-image-maps}

Se a sua página de imagem ou eCatalog incluir mais de um Mapa de imagem e os mapas se sobrepõem, você pode determinar como os mapas se sobrepõem. Para fazer isso, altere a ordem dos mapas na lista Mapa de imagem. Arraste os nomes para cima ou para baixo da lista. A altura em que um nome está na lista determina se o Mapa de imagem se sobrepõe a outros Mapas de imagem.

### Importar dados do mapa de imagem {#importing-image-map-data}

Em vez de inserir dados do Mapa de imagem em cada página, você pode importar os dados da imagem, do Conjunto de rotação ou do eCatalog para a tela do Resumo do mapa. Você importa os dados do Mapa de imagem no formulário de um arquivo delimitado por tabulação ou XML DTD. Os campos no arquivo devem estar na ordem mostrada na tela Mapear resumo : Nome, Rótulos de sumário, Mapas, URLs, Texto de sobreposição, Outras ações e Strings de pesquisa. Importar dados do mapa de imagem salva o trabalho de inserir os dados na Lista de mapa de imagem à medida que você cria cada mapa de imagem.

**Para importar dados do Mapa de imagem:**

1. Vá para a página do editor de Mapa de imagem (para imagens ou em Conjuntos de rotação) ou para a guia Páginas de mapa da tela de edição do eCatalog.
1. Selecione **[!UICONTROL Import Metadata]**.
1. Na caixa de diálogo Fazer upload de metadados , selecione Imagem ou Mapa de imagem para fazer upload dos metadados do tipo de propriedade do ativo desejado.
1. Na lista suspensa Gerar arquivo , selecione o tipo de arquivo que deseja criar.
1. (Opcional) Selecione **[!UICONTROL Generate]** para visualizar os dados resultantes com base no tipo de arquivo que deseja criar. Selecione **[!UICONTROL Close]** para retornar à caixa de diálogo Fazer upload de metadados .
1. Navegue até o arquivo que deseja fazer upload. No campo de texto Nome do arquivo , especifique o nome do arquivo gerado.
1. (Opcional) No campo Nome do trabalho , especifique um nome para o trabalho de upload de metadados.
1. Selecione **[!UICONTROL Upload]**.

### Copiar mapas de imagem {#copying-image-maps}

Você pode copiar mapas de imagem de uma imagem ou de uma página de catálogo eletrônico para outra. Use **[!UICONTROL Copy Image Map]** para que um cabeçalho comece a criá-los. Também é possível copiar Mapas de imagem para recriá-los em imagens ou páginas que compartilham layout ou estrutura de mapeamento.

Por exemplo, copiar mapas de imagem em um eCatalog é uma maneira conveniente de copiar todos os mapas de imagem entre versões de idioma estrangeiro do mesmo eCatalog. Para obter melhores resultados, a cópia é mais bem-sucedida se você copiar entre eCatalogs com o mesmo número de páginas e as mesmas imagens. Se o eCatalog para o qual você copia já contiver mapas de imagem, esses mapas de imagem serão excluídos quando a cópia for feita.

**Para copiar mapas de imagem:**

1. Vá para a página do editor de Mapa de imagem (para imagens ou em Conjuntos de rotação) ou para a guia Páginas de mapa da tela de edição do eCatalog.
1. Selecione **[!UICONTROL Copy Maps to]**.
1. Siga um destes procedimentos, com base em se você estiver copiando mapas de imagem de imagens ou copiando mapas de imagem de um eCatalog:

   * (Imagens) Na tela Selecionar imagens , selecione as imagens para as quais deseja copiar os Mapas de imagens.
   * (Catálogo eletrônico) Na tela Selecionar ativo, selecione as imagens ou as páginas do eCatalog para as quais deseja copiar os mapas de imagem.

1. Escolha **[!UICONTROL Select]**.

## Usar um modelo para inserir JavaScript e URLs {#using-a-template-to-enter-javascript-and-urls}

Você pode definir um modelo de URL (também conhecido como modelo Href) para tornar a inserção de URLs de mapa de imagem mais fácil e eficiente. Defina um modelo de URL se a maioria dos URLs do mapa de imagem compartilhar um formato fixo e comum. Ao inserir a parte do URL que é fixa como modelo de URL, não é necessário inserir essa parte do URL sempre que criar um Mapa de imagem. Seu modelo de URL também pode conter comandos, nomes de caminho e parâmetros do JavaScript. Por padrão, o modelo de URL contém um manipulador JavaScript do Adobe Classic proprietário chamado `loadProduct` que abre a imagem em uma nova janela.

>[!NOTE]
>
>Quando você adiciona o código JavaScript ao atributo HREF do mapa de imagem, o código é executado no computador do cliente. Portanto, verifique se o código JavaScript é seguro.

### Sobre templates de URL {#about-url-templates}

O modelo de URL funciona substituindo o conteúdo da coluna URL na lista Mapa de imagem pelos sinais de dólar duplo (‘$$’) no modelo:

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Você coloca todos os valores que não mudam entre os mapas de imagem no modelo de URL. Adicione apenas os valores que mudam na coluna URL da lista Mapa de imagem. Por exemplo:

* Modelo de URL - `javascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* Valor do URL - `product.htm`
* URL real gerado - `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

Por padrão, o modelo de URL inclui um manipulador JavaScript do Adobe Classic proprietário chamado `loadProduct` que abre uma nova janela com o destino do URL. No entanto, você pode usar qualquer código JavaScript para substituir esse manipulador JavaScript ou usar um dos seguintes manipuladores do Adobe Dynamic Media Classic:

* `loadProductCW` - Exibe o destino do URL especificado na coluna URL na janela atual. Esse manipulador é principalmente para eCatalogs integradas em uma página de um site.

* `loadProductPW` - Exibe o destino do URL especificado na coluna URL na janela principal (a página que abriu o atual). A janela atual permanece aberta, mas a janela pai é alterada para exibir o destino do URL.

   >[!NOTE]
   >
   >O manipulador `loadProductPW` não oferece suporte a visualizadores DHTML e HTML5.

### Criar um modelo de URL {#creating-a-url-template}

1. Na tela Editor de mapa (imagens ou Conjuntos de rotação) ou na guia Mapear páginas da tela Catálogo eletrônico (eCatalogs), selecione Editar ao lado da opção Modelo de URL. A caixa de diálogo Editar modelo de mapa é aberta.
1. Insira o código JavaScript e o URL completo (com a parte variável substituída por cifrões [$]). Você pode colar o código clicando com o botão direito do mouse e escolhendo **[!UICONTROL Paste]**.
1. Selecione **[!UICONTROL Save]**.

### Gerenciar modelos de URL {#handling-url-templates}

A página Editor de mapa (imagens e Conjuntos de rotação) e a guia Páginas de mapa da tela eCatalog (eCatalogs) oferecem esses comandos para manipular modelos de URL:

* **Opção de modelo de URL**  - Selecione a opção Modelo de URL para aplicar seu modelo de URL a todos os mapas de imagem em uma página de imagem ou eCatalog.

* **Opção de modelo**  - Desmarque uma opção de modelo na lista Mapa de imagem do URL se não quiser que um Mapa de imagem individual use o modelo de URL.

## Definir outras ações para Mapas de imagem {#defining-other-actions-for-image-maps}

Você pode selecionar o menu **[!UICONTROL Show]** e escolher **[!UICONTROL Other Actions]** para acionar ações diferentes de sobrepor texto e inicializações de página da Web. Quando o usuário move o ponteiro sobre um Mapa de imagem, você pode iniciar uma ação. Essas ações são atributos definidos para mapas de imagem do lado do cliente pelas especificações HTML do World Wide Web Consortium. Eles incluem:

* **`accesskey`** - Aciona uma ação quando o usuário pressiona uma tecla designada no teclado.

* **`onfocus`** - Dispara um evento quando o Mapa de imagem recebe foco, por cursor, tabulação ou pressionando uma tecla de acesso. Por exemplo, você pode iniciar uma página da Web quando o Mapa de imagem recebe o foco e o fecha quando o Mapa de imagem perde o foco.

* **`onblur`** - Dispara um evento quando o Mapa de imagem perde o foco, seja pelo cursor ou por meio de uma tabulação.

**Para definir outras ações para os Mapas de imagem:**

1. Na tela Editor de mapa (imagens e Conjuntos de rotação) ou na guia Páginas de mapa da tela Catálogo eletrônico (eCatalogs), selecione o menu **[!UICONTROL Show]** e selecione **[!UICONTROL Other Actions]**.
1. Usando a sintaxe especificada pelas especificações HTML do World Wide Web Consortium, adicione os atributos suportados na coluna Outras ações da lista Mapa de imagem.
1. Selecione **[!UICONTROL Save]**.

Selecione o menu **[!UICONTROL Show]** e selecione **[!UICONTROL Both]** se desejar que um Mapa de imagem tenha um texto sobreposto e uma ação.

## Criar mapas de imagem no Adobe Acrobat ou Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Você pode criar mapas de imagem ao criar seu eCatalog no Adobe Acrobat ou no Adobe InDesign.

No Acrobat ou InDesign, crie referências de hiperlink onde deseja que os Mapas de imagem apareçam e especifique os locais do URL para o mapa de imagem. Selecionar a opção Extrair links ao carregar o arquivo PDF no Adobe Dynamic Media Classic converte automaticamente os links para os mapas de imagem.

Para obter mais informações, consulte Ajuda do Adobe InDesign ou Ajuda do Adobe Acrobat.

### Para criar mapas de imagem no Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. No InDesign, vá para **[!UICONTROL Windows®]** > **[!UICONTROL Interactive]** > **[!UICONTROL Hyperlinks]**.
1. No painel Hiperlinks, selecione o texto, quadro ou gráfico que deseja transformar em um Mapa de imagem.
1. Selecione **[!UICONTROL New Hyperlink]** no menu do painel.
1. Na caixa de diálogo Novo hiperlink, no menu **[!UICONTROL Link To]**, escolha **[!UICONTROL URL]**.
1. Digite ou cole a ID do produto na caixa URL.
1. Selecione **[!UICONTROL OK]**. (O Adobe Dynamic Media Classic conclui o URL usando o modelo de URL do mapa de imagem.)

   >[!NOTE]
   >
   >Não é necessário definir opções de aparência no Adobe InDesign. Você pode especificar a aparência no Adobe Dynamic Media Classic.

1. Repita as etapas de 2 a 6 para todos os mapas de imagem que deseja criar.
1. Exportar o arquivo como PDF.
1. Faça upload do PDF para o Adobe Dynamic Media Classic.
1. Em **[!UICONTROL PDF Options]**, selecione **[!UICONTROL Extract Links]**.

### Para criar mapas de imagem no Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. No Acrobat, vá para **[!UICONTROL Tools]** > **[!UICONTROL Advanced Editing]** > **[!UICONTROL Link Tool]**.
1. Arraste para criar o Mapa de imagem.
1. Na caixa Criar link , selecione **[!UICONTROL Custom Link]** e selecione **[!UICONTROL Next]**.

>[!NOTE]
>
>Não é necessário definir opções de aparência no Adobe Acrobat. Você pode especificar a aparência no Adobe Dynamic Media Classic.

1. Na caixa Propriedades do link, selecione **[!UICONTROL Actions]**.
1. Selecione **[!UICONTROL Open A Web Link]** no menu Selecionar ação e selecione **[!UICONTROL Add]**.
1. Digite a ID do produto para o Mapa de imagem na caixa Editar URL e selecione **[!UICONTROL OK]**. (O Adobe Dynamic Media Classic conclui o URL usando o modelo de URL do mapa de imagem.)
1. Repita as etapas de 1 a 7 para todos os mapas de imagem que deseja criar.
1. Salve o arquivo.
1. Carregue o PDF no Adobe Dynamic Media Classic e selecione Extrair links nas Opções de PDF.
