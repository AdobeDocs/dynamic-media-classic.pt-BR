---
title: Criar um conjunto de rotação
description: Saiba como criar um Conjunto de rotação no Adobe Dynamic Media Classic.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
source-git-commit: ac9cba2c33fb1df65e64746dea2557632b7b2903
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# Criar um conjunto de rotação{#creating-a-spin-set}

Para criar um Conjunto de rotação eficaz, certifique-se de fotografar as imagens corretamente. Você pode criar um Conjunto de rotação no Adobe Dynamic Media Classic selecionando o botão Criar e escolhendo Conjuntos de rotação. Edite Conjuntos de rotação na tela Conjuntos de rotação .

>[!NOTE]
>
>As versões anteriores do Adobe Dynamic Media Classic não ofereciam Conjuntos de rotação bidimensionais. Se você criou um Conjunto de rotação em uma versão anterior do Adobe Dynamic Media Classic, não poderá salvar seu Conjunto de rotação unidimensional sem primeiro salvá-lo com um nome diferente. Selecionar **[!UICONTROL Save As]** na tela Conjunto de rotação e insira um novo nome para que você possa editá-lo no Adobe Dynamic Media Classic.

## Diretrizes para fotografar imagens do Conjunto de rotação {#guidelines-for-shooting-spin-set-images}

Em geral, quanto mais imagens você tiver em um Conjunto de rotação, melhor será o efeito giratório da imagem. No entanto, incluir muitas imagens no conjunto também aumenta a quantidade de tempo que as imagens levam para serem carregadas. A Adobe Dynamic Media Classic recomenda estas diretrizes para fotografar imagens para uso em Conjuntos de rotação:

* No mínimo, use 8 a 12 imagens em um conjunto de rotação unidimensional e 16 a 24 imagens em um conjunto de rotação bidimensional.
* Usar um formato sem perdas; TIFF e PNG são recomendadas.
* Mascarar todas as imagens para que o item apareça em um plano de fundo branco ou de alto contraste. Como opção, adicione sombras.
* Verifique se os detalhes do produto estão bem iluminados e em foco.
* Use imagens de rotação para roupas de moda com um manequim ou modelo. Frequentemente, o manequim é mascarado (utilizando um manequim de vidro) ou na imagem aparece um manequim/moldura estilizada. Você pode criar um conjunto de rotação no modelo definindo o número de ângulos. Marque cada ângulo com uma fita no chão para que você possa guiar o modelo para pisar e olhar na direção de cada tomada.

## Criar um conjunto de rotação {#create}

A ordem em que o Conjunto de rotação é criado ou criado no Adobe Dynamic Media Classic é importante. Dependendo de como você ordena os ativos quando você arrasta e solta imagens na grade na página Conjunto de rotação , o Conjunto de rotação gira em uma determinada direção . Portanto, a ordem em que é exibido visualmente no construtor é como o ativo é executado quando um usuário move o ponteiro do mouse ou move o dedo, da esquerda para a direita.

Ao criar um conjunto, a variável **[!UICONTROL Publish after save]** afeta o conjunto e o conjunto de membros das seguintes maneiras:

| **[!UICONTROL Publish after save]** opção selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
| --- | --- | --- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros do conjunto mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar ativos manualmente](publishing-files.md#manually-publishing-assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually-unpublishing-assets).

>[!NOTE]
>
>Ao criar um Conjunto de rotação, o Adobe recomenda a diretriz de práticas recomendadas e o limite imposto a seguir.
>
>* Número máximo de linhas/colunas por Conjunto de rotação 2D
   > 
   >   * Prática recomendada: 1000
   >   * Limite imposto: 1000


Depois de salvar um Conjunto de rotação, você pode usar Visualização na compilação: Página Conjunto de rotação para ver a aparência do seu Conjunto de rotação no visualizador padrão.

**Para criar um Conjunto de rotação:**

1. No **[!UICONTROL Build]** , selecione **[!UICONTROL Spin Sets]**.
1. Na caixa de diálogo Tamanho do conjunto de rotação, defina o número de linhas e células desejado.

   Para criar um conjunto de rotação unidimensional, selecione apenas uma linha.

   Para criar um Conjunto de rotação bidimensional, selecione duas ou mais linhas.

1. Selecionar **[!UICONTROL OK]**.
1. Arraste e solte imagens na grade na tela Conjunto de rotação .
1. Quando terminar, próximo ao canto inferior direito da página, verifique se **Publicar após salvar** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]**.
1. Na caixa de diálogo Salvar , selecione uma pasta para armazenar o conjunto de rotação. No campo Nome do arquivo , insira o nome do conjunto de rotação.
1. Selecionar **[!UICONTROL Save]**.

## Editar um conjunto de rotação {#editing-a-spin-set}

Se você editar um conjunto publicado ou não, a variável **[!UICONTROL Publish after save]** afeta o conjunto e o conjunto de membros das seguintes maneiras:

| Definir já publicado? | **[!UICONTROL Publish after save]** opção selecionada antes de salvar a edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
| --- | --- | --- | --- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado. Qualquer novo conjunto de membros adicionado durante a edição manterá o estado publicado ou não. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto adicionados durante a edição mantêm o estado publicado ou não. |

Consulte também [Publicar ativos manualmente](publishing-files.md#manually-publishing-assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually-unpublishing-assets).

**Para editar um Conjunto de rotação:**

1. Selecione a sobreposição do Conjunto de rotação **[!UICONTROL Edit]** botão.
1. Siga um destes procedimentos:

   * **Remoção de imagens** - Selecione a imagem e selecione **[!UICONTROL Delete]**.

   * **Adição de imagens** - Arraste a imagem para uma célula.

   * **Reorganizando linhas (conjuntos de rotação bidimensionais)** - Selecione uma caixa de seletor de linha (à esquerda da linha) e selecione **[!UICONTROL Move Row Down]** ou **[!UICONTROL Move Row Up]**.

   * **Adição de linhas e células** - Digite um número na caixa Linhas e na caixa Células para determinar o número de linhas e o número de células em cada linha.

1. Quando a edição for concluída, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]**, selecione uma pasta de armazenamento, insira um nome para o conjunto e selecione **[!UICONTROL Save]**.

## Excluir um conjunto de rotação {#deleting-a-spin-set}

Ao excluir um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) desse conjunto não são afetados; em vez disso, cada um mantém seu estado publicado ou não publicado.

Consulte também [Publicar ativos manualmente](publishing-files.md#manually-publishing-assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually-unpublishing-assets).

**Para excluir um Conjunto de rotação:**

1. Na Exibição de Grade, Exibição de Lista ou Exibição de Detalhes, selecione um ou mais Conjuntos de rotação.
1. Na Barra de navegação global, acesse **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
