---
title: Criar um conjunto de rotação
seo-title: Criar um conjunto de rotação
description: 'null'
seo-description: Saiba como criar um Conjunto de rotação.
uuid: 697 bd 78 f -5 e 39-46 bf-aa 6 d-ad 8 ab 99 fe 40 e
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/spin_ sets
discoiquuid: 735 b 5867-e 249-4627-a 5 a 5-25 c 19 c 2255 bf
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Criar um conjunto de rotação{#creating-a-spin-set}

Para criar um Conjunto de rotação eficaz, certifique-se de que você capture as imagens corretamente. Você pode criar um Conjunto de rotação no Dynamic Media Classic selecionando o botão Build e escolhendo Conjuntos de rotação. Editar conjuntos de rotação na tela Conjuntos de rotação.

>[!NOTE]
>
>As versões anteriores do Dynamic Media Classic não ofereciam Conjuntos de rotação bidimensionais. Se você criou um Conjunto de rotação em uma versão anterior do Dynamic Media Classic, não é possível salvar o Conjunto de rotação unidimensional sem salvá-lo com outro nome. Clique em Salvar como na tela de Conjunto de rotação e digite um novo nome para que você possa editá-lo no Dynamic Media Classic.

## Diretrizes para a captura de imagens de conjunto de rotação {#guidelines-for-shooting-spin-set-images}

Em geral, quanto mais imagens você tiver em um Conjunto de rotação, melhor será o efeito de rotação de imagem. No entanto, incluir muitas imagens no conjunto também aumenta o tempo necessário para que as imagens sejam carregadas. O Dynamic Media Classic recomenda essas diretrizes para a captura de imagens para uso em Conjuntos de rotação:

* No mínimo, use imagens de 8-12 em um conjunto de rotação unidimensional e 16-24 imagens em um Conjunto de rotação bidimensional.
* Use um formato sem perdas; São recomendados TIFF e PNG.
* Mascara todas as imagens para que o item apareça em um plano de fundo preto ou outro de alto contraste. Como opção, adicione sombras.
* Certifique-se de que os detalhes do produto estejam bem visíveis e em foco.
* Pegue imagens de rotação para roupas de moda com um mannein ou modelo. Geralmente, o mannein é completamente mascarado (usando um vidro mannein) ou um mannein/roupas estilizado é mostrado na imagem. É possível criar um conjunto de rotação no modelo definindo o número de ângulos. Marque cada ângulo com fita no chão para orientar o modelo para a etapa e observar a direção de cada captura.

## Criar um conjunto de rotação {#create}

Esteja ciente de que a ordem em que o Conjunto de rotação é criado ou criado no Sistema de publicação Scene 7 é importante. Dependendo de como você ordena os ativos quando arrasta e solta imagens na grade na página Conjunto de rotação, o Conjunto de rotação gira em uma determinada direção. Assim, a ordem em que é exibida visualmente no construtor é como o ativo é percorrido quando um usuário move o ponteiro do mouse ou move seu dedo, da esquerda para a direita.

Quando você cria um conjunto, **a opção Publicar depois de salvar** afeta o conjunto e os membros definidos das seguintes maneiras:

| A opção «Publicar após salvar» selecionada antes de salvar? | Estado de conjunto após salvar | Estado dos membros definidos após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros podem reter seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually-publishing-assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually-unpublishing-assets).

Depois de salvar um Conjunto de rotação, você pode usar a opção Visualizar na compilação: Página de conjunto de rotação para ver a aparência do Conjunto de rotação no visualizador padrão.

**Para criar um Conjunto de rotação**

1. No menu suspenso **Build** , clique em Conjuntos **de rotação**.
1. Na caixa de diálogo Tamanho do conjunto de rotação, defina o número de linhas e células desejadas.

   Para fazer um conjunto de rotação unidimensional, selecione apenas uma linha.

   Para criar um Conjunto de rotação bidimensional, selecione duas ou mais linhas.

1. Clique **em OK**.
1. Arraste e solte imagens na grade na tela Conjunto de rotação.
1. Quando terminar, próximo ao canto inferior direito da página, certifique-se de **que Publicar depois de salvar** esteja selecionado (padrão).
1. Clique **em Salvar**.
1. Na caixa de diálogo Salvar, selecione uma pasta para armazenar o conjunto de rotação. No campo Nome do arquivo, digite o nome do conjunto de rotação.
1. Clique **em Salvar**.

## Edição de um conjunto de rotação {#editing-a-spin-set}

Se você editar um conjunto publicado ou um conjunto não publicado, **a opção Publicar depois de salvar** afeta o conjunto e os membros definidos das seguintes maneiras:

| Já foi publicado? | A opção «Publicar após salvar» selecionada antes de salvar sua edição? | Estado de conjunto após salvar | Estado dos membros definidos após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros definidos existentes mantêm seu estado publicado. Todos os novos membros definidos durante a edição mantêm seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros definidos e todos os novos membros definidos durante a edição mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually-publishing-assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually-unpublishing-assets).

**Para editar um Conjunto de rotação**

1. Clique no botão **Editar borda do** conjunto de rotação.
1. Execute um dos procedimentos a seguir:

   **Remover imagens**

   Selecione a imagem e clique **em Excluir**.

   **Adicionar imagens**

   Arraste a imagem para uma célula.

   **Reordenar linhas (conjuntos de rotação bidimensionais)**

   Clique em uma caixa seletor de linha (à esquerda da linha) e clique **em Mover linha para baixo** ou **Mover linha para cima**.

   **Adicionar linhas e células**

   Insira um número na caixa Linhas e na caixa Células para determinar o número de linhas e o número de células em cada linha.

1. Quando terminar de editar, próximo ao canto inferior direito da página, certifique-se de **que Publicar depois de salvar** esteja selecionado (padrão).
1. Clique **em Salvar**, selecione uma pasta de armazenamento, digite um nome para o conjunto e clique **em Salvar**.

## Excluindo um conjunto de rotação {#deleting-a-spin-set}

Quando um conjunto é excluído, o próprio conjunto é movido para a lixeira. No entanto, os membros (ou «filhos») dentro desse conjunto não serão afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Consulte também [Publicar manualmente ativos](publishing-files.md#manually-publishing-assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually-unpublishing-assets).

**Para excluir um conjunto de rotação**

1. Na Exibição de grade, Exibição de lista ou Exibição de detalhes, selecione um ou mais Conjuntos de rotação.
1. Na barra de navegação global, clique **em Arquivo** &gt; **Excluir** &gt; **Excluir**.

