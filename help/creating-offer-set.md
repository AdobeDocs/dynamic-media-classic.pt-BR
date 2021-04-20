---
title: Criação de um conjunto de ofertas
description: Saiba como criar um conjunto de ofertas.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1213'
ht-degree: 0%

---


# Criação de um conjunto de ofertas{#creating-an-offer-set}

Você pode criar qualquer um dos seguintes tipos de conjuntos de ofertas:

* Vídeo
* Modelo parametrizado
* Imagem

Para modelos, clique em **Adicionar e Visualizar** e defina os parâmetros escolhidos. Os outros tipos de conjunto de ofertas não incluem parâmetros, mas você ainda pode personalizá-los clicando em **Preview** e alterando as predefinições disponíveis.

O Dynamic Media Classic oferece ferramentas para edição e criação de conjuntos de ofertas.

>[!NOTE]
>
>Antes de criar um conjunto de ofertas, publique todos os ativos que pretende usar para o conjunto do Dynamic Media Classic. Consulte [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

## Tipos de conjuntos de ofertas {#types-of-offer-sets}

Crie um conjunto de ofertas a partir dos seguintes tipos de conjuntos de ofertas:

* ****
ImagensVocê pode reunir imagens para um conjunto de ofertas. Cada imagem inclui uma oferta diferente no conjunto.

* ****
Modelo de imagemVocê pode parametrizar modelos de imagem no Dynamic Media Classic com o comando Criar > Noções básicas do modelo. Por meio de parâmetros, componentes do modelo — o texto em quadros de texto, as diferentes imagens — podem ser trocados e personalizados. Para um conjunto de ofertas, você pode usar parâmetros de modelo para criar variações na mesma imagem em seu conjunto de ofertas, por exemplo. Para obter informações sobre como criar e parametrizar modelos de imagem, consulte Criação de parâmetros de modelo.

* ****
VídeoVocê pode montar vídeo para um conjunto de ofertas. Cada vídeo é uma oferta diferente no conjunto.

## Criação de um conjunto de ofertas com um modelo parametrizado {#creating-an-offer-set-with-a-parameterized-template}

Quando você cria um Conjunto de Ofertas, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| Opção &quot;Publicar após salvar&quot; selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros do conjunto mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um conjunto de ofertas com um modelo parametrizado**

1. Selecione o modelo ou banner.
1. Clique em **Criar** > **Conjunto de Ofertas do Test&amp;Target**.

   A página Conjunto de ofertas do Test&amp;Target lista as ofertas no conjunto de ofertas. O primeiro item na lista é o objeto .

1. Selecione o objeto e clique em **Adicionar e Visualizar**.

   O lado esquerdo da página lista os parâmetros no modelo e seus valores.

1. Altere os valores do parâmetro para criar a oferta. Por exemplo, insira texto diferente em um campo de texto, altere o tamanho de uma camada, troque uma imagem por outra ou escolha uma predefinição do visualizador diferente.
1. Clique em **Salvar** ou **Salvar como** para salvar a oferta como parte do conjunto de ofertas.

   A página Conjunto de ofertas do Test&amp;Target lista as ofertas que você criou.

1. Repita as etapas de 3 a 5 para criar mais ofertas para o conjunto.
1. Quando terminar, próximo ao canto inferior direito da página, verifique se **Publish after save** está selecionado (padrão).
1. Clique em **Fechar**, insira um nome para o conjunto de ofertas e clique em **Salvar**.

Antes de fechar a página Conjunto de ofertas do Test&amp;Target, envie a oferta para Target Standard/Premium. Consulte [Envio de conjuntos de ofertas para o Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Criação de um conjunto de ofertas com imagens ou vídeos {#creating-an-offer-set-with-images-or-videos}

Quando você cria um Conjunto de Ofertas, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| Opção &quot;Publicar após salvar&quot; selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros do conjunto mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um conjunto de ofertas com imagens ou vídeos**

1. Monte imagens ou vídeos para o conjunto de ofertas. Comece na tela Conjunto de Ofertas do Test&amp;Target ou na Exibição de Grade ou em Lista e use um dos seguintes métodos:

   * **Tela Conjunto de ofertas do Test&amp;TargetClique em**   **[!UICONTROL Build > Test&Target Offer Set]**. Arraste imagens ou vídeos para a tela. Para criar vários tamanhos de vídeos ou imagens, arraste várias cópias da imagem ou do vídeo e defina cada tamanho individualmente.

   * **Exibição em grade ou em listaSelecione as imagens ou os vídeos e clique em**   **[!UICONTROL Build > Test&Target Offer Set]**.

1. Como opção, selecione uma imagem ou vídeo e clique em **Visualizar**. Na página Visualizar ofertas , é possível alterar o tamanho e a aparência da imagem ou do vídeo selecionado. Ou você pode alterar todas as imagens ou vídeos no conjunto de ofertas.

   * Escolha uma predefinição para alterar a aparência e o tamanho da imagem ou do vídeo.
   * Clique na caixa de seleção Selecionar predefinições para tudo para aplicar a predefinição que você escolheu a todas as ofertas do conjunto de ofertas.

   Clique em **Save** para salvar as alterações na oferta de imagem ou vídeo. Em seguida, clique em **Fechar** para retornar à página Conjunto de Ofertas do Test&amp;Target.

1. Depois de concluir a criação de ofertas para o conjunto de ofertas e escolher Predefinições de imagem para imagens diferentes, verifique se **Publicar após salvar** está selecionado (padrão).
1. Clique em **Save**, insira um nome para o conjunto de ofertas e clique em **Save**.

Antes de fechar a página Conjunto de ofertas do Test&amp;Target, envie a oferta para Target Standard/Premium. Consulte [Envio de conjuntos de ofertas para o Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Editar um conjunto de ofertas {#editing-an-offer-set}

Dependendo de você editar um conjunto publicado ou não, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| Definir já publicado? | Opção &quot;Publicar após salvar&quot; selecionada antes de salvar a edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado.Qualquer novo conjunto de membros adicionado durante a edição mantém seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto adicionados durante a edição mantêm o estado publicado ou não. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um conjunto de ofertas**

1. Para editar um conjunto de ofertas, exiba o conjunto de ofertas na Exibição de grade ou na Exibição de lista e clique em seu botão **Editar** de sobreposição.
1. Na página Conjunto de ofertas do Test&amp;Target, execute um dos seguintes procedimentos:

   * **Remoção de uma**
ofertaSelecione a oferta e clique em 
**** Excluir para remover uma oferta do conjunto.
   * **Adicionar uma**
ofertaA forma como você adiciona uma oferta depende do tipo de conjunto de ofertas com o qual você está trabalhando:
   * ****
ModelosClique 
**Adicionar e visualizar** e, na página Adicionar e visualizar ofertas , crie outra oferta.
   * **Imagens e**
vídeosArraste uma imagem ou vídeo até a página Conjunto de ofertas do Test&amp;Target.
   >[!NOTE]
   >
   >Não é possível excluir um conjunto de ofertas associado a uma campanha. Para excluir um conjunto de ofertas associado a uma campanha, faça logon no Target Standard/Premium e remova as associações de campanha primeiro. Mesmo depois de cancelar a associação de uma campanha, o ativo só pode ser excluído do Dynamic Media Classic, exigindo um logon no Target Standard/Premium, e não do Target Standard/Premium.

1. Ao terminar a edição, próximo ao canto inferior direito da página, verifique se **Publish after save** está selecionado (padrão).
1. Clique em **Salvar**, selecione uma pasta de armazenamento, insira um nome para o conjunto e clique em **Salvar**.

## Excluindo um conjunto de ofertas {#deleting-an-offer-set}

Ao excluir um Conjunto de ofertas, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) desse conjunto não são afetados; em vez disso, cada um mantém seu estado publicado ou não publicado.

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um conjunto de ofertas**

1. Na Exibição de Grade, Exibição de Lista ou Exibição de Detalhes, selecione um ou mais Conjuntos de Ofertas.
1. Na Barra de Navegação Global, clique em **Arquivo** > **Excluir** > **Excluir**.

>[!MORELIKETHIS]
>
>* [Criação de parâmetros de modelo](creating-template-parameters.md#creating_template_parameters)

