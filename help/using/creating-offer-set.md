---
title: Criar um conjunto de ofertas
description: Saiba como criar um conjunto de ofertas no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1159'
ht-degree: 0%

---

# Criar um conjunto de ofertas {#creating-an-offer-set}

Você pode criar qualquer um dos seguintes tipos de conjuntos de ofertas:

* Vídeo
* Modelo com parâmetros
* Imagem

Para modelos, selecione **[!UICONTROL Add and Preview]**, em seguida, defina os parâmetros escolhidos. Outros tipos de conjunto de ofertas não incluem parâmetros, mas você ainda pode personalizá-los selecionando **[!UICONTROL Preview]** e alterar as predefinições disponíveis.

O Adobe Dynamic Media Classic oferece ferramentas para edição e criação de conjuntos de ofertas.

>[!NOTE]
>
>Antes de criar um conjunto de ofertas, publique todos os ativos que pretende usar para o conjunto no Adobe Dynamic Media Classic. Consulte [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

## Tipos de conjuntos de ofertas {#types-of-offer-sets}

Crie um conjunto de ofertas a partir dos seguintes tipos de conjuntos de ofertas:

* **Imagens**: é possível montar imagens para um conjunto de ofertas. Cada imagem inclui uma oferta diferente no conjunto.

* **Modelo de imagem**: é possível parametrizar modelos de imagem no Adobe Dynamic Media Classic com o **[!UICONTROL Build]** > Noções básicas do modelo. Por meio de parâmetros, os componentes do modelo — o texto em quadros de texto, as diferentes imagens — podem ser trocados e personalizados. Para um conjunto de ofertas, você pode usar parâmetros de modelo para criar variações na mesma imagem no conjunto de ofertas, por exemplo. Para obter informações sobre como criar e parametrizar modelos de imagem, consulte [Criar parâmetros de modelo](creating-template-parameters.md#creating_template_parameters).

Consulte também [Noções básicas de modelo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) vídeo de treinamento.

* **Vídeo**: é possível montar vídeos para um conjunto de ofertas. Cada vídeo é uma oferta diferente no conjunto.

## Criar um conjunto de ofertas com um modelo com parâmetros {#creating-an-offer-set-with-a-parameterized-template}

Ao criar um Conjunto de ofertas, a variável **[!UICONTROL Publish after save]** opção afeta os membros set e set das seguintes maneiras:

| **[!UICONTROL Publish after save]** opção selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos mantêm seu estado publicado ou não publicado. |

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um conjunto de ofertas com um template parametrizado:**

1. Selecione o modelo ou banner.
1. Ir para **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

   A página Conjunto de ofertas Test&amp;Target lista as ofertas no conjunto de ofertas. O primeiro item da lista é o objeto.

1. Selecione o objeto e selecione **[!UICONTROL Add & Preview]**.

   O lado esquerdo da página lista os parâmetros no modelo e seus valores.

1. Altere os valores de parâmetro para criar a oferta. Por exemplo, digite um texto diferente em um campo de texto, altere o tamanho de uma camada, troque uma imagem por outra ou escolha outra Predefinição do visualizador.
1. Selecionar **[!UICONTROL Save]** ou **[!UICONTROL Save As**]** para salvar a oferta como parte do conjunto de ofertas.

   A página Conjunto de ofertas Test&amp;Target lista as ofertas que você criou.

1. Repita as etapas de 3 a 5 para criar mais ofertas para o conjunto.
1. Ao concluir, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save*]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Close]**, digite um nome para o conjunto de ofertas e selecione **[!UICONTROL Save]**.

Antes de fechar a página Conjunto de ofertas do Test&amp;Target, envie o conjunto de ofertas para o Adobe Target Standard/Premium. Consulte [Encaminhar conjuntos de ofertas para Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Criar um conjunto de ofertas com imagens ou vídeos {#creating-an-offer-set-with-images-or-videos}

Ao criar um Conjunto de ofertas, a variável **[!UICONTROL Publish after save]** opção afeta os membros set e set das seguintes maneiras:

| **[!UICONTROL Publish after save]** opção selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos mantêm seu estado publicado ou não publicado. |

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um conjunto de ofertas com imagens ou vídeos:**

1. Monte imagens ou vídeos para o conjunto de ofertas. Comece na tela Conjunto de ofertas Test&amp;Target ou na Exibição em grade ou em lista e use um dos seguintes métodos:

   * **Tela Conjunto de ofertas Test&amp;Target**: Vá para **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**. Arraste imagens ou vídeos para a tela. Para criar vídeos ou imagens de tamanhos variados, arraste várias cópias da imagem ou do vídeo e defina cada tamanho individualmente.

   * **Exibição em grade ou em lista**: selecione as imagens ou os vídeos e vá para **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

1. Como opção, selecione uma imagem ou vídeo e **[!UICONTROL Preview]**. Na página Visualizar ofertas, é possível alterar o tamanho e a aparência da imagem ou do vídeo selecionado. Ou você pode alterar todas as imagens ou vídeos no conjunto de ofertas.

   * Escolha uma predefinição para alterar a aparência e o tamanho da imagem ou do vídeo.
   * Para aplicar a predefinição escolhida a todas as ofertas do conjunto de ofertas, selecione a **[!UICONTROL Select Presets to All]** caixa de seleção

   Selecionar **[!UICONTROL Save]** para salvar as alterações na oferta de imagem ou vídeo. Em seguida, selecione **[!UICONTROL Close]** para retornar à página Conjunto de ofertas Test&amp;Target.

1. Depois de concluir a criação de ofertas para o conjunto de ofertas e escolher Predefinições de imagem para imagens diferentes, verifique se **[!UICONTROL Publish after save]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]** e insira um nome para o conjunto de ofertas e selecione **[!UICONTROL Save]**.

Antes de fechar a página Conjunto de ofertas do Test&amp;Target, envie o conjunto de ofertas para o Adobe Target Standard/Premium. Consulte [Encaminhar conjuntos de ofertas para Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Editar um conjunto de ofertas {#editing-an-offer-set}

Se você editar um conjunto publicado ou não, a variável **[!UICONTROL Publish after save]** opção afeta os membros set e set das seguintes maneiras:

| Conjunto já publicado? | **[!UICONTROL Publish after save]** opção selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- | --- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existentes mantêm seu estado publicado. Qualquer novo membro do conjunto adicionado durante sua edição manterá seu estado publicado ou não. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existentes e os novos membros do conjunto adicionados durante a edição mantêm seus estados publicado ou não. |

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um conjunto de ofertas:**

1. Para editar um conjunto de ofertas, exiba o conjunto de ofertas na Exibição de grade ou na Exibição de lista e selecione seu **[!UICONTROL Edit]** botão de rolagem.
1. Na página Conjunto de ofertas Test&amp;Target, siga um destes procedimentos:

   * **Remoção de uma oferta**: selecione a oferta e, em seguida, **[!UICONTROL Delete]** para remover uma oferta do conjunto.
   * **Adição de uma oferta**: como você adiciona uma oferta depende do tipo de conjunto de ofertas com o qual você está trabalhando:
      * **Modelos**: Selecionar **[!UICONTROL Add & Preview]**, e na página Adicionar e visualizar ofertas, crie outra oferta.
      * **Imagens e vídeos**: arraste uma imagem ou vídeo para a página Conjunto de ofertas Test&amp;Target.

   >[!NOTE]
   >
   >Não é possível excluir um conjunto de ofertas associado a uma campanha. Para excluir um conjunto de ofertas associado a uma campanha, faça logon no Adobe Target Standard/Premium e remova as associações de campanha primeiro. Mesmo depois de desassociar-se de uma campanha, o ativo só pode ser excluído do Adobe Dynamic Media Classic, o que exige um logon no Adobe Target Standard/Premium, e não do Adobe Target Standard/Premium.

1. Ao concluir a edição, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]**, selecione uma pasta de armazenamento, digite um nome para o conjunto e selecione **[!UICONTROL Save]**.

## Excluir um conjunto de ofertas {#delet-an-offer-set}

Quando você exclui um Conjunto de ofertas, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um conjunto de ofertas:**

1. Na Exibição em Grade, Exibição em Lista ou Exibição de Detalhes, selecione um conjunto de ofertas ou mais.
1. Na Barra de navegação global, acesse **[!UICONTROL File]** > **[!UICONTROL Delete]** > **Excluir**.

>[!MORELIKETHIS]
>
>* [Criação de parâmetros de modelo](creating-template-parameters.md#creating_template_parameters)
