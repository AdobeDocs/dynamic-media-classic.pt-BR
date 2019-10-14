---
title: Criação de um conjunto de rotação
seo-title: Criação de um conjunto de rotação
description: nulo
seo-description: Saiba como criar um Conjunto de rotação.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: referência
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/category/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Criação de um conjunto de rotação{#creating-a-spin-set}

Para criar um conjunto de rotação eficaz, certifique-se de capturar as imagens corretamente. Você pode criar um Conjunto de rotação no Dynamic Media Classic selecionando o botão Criar e escolhendo Conjuntos de rotação. Edite Conjuntos de rotação na tela Conjuntos de rotação.

>[!NOTE]
>
>As versões anteriores do Dynamic Media Classic não ofereciam Conjuntos de rotação bidimensionais. Se você tiver criado um Conjunto de rotação em uma versão anterior do Dynamic Media Classic, não poderá salvar seu Conjunto de rotação unidimensional sem primeiro salvá-lo com um nome diferente. Clique em Salvar como na tela Conjunto de rotação e insira um novo nome para que você possa editá-lo no Dynamic Media Classic.

## Diretrizes para fotografar imagens do Spin Set {#guidelines-for-shooting-spin-set-images}

Em geral, quanto mais imagens você tiver em um Conjunto de rotação, melhor será o efeito de rotação da imagem. Entretanto, a inclusão de muitas imagens no conjunto também aumenta a quantidade de tempo necessário para carregar as imagens. O Dynamic Media Classic recomenda estas diretrizes para fotografar imagens para uso em Conjuntos de rotação:

* No mínimo, use 8 a 12 imagens em um conjunto de rotação unidimensional e 16 a 24 imagens em um conjunto de rotação bidimensional.
* Usar um formato sem perdas; TIFF e PNG são recomendados.
* Mascarar todas as imagens para que o item apareça em um fundo branco puro ou em outro plano de alto contraste. Como opção, adicione sombras.
* Verifique se os detalhes do produto estão bem iluminados e em foco.
* Leve imagens de rotação para roupas de moda com um manequim ou modelo. Muitas vezes o manequim é completamente mascarado (utilizando um manequim de vidro) ou na imagem é apresentado um manequim/forma estilizada. É possível criar um conjunto de rotação no modelo definindo o número de ângulos. Marque cada ângulo com uma fita no chão para guiar o modelo a pisar e olhe na direção de cada tomada.

## Criação de um conjunto de rotação {#create}

Esteja ciente de que a ordem em que o Conjunto de rotação é criado ou criado no Scene7 Publishing System é importante. Dependendo de como você ordena os ativos quando arrasta e solta imagens na grade na página Conjunto de rotação, o Conjunto de rotação gira em uma determinada direção. Portanto, a ordem em que é exibido visualmente no construtor é como o ativo é girado quando um usuário move o ponteiro do mouse ou move o dedo, da esquerda para a direita.

Quando você cria um conjunto, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| opção "Publicar após salvar" selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos retêm seu estado publicado ou não publicado. |

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually-publishing-assets) a publicação de ativos [](publishing-files.md#manually-unpublishing-assets)manualmente.

Depois de salvar um conjunto de rotação, você pode usar Visualizar na compilação: Página de conjunto de rotação para ver a aparência do seu conjunto de rotação no visualizador padrão.

**Para criar um conjunto de giros**

1. No menu suspenso **Criar** , clique em Conjuntos de **rotação**.
1. Na caixa de diálogo Tamanho do conjunto de rotação, defina o número de linhas e células desejado.

   Para criar um conjunto de rotação unidimensional, selecione apenas uma linha.

   Para criar um conjunto de rotação bidimensional, selecione duas ou mais linhas.

1. Clique em **OK**.
1. Arraste e solte imagens na grade na tela Conjunto de rotação.
1. Quando terminar, próximo ao canto inferior direito da página, verifique se a opção **Publicar após salvar** está selecionada (padrão).
1. Clique em **Salvar**.
1. Na caixa de diálogo Salvar, selecione uma pasta para armazenar seu conjunto de rotação. No campo Nome do arquivo, digite o nome do conjunto de spin.
1. Clique em **Salvar**.

## Edição de um conjunto de rotação {#editing-a-spin-set}

Dependendo de se você editar um conjunto publicado ou não publicado, a opção **Publicar após salvar** afetará o conjunto e definirá os membros das seguintes maneiras:

| Definir já publicado? | Opção "Publicar após salvar" selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado.Qualquer novo conjunto de membros adicionado durante a edição mantém seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto que você tiver adicionado durante a edição manterão seu estado publicado ou não publicado. |

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually-publishing-assets) a publicação de ativos [](publishing-files.md#manually-unpublishing-assets)manualmente.

**Para editar um conjunto de giros**

1. Clique no botão **Editar** sobreposição do Conjunto de rotação.
1. Execute um dos procedimentos a seguir:

   * **Remoção de imagens** Selecione a imagem e clique em **Excluir**.

   * **Adicionar imagens** Arraste a imagem para dentro de uma célula.

   * **Reorganizando linhas (Conjuntos de rotação bidimensionais)** Clique em uma caixa seletor de linhas (à esquerda da linha) e, em seguida, clique em **Mover linha para baixo** ou **Mover linha para cima**.

   * **Adicionando linhas e células** Insira um número na caixa Linhas e Células para determinar o número de linhas e o número de células em cada linha.

1. Quando terminar a edição, próximo ao canto inferior direito da página, certifique-se de que a opção **Publicar após salvar** esteja selecionada (padrão).
1. Clique em **Salvar**, selecione uma pasta de armazenamento, digite um nome para o conjunto e clique em **Salvar**.

## Excluindo um conjunto de rotação {#deleting-a-spin-set}

Ao excluir um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou "filhos") dentro desse conjunto não são afetados; em vez disso, cada um deles mantém seu estado publicado ou não publicado.

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually-publishing-assets) a publicação de ativos [](publishing-files.md#manually-unpublishing-assets)manualmente.

**Para excluir um conjunto de rotação**

1. Na Exibição de grade, Exibição de lista ou Exibição de detalhes, selecione um ou mais Conjuntos de rotação.
1. Na barra de navegação global, clique em **Arquivo** &gt; **Excluir** &gt; **Excluir**.

