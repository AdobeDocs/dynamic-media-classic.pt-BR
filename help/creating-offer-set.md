---
title: Criação de um conjunto de ofertas
description: Saiba como criar um conjunto de ofertas.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---


# Criação de um conjunto de ofertas{#creating-an-offer-set}

Você pode criar qualquer um dos seguintes tipos de conjuntos de ofertas:

* Vídeo
* Modelo parametrizado
* Imagem

Para modelos, clique em **Adicionar e Pré-visualização** e defina os parâmetros escolhidos. Os outros tipos de conjunto de ofertas não incluem parâmetros, mas você ainda pode personalizá-los clicando em **Pré-visualização** e alterando as predefinições disponíveis.

Ferramentas do Dynamic Media Classic oferta para edição e criação de conjuntos de ofertas.

>[!NOTE]
>
>Antes de criar um conjunto de ofertas, certifique-se de publicar todos os ativos que pretende usar para o conjunto no Dynamic Media Classic. Consulte [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

## Tipos de conjuntos de ofertas {#types-of-offer-sets}

Crie um conjunto de ofertas dos seguintes tipos de conjuntos de ofertas:

* ****
ImagensVocê pode reunir imagens para um conjunto de ofertas. Cada imagem inclui uma oferta diferente no conjunto.

* **Modelo**
de imagemÉ possível parametrizar modelos de imagem no Dynamic Media Classic com o comando Criar > Noções básicas do modelo. Através de parâmetros, componentes do modelo — o texto em quadros de texto, as diferentes imagens... pode ser trocado e personalizado. Para um conjunto de ofertas, você pode usar parâmetros de modelo para criar variações na mesma imagem no conjunto de ofertas, por exemplo. Para obter informações sobre como criar e parametrizar modelos de imagem, consulte Criar parâmetros de modelo.

* ****
VídeoVocê pode montar vídeo para um conjunto de ofertas. Cada vídeo é uma oferta diferente no conjunto.

## Criação de um conjunto de ofertas com um modelo parametrizado {#creating-an-offer-set-with-a-parameterized-template}

Quando você cria um Conjunto de Ofertas, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| opção &quot;Publicar após salvar&quot; selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos retêm seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um conjunto de ofertas com um modelo parametrizado**

1. Selecione o modelo ou banner.
1. Clique em **Build** > **Conjunto de Ofertas do Test&amp;Público alvo**.

   A página Conjunto de Ofertas do Test&amp;Público alvo lista no conjunto de ofertas. O primeiro item na lista é o objeto.

1. Selecione o objeto e clique em **Adicionar e Pré-visualização**.

   O lado esquerdo da página lista parâmetros no modelo e seus valores.

1. Altere os valores de parâmetro para criar a oferta. Por exemplo, insira um texto diferente em um campo de texto, altere o tamanho de uma camada, troque uma imagem por outra ou escolha uma predefinição de visualizador diferente.
1. Clique em **Salvar** ou **Salvar como** para salvar a oferta como parte do conjunto de ofertas.

   A página Conjunto de Ofertas do Test&amp;Público alvo lista as ofertas que você criou.

1. Repita as etapas de 3 a 5 para criar mais ofertas para o conjunto.
1. Quando terminar, próximo ao canto inferior direito da página, certifique-se de que **Publicar após salvar** esteja selecionado (padrão).
1. Clique em **Fechar**, insira um nome para o conjunto de ofertas e clique em **Salvar**.

Antes de fechar a página Conjunto de Ofertas do Test&amp;Público alvo, envie a oferta para o Target Standard/Premium. Consulte [Encaminhando conjuntos de ofertas para Test&amp;Público alvo](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Criação de um conjunto de ofertas com imagens ou vídeos {#creating-an-offer-set-with-images-or-videos}

Quando você cria um Conjunto de Ofertas, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| opção &quot;Publicar após salvar&quot; selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos retêm seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um conjunto de ofertas com imagens ou vídeos**

1. Montar imagens ou vídeos para o conjunto de ofertas. Start na tela Conjunto de Ofertas do Test&amp;Público alvo ou na Visualização da Grade ou na Visualização da Lista e use um dos seguintes métodos:

   * **TelaClick do conjunto de Ofertas do Test&amp;Público alvo**   **[!UICONTROL Build > Test&Target Offer Set]**. Arraste imagens ou vídeos para a tela. Para criar tamanhos variados de vídeos ou imagens, arraste várias cópias da imagem ou do vídeo e defina cada tamanho individualmente.

   * **Grade ou** exibição de ListaSelecione as imagens ou os vídeos e clique em  **[!UICONTROL Build > Test&Target Offer Set]**.

1. Como opção, selecione uma imagem ou vídeo e clique em **Pré-visualização**. Na página Ofertas de Pré-visualização, é possível alterar o tamanho e a aparência da imagem ou do vídeo selecionado. Ou você pode alterar todas as imagens ou vídeos no conjunto de ofertas.

   * Escolha uma predefinição para alterar a aparência e o tamanho da imagem ou do vídeo.
   * Clique na caixa de seleção Selecionar predefinições para tudo para aplicar a predefinição que você escolheu a todas as ofertas do conjunto de ofertas.

   Clique em **Salvar** para salvar suas alterações na imagem ou oferta de vídeo. Em seguida, clique em **Fechar** para retornar à página Conjunto de Ofertas do Test&amp;Público alvo.

1. Depois de terminar de criar ofertas para o conjunto de ofertas e escolher Predefinições de imagem para imagens diferentes, certifique-se de que **Publicar após salvar** esteja selecionado (padrão).
1. Clique em **Salvar** e insira um nome para o conjunto de ofertas e clique em **Salvar**.

Antes de fechar a página Conjunto de Ofertas do Test&amp;Público alvo, envie a oferta para o Target Standard/Premium. Consulte [Encaminhando conjuntos de ofertas para Test&amp;Público alvo](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Edição de um conjunto de Ofertas {#editing-an-offer-set}

Dependendo de você editar um conjunto publicado ou não publicado, a opção **Publicar após salvar** afetará o conjunto e definirá os membros das seguintes maneiras:

| Definir já publicado? | Opção &quot;Publicar após salvar&quot; selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado.Qualquer novo conjunto de membros adicionado durante a edição mantém seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto que você tiver adicionado durante a edição manterão seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um Conjunto de Ofertas**

1. Para editar um conjunto de ofertas, exiba o conjunto de ofertas em visualização de Grade ou visualização de Lista e clique em seu botão de sobreposição **Editar**.
1. Na página Conjunto de Ofertas do Test&amp;Público alvo, execute um dos procedimentos a seguir:

   * **Remoção de uma**
ofertaSelecione a oferta e clique em 
**Exclua** para remover uma oferta do conjunto.
   * **Adicionar uma**
ofertaA forma como você adiciona uma oferta depende do tipo de conjunto de ofertas com o qual você está trabalhando:
   * ****
ModelosClique 
**Adicionar e Pré-visualização** e, na página Adicionar e Pré-visualização Ofertas, crie outra oferta.
   * **Imagens e**
vídeosArraste uma imagem ou vídeo até a página Conjunto de Ofertas do Test&amp;Público alvo.
   >[!NOTE]
   >
   >Não é possível excluir um conjunto de ofertas associado a uma campanha. Para excluir um conjunto de ofertas associado a uma campanha, faça logon no Target Standard/Premium e remova as associações de campanhas primeiro. Mesmo depois de cancelar a associação de uma campanha, o ativo só pode ser excluído do Dyanmic Media Classic, exigindo um logon no Target Standard/Premium, e não no Target Standard/Premium.

1. Quando terminar a edição, próximo ao canto inferior direito da página, certifique-se de que **Publicar após salvar** esteja selecionado (padrão).
1. Clique em **Salvar**, selecione uma pasta de armazenamento, digite um nome para o conjunto e clique em **Salvar**.

## Excluindo um Conjunto de Ofertas {#deleting-an-offer-set}

Quando você exclui um Conjunto de Ofertas, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um deles mantém seu estado publicado ou não publicado.

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um Conjunto de Ofertas**

1. Na Visualização de grade, Visualização de Lista ou Detalhes, selecione um ou mais conjuntos de Ofertas.
1. Na barra de navegação global, clique em **Arquivo** > **Excluir** > **Excluir**.

>[!MORELIKETHIS]
>
>* [Criação de parâmetros de modelo](creating-template-parameters.md#creating_template_parameters)

