---
title: Criação de um conjunto de mídia mista
seo-title: Criação de um conjunto de mídia mista
description: nulo
seo-description: Saiba como criar um Conjunto de mídia mista.
uuid: a0c6e5fa-7a85-4376-b9a3-b72ae63d3d95
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0ff9e763-897c-4ba5-b606-a95d5e45f35e
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---


# Criação de um conjunto de mídia mista{#creating-a-mixed-media-set}

Crie um conjunto de mídia mista quando quiser combinar vários tipos de visualizadores em uma apresentação. Certifique-se de que seus arquivos, Conjuntos de imagens, Conjuntos de amostras e Conjuntos de rotação estejam prontos para publicação antes de adicioná-los ao Conjunto de mídia mista.

![Conjunto de mídia mista](/help/assets/mm_mixed_media_set.png)

## Criar um conjunto de mídia mista {#create-a-mixed-media-set}

Quando você cria um conjunto, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| opção &quot;Publicar após salvar&quot; selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos retêm seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um conjunto de mídia mista**

1. Clique em **Build** > **Conjuntos de mídia mista**.
1. Arraste os vídeos, os Conjuntos de imagens, os Conjuntos de rotação e as amostras da Biblioteca de ativos para a tela Conjunto de mídia mista.

   >[!NOTE]
   >
   >Os Conjuntos de mídia mista não suportam ativos com nomes de arquivo que contenham qualquer um dos seguintes caracteres: ( ) { }.

1. Execute um dos procedimentos a seguir:

   * Para adicionar uma trilha sonora, arraste um arquivo de áudio da Biblioteca de ativos para a caixa Trilha sonora. A trilha sonora é reproduzida enquanto as imagens são exibidas. Ele para quando o vídeo é reproduzido.
   * Para alterar a ordem dos conjuntos, arraste-os para novos locais na tela Mixed Media Set. A ordem dos conjuntos na tela determina a ordem da esquerda para a direita na qual os usuários veem os conjuntos no Visualizador de conjunto de mídia mista.
   * (Opcional) Para adicionar uma miniatura personalizada para representar um vídeo no Visualizador, arraste um arquivo de imagem da Biblioteca de ativos para a caixa de espaço reservado Miniaturas.

1. Perto do canto inferior direito da página, verifique se **Publicar após salvar** está selecionado (padrão).
1. Clique em **Salvar**, selecione uma pasta para armazenar seu Conjunto de Mídias Misto, digite um nome para o conjunto e clique em **Salvar**.

   Clique em **Pré-visualização** para ver a aparência do conjunto de imagens combinado em um visualizador de conjunto de imagens.

## Editar um conjunto de mídia mista {#edit-a-mixed-media-set}

Você pode editar um Conjunto de mídia mista. Se quiser editar um conjunto em um Conjunto de mídias mistas, abra-o separadamente, edite-o e salve-o. As edições são exibidas no conjunto Mídia mista.

Dependendo de você editar um conjunto publicado ou não publicado, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| Definir já publicado? | Opção &quot;Publicar após salvar&quot; selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado.Qualquer novo conjunto de membros adicionado durante a edição mantém seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto que você tiver adicionado durante a edição manterão seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um conjunto de mídia mista**

1. Clique no botão **Editar** da sobreposição do Conjunto de Mídias Misto.
1. Execute um dos procedimentos a seguir:

   * Para remover itens, selecione-os e clique em **Excluir**.
   * Para reorganizar itens, arraste-os para novos locais.

1. Quando terminar de editar o conjunto, próximo ao canto inferior direito da página, certifique-se de que **Publicar após salvar** esteja selecionado (padrão).
1. Clique em **Salvar** ou **Salvar como**.

## Excluindo um conjunto de mídia mista {#deleting-a-mixed-media-set}

Ao excluir um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um deles mantém seu estado publicado ou não publicado.

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um conjunto de mídia mista**

1. Na Visualização de grade, Visualização de Lista ou Detalhes, selecione um ou mais conjuntos de mídia mista.
1. Na barra de navegação global, clique em **Arquivo** > **Excluir** > **Excluir**.

