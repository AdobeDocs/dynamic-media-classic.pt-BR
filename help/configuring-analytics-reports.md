---
title: Configuração de relatórios da Adobe Analytics
description: Saiba como configurar relatórios do Adobe Analytics.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1192'
ht-degree: 0%

---


# Configuração de relatórios do Adobe Analytics{#configuring-adobe-analytics-reports}

Para informar à Adobe Analytics quais informações você deseja nos relatórios da Adobe Analytics, acesse a tela Configuração do Adobe Analytics. Depois de configurar os relatórios, essa tela lista, para cada evento do visualizador sobre o qual você deseja obter informações, uma variável do Adobe Analytics correspondente e uma variável do Dynamic Media Classic. Essas combinações de variáveis eventos do visualizador-Adobe Analytics variável-Dynamic Media Classic determinam quais informações são reportadas.

Além de associar eventos do visualizador a variáveis, a tela Configuração do Adobe Analytics oferta ferramentas para ativar, editar e excluir eventos do visualizador.

>[!NOTE]
>
>Sempre que alterar as configurações de Relatório do Adobe Analytics no Adobe Analytics, certifique-se de fazer logon novamente no Adobe Analytics a partir do Adobe Dynamic Media Classic, salvar novamente as configurações do Adobe Analytics e publicar novamente.

Consulte [Efetue logon no Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Consulte [Publicar informações de configuração](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Atribuindo variáveis do Adobe Analytics a eventos e variáveis do visualizador do Dynamic Media Classic {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Use a tela Configuração do Adobe Analytics para associar eventos do visualizador a variáveis do Adobe Analytics e variáveis do Dynamic Media Classic. Para cada evento do visualizador, escolha uma variável Adobe Analytics e uma variável Dynamic Media Classic. Para obter instruções sobre como abrir a tela Configuração do Adobe Analytics, consulte [Faça logon no Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Para atribuir variáveis do Adobe Analytics a eventos e variáveis do visualizador do Dynamic Media Classic**

1. Depois de fazer logon no Adobe Analytics pelo Dynamic Media Classic e selecionar um conjunto de relatórios, na página Configuração do Adobe Analytics, na coluna à direita da tabela, ative um evento do visualizador clicando em **Ativar**.
1. Na coluna Variáveis, exiba o seletor de pares de variáveis clicando no botão de seta do Evento do visualizador desejado.

   Consulte [eventos do visualizador](configuring-analytics-reports.md#viewer_events).

1. Adicione uma variável do Dynamic Media Classic.

   Consulte [Variáveis do Dynamic Media Classic](configuring-analytics-reports.md#scene7_variables).

1. Adicione uma variável do Adobe Analytics.
1. (Opcional) Para adicionar outro par de variáveis, clique em **Adicionar**.
1. Clique em **Salvar**.

   Depois de clicar em Salvar, o evento do visualizador, sua variável Adobe Analytics e sua variável Dynamic Media Classic são listados na tela Configuração do Adobe Analytics.

1. No canto inferior direito, clique em **Fechar**.
1. Clique em **Publicar** > **Enviar publicação** para executar uma publicação do Servidor de imagens.

   A publicação é necessária para que as informações contidas nos visualizadores estejam disponíveis nos servidores Dynamic Media Classic.

### Eventos do visualizador {#viewer-events}

Os eventos do visualizador descrevem as ações que os usuários executam com visualizadores do Dynamic Media Classic. Quando um usuário inicia uma determinada ação, como clicar em uma miniatura ou iniciar ou parar um vídeo, o visualizador &quot;transmite&quot; um evento para a página da Web, juntamente com os dados associados a esse evento.

A tabela a seguir descreve os eventos do visualizador que podem ser adicionados à tela Configuração do Adobe Analytics.

| Evento do visualizador | Suporte e visualizadores da plataforma HTML5 Viewer | Descrição |
|--- |--- |--- |
| CARREGAR | **X** (eCatalog, Flyout, SpinSet, Video, Zoom) | Quando um usuário start no visualizador. |
| PÁGINA | **X**  (eCatalog) | Em eCatalogs, quando um usuário gira uma página; em visualizadores de zoom direcionados, quando um usuário clica em um público alvo diferente ou em uma amostra de cor. |
| SWAP | **X**  (eCatalog, Flyout, SpinSet, Video, Zoom) | Quando um usuário clica em uma miniatura diferente para visualização de uma imagem diferente. |
| ITEM | **X**  (eCatalog) | Em visualizadores que suportam mapas de imagem nos quais sobreposições são definidas, quando um usuário posiciona o ponteiro sobre um mapa de imagem para ler o texto de sobreposição. |
| HREF | **X**  (eCatalog) | Em visualizadores que suportam Mapas de imagem, quando um usuário clica em um URL em um Mapa de imagem. |
| PÚBLICO ALVO |  | Em visualizadores de zoom direcionados, quando um usuário clica em um público alvo de zoom para aumentar o zoom em parte de uma imagem. |
| PESQUISA |  | Em eCatalogs, quando um usuário realiza uma pesquisa de palavra. |
| JOGAR | **X**  (Vídeo) | Em visualizadores de vídeo, quando um usuário clica em Reproduzir para start reproduzindo um vídeo.<br><br>**Observação:** se você estiver usando o relatórios de vídeo baseado em pulsação do Adobe Analytics, não será necessário mapear nenhuma variável para esse evento do visualizador ao configurar o Adobe Analytics no Dynamic Media Classic. O Video Heartbeat funciona com visualizadores Dynamic Media Classic HTML5 e MixedMedia prontos para uso. O player de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo da Adobe Analytics. Consulte [Ativando os relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| PAUSA | **X** (Vídeo) | Nos visualizadores de vídeo, quando um usuário clica em Pausar para pausar um vídeo.<br><br>**Observação:** se você estiver usando o relatórios de vídeo baseado em pulsação do Adobe Analytics, não será necessário mapear nenhuma variável para esse evento do visualizador ao configurar o Adobe Analytics no Dynamic Media Classic. O Video Heartbeat funciona com visualizadores Dynamic Media Classic HTML5 e MixedMedia prontos para uso. O player de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo da Adobe Analytics. Consulte [Ativando os relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| PARAR | **X** (Vídeo) | Nos visualizadores de vídeo, quando um usuário clica em Parar para parar a reprodução de um vídeo.<br><br>**Observação:** se você estiver usando o relatórios de vídeo baseado em pulsação do Adobe Analytics, não será necessário mapear nenhuma variável para esse evento do visualizador ao configurar o Adobe Analytics no Dynamic Media Classic. O Video Heartbeat funciona com visualizadores Dynamic Media Classic HTML5 e MixedMedia prontos para uso. O player de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo da Adobe Analytics. Consulte [Ativando os relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| MARCO | **X**  (Vídeo) | Nos visualizadores de vídeo, eventos de marco são gerados quando o usuário assiste 0, 25, 50, 75 ou 100% do vídeo.<br><br>**Observação:** se você estiver usando o relatórios de vídeo baseado em pulsação do Adobe Analytics, não será necessário mapear nenhuma variável para esse evento do visualizador ao configurar o Adobe Analytics no Dynamic Media Classic. O Video Heartbeat funciona com visualizadores Dynamic Media Classic HTML5 e MixedMedia prontos para uso. O player de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo da Adobe Analytics. Consulte [Ativando os relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| SWATCH | X (Flyout, Zoom) | Esse evento do visualizador é mapeado para o evento do visualizador PAGE no Dynamic Media Classic. |
| ZOOM | **X**  (eCatalog, SpinSet, Zoom) | Não rastreado pelo Adobe Analytics.<br> |
| PAN | **X**  (eCatalog, SpinSet, Zoom) | Não rastreado pelo Adobe Analytics.<br> |
| SPIN | **X**  (SpinSet) | Não rastreado pelo Adobe Analytics.<br> |


### Variáveis do Dynamic Media Classic {#scene-variables}

Para cada evento do visualizador na tela Configuração do Adobe Analytics, escolha uma variável Adobe Analytics e uma *variável Dynamic Media Classic*. As variáveis do Dynamic Media Classic representam dados que você pode obter para um relatório. Por exemplo, a variável `searchTerm` lista palavras-chave usadas em pesquisas do eCatalog.

A tabela a seguir descreve as variáveis do Dynamic Media Classic.

| Variável Dynamic Media Classic | Descrição |
|--- |:--- |
| ativo | ID de ativo do Dynamic Media Classic ou arquivo de caminho de vídeo. |
| viewerId | Um número arbitrário atribuído a cada tipo de visualizador diferente. |
| pageLabel | Em eCatalogs, a página que um visualizador exibe. |
| label | O valor do rótulo (uma string). |
| quadro | A referência de página ou página em um Conjunto de imagens. |
| rollover_keyRaw | Todo o valor HREF, não apenas qualquer parte processada dele. |
| rollover_keyProc | A ID de um item referenciado em um Mapa de imagem (válido para eventos href e item). |
| searchTerm | Um termo usado na pesquisa do eCatalog. |
| timeStamp | Reproduzir, Parar e Pausar escolhidos em visualizadores de vídeo. |
| progresso | A porcentagem de um evento de marco concluído. |
| targetId | O valor da id (um número). |

## Ativar, editar e excluir eventos do visualizador {#activating-editing-and-deleting-viewer-events}

Na tela Configuração do Adobe Analytics, você pode ativar, editar e excluir eventos do visualizador:

* ****
AtivandoClique  **[!UICONTROL Enable]** para ativar ou  **[!UICONTROL Disable]** desativar um evento do visualizador selecionado.

* ****
EdiçãoSelecione um evento do visualizador e clique no botão  **[!UICONTROL View/Edit]** Variáveis cinza. Nas listas suspensas Variável clássica Dynamic Media e Variável Adobe Analytics, escolha uma variável diferente de cada lista respectiva. Para obter mais informações, consulte Atribuindo variáveis do Adobe Analytics a eventos e variáveis do visualizador do Dynamic Media Classic.

* ****
ExcluindoSelecione um evento do visualizador e clique no botão  **[!UICONTROL View/Edit]** Variáveis cinza. Clique em **[!UICONTROL Delete]**.
