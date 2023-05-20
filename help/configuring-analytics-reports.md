---
title: Configurar relatórios do Adobe Analytics
description: Saiba como configurar relatórios do Adobe Analytics no Adobe Dynamic Media Classic.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1214'
ht-degree: 0%

---

# Configurar relatórios do Adobe Analytics{#configuring-adobe-analytics-reports}

Para informar ao Adobe Analytics quais informações você deseja incluir nos relatórios do Adobe Analytics, vá para a tela Configuração do Adobe Analytics. Depois de configurar relatórios, essa tela lista, para cada evento do visualizador sobre o qual deseja obter informações, uma variável do Adobe Analytics e uma variável do Adobe Dynamic Media Classic correspondentes. Essas combinações de variáveis do visualizador events-Adobe Analytics variable-Adobe Dynamic Media Classic determinam quais informações são relatadas.

Além de associar eventos do visualizador a variáveis, a tela Configuração do Adobe Analytics oferece ferramentas para ativar, editar e excluir eventos do visualizador.

>[!NOTE]
>
>Sempre que você alterar as configurações do Relatório do Adobe Analytics no Adobe Analytics, certifique-se de fazer logon novamente no Adobe Analytics a partir do Adobe Dynamic Media Classic, salvar novamente as configurações do Adobe Analytics e publicar novamente.

Consulte [Fazer logon no Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Consulte [Publicar informações de configuração](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Atribuir variáveis do Adobe Analytics a eventos e variáveis do visualizador do Adobe Dynamic Media Classic {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Use a tela Configuração do Adobe Analytics para associar eventos do visualizador a variáveis do Adobe Analytics e variáveis do Adobe Dynamic Media Classic. Para cada evento do visualizador, escolha uma variável do Adobe Analytics e uma variável do Adobe Dynamic Media Classic. Para obter instruções sobre como abrir a tela Configuração do Adobe Analytics, consulte [Fazer logon no Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Para atribuir variáveis do Adobe Analytics a eventos e variáveis do visualizador do Adobe Dynamic Media Classic:**

1. Depois de fazer logon no Adobe Analytics a partir do Adobe Dynamic Media Classic e selecionar um conjunto de relatórios, na página Configuração do Adobe Analytics, na coluna da tabela à direita, ative um evento do visualizador selecionando **[!UICONTROL Enable]**.
1. Na coluna Variáveis, exiba o seletor de par de variáveis selecionando o botão de seta para o Evento do visualizador desejado.

   Consulte [Eventos do visualizador](configuring-analytics-reports.md#viewer_events).

1. Adicione uma variável do Adobe Dynamic Media Classic.

   Consulte [Variáveis do Adobe Dynamic Media Classic](configuring-analytics-reports.md#scene7_variables).

1. Adicione uma variável do Adobe Analytics.
1. (Opcional) Para adicionar outro par de variáveis, selecione **[!UICONTROL Add]**.
1. Selecionar **[!UICONTROL Save]**.

   Depois de selecionar **[!UICONTROL Save]**, o evento do visualizador, sua variável do Adobe Analytics e sua variável do Adobe Dynamic Media Classic são listados na tela Configuração do Adobe Analytics.

1. No canto inferior direito, selecione **[!UICONTROL Close]**.
1. Ir para **[!UICONTROL Publish]** > **[!UICONTROL Submit Publish]** para executar uma publicação do Servidor de imagens.

   A publicação é necessária para que as informações contidas nos visualizadores estejam disponíveis nos servidores do Adobe Dynamic Media Classic.

### Eventos do visualizador {#viewer-events}

Os eventos do visualizador descrevem as ações que os usuários executam com visualizadores do Adobe Dynamic Media Classic. Quando um usuário inicia uma determinada ação, como selecionar uma miniatura ou iniciar ou parar um vídeo, o visualizador &quot;transmite&quot; um evento para a página da Web, juntamente com os dados associados a esse evento.

A tabela a seguir descreve os eventos do visualizador que podem ser adicionados à tela Configuração do Adobe Analytics.

| Evento do visualizador | Suporte e visualizadores da HTML5 Viewer Platform | Descrição |
| --- | --- | --- |
| CARREGAR | **X** (eCatalog, Flyout, SpinSet, Vídeo, Zoom) | Quando um usuário inicia um visualizador |
| PÁGINA | **X**  (eCatalog) | Em eCatalogs, quando um usuário gira uma página; em visualizadores de zoom direcionados, quando um usuário seleciona um destino diferente ou uma amostra de cor. |
| TROCAR | **X**  (eCatalog, Flyout, SpinSet, Vídeo, Zoom) | Quando um usuário seleciona uma miniatura diferente para visualizar uma imagem diferente. |
| ITEM | **X**  (eCatalog) | Em visualizadores compatíveis com Mapas de imagem nos quais as sobreposições são definidas, quando um usuário passa o ponteiro sobre um Mapa de imagem para ler o texto da sobreposição. |
| HREF | **X**  (eCatalog) | Em visualizadores compatíveis com Mapas de imagem, quando um usuário seleciona um URL em um Mapa de imagem. |
| TARGET |  | Em visualizadores de zoom direcionados, quando um usuário seleciona um destino de zoom para aplicar zoom a parte de uma imagem. |
| PESQUISAR |  | Em eCatalogs, quando um usuário realiza uma pesquisa de palavra. |
| PLAY | **X**  (Vídeo) | Em Visualizadores de vídeo, quando um usuário seleciona Reproduzir para começar a reproduzir um vídeo.<br><br>**Nota:** Se estiver usando relatórios de vídeo baseados em pulsação do Adobe Analytics, não será necessário mapear variáveis para esse evento do visualizador ao configurar o Adobe Analytics no Adobe Dynamic Media Classic. O Video Heartbeat funciona com visualizadores Adobe Dynamic Media Classic HTML5 Video e MixedMedia prontos para uso. O reprodutor de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo do Adobe Analytics. Consulte [Ativar relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| PAUSAR | **X** (Vídeo) | Em Visualizadores de vídeo, quando um usuário seleciona **[!UICONTROL Pause]** para congelar um vídeo.<br><br>**Nota:** Se estiver usando relatórios de vídeo baseados em pulsação do Adobe Analytics, não será necessário mapear variáveis para esse evento do visualizador ao configurar o Adobe Analytics no Adobe Dynamic Media Classic. O Video Heartbeat funciona com visualizadores Adobe Dynamic Media Classic HTML5 Video e MixedMedia prontos para uso. O reprodutor de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo do Adobe Analytics. Consulte [Ativar relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| PARAR | **X** (Vídeo) | Em Visualizadores de vídeo, quando um usuário seleciona **[!UICONTROL Stop]** para parar de reproduzir um vídeo.<br><br>**Nota:** Se estiver usando relatórios de vídeo baseados em pulsação do Adobe Analytics, não será necessário mapear variáveis para esse evento do visualizador ao configurar o Adobe Analytics no Adobe Dynamic Media Classic. O Video Heartbeat funciona com visualizadores Adobe Dynamic Media Classic HTML5 Video e MixedMedia prontos para uso. O reprodutor de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo do Adobe Analytics. Consulte [Ativar relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| ETAPA | **X**  (Vídeo) | Em visualizadores de vídeo, os eventos marcantes são gerados quando o usuário assiste a 0, 25, 50, 75 ou 100% do vídeo.<br><br>**Nota:** Se estiver usando relatórios de vídeo baseados em pulsação do Adobe Analytics, não será necessário mapear variáveis para esse evento do visualizador ao configurar o Adobe Analytics no Adobe Dynamic Media Classic. O Video Heartbeat funciona com visualizadores Adobe Dynamic Media Classic HTML5 Video e MixedMedia prontos para uso. O reprodutor de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo do Adobe Analytics. Consulte [Ativar relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| AMOSTRA | **X** (Flyout, Zoom) | Este evento do visualizador é mapeado para o evento do visualizador de PÁGINA no Adobe Dynamic Media Classic. |
| ZOOM | **X** (eCatalog, SpinSet, Zoom) | Não rastreado pelo Adobe Analytics. |
| PAN | **X** (eCatalog, SpinSet, Zoom) | Não rastreado pelo Adobe Analytics. |
| ROTAÇÃO | **X** (SpinSet) | Não rastreado pelo Adobe Analytics. |

### Variáveis do Adobe Dynamic Media Classic {#scene-variables}

Para cada evento do visualizador na tela Configuração do Adobe Analytics, escolha uma variável do Adobe Analytics e um *variável do Adobe Dynamic Media Classic*. As variáveis do Adobe Dynamic Media Classic representam dados que podem ser obtidos para um relatório. Por exemplo, a variável `searchTerm` lista de palavras-chave usadas em pesquisas de eCatalog.

A tabela a seguir descreve as variáveis do Adobe Dynamic Media Classic:

| variável do Adobe Dynamic Media Classic | Descrição |
| --- | --- |
| ativo | ID do ativo Adobe Dynamic Media Classic ou arquivo de caminho do vídeo. |
| viewerId | Um número arbitrário atribuído a cada tipo de visualizador diferente. |
| pageLabel | Nos eCatalogs, a página que um visualizador exibe. |
| rótulo | O valor do rótulo (uma string). |
| quadro | A referência de página ou página em um Conjunto de imagens. |
| rollover_keyRaw | Todo o valor HREF, não apenas qualquer parte processada dele. |
| rollover_keyProc | A ID de um item referenciado em um Mapa de imagem (válido para eventos href e item). |
| searchTerm | Um termo usado na pesquisa de eCatalog. |
| timeStamp | Reproduzir, Interromper e Pausar escolhidos nos visualizadores de vídeo. |
| progresso | A porcentagem de um evento de marco que está concluída. |
| targetId | O valor de id (um número). |

## Ativar, editar e excluir eventos do visualizador {#activating-editing-and-deleting-viewer-events}

Na tela Configuração do Adobe Analytics, você pode ativar, editar e excluir eventos do visualizador:

* **Ativar** - Selecionar **[!UICONTROL Enable]** para ativar ou **[!UICONTROL Disable]** para desativar um evento do visualizador selecionado.

* **Editar** - Selecione um evento de visualizador e selecione **[!UICONTROL View/Edit]** Botão cinza de variáveis. Nas listas suspensas Variável Adobe Dynamic Media Classic e Variável Adobe Analytics, escolha uma variável diferente de cada lista. Para obter mais informações, consulte [Atribuição de variáveis do Adobe Analytics a eventos e variáveis do visualizador do Adobe Dynamic Media Classic](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **Excluir** - Selecione um evento do visualizador e selecione **[!UICONTROL View/Edit]** Botão cinza de variáveis. Selecionar **[!UICONTROL Delete]**.
