---
title: Criação de um conjunto de mídia mista
seo-title: Criação de um conjunto de mídia mista
description: 'null'
seo-description: Saiba como criar um Conjunto de mídia misto.
uuid: a 0 c 6 e 5 fa -7 a 85-4376-b 9 a 3-b 72 ae 63 d 3 d 95
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 0 ff 9 e 763-897 c -4 ba 5-b 606-a 95 d 5 e 45 f 35 e
translation-type: tm+mt
source-git-commit: 2f99190eb0c346b87402e69c4067e94365042339

---


# Criação de um conjunto de mídia mista{#creating-a-mixed-media-set}

Crie um conjunto de mídia mista quando quiser combinar vários tipos de visualizadores em uma apresentação. Verifique se os arquivos, Conjuntos de imagens, Conjuntos de amostras e Rotação estão prontos para serem publicados antes de adicioná-los ao Conjunto de mídia mista.

![Conjunto de mídia mista](/help/assets/mm_mixed_media_set.png)

## Criar um conjunto de mídia mista {#create-a-mixed-media-set}

Quando você cria um conjunto, **a opção Publicar depois de salvar** afeta o conjunto e os membros definidos das seguintes maneiras:

| A opção «Publicar após salvar» selecionada antes de salvar? | Estado de conjunto após salvar | Estado dos membros definidos após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros podem reter seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um conjunto de mídia mista**

1. Clique **em Criar** &gt; **Conjuntos de mídia mista**.
1. Arraste os vídeos, Conjuntos de imagens, Conjuntos de rotação e amostras da Biblioteca de ativos para a tela Conjunto de mídia mista.

   >[!NOTE]
   >
   >Os conjuntos de mídia mista não oferecem suporte a ativos com nomes de arquivo que contêm qualquer um dos seguintes caracteres: () {}.

1. Execute um dos procedimentos a seguir:

   * Para adicionar uma trilha sonora, arraste um arquivo de áudio da Biblioteca de ativos para a caixa Soundtrack. A trilha sonora é reproduzida enquanto as imagens são exibidas. Ela é interrompida quando o vídeo é reproduzido.
   * Para alterar a ordem dos conjuntos, arraste-os para novos locais na tela Conjunto de mídia mista. A ordem dos conjuntos na tela determina a ordem da esquerda para a direita no qual os usuários veem conjuntos no Visualizador de conjunto de mídia mista.
   * (Opcional) Para adicionar uma miniatura personalizada para representar um vídeo no Visualizador, arraste um arquivo de imagem da Biblioteca de ativos para a caixa de espaço reservado Miniatura.

1. Próximo ao canto inferior direito da página, certifique-se de **que Publicar depois de salvar** esteja selecionado (padrão).
1. Clique **em Salvar**, selecione uma pasta para armazenar o Conjunto de mídia mista, insira um nome para o conjunto e clique **em Salvar**.

   Clique **em Visualizar** para ver a aparência do Conjunto de imagens de combinação em um Visualizador de imagens.

## Editar um conjunto de mídia mista {#edit-a-mixed-media-set}

Você pode editar um Conjunto de mídia misto. Se você quiser editar um conjunto em um Conjunto de mídia mista, abra-o separadamente, edite-o e salve-o. As edições aparecem no conjunto de mídia mista.

Se você editar um conjunto publicado ou não publicado, **a opção Publicar depois de salvar** afeta o conjunto e os membros definidos das seguintes maneiras:

| Já foi publicado? | A opção «Publicar após salvar» selecionada antes de salvar sua edição? | Estado de conjunto após salvar | Estado dos membros definidos após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros definidos existentes mantêm seu estado publicado. Todos os novos membros definidos durante a edição mantêm seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros definidos e todos os novos membros definidos durante a edição mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um conjunto de mídia mista**

1. Clique no botão **Editar borda do** conjunto de mídia mista.
1. Execute um dos procedimentos a seguir:

   * Para remover itens, selecione-os e clique **em Excluir**.
   * Para reordenar itens, arraste-os para novos locais.

1. Quando terminar de editar o conjunto, próximo ao canto inferior direito da página, certifique-se de **que Publicar depois de salvar** esteja selecionado (padrão).
1. Clique **em Salvar** ou **Salvar como**.

## Excluindo um conjunto de mídia mista {#deleting-a-mixed-media-set}

Quando um conjunto é excluído, o próprio conjunto é movido para a lixeira. No entanto, os membros (ou «filhos») dentro desse conjunto não serão afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um conjunto de mídia mista**

1. Na Exibição de grade, Exibição de lista ou Exibição de detalhes, selecione um ou mais Conjuntos de mídia mista.
1. Na barra de navegação global, clique **em Arquivo** &gt; **Excluir** &gt; **Excluir**.

