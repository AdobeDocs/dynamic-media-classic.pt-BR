---
title: Criação de um conjunto de ofertas
seo-title: Criação de um conjunto de ofertas
description: nulo
seo-description: Saiba como criar um conjunto de ofertas.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: referência
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/category/target_classic_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Criação de um conjunto de ofertas{#creating-an-offer-set}

Você pode criar qualquer um dos seguintes tipos de conjuntos de ofertas:

*  Vídeo
* Modelo parametrizado
* Imagem

Para modelos, clique em **Adicionar e Visualizar** e defina os parâmetros escolhidos. Os outros tipos de conjunto de ofertas não incluem parâmetros, mas você ainda pode personalizá-los clicando em **Visualizar** e alterando as predefinições disponíveis.

O Dynamic Media Classic oferece ferramentas para edição e criação de conjuntos de ofertas.

>[!NOTE]
>
>Antes de criar um conjunto de ofertas, certifique-se de publicar todos os ativos que pretende usar para o conjunto definido como Scene7 Publishing System. Consulte Publicação [manual de ativos](publishing-files.md#manually_publishing_assets) e cancelamento [manual de publicação de ativos](publishing-files.md#manually_unpublishing_assets).

## Tipos de conjuntos de ofertas {#types-of-offer-sets}

Crie um conjunto de ofertas dos seguintes tipos de conjuntos de ofertas:

* **Imagens** Você pode reunir imagens para um conjunto de ofertas. Cada imagem inclui uma oferta diferente no conjunto.

* **Modelo** de imagem Você pode parametrizar modelos de imagem no Dynamic Media Classic com o comando Criar &gt; Fundamentos do modelo. Através de parâmetros, componentes do modelo — o texto em quadros de texto, as diferentes imagens... pode ser trocado e personalizado. Para um conjunto de ofertas, você pode usar parâmetros de modelo para criar variações na mesma imagem no conjunto de ofertas, por exemplo. Para obter informações sobre como criar e parametrizar modelos de imagem, consulte Criar parâmetros de modelo.

* **Vídeo** Você pode montar vídeo para um conjunto de ofertas. Cada vídeo é uma oferta diferente no conjunto.

## Criação de um conjunto de ofertas com um modelo parametrizado {#creating-an-offer-set-with-a-parameterized-template}

Quando você cria um Conjunto de ofertas, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| opção "Publicar após salvar" selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos retêm seu estado publicado ou não publicado. |

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually_publishing_assets) a publicação de ativos [](publishing-files.md#manually_unpublishing_assets)manualmente.

**Para criar um conjunto de ofertas com um modelo parametrizado**

1. Selecione o modelo ou banner.
1. Clique em **Criar** &gt; Conjunto de ofertas **do** Target Classic.

   A página Conjunto de ofertas do Target Classic lista as ofertas no conjunto de ofertas. O primeiro item na lista é o objeto.

1. Selecione o objeto e clique em **Adicionar e visualizar**.

   O lado esquerdo da página lista os parâmetros no modelo e seus valores.

1. Altere os valores de parâmetro para criar a oferta. Por exemplo, insira um texto diferente em um campo de texto, altere o tamanho de uma camada, troque uma imagem por outra ou escolha uma predefinição de visualizador diferente.
1. Clique em **Salvar** ou **Salvar como** para salvar a oferta como parte do conjunto de ofertas.

   A página Conjunto de ofertas clássicas do Target lista as ofertas que você criou.

1. Repita as etapas de 3 a 5 para criar mais ofertas para o conjunto.
1. Quando terminar, próximo ao canto inferior direito da página, verifique se a opção **Publicar após salvar** está selecionada (padrão).
1. Clique em **Fechar**, insira um nome para o conjunto de ofertas e clique em **Salvar**.

Antes de fechar a página Conjunto de ofertas do Target Classic, envie a oferta para o Target Classic. Consulte [Envio de conjuntos de ofertas para o Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Criar um conjunto de ofertas com imagens ou vídeos {#creating-an-offer-set-with-images-or-videos}

Quando você cria um Conjunto de ofertas, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| opção "Publicar após salvar" selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos retêm seu estado publicado ou não publicado. |

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually_publishing_assets) a publicação de ativos [](publishing-files.md#manually_unpublishing_assets)manualmente.

**Para criar um conjunto de ofertas com imagens ou vídeos**

1. Montar imagens ou vídeos para o conjunto de ofertas. Comece na tela Conjunto de ofertas do Target Classic ou na Exibição de grade ou Exibição de lista e use um dos seguintes métodos:

   * **Tela** Conjunto de ofertas do Target Classic Clique em Criar &gt; Conjunto de ofertas do Target Classic. Arraste imagens ou vídeos para a tela. Para criar tamanhos variados de vídeos ou imagens, arraste várias cópias da imagem ou do vídeo e defina cada tamanho individualmente.

   * **Exibição** de grade ou listaSelecione as imagens ou vídeos e clique em Criar &gt; Conjunto de ofertas clássicas do Target.

1. Como opção, selecione uma imagem ou vídeo e clique em **Visualizar**. Na página Visualizar ofertas, é possível alterar o tamanho e a aparência da imagem ou do vídeo selecionado. Ou você pode alterar todas as imagens ou vídeos no conjunto de ofertas.

   * Escolha uma predefinição para alterar a aparência e o tamanho da imagem ou do vídeo.
   * Clique na caixa de seleção Selecionar predefinições para tudo para aplicar a predefinição que você escolheu a todas as ofertas no conjunto de ofertas.
   Clique em **Salvar** para salvar as alterações na oferta de imagem ou vídeo. Em seguida, clique em **Fechar** para retornar à página Conjunto de ofertas do Target Classic.

1. Depois de concluir a criação de ofertas para o conjunto de ofertas e escolher Predefinições de imagens para diferentes imagens, verifique se a opção **Publicar após salvar** está selecionada (padrão).
1. Clique em **Salvar** e insira um nome para o conjunto de ofertas e clique em **Salvar**.

Antes de fechar a página Conjunto de ofertas do Target Classic, envie a oferta para o Target Classic. Consulte [Envio de conjuntos de ofertas para o Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Editar um conjunto de ofertas {#editing-an-offer-set}

Dependendo de se você editar um conjunto publicado ou não publicado, a opção **Publicar após salvar** afetará o conjunto e definirá os membros das seguintes maneiras:

| Definir já publicado? | Opção "Publicar após salvar" selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado.Qualquer novo conjunto de membros adicionado durante a edição mantém seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto que você tiver adicionado durante a edição manterão seu estado publicado ou não publicado. |

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually_publishing_assets) a publicação de ativos [](publishing-files.md#manually_unpublishing_assets)manualmente.

**Para editar um conjunto de ofertas**

1. Para editar um conjunto de ofertas, exiba o conjunto de ofertas na Exibição de grade ou na Exibição de lista e clique no botão **Editar** sobreposição.
1. Na página Conjunto de ofertas do Target Classic, execute um dos procedimentos a seguir:

   * **Remoção de uma oferta** Selecione a oferta e clique em **Excluir** para remover uma oferta do conjunto.
   * **Adicionando uma oferta** Como você adiciona uma oferta depende do tipo de conjunto de ofertas com o qual você está trabalhando:
   * **Modelos** Clique em **Adicionar e visualizar** e, na página Adicionar e visualizar ofertas, crie outra oferta.
   * **Imagens e vídeos** Arraste uma imagem ou vídeo até a página Conjunto de ofertas do Target Classic.
   >[!NOTE]
   >
   >Não é possível excluir um conjunto de ofertas associado a uma campanha. Para excluir um conjunto de ofertas associado a uma campanha, faça logon no Target Classic e remova as associações de campanha primeiro. Mesmo depois de cancelar a associação de uma campanha, o ativo só pode ser excluído do Scene7 Publishing System, exigindo um logon no Target Classic, e não do Target Classic.

1. Ao terminar a edição, próximo ao canto inferior direito da página, certifique-se de que a opção **Publicar após salvar** esteja selecionada (padrão).
1. Clique em **Salvar**, selecione uma pasta de armazenamento, digite um nome para o conjunto e clique em **Salvar**.

## Excluindo um Conjunto de Ofertas {#deleting-an-offer-set}

Quando você exclui um Conjunto de ofertas, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou "filhos") dentro desse conjunto não são afetados; em vez disso, cada um deles mantém seu estado publicado ou não publicado.

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually_publishing_assets) a publicação de ativos [](publishing-files.md#manually_unpublishing_assets)manualmente.

**Para excluir um conjunto de ofertas**

1. Na Exibição de grade, Exibição de lista ou Exibição de detalhes, selecione um ou mais Conjuntos de ofertas.
1. Na barra de navegação global, clique em **Arquivo** &gt; **Excluir** &gt; **Excluir**.

>[!MORELIKETHIS]
>
>* [Criação de parâmetros de modelo](creating-template-parameters.md#creating_template_parameters)

