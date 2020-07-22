---
title: Criação de um conjunto de amostras
seo-title: Criação de um conjunto de amostras
description: nulo
seo-description: Saiba como criar um conjunto de amostras.
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---


# Criação de um conjunto de amostras{#creating-a-swatch-set}

Um Conjunto de amostras oferece aos usuários a oportunidade de visualização de um item em uma cor, padrão ou conclusão diferente. Para criar um Conjunto de amostras com amostras de cores, é necessário ter uma imagem para cada cor, padrão ou acabamento diferente que deseja apresentar aos usuários. Você também precisa de uma cor, padrão ou amostra de fim para cada cor, padrão ou fim.

Por exemplo, suponha que você queira apresentar imagens de maiúsculas com diferentes notas coloridas; as contas são vermelhas, verdes e azuis. Neste caso, você precisa de três tiros do mesmo chapéu. Você precisa de um tiro com um vermelho, um com um verde, e outro com uma conta azul. Você também precisa de uma amostra de cor vermelha, verde e azul. As amostras de cores servem como miniaturas que os usuários clicam no Visualizador do conjunto de amostras para ver a tampa vermelha, com borda verde ou com borda azul.

## Criação de um conjunto de amostras {#create}

Quando você cria um conjunto, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:
| Opção &quot;Publicar após salvar&quot; selecionada antes de salvar?|Estado do conjunto após salvar|Estado do conjunto de membros após salvar|
|— |— |— |
|Sim|Publicado|Publicado|
|Não|Não|Não publicado|Os membros do conjunto mantêm o estado publicado ou não publicado.|

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually_publishing_assets) a publicação de ativos [](publishing-files.md#manually_unpublishing_assets)manualmente.

**Para criar um conjunto de amostras**

1. Execute um dos procedimentos a seguir:

   **Selecione as imagens primeiro** no painel Procurar, selecione as imagens e clique em Criar > Conjuntos de amostras.

   **Start na tela** Conjunto de amostras Clique em Criar > Conjuntos de amostras. Selecione uma pasta na Biblioteca de ativos e arraste as imagens até a seção Visualizações da página Conjunto de amostras.

1. Arraste cores, padrões ou finalizações da amostra para a caixa de espaço reservado Amostras na página Conjunto de amostras.

   Certifique-se de que a cor, o padrão ou a amostra de término que você arrasta para cada espaço reservado representa a cor, o padrão ou o término da imagem adjacente.

1. Para alterar a ordem das imagens no Conjunto de amostras, arraste as imagens para novos locais.
1. Próximo ao canto inferior direito da página, verifique se a opção **Publicar após salvar** está selecionada (padrão).
1. Clique em **Salvar**, selecione uma pasta para armazenar seu conjunto de amostras de cores, digite um nome para o conjunto e clique em Enviar.
1. Para ver o Conjunto de amostras no Visualizador do Conjunto de amostras, clique em **Pré-visualização** na tela Conjunto de amostras. Você pode clicar em miniaturas de amostra no Visualizador do conjunto de amostras para ver como elas se comportam.

## Edição de um conjunto de amostras {#editing-a-swatch-set}

Dependendo de você editar um conjunto publicado ou não publicado, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| Definir já publicado? | Opção &quot;Publicar após salvar&quot; selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado.Qualquer novo conjunto de membros adicionado durante a edição mantém seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto que você tiver adicionado durante a edição manterão seu estado publicado ou não publicado. |

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually_publishing_assets) a publicação de ativos [](publishing-files.md#manually_unpublishing_assets)manualmente.

**Para editar um conjunto de amostras**

1. Na visualização de Grade, navegue até um SwatchSet e, abaixo da imagem, clique em **Editar**.
1. Execute um dos procedimentos a seguir:

   * Para adicionar uma imagem (publicada ou não publicada), arraste-a de uma pasta em Adicionar ativos para a página de **Visualizações** do Conjunto de amostras.
   * Para remover uma imagem, selecione-a e clique em **Excluir** na barra de ferramentas.
   * Para reorganizar imagens, arraste uma imagem para uma nova posição.

1. Quando terminar de editar o conjunto, próximo ao canto inferior direito da página, certifique-se de que **Publicar após salvar** está selecionado (padrão).
1. Clique em **Salvar**, selecione uma pasta de armazenamento, digite um nome para o conjunto e clique em **Salvar**.

## Excluindo um conjunto de amostras {#deleting-a-swatch-set}

Ao excluir um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um deles mantém seu estado publicado ou não publicado.

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually_publishing_assets) a publicação de ativos [](publishing-files.md#manually_unpublishing_assets)manualmente.

**Para excluir um conjunto de amostras**

1. Na Visualização de grade, Visualização de Lista ou Detalhes, selecione um ou mais conjuntos de amostras.
1. Na barra de navegação global, clique em **Arquivo** > **Excluir** > **Excluir**.

