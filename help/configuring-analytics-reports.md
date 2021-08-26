---
title: Configurar relatórios do Adobe Analytics
description: Saiba como configurar relatórios do Adobe Analytics no Adobe Dynamic Media Classic.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1211'
ht-degree: 0%

---

# Configurar relatórios do Adobe Analytics{#configuring-adobe-analytics-reports}

Para informar ao Adobe Analytics quais informações você deseja nos relatórios do Adobe Analytics, acesse a tela Configuração do Adobe Analytics . Após configurar os relatórios, essa tela lista, para cada evento do visualizador sobre o qual você deseja obter informações, uma variável do Adobe Analytics correspondente e a variável do Adobe Dynamic Media Classic. Estes eventos do visualizador - Variável Adobe Analytics - Adobe Dynamic Media Classic combinações determinam quais informações são relatadas.

Além de associar eventos do visualizador com variáveis, a tela Configuração do Adobe Analytics oferece ferramentas para ativar, editar e excluir eventos do visualizador.

>[!NOTE]
>
>Sempre que alterar as configurações do Relatório do Adobe Analytics no Adobe Analytics, certifique-se de fazer logon novamente no Adobe Analytics a partir do Adobe Dynamic Media Classic, salvar novamente as configurações do Adobe Analytics e, em seguida, republicar.

Consulte [Fazer logon no Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Consulte [Publicar informações de configuração](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Atribuir variáveis do Adobe Analytics a eventos e variáveis do visualizador do Adobe Dynamic Media Classic {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Use a tela Configuração do Adobe Analytics para associar eventos do visualizador com variáveis Adobe Analytics e variáveis Adobe Dynamic Media Classic. Para cada evento do visualizador, escolha uma variável Adobe Analytics e uma variável Adobe Dynamic Media Classic. Para obter instruções sobre como abrir a tela Configuração do Adobe Analytics, consulte [Fazer logon no Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Para atribuir variáveis do Adobe Analytics aos eventos e variáveis do visualizador do Adobe Dynamic Media Classic:**

1. Depois de fazer logon no Adobe Analytics pelo Adobe Dynamic Media Classic e selecionar um conjunto de relatórios, na página Configuração do Adobe Analytics, na coluna da tabela direita, ative um evento do visualizador selecionando **[!UICONTROL Enable]**.
1. Na coluna Variáveis , exiba o seletor de par de variáveis selecionando o botão de seta para o Evento do visualizador desejado.

   Consulte [Eventos do visualizador](configuring-analytics-reports.md#viewer_events).

1. Adicione uma variável Adobe Dynamic Media Classic.

   Consulte [Variáveis do Adobe Dynamic Media Classic](configuring-analytics-reports.md#scene7_variables).

1. Adicione uma variável Adobe Analytics.
1. (Opcional) Para adicionar outro par de variáveis, selecione **[!UICONTROL Add]**.
1. Selecione **[!UICONTROL Save]**.

   Depois de selecionar **[!UICONTROL Save]**, o evento do visualizador, sua variável Adobe Analytics e sua variável Adobe Dynamic Media Classic, são listados na tela Configuração do Adobe Analytics.

1. No canto inferior direito, selecione **[!UICONTROL Close]**.
1. Vá para **[!UICONTROL Publish]** > **[!UICONTROL Submit Publish]** para executar uma publicação do Image Serving.

   A publicação é necessária para que as informações contidas nos visualizadores estejam disponíveis nos servidores Adobe Dynamic Media Classic.

### Eventos do visualizador {#viewer-events}

Os eventos do visualizador descrevem as ações que os usuários executam com os visualizadores Adobe Dynamic Media Classic. Quando um usuário inicia uma determinada ação, como selecionar uma miniatura ou iniciar ou parar um vídeo, o visualizador &quot;transmite&quot; um evento para a página da Web, juntamente com os dados associados a esse evento.

A tabela a seguir descreve os eventos do visualizador que podem ser adicionados à tela Configuração do Adobe Analytics.

| Evento do visualizador | Suporte e visualizadores da Plataforma do visualizador HTML5 | Descrição |
| --- | --- | --- |
| CARREGAR | **X** (Catálogo eletrônico, Submenu, Conjunto de rotação, Vídeo, Zoom) | Quando um usuário inicia um visualizador |
| PÁGINA | **X**   (Catálogo eletrônico) | Em eCatalogs, quando um usuário transforma uma página; em visualizadores de zoom direcionados, quando um usuário seleciona um destino diferente ou uma amostra de cor. |
| SWAP | **X**  (Catálogo eletrônico, Submenu, Conjunto de rotação, Vídeo, Zoom) | Quando um usuário seleciona uma miniatura diferente para exibir uma imagem diferente. |
| ITEM | **X**   (Catálogo eletrônico) | Nos visualizadores que suportam mapas de imagem nos quais as sobreposições são definidas, quando um usuário passa o ponteiro sobre um mapa de imagem para ler o texto sobreposto. |
| HREF | **X**   (Catálogo eletrônico) | Em visualizadores compatíveis com mapas de imagem, quando um usuário seleciona um URL em um mapa de imagem. |
| TARGET |  | Em visualizadores de zoom direcionados, quando um usuário seleciona um direcionamento de zoom para ampliar para parte de uma imagem. |
| PESQUISA |  | Em Catálogos eletrônicos, quando um usuário realiza uma pesquisa por palavras. |
| REPRODUZIR | **X**   (Vídeo) | Nos visualizadores de vídeo, quando um usuário seleciona Reproduzir para iniciar a reprodução de um vídeo.<br><br>**Observação:** se estiver usando os relatórios de vídeo baseados em pulsação do Adobe Analytics, não será necessário mapear variáveis para esse evento do visualizador ao configurar o Adobe Analytics no Adobe Dynamic Media Classic. O Video Heartbeat funciona com os visualizadores de vídeo Dynamic Media Classic HTML5 e MixedMedia prontos para uso. O reprodutor de vídeo gera dados de rastreamento para visualização nos Relatórios de vídeo do Adobe Analytics. Consulte [Ativar relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| PAUSA | **X**  (Vídeo) | Em visualizadores de vídeo, quando um usuário seleciona **[!UICONTROL Pause]** para congelar um vídeo.<br><br>**Observação:** se estiver usando os relatórios de vídeo baseados em pulsação do Adobe Analytics, não será necessário mapear variáveis para esse evento do visualizador ao configurar o Adobe Analytics no Adobe Dynamic Media Classic. O Video Heartbeat funciona com os visualizadores de vídeo Dynamic Media Classic HTML5 e MixedMedia prontos para uso. O reprodutor de vídeo gera dados de rastreamento para visualização nos Relatórios de vídeo do Adobe Analytics. Consulte [Ativar relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| PARAR | **X**  (Vídeo) | Em visualizadores de vídeo, quando um usuário seleciona **[!UICONTROL Stop]** para parar de reproduzir um vídeo.<br><br>**Observação:** se estiver usando os relatórios de vídeo baseados em pulsação do Adobe Analytics, não será necessário mapear variáveis para esse evento do visualizador ao configurar o Adobe Analytics no Adobe Dynamic Media Classic. O Video Heartbeat funciona com os visualizadores de vídeo Dynamic Media Classic HTML5 e MixedMedia prontos para uso. O reprodutor de vídeo gera dados de rastreamento para visualização nos Relatórios de vídeo do Adobe Analytics. Consulte [Ativar relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| MARCO | **X**   (Vídeo) | Em visualizadores de vídeo, os eventos de marco são gerados quando o usuário assiste 0, 25, 50, 75 ou 100% do vídeo.<br><br>**Observação:** se estiver usando os relatórios de vídeo baseados em pulsação do Adobe Analytics, não será necessário mapear variáveis para esse evento do visualizador ao configurar o Adobe Analytics no Adobe Dynamic Media Classic. O Video Heartbeat funciona com os visualizadores de vídeo Dynamic Media Classic HTML5 e MixedMedia prontos para uso. O reprodutor de vídeo gera dados de rastreamento para visualização nos Relatórios de vídeo do Adobe Analytics. Consulte [Ativar relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| SWATCH | **X**  (Flyout, Zoom) | Este evento do visualizador é mapeado para o evento do visualizador PAGE no Adobe Dynamic Media Classic. |
| ZOOM | **X** (eCatalog, SpinSet, Zoom) | Não rastreado pelo Adobe Analytics. |
| PAN | **X** (eCatalog, SpinSet, Zoom) | Não rastreado pelo Adobe Analytics. |
| SPIN | **X**  (SpinSet) | Não rastreado pelo Adobe Analytics. |

### Variáveis do Adobe Dynamic Media Classic {#scene-variables}

Para cada evento do visualizador na tela Configuração do Adobe Analytics, escolha uma variável Adobe Analytics e uma *Variável Adobe Dynamic Media Classic*. As variáveis do Adobe Dynamic Media Classic representam os dados que você pode obter para um relatório. Por exemplo, a variável `searchTerm` lista palavras-chave usadas em pesquisas do eCatalog.

A tabela a seguir descreve as variáveis do Adobe Dynamic Media Classic:

| Variável Adobe Dynamic Media Classic | Descrição |
| --- | --- |
| ativo | ID de ativo do Adobe Dynamic Media Classic ou arquivo de caminho de vídeo. |
| viewerId | Um número arbitrário atribuído a cada tipo de visualizador diferente. |
| pageLabel | Em eCatalogs, a página que um visualizador exibe. |
| label | O valor do rótulo (uma string). |
| quadro | A página ou referência de página em um Conjunto de imagens. |
| rolover_keyRaw | O valor HREF inteiro, não apenas qualquer parte processada dele. |
| rolover_keyProc | A ID de um item referenciado em um Mapa de imagem (válido para eventos href e item). |
| searchTerm | Um termo que é usado na pesquisa do eCatalog. |
| timeStamp | Reproduzir, Parar e Pausar escolhidos em visualizadores de vídeo. |
| progresso | A porcentagem de um evento de marco concluído. |
| targetId | O valor da id (um número). |

## Ativar, editar e excluir eventos do visualizador {#activating-editing-and-deleting-viewer-events}

Na tela Configuração do Adobe Analytics, é possível ativar, editar e excluir eventos do visualizador:

* **Ativar**  - Selecione  **[!UICONTROL Enable]** para ativar ou  **[!UICONTROL Disable]** para desativar um evento de visualizador selecionado.

* **Editar**  - Selecione um evento do visualizador e selecione o botão  **[!UICONTROL View/Edit]** Variables cinza. Nas listas suspensas Variável clássica e Variável Adobe Analytics do Adobe Dynamic Media , escolha uma variável diferente de cada lista respectiva. Para obter mais informações, consulte [Atribuindo variáveis do Adobe Analytics aos eventos e variáveis do visualizador do Adobe Classic](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **Excluir**  - Selecione um evento do visualizador e selecione o botão cinza  **[!UICONTROL View/Edit]** Variáveis. Selecione **[!UICONTROL Delete]**.
