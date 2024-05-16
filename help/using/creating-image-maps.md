---
title: Criar mapas de imagem
description: Saiba como criar Mapas de imagem no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '2368'
ht-degree: 0%

---

# Criar mapas de imagem {#creating-image-maps}

Um Mapa de imagem é uma região em uma imagem, uma página de eCatalog ou uma imagem em um SpinSet que exibe um painel de sobreposição com texto. Quando o usuário seleciona um Mapa de imagem, uma ação de algum tipo é acionada. Por exemplo, uma página da Web é iniciada para que o usuário possa saber mais sobre um produto. Um contorno é exibido ao redor de um Mapa de imagem quando o usuário move o ponteiro sobre ele.

Além da capacidade de criar Mapas de imagem no Adobe Dynamic Media Classic, você também pode criar Mapas de imagem ao criar um catálogo no Adobe Acrobat ou no Adobe InDesign.

Ao criar Mapas de imagem, você pode executar um dos seguintes procedimentos:

* Insira o texto de sobreposição.
* Insira JavaScript e URLs para iniciar páginas da Web.
* Crie modelos de URL para Mapas de imagem.
* Copie Mapas de imagem para outras imagens, páginas de eCatalog ou SpinSets.
* Exportar mapas de imagem para CSV ou XML.
* Importe metadados de imagem de um arquivo delimitado por tabulação ou de um arquivo XML.
* Defina Outras ações conforme determinado pelo World Wide Web Consortium.
* Visualizar mapas de imagem.

## Desenhar e ajustar um Mapa de imagem {#drawing-and-adjusting-an-image-map}

1. Siga um destes procedimentos:

   * Se estiver trabalhando com uma imagem na Exibição em Grade ou em Lista, na lista suspensa Editar, selecione **[!UICONTROL Image Map]**. Ou abra-a na Exibição de Detalhes e selecione **[!UICONTROL Image Map]** acima da imagem.
   * Se estiver trabalhando com um SpinSet na Exibição em grade ou em lista, selecione **[!UICONTROL Edit]**. Ou abra-a na Exibição de Detalhes e selecione **[!UICONTROL Edit]**. Selecione um ativo de imagem e selecione **[!UICONTROL Image Map]**.
   * Se você estiver trabalhando com um eCatalog, na Exibição em Grade, Exibição em Lista, Exibição Detalhada, selecione **[!UICONTROL Edit]**. Selecione o **[!UICONTROL Map Pages]** guia.

   ![Ilustração do Mapa de imagem](assets/ma_image_map.png)

1. Desenhe um mapa de imagem retangular ou poligonal (em vários lados):

   * **Mapa retangular**: selecione a ferramenta Mapa de imagem de retângulo e arraste na página para criar o retângulo. Para adicionar um ponto a um mapa retangular (alterando-o para um mapa de polígono), pressione Ctrl, coloque a ferramenta de inserção no local desejado e selecione.

   * **Mapa poligonal**: selecione a ferramenta Mapa de Imagem de Polígono e selecione pontos no perímetro da área da imagem que você deseja delimitar. Use o controle deslizante de densidade do polígono para variar a densidade do ponto no polígono. A densidade original é lembrada se você selecionar outros mapas. Se algum ponto for adicionado, excluído ou movido no polígono, a densidade original será perdida. O controle deslizante é redefinido para seu valor máximo.

1. Insira um nome para o Mapa de imagem, se desejado, na lista Mapa de imagem. Depois de desenhar um Mapa de imagem, o Adobe Dynamic Media Classic atribui um nome a ele.

   Para criar o nome, o Adobe Dynamic Media Classic anexa um número sequencial ao nome da imagem ou página de eCatalog com a qual você está trabalhando. Você pode inserir um nome de sua escolha.

1. Se quiser que os usuários abram uma nova página da Web ao selecionar o Mapa de imagem, insira o URL na lista Mapa de imagem.

   Consulte [para inserir JavaScript e URLs](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Para exibir o texto de rolagem quando os usuários moverem o ponteiro sobre o Mapa de imagem, insira o texto na lista Mapa de imagem. Na lista Mapa de imagem, selecione a variável **[!UICONTROL Show]** e selecione **[!UICONTROL Rollover Text]**. Em seguida, insira o texto que deseja que os usuários vejam na tela. Você pode escrever o texto em um processador de texto e copiá-lo no campo de texto &#39;Sobreposição&#39;.

1. Se quiser que outro efeito de ação ocorra quando os usuários moverem o mouse sobre um Mapa de imagem, defina a ação. No **[!UICONTROL Show]** selecione **[!UICONTROL Other Actions]**. Insira os atributos da ação. (Vá para **[!UICONTROL Show]** > **[!UICONTROL Both]** para criar um texto de sobreposição e uma ação para um Mapa de imagem.)

   Consulte [Definir outras ações para Mapas de imagem](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Opcional) Siga qualquer um destes procedimentos:

   * Para visualizar Mapas de imagem, selecione **[!UICONTROL Preview]**.
   * Para excluir um Mapa de Imagem ou vértice do polígono, selecione uma forma na imagem e selecione **[!UICONTROL Delete]**. Ou, para um eCatalog, na guia Ordenar páginas, selecione **[!UICONTROL Clear Maps]** para remover Mapas de imagem de todas as páginas.
   * Para remover um:
      * Mapa de imagem de uma imagem
      * uma imagem em um SpinSet
      * ou uma página de eCatalog

     temporariamente, sem excluí-lo, desmarque a opção Ativado apropriada na lista Mapa de imagem.

1. Selecionar **[!UICONTROL Save]**.

### Ajustar a posição, a forma e o tamanho dos Mapas de imagem {#adjusting-the-position-shape-and-size-of-image-maps}

Para alterar a posição, a forma e o tamanho de um Mapa de Imagem, selecione o botão Mapa de Imagem. Em seguida, selecione o **[!UICONTROL Pan]** e siga estas instruções:

* **Alterar posição**: mova o ponteiro próximo à borda do Mapa de imagem, mas não acima dela. Ao visualizar o ícone de seta de quatro pontas, arraste o mapa para um novo local.

* **Alterar tamanho e forma**: a forma como você altera a forma e o tamanho de um Mapa de imagem depende de você estar trabalhando com um Mapa de imagem retangular ou poligonal:

>[!TIP]
>
>Você pode arrastar o controle deslizante Tamanho na parte inferior da tela para alterar visualizações e obter uma melhor visualização do Mapa de imagem.

* **Mapa de imagem retangular**: mova o ponteiro sobre um lado ou canto do Mapa de imagem. Ao visualizar o ícone de seta de duas pontas, comece a arrastar. Mantenha pressionada a tecla Shift enquanto arrasta para alterar o tamanho, mas manter a proporção (a forma).

* **Mapa de imagem poligonal**: arraste uma alça de seleção quadrada. Para criar uma alça de seleção, selecione a borda do Mapa de imagem e comece a arrastar.

### Manipular mapas de imagem sobrepostos {#handling-overlapping-image-maps}

Se sua página de imagem ou eCatalog incluir mais de um Mapa de imagem e os mapas se sobrepuserem, você poderá determinar como os mapas se sobrepõem. Para fazer isso, altere a ordem dos mapas na lista Mapa de imagem. Arraste os nomes para cima ou para baixo na lista. A altura de um nome na lista determina se o Mapa de imagem se sobrepõe a outros Mapas de imagem.

### Importar dados do Mapa de imagem {#importing-image-map-data}

Em vez de inserir dados do Mapa de imagem em cada página, você pode importar os dados da imagem, do Conjunto de rotação ou do eCatalog na tela Resumo do mapa. Importe os dados do Mapa de imagem no formato de um arquivo delimitado por tabulação ou DTD XML. Os campos no arquivo devem estar na ordem mostrada na tela Resumo do Mapa: Nome, Rótulos do índice, Mapas, URLs, Texto de rolagem, Outras ações e Strings de pesquisa. A importação de dados do Mapa de imagem evita a dificuldade de inserir os dados na lista do Mapa de imagem à medida que você cria cada Mapa de imagem.

**Para importar dados do Mapa de imagem:**

1. Vá para a página do editor de Mapa de imagem (para imagens ou imagens em SpinSets) ou para a guia Páginas de mapa da tela de edição do eCatalog.
1. Selecionar **[!UICONTROL Import Metadata]**.
1. Na caixa de diálogo Fazer upload de metadados, selecione Imagem ou Mapa de imagem para fazer upload dos metadados do tipo de propriedade do ativo desejado.
1. No `Generate File` selecione o tipo de arquivo que deseja criar.
1. (Opcional) Selecione **[!UICONTROL Generate]** para visualizar os dados resultantes com base no tipo de arquivo que você deseja criar. Selecionar **[!UICONTROL Close]** para retornar à caixa de diálogo Fazer upload de metadados.
1. Navegue até o arquivo que deseja fazer upload. No campo de texto Nome do arquivo, especifique o nome do arquivo gerado.
1. (Opcional) No campo Nome do trabalho, especifique um nome para o trabalho de upload de metadados.
1. Selecionar **[!UICONTROL Upload]**.

### Copiar mapas de imagem {#copying-image-maps}

É possível copiar Mapas de imagem de uma imagem ou de uma página de eCatalog para outra. Uso **[!UICONTROL Copy Image Map]** para começar a criá-las. Também é possível copiar Mapas de imagem para recriá-los em imagens ou páginas que compartilham layout ou estrutura de mapeamento.

Por exemplo, copiar Mapas de imagens em um eCatalog é uma maneira conveniente de copiar todos os Mapas de imagens entre versões em outros idiomas do mesmo eCatalog. Para obter melhores resultados, a cópia é mais bem-sucedida se você copiar entre eCatalogs com o mesmo número de páginas e as mesmas imagens. Se o eCatalog para o qual você copiar já contiver Mapas de imagem, esses Mapas de imagem serão excluídos quando a cópia for feita.

**Para copiar Mapas de Imagem:**

1. Vá para a página do editor de Mapa de imagem (para imagens ou imagens em SpinSets) ou para a guia Páginas de mapa da tela de edição do eCatalog.
1. Selecionar **[!UICONTROL Copy Maps to]**.
1. Desempenhe uma das ações a seguir, com base no caso de você estar copiando Mapas de imagem de imagens ou copiando Mapas de imagem de um eCatalog:

   * (Imagens) Na tela Selecionar imagens, selecione as imagens para as quais deseja copiar os Mapas de imagem.
   * (eCatalog) Na tela Selecionar ativo, selecione as imagens ou páginas de eCatalog para as quais deseja copiar os Mapas de imagem.

1. Escolher **[!UICONTROL Select]**.

## Use um modelo para inserir JavaScript e URLs {#using-a-template-to-enter-javascript-and-urls}

Você pode definir um modelo de URL (também conhecido como modelo Href) para tornar a inserção de URLs do Mapa de imagem mais fácil e eficiente. Defina um modelo de URL se a maioria dos URLs do Mapa de imagem compartilhar um formato comum e fixo. Ao inserir a parte do URL que é fixa como o modelo de URL, não é necessário inserir essa parte do URL toda vez que você criar um Mapa de imagem. Seu modelo de URL também pode conter comandos JavaScript, nomes de caminho e parâmetros. Por padrão, o modelo de URL contém um manipulador Adobe Dynamic Media Classic JavaScript proprietário chamado `loadProduct` que abre a imagem em uma nova janela.

>[!NOTE]
>
>Ao adicionar o código JavaScript ao atributo HREF do Mapa de imagem, ele é executado no computador do cliente. Portanto, verifique se o código JavaScript é seguro.

### Sobre modelos de URL {#about-url-templates}

O modelo de URL funciona substituindo o conteúdo da coluna URL na lista Mapa de imagem. Ele o substitui pelos sinais de cifrão duplo (&#39;$$&#39;) no modelo:

```as3
Javascript:loadProduct('$$');void(0);
```

Você coloca todos os valores que não são alterados entre Mapas de imagem no modelo de URL. Adicione apenas os valores que são alterados na coluna URL na lista Mapa de imagem. Por exemplo:

* Modelo de URL: `javascript:loadProduct('https://www.examplesitehere.com/$$');void(0);`
* Valor do URL: `product.htm`
* URL real gerado: `javascript:loadProduct('https://www.examplesitehere.com/product.html);void(0);`

Por padrão, o modelo de URL inclui um manipulador Adobe Dynamic Media Classic JavaScript proprietário chamado `loadProduct` que abre uma nova janela com o destino do URL. No entanto, você pode usar qualquer código JavaScript para substituir esse manipulador JavaScript ou usar um dos seguintes manipuladores Adobe Dynamic Media Classic:

* `loadProductCW`: exibe o destino do URL especificado na coluna URL na janela atual. Esse manipulador é principalmente para eCatalogs que são integrados em uma página em um site.

* `loadProductPW`: exibe o destino do URL especificado na coluna URL na janela principal (a página que abriu a atual). A janela atual permanece aberta, mas a janela pai é alterada para exibir o destino do URL.

  >[!NOTE]
  >
  >O manipulador `loadProductPW` O não é compatível com visualizadores DHTML e HTML5.

### Criar um modelo de URL {#creating-a-url-template}

1. Na tela Editor de mapas (imagens ou SpinSets) ou na guia Mapear páginas da tela eCatalog (eCatalogs), selecione Editar ao lado da opção de modelo de URL. A caixa de diálogo Editar modelo de mapa é aberta.
1. Insira o código JavaScript e o URL completo (com a parte da variável substituída por cifrões) [$$]). Você pode colar o código clicando com o botão direito do mouse e escolhendo **[!UICONTROL Paste]**.
1. Selecionar **[!UICONTROL Save]**.

### Lidar com modelos de URL {#handling-url-templates}

A página Editor de mapa (imagens e SpinSets) e a guia Páginas de mapa da tela eCatalog (eCatalogs) oferecem estes comandos para manipular modelos de URL:

* **Opção de modelo de URL**: selecione a opção de modelo de URL para aplicar seu modelo de URL a todos os Mapas de imagem em uma página de imagem ou eCatalog.

* **Opção de modelo**: Desmarque uma opção Modelo na lista Mapa de imagem do URL se não quiser que um Mapa de imagem individual use o modelo de URL.

## Definir outras ações para Mapas de imagem {#defining-other-actions-for-image-maps}

É possível selecionar a variável **[!UICONTROL Show]** e escolha **[!UICONTROL Other Actions]** para acionar ações diferentes de texto de sobreposição e inicializações de página da Web. Quando o usuário move o ponteiro sobre um Mapa de imagem, é possível iniciar uma ação. Essas ações são atributos definidos para mapas de imagem do lado do cliente pelas especificações de HTML do World Wide Web Consortium. Eles incluem:

* **`accesskey`**: aciona uma ação quando o usuário pressiona uma tecla designada no teclado.

* **`onfocus`**: aciona um evento quando o Mapa de imagem recebe foco — pelo cursor, tabulação ou pressionando uma tecla de acesso. Por exemplo, é possível iniciar uma página da Web quando o Mapa de imagem recebe o foco e fechá-lo quando o Mapa de imagem perde o foco.

* **`onblur`**: aciona um evento quando o Mapa de imagem perde o foco, seja pelo cursor ou pela tabulação.

**Para definir outras ações para Mapas de imagem:**

1. Na tela Editor de mapas (imagens e SpinSets) ou na guia Mapear páginas da tela eCatalog (eCatalogs), selecione a **[!UICONTROL Show]** e selecione **[!UICONTROL Other Actions]**.
1. Usando a sintaxe especificada pelas especificações de HTML do World Wide Web Consortium, adicione os atributos compatíveis na coluna Outras ações da lista Mapa de imagem.
1. Selecionar **[!UICONTROL Save]**.

Selecione o **[!UICONTROL Show]** e selecione **[!UICONTROL Both]** se quiser que um Mapa de imagem tenha um texto de sobreposição e uma ação.

## Criar mapas de imagem no Adobe Acrobat ou no Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

É possível criar Mapas de imagem ao projetar seu eCatalog no Adobe Acrobat ou Adobe InDesign.

No Adobe Acrobat ou Adobe InDesign, crie referências de hiperlink onde deseja que os Mapas de imagem sejam exibidos e especifique os locais de URL para o Mapa de imagem. Selecionar a opção Extrair links ao fazer upload do arquivo de PDF no Adobe Dynamic Media Classic converte automaticamente os links para Mapas de imagem.

Para obter mais informações, consulte Ajuda do Adobe InDesign ou Ajuda do Adobe Acrobat.

### Para criar Mapas de imagem no Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. No Adobe InDesign, acesse **[!UICONTROL Windows®]** > **[!UICONTROL Interactive]** > **[!UICONTROL Hyperlinks]**.
1. No painel &#39;Hiperlinks&#39;, selecione o texto, o quadro ou o gráfico que deseja transformar em um mapa de imagem.
1. Selecionar **[!UICONTROL New Hyperlink]** no menu do painel.
1. Na caixa de diálogo Novo hiperlink, no **[!UICONTROL Link To]** selecione o **[!UICONTROL URL]**.
1. Digite ou cole a ID do produto na caixa URL.
1. Selecionar **[!UICONTROL OK]**. (O Adobe Dynamic Media Classic conclui o URL usando o modelo de URL do Mapa de imagem.)

   >[!NOTE]
   >
   >Não é necessário definir as opções de aparência no Adobe InDesign. Você pode especificar a aparência no Adobe Dynamic Media Classic.

1. Repita as etapas de 2 a 6 para todos os Mapas de imagem que deseja criar.
1. Exporte o arquivo como um PDF.
1. Carregue o PDF para o Adobe Dynamic Media Classic.
1. Entrada **[!UICONTROL PDF Options]**, selecione **[!UICONTROL Extract Links]**.

### Para criar Mapas de imagem no Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. No Adobe Acrobat, acesse **[!UICONTROL Tools]** > **[!UICONTROL Advanced Editing]** > **[!UICONTROL Link Tool]**.
1. Arraste para criar o Mapa de imagem.
1. Na caixa Criar link, selecione **[!UICONTROL Custom Link]** e selecione **[!UICONTROL Next]**.

>[!NOTE]
>
>Não é necessário definir as opções de aparência no Adobe Acrobat. Você pode especificar a aparência no Adobe Dynamic Media Classic.

1. Na caixa Propriedades do link, selecione **[!UICONTROL Actions]**.
1. Selecionar **[!UICONTROL Open A Web Link]** no menu Selecionar ação e selecione **[!UICONTROL Add]**.
1. Digite a ID do produto para o Mapa de imagem na caixa Editar URL e selecione **[!UICONTROL OK]**. (O Adobe Dynamic Media Classic conclui o URL usando o modelo de URL do Mapa de imagem.)
1. Repita as etapas de 1 a 7 para todos os Mapas de imagem que deseja criar.
1. Salve o arquivo.
1. Faça upload do PDF para o Adobe Dynamic Media Classic e selecione Extrair links nas Opções de PDF.
