---
title: Criação de um conjunto de mídia mista
description: Saiba como criar um Conjunto de mídias mistas.
uuid: a0c6e5fa-7a85-4376-b9a3-b72ae63d3d95
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0ff9e763-897c-4ba5-b606-a95d5e45f35e
feature: Dynamic Media Classic,Visualizadores,Conjuntos de mídias mistas
role: Profissional
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---


# Criação de um conjunto de mídia mista{#creating-a-mixed-media-set}

Crie um Conjunto de mídias mistas quando quiser combinar vários tipos de visualizadores em uma apresentação. Certifique-se de que os arquivos, os Conjuntos de imagens, os Conjuntos de amostras e os Conjuntos de rotação estejam prontos para publicação antes de adicioná-los ao Conjunto de mídias mistas.

![Conjunto de mídias mistas](/help/assets/mm_mixed_media_set.png)

## Criar um conjunto de mídia mista {#create-a-mixed-media-set}

Ao criar um conjunto, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| Opção &quot;Publicar após salvar&quot; selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros do conjunto mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um Conjunto de mídias mistas**

1. Clique em **Criar** > **Conjuntos de mídias mistas**.
1. Arraste os vídeos, os Conjuntos de imagens, os Conjuntos de rotação e as amostras da Biblioteca de ativos para a tela Conjunto de mídias mistas.

   >[!NOTE]
   >
   >Os Conjuntos de mídia mista não são compatíveis com ativos com nomes de arquivo que contêm qualquer um dos seguintes caracteres: ( ) { }.

1. Siga um destes procedimentos:

   * Para adicionar uma trilha sonora, arraste um arquivo de áudio da Biblioteca de ativos para a caixa Trilha sonora. A trilha sonora é reproduzida enquanto as imagens são exibidas. Ele para quando o vídeo é reproduzido.
   * Para alterar a ordem dos conjuntos, arraste-os para novos locais na tela Conjunto de mídias mistas. A ordem dos conjuntos na tela determina a ordem da esquerda para a direita na qual os usuários veem os conjuntos no Visualizador de conjunto de mídias mistas.
   * (Opcional) Para adicionar uma miniatura personalizada para representar um vídeo no Visualizador, arraste um arquivo de imagem da Biblioteca de ativos para a caixa de espaço reservado Miniatura .

1. Próximo ao canto inferior direito da página, verifique se **Publish after save** está selecionado (padrão).
1. Clique em **Salvar**, selecione uma pasta para armazenar o Conjunto de mídias mistas, insira um nome para o conjunto e clique em **Salvar**.

   Clique em **Visualizar** para ver a aparência do Conjunto de imagens de combinação em um Visualizador de conjunto de imagens.

## Editar um conjunto de mídia mista {#edit-a-mixed-media-set}

Você pode editar um Conjunto de mídias mistas. Se quiser editar um conjunto em um Conjunto de mídias mistas, abra esse conjunto separadamente, edite-o e salve-o. As edições são exibidas no conjunto Mídia mista.

Dependendo de você editar um conjunto publicado ou não, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| Definir já publicado? | Opção &quot;Publicar após salvar&quot; selecionada antes de salvar a edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado.Qualquer novo conjunto de membros adicionado durante a edição mantém seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto adicionados durante a edição mantêm o estado publicado ou não. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um conjunto de mídia mista**

1. Clique no botão **Editar** da substituição do Conjunto de mídias mistas.
1. Siga um destes procedimentos:

   * Para remover itens, selecione-os e clique em **Delete**.
   * Para reorganizar os itens, arraste-os para novos locais.

1. Quando terminar de editar o conjunto, próximo ao canto inferior direito da página, verifique se **Publish after save** está selecionado (padrão).
1. Clique em **Salvar** ou **Salvar como**.

## Excluindo um conjunto de mídia mista {#deleting-a-mixed-media-set}

Ao excluir um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) desse conjunto não são afetados; em vez disso, cada um mantém seu estado publicado ou não publicado.

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um conjunto de mídias mistas**

1. Na Exibição de grade, Exibição de lista ou Exibição de detalhes, selecione um ou mais Conjuntos de mídias mistas.
1. Na Barra de Navegação Global, clique em **Arquivo** > **Excluir** > **Excluir**.

