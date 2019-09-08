---
title: Criação de um conjunto de ofertas
seo-title: Criação de um conjunto de ofertas
description: 'null'
seo-description: Saiba como criar um conjunto de ofertas.
uuid: 6 d 6 a 4 af 9-70 c 0-4 cfa -9 a 8 f -855 d 6 adfcc 8 f
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/target_ classic_ integration
discoiquuid: 59 b 6437 d-c 21 e -4929-9291-3032 dbb 34565
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Criação de um conjunto de ofertas{#creating-an-offer-set}

Você pode criar qualquer um dos seguintes tipos de conjuntos de ofertas:

* Vídeo
* Modelo paramétrico
* Imagem

Em modelos, clique **em Adicionar e visualizar** e defina os parâmetros escolhidos. Os outros tipos de conjunto de ofertas não incluem parâmetros, mas você ainda pode personalizá-los clicando **em Visualizar** e alterando as predefinições disponíveis.

O Dynamic Media Classic oferece ferramentas para edição e criação de conjuntos de ofertas.

>[!NOTE]
>
>Antes de criar um conjunto de ofertas, certifique-se de publicar todos os ativos que pretende usar para o conjunto de publicação do Scene 7. Consulte [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

## Tipos de conjuntos de ofertas {#types-of-offer-sets}

Crie um conjunto de ofertas com base nos seguintes tipos de conjuntos de ofertas:

**Imagens** É possível montar imagens para um conjunto de ofertas. Cada imagem inclui uma oferta diferente no conjunto.

**Modelo de imagem** Você pode exemplificar os modelos de imagem no Dynamic Media Classic com o comando Build &gt; Modelo básico. Por meio de parâmetros, componentes do modelo— o texto em quadros de texto, as diferentes imagens— podem ser trocados e personalizados. Para um conjunto de ofertas, você pode usar parâmetros de modelo para criar variações na mesma imagem em seu conjunto de ofertas, por exemplo. Para obter informações sobre criação e modelagem de modelos de imagens, consulte Criar parâmetros de modelo.

**Vídeo** Você pode montar vídeo para um conjunto de ofertas. Cada vídeo é uma oferta diferente no conjunto.

## Criação de uma oferta definida com um modelo paramétrico {#creating-an-offer-set-with-a-parameterized-template}

Quando você cria um Conjunto de ofertas, **a opção Publicar depois de salvar** afeta o conjunto e os membros definidos das seguintes maneiras:

| A opção «Publicar após salvar» selecionada antes de salvar? | Estado de conjunto após salvar | Estado dos membros definidos após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros podem reter seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar uma oferta definida com um modelo paramétrico**

1. Selecione o modelo ou o banner.
1. Clique **em Criar** &gt; **Conjunto de ofertas do Target Classic**.

   A página Conjunto de ofertas do Target Classic lista ofertas no conjunto de ofertas. O primeiro item na lista é o objeto.

1. Selecione o objeto e clique **em Adicionar e visualizar**.

   O lado esquerdo da página lista parâmetros no modelo e seus valores.

1. Altere os valores de parâmetro para criar a oferta. Por exemplo, insira um texto diferente em um campo de texto, altere o tamanho de uma camada, troque uma imagem para outro ou escolha uma predefinição diferente do visualizador.
1. Clique **em Salvar** ou **Salvar como** para salvar a oferta como parte do conjunto de ofertas.

   A página do Target Classic Offer Set lista as ofertas que você criou.

1. Repita as etapas de 3 a 5 para criar mais ofertas para o conjunto.
1. Ao terminar, próximo ao canto inferior direito da página, certifique-se de **que Publicar depois de salvar** esteja selecionado (padrão).
1. Clique **em Fechar**, insira um nome para o conjunto de ofertas e clique **em Salvar**.

Antes de fechar a página Conjunto de ofertas do Target Classic, envie a oferta definida para o Target Classic. Consulte [Mover conjuntos de ofertas para o Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Criação de uma oferta definida com imagens ou vídeos {#creating-an-offer-set-with-images-or-videos}

Quando você cria um Conjunto de ofertas, **a opção Publicar depois de salvar** afeta o conjunto e os membros definidos das seguintes maneiras:

| A opção «Publicar após salvar» selecionada antes de salvar? | Estado de conjunto após salvar | Estado dos membros definidos após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros podem reter seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Criação de uma oferta definida com imagens ou vídeos**

1. Montar imagens ou vídeos para o conjunto de ofertas. Comece na tela Conjunto de ofertas do Target Classic ou na Exibição de grade ou Exibição de lista e use um dos seguintes métodos:

   **Tela Conjunto de ofertas do Target Classic** Clique em Criar &gt; Conjunto de ofertas do Target Classic. Arraste imagens ou vídeos para a tela. Para criar tamanhos variados de vídeos ou imagens, arraste várias cópias da imagem ou vídeo e defina cada tamanho individualmente.

   **Exibição de grade ou Lista** Selecione as imagens ou vídeos e clique em Criar &gt; Conjunto de ofertas do Target Classic.

1. Opcionalmente, selecione uma imagem ou vídeo e clique **em Visualizar**. Na página Visualizar ofertas, é possível alterar o tamanho e a aparência da imagem ou do vídeo selecionado. Ou você pode alterar todas as imagens ou vídeos no conjunto de ofertas.

   * Escolha uma Predefinição para alterar a aparência e o tamanho da imagem ou do vídeo.
   * Clique na caixa de seleção Selecionar predefinições para todos para aplicar a predefinição escolhida a todas as ofertas no conjunto de ofertas.
   Clique **em Salvar** para salvar as alterações na oferta de imagem ou vídeo. Em seguida, clique **em Fechar** para retornar à página Conjunto de ofertas do Target Classic.

1. Depois de concluir a criação de ofertas para o conjunto de ofertas e escolher Predefinições de imagens para diferentes imagens, certifique-se de **que Publicar depois de salvar** esteja selecionado (padrão).
1. Clique **em Salvar** e insira um nome para o conjunto de ofertas e clique **em Salvar**.

Antes de fechar a página Conjunto de ofertas do Target Classic, envie a oferta definida para o Target Classic. Consulte [Mover conjuntos de ofertas para o Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Edição de um conjunto de ofertas {#editing-an-offer-set}

Se você editar um conjunto publicado ou um conjunto não publicado, **a opção Publicar depois de salvar** afeta o conjunto e os membros definidos das seguintes maneiras:

| Já foi publicado? | A opção «Publicar após salvar» selecionada antes de salvar sua edição? | Estado de conjunto após salvar | Estado dos membros definidos após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros definidos existentes mantêm seu estado publicado. Todos os novos membros definidos durante a edição mantêm seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros definidos e todos os novos membros definidos durante a edição mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um conjunto de ofertas**

1. Para editar um conjunto de ofertas, exiba o conjunto de ofertas definido na exibição de Grade ou em Lista e clique no **botão Editar** sobreposições.
1. Na página Conjunto de ofertas do Target Classic, execute um dos procedimentos a seguir:

   **Remover uma oferta**

   Selecione a oferta e clique **em Excluir** para remover uma oferta do conjunto.

   **Adição de uma oferta**

   A forma como você adiciona uma oferta depende do tipo de conjunto de ofertas que está trabalhando com:

   * Modelos: Clique **em Adicionar e visualizar** e, na página Adicionar e visualizar ofertas, crie outra oferta.
   * Imagens e vídeos: Arraste uma imagem ou vídeo para a página Conjunto de ofertas do Target Classic.
   ***Observação**: Não é possível excluir um conjunto de ofertas associado a uma campanha. Para excluir um conjunto de ofertas associado a uma campanha, faça logon no Target Classic e remova as associações de campanhas primeiro. Mesmo depois de desassociar de uma campanha, o ativo só pode ser excluído do Sistema de publicação Scene 7, exigindo um logon no Target Classic e não no Target Classic.*

1. Quando terminar de editar, próximo ao canto inferior direito da página, certifique-se de **que Publicar depois de salvar** esteja selecionado (padrão).
1. Clique **em Salvar**, selecione uma pasta de armazenamento, digite um nome para o conjunto e clique **em Salvar**.

## Excluindo um conjunto de ofertas {#deleting-an-offer-set}

Quando você exclui um Conjunto de ofertas, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou «filhos») dentro desse conjunto não serão afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um conjunto de ofertas**

1. Na Exibição de grade, Exibição de lista ou Exibição de detalhes, selecione um ou mais Conjuntos de ofertas.
1. Na barra de navegação global, clique **em Arquivo** &gt; **Excluir** &gt; **Excluir**.

>[!MORELIKETHIS]
>
>* [Criação de parâmetros de modelo](creating-template-parameters.md#creating_template_parameters)

