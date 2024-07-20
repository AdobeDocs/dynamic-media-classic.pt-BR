---
title: Criar um conjunto de ofertas
description: Saiba como criar um Conjunto de ofertas no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1159'
ht-degree: 0%

---

# Criar um conjunto de ofertas {#creating-an-offer-set}

Você pode criar qualquer um dos seguintes tipos de Conjuntos de ofertas:

* Vídeo
* Modelo com parâmetros
* Imagem

Para modelos, selecione **[!UICONTROL Add and Preview]** e defina os parâmetros escolhidos. Outros tipos de Conjunto de ofertas não incluem parâmetros, mas você ainda pode personalizá-los selecionando **[!UICONTROL Preview]** e alterando as predefinições disponíveis.

O Adobe Dynamic Media Classic oferece ferramentas para edição e criação de Conjuntos de ofertas.

>[!NOTE]
>
>Antes de criar um Conjunto de ofertas, publique todos os ativos que pretende usar para o conjunto no Adobe Dynamic Media Classic. Consulte [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

## Tipos de conjuntos de ofertas {#types-of-offer-sets}

Crie um Conjunto de ofertas a partir dos seguintes tipos de Conjuntos de ofertas:

* **Imagens**: é possível reunir imagens para um Conjunto de Ofertas. Cada imagem inclui uma oferta diferente no conjunto.

* **Modelo de imagem**: você pode parametrizar modelos de imagem no Adobe Dynamic Media Classic com o comando **[!UICONTROL Build]** > Noções básicas do modelo. Por meio de parâmetros, componentes do modelo, o texto em quadros de texto e as diferentes imagens podem ser trocados e personalizados. Para um Conjunto de ofertas, você pode usar parâmetros de modelo para criar variações na mesma imagem no Conjunto de ofertas, por exemplo. Para obter informações sobre como criar e parametrizar modelos de imagem, consulte [Criar parâmetros de modelo](creating-template-parameters.md#creating_template_parameters).

Veja também o vídeo de treinamento [Noções básicas do modelo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

* **Vídeo**: você pode reunir vídeo para um Conjunto de Ofertas. Cada vídeo é uma oferta diferente no conjunto.

## Criar um conjunto de ofertas com um modelo com parâmetros {#creating-an-offer-set-with-a-parameterized-template}

Ao criar um Conjunto de Ofertas, a opção **[!UICONTROL Publish after a save]** afeta o conjunto e os membros do conjunto das seguintes maneiras:

| **[!UICONTROL Publish after a save]** opção selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um Conjunto de Ofertas com um modelo parametrizado:**

1. Selecione o modelo ou banner.
1. Vá para **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

   A página Conjunto de ofertas Test&amp;Target lista as ofertas no Conjunto de ofertas. O primeiro item da lista é o objeto.

1. Selecione o objeto e selecione **[!UICONTROL Add & Preview]**.

   O lado esquerdo da página lista os parâmetros no modelo e seus valores.

1. Altere os valores de parâmetro para criar a oferta. Por exemplo, digite um texto diferente em um campo de texto, altere o tamanho de uma camada, troque uma imagem por outra ou escolha outra Predefinição do visualizador.
1. Selecione **[!UICONTROL Save]** ou **[!UICONTROL Save As**]** para salvar a oferta como parte do Conjunto de ofertas.

   A página Conjunto de ofertas Test&amp;Target lista as ofertas que você criou.

1. Repita as etapas de 3 a 5 para criar mais ofertas para o conjunto.
1. Quando terminar, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after a save*]** está selecionado (padrão).
1. Selecione **[!UICONTROL Close]**, insira um nome para o Conjunto de ofertas e selecione **[!UICONTROL Save]**.

Antes de fechar a página Conjunto de ofertas do Test&amp;Target, envie o Conjunto de ofertas para o Adobe Target Standard/Premium. Consulte [Enviar conjuntos de ofertas para Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Criar um conjunto de ofertas com imagens ou vídeos {#creating-an-offer-set-with-images-or-videos}

Ao criar um Conjunto de Ofertas, a opção **[!UICONTROL Publish after a save]** afeta o conjunto e os membros do conjunto das seguintes maneiras:

| **[!UICONTROL Publish after a save]** opção selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um Conjunto de Ofertas com imagens ou vídeos:**

1. Montar imagens ou vídeos para o Conjunto de ofertas. Comece na tela Conjunto de ofertas Test&amp;Target ou na Exibição em grade ou em lista e use um dos seguintes métodos:

   * **Tela do Conjunto de Ofertas Test&amp;Target**: Vá para **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**. Arraste imagens ou vídeos para a tela. Para criar vídeos ou imagens de tamanhos variados, arraste várias cópias da imagem ou do vídeo e defina cada tamanho individualmente.

   * **Exibição em Grade ou em Lista**: selecione as imagens ou os vídeos e vá para **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

1. Opcionalmente, selecione uma imagem ou vídeo e selecione **[!UICONTROL Preview]**. Na página Visualizar ofertas, é possível alterar o tamanho e a aparência da imagem ou do vídeo selecionado. Ou você pode alterar todas as imagens ou vídeos no Conjunto de ofertas.

   * Escolha uma predefinição para alterar a aparência e o tamanho da imagem ou do vídeo.
   * Para aplicar a predefinição escolhida a todas as ofertas do Conjunto de ofertas, marque a caixa de seleção **[!UICONTROL Select Presets to All]**.

   Selecione **[!UICONTROL Save]** para salvar suas alterações na oferta de imagem ou vídeo. Em seguida, selecione **[!UICONTROL Close]** para retornar à página Conjunto de ofertas do Test&amp;Target.

1. Depois de concluir a criação de ofertas para o Conjunto de ofertas e escolher Predefinições de imagens para imagens diferentes, verifique se **[!UICONTROL Publish after a save]** está selecionado (padrão).
1. Selecione **[!UICONTROL Save]**, insira um nome para o Conjunto de ofertas e selecione **[!UICONTROL Save]**.

Antes de fechar a página Conjunto de ofertas do Test&amp;Target, envie o Conjunto de ofertas para o Adobe Target Standard/Premium. Consulte [Enviar conjuntos de ofertas para Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Editar um conjunto de ofertas {#editing-an-offer-set}

Se você editar um conjunto publicado ou um conjunto não publicado, a opção **[!UICONTROL Publish after a save]** afetará o conjunto e os membros do conjunto das seguintes maneiras:

| Conjunto já publicado? | **[!UICONTROL Publish after a save]** opção selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- | --- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existentes mantêm seu estado publicado. Qualquer novo membro do conjunto adicionado durante sua edição manterá seu estado publicado ou não. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existentes e os novos membros do conjunto adicionados durante a edição mantêm seus estados publicado ou não. |

Consulte também [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um Conjunto de Ofertas:**

1. Para editar um Conjunto de ofertas, exiba o Conjunto de ofertas na Exibição de grade ou na Exibição de lista e selecione o botão de substituição **[!UICONTROL Edit]**.
1. Na página Conjunto de ofertas Test&amp;Target, siga um destes procedimentos:

   * **Removendo uma oferta**: selecione a oferta e, em seguida, selecione **[!UICONTROL Delete]** para remover uma oferta do conjunto.
   * **Adicionando uma oferta**: como você adiciona uma oferta depende do tipo de Conjunto de Ofertas com o qual você está trabalhando:
      * **Modelos**: selecione **[!UICONTROL Add & Preview]** e, na página Adicionar e Visualizar Ofertas, crie outra oferta.
      * **Imagens e vídeos**: arraste uma imagem ou vídeo para a página Conjunto de ofertas do Test&amp;Target.

   >[!NOTE]
   >
   >Não é possível excluir um Conjunto de ofertas associado a uma campanha. Para excluir um Conjunto de ofertas associado a uma campanha, faça logon no Adobe Target Standard/Premium e remova as associações de campanha primeiro. Mesmo depois de desassociar-se de uma campanha, o ativo só pode ser excluído do Adobe Dynamic Media Classic, o que exige um logon no Adobe Target Standard/Premium, e não do Adobe Target Standard/Premium.

1. Ao concluir a edição, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after a save]** está selecionado (padrão).
1. Selecione **[!UICONTROL Save]**, selecione uma pasta de armazenamento, insira um nome para o conjunto e selecione **[!UICONTROL Save]**.

## Excluir um conjunto de ofertas {#delet-an-offer-set}

Quando você exclui um Conjunto de ofertas, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Consulte também [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um Conjunto de Ofertas:**

1. Na Exibição em grade, Exibição em lista ou Exibição de detalhes, selecione um Conjunto de ofertas ou mais.
1. Na Barra de Navegação Global, vá para **[!UICONTROL File]** > **[!UICONTROL Delete]** > **Excluir**.

>[!MORELIKETHIS]
>
>* [Criando parâmetros de modelo](creating-template-parameters.md#creating_template_parameters)
