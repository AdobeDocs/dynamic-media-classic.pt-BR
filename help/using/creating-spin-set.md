---
title: Criar um grupo de rotação
description: Saiba como criar um Conjunto de rotação no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# Criar um grupo de rotação{#creating-a-spin-set}

Para criar um Spin Set eficaz, certifique-se de fotografar as imagens corretamente. Você pode criar um Conjunto de rotação no Adobe Dynamic Media Classic selecionando o botão Criar e escolhendo Conjuntos de rotação. Editar conjuntos de rotação na tela Conjuntos de rotação.

>[!NOTE]
>
>As versões anteriores do Adobe Dynamic Media Classic não ofereciam Spin Sets bidimensionais. Se você criou um Conjunto de rotação em uma versão anterior do Adobe Dynamic Media Classic, salve-o com um nome diferente e, em seguida, salve seu Conjunto de rotação unidimensional. Selecione **[!UICONTROL Save As]** na tela Conjunto de rotação e digite um novo nome para poder editá-lo no Adobe Dynamic Media Classic.

## Diretrizes para fotografar imagens do grupo de rotação {#guidelines-for-shooting-spin-set-images}

Em geral, quanto mais imagens você tiver em um Conjunto de rotação, melhor será o efeito de rotação da imagem. No entanto, a inclusão de muitas imagens no conjunto também aumenta a quantidade de tempo que as imagens levam para serem carregadas. A Adobe Dynamic Media Classic recomenda estas diretrizes para fotografar imagens para uso em conjuntos de rotação:

* No mínimo, use 8 a 12 imagens em um Conjunto de rotação unidimensional e 16 a 24 imagens em um Conjunto de rotação bidimensional.
* Usar um formato sem perdas; TIFF e PNG são recomendados.
* Mascarar todas as imagens para que o item apareça em branco puro ou em outro plano de fundo de alto contraste. Como opção, adicione sombras.
* Verifique se os detalhes do produto estão bem iluminados e em foco.
* Faça imagens giratórias para roupas de moda com um manequim ou modelo. Muitas vezes, o manequim é mascarado (usando um manequim de vidro) ou um manequim estilizado/costureira é mostrado na imagem. Você pode criar um Conjunto de rotação no modelo definindo o número de ângulos. Marque cada ângulo com fita no chão para que você possa guiar o modelo para pisar e olhar na direção de cada tomada.

## Criar um grupo de rotação {#create}

A ordem em que o conjunto de rotação é criado ou criado no Adobe Dynamic Media Classic é importante. Dependendo de como você ordena os ativos ao arrastar e soltar imagens na grade na página Conjunto de rotação, o Conjunto de rotação gira em uma determinada direção. Portanto, a ordem em que ele é exibido visualmente no construtor é como o ativo é girado quando um usuário move o ponteiro do mouse ou move o dedo, da esquerda para a direita.

Ao criar um conjunto, a opção **[!UICONTROL Publish after a save]** afeta o conjunto e os membros do conjunto das seguintes maneiras:

| **[!UICONTROL Publish after a save]** opção selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar ativos manualmente](publishing-files.md#manually-publishing-assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually-unpublishing-assets).

Ao criar um Conjunto de rotação, a Adobe recomenda a seguinte prática recomendada e impõe o seguinte limite:

| Tipo de limite do grupo de rotação | Prática recomendada | Limite imposto |
| --- | --- | --- |
| Número máximo de linhas/colunas por conjunto 2D | 12 a 18 imagens por conjunto | 1000 |

Consulte também [limitações do Dynamic Media](/help/using/limitations.md).

Depois de salvar um Conjunto de rotação, você pode usar Visualizar na página Criar: Conjunto de rotação para ver a aparência do seu Conjunto de rotação no visualizador padrão.

**Para criar um Conjunto de Rotação:**

1. No menu suspenso **[!UICONTROL Build]**, selecione **[!UICONTROL Spin Sets]**.
1. Na caixa de diálogo Definir tamanho de rotação, defina o número de linhas e células desejadas.

   Para criar um Conjunto de rotação unidimensional, selecione somente uma linha.

   Para criar um Conjunto de rotação bidimensional, selecione duas ou mais linhas.

1. Selecione **[!UICONTROL OK]**.
1. Arraste e solte imagens na grade na tela Conjunto de rotação.
1. Quando terminar, próximo ao canto inferior direito da página, verifique se **Publicar após salvar** está selecionado (padrão).
1. Selecione **[!UICONTROL Save]**.
1. Na caixa de diálogo Salvar, selecione uma pasta para armazenar o Conjunto de rotação. No campo Nome do arquivo, digite o nome do conjunto de rotação.
1. Selecione **[!UICONTROL Save]**.

## Editar um grupo de rotação {#editing-a-spin-set}

Se você editar um conjunto publicado ou um conjunto não publicado, a opção **[!UICONTROL Publish after a save]** afetará o conjunto e os membros do conjunto das seguintes maneiras:

| Conjunto já publicado? | **[!UICONTROL Publish after a save]** opção selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- | --- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existentes mantêm seu estado publicado. Qualquer novo membro do conjunto adicionado durante sua edição manterá seu estado publicado ou não. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existentes e os novos membros do conjunto adicionados durante a edição mantêm seus estados publicado ou não. |

Consulte também [Publicar ativos manualmente](publishing-files.md#manually-publishing-assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually-unpublishing-assets).

**Para editar um Conjunto de Rotação:**

1. Selecione o botão de sobreposição **[!UICONTROL Edit]** do Conjunto de rotação.
1. Siga um destes procedimentos:

   * **Removendo imagens**: selecione a imagem e **[!UICONTROL Delete]**.

   * **Adicionando imagens**: arraste a imagem para uma célula.

   * **Reorganização de linhas (Conjuntos de Rotação bidimensionais)**: selecione uma caixa de seletor de linha (à esquerda da linha) e selecione **[!UICONTROL Move Row Down]** ou **[!UICONTROL Move Row Up]**.

   * **Adicionando linhas e células**: digite um número na caixa Linhas e na caixa Células para determinar o número de linhas e o número de células em cada linha.

1. Quando você terminar a edição, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after a save]** está selecionado (padrão).
1. Selecione **[!UICONTROL Save]**, selecione uma pasta de armazenamento, insira um nome para o conjunto e selecione **[!UICONTROL Save]**.

## Excluir um grupo de rotação

Quando você exclui um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Consulte também [Publicar ativos manualmente](publishing-files.md#manually-publishing-assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually-unpublishing-assets).

**Para excluir um grupo de rotação:**

1. Na Exibição em grade, Exibição em lista ou Exibição de detalhes, selecione um ou mais Conjuntos de rotação.
1. Na Barra de Navegação Global, vá para **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
