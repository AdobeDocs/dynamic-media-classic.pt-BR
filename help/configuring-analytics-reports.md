---
title: Configuração dos relatórios do Adobe Analytics
seo-title: Configuração dos relatórios do Adobe Analytics
description: 'null'
seo-description: Saiba como configurar os relatórios do Adobe Analytics.
uuid: bf 210 f 68-dcb 0-4 e 86-be 04-0 a 8 b 2117 ef 2 a
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/adobe_ analytics_ instrumentation_ kit
discoiquuid: f 4 c 8 c 2 b 3-cc 95-416 f -9 a 5 d-da 81 c 231 dfc 2
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Configuração dos relatórios do Adobe Analytics{#configuring-adobe-analytics-reports}

Para informar ao Adobe Analytics quais informações você deseja nos relatórios do Adobe Analytics, vá para a tela Configuração do Adobe Analytics. Depois de configurar relatórios, esta tela lista, para cada evento do visualizador que você deseja obter informações sobre, uma variável correspondente do Adobe Analytics e uma variável do Dynamic Media clássica. Essas combinações de variáveis do visualizador do Adobe Analytics-Dynamic Media Classic determinam quais informações são relatadas.

Além de associar eventos do visualizador com variáveis, a tela Configuração do Adobe Analytics oferece ferramentas para ativar, editar e excluir eventos do visualizador.

>[!NOTE]
>
>Sempre que você alterar as configurações de relatório do Adobe Analytics no Adobe Analytics, certifique-se de fazer logon novamente no Adobe Analytics a partir do Adobe Scene 7 Publishing System, salvar novamente as configurações de configuração do Adobe Analytics e republicar.

Consulte [Logon no Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Consulte [Publicar informações](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)de configuração.

## Atribuição de variáveis do Adobe Analytics aos eventos e variáveis do visualizador do Dynamic Media Classic {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Use a tela Configuração do Adobe Analytics para associar eventos do visualizador com variáveis do Adobe Analytics e variáveis do Dynamic Media Classic. Para cada evento do visualizador, escolha uma variável do Adobe Analytics e uma variável do Dynamic Media Classic. Para obter instruções sobre como abrir a tela Configuração do Adobe Analytics, consulte [Fazer logon no Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Para atribuir variáveis do Adobe Analytics aos eventos e variáveis do visualizador do Dynamic Media Classic**

1. Depois de fazer logon no Adobe Analytics a partir do Dynamic Media Classic e selecionar um conjunto de relatórios, na página Configuração do Adobe Analytics, na coluna da extrema direita da tabela, ative um evento do visualizador clicando **em Ativar**.
1. Na coluna Variáveis, exiba o seletor de par da variável clicando no botão de seta do Evento do visualizador desejado.

   Consulte [Eventos do visualizador](configuring-analytics-reports.md#viewer_events).

1. Adicione uma variável do Dynamic Media Classic.

   Consulte [Variáveis do Dynamic Media Classic](configuring-analytics-reports.md#scene7_variables).

1. Adicione uma variável do Adobe Analytics.
1. (Opcional) Para adicionar outro par de variável, clique **em Adicionar**.
1. Clique **em Salvar**.

   Depois de clicar em Salvar, o evento do visualizador, sua variável do Adobe Analytics e sua variável do Dynamic Media Classic estão listados na tela Configuração do Adobe Analytics.

1. No canto inferior direito, clique **em Fechar**.
1. Clique **em Publicar** &gt; **Enviar publicação** para executar uma publicação de serviço de imagem.

   A publicação é necessária para que as informações contidas nos visualizadores estejam disponíveis nos servidores do Dynamic Media Classic.

### Eventos do visualizador {#viewer-events}

Os eventos do visualizador descrevem ações que os usuários executam com visualizadores do Dynamic Media Classic. Quando um usuário inicia uma determinada ação, como clicar em uma miniatura ou iniciar ou parar um vídeo, o visualizador «transmite» um evento à página da Web, juntamente com os dados associados a esse evento.

A tabela a seguir descreve os eventos do visualizador que podem ser adicionados à tela Configuração do Adobe Analytics.

| Evento do visualizador | Suporte e visualizadores da plataforma visualizador HTML 5 | Descrição |
|--- |--- |--- |
| LOAD | **X** (ecatalog, Flyout, spinset, Vídeo, Zoom) | Quando um usuário inicia o visualizador. |
| PAGE | **X** (ecatalog) | No ecatalogs, quando um usuário transforma uma página; em visualizadores de zoom direcionados, quando um usuário clica em um destino diferente ou em uma amostra de cor. |
| TROCAR | **X** (ecatalog, Flyout, spinset, Vídeo, Zoom) | Quando um usuário clica em uma miniatura diferente para exibir uma imagem diferente. |
| ITEM | **X** (ecatalog) | Nos visualizadores que suportam Mapas de imagem em quais sobreposições são definidas, quando um usuário posiciona o ponteiro sobre um Mapa de imagem para ler o texto de sobreposição. |
| HREF | **X** (ecatalog) | Nos visualizadores que suportam Mapas de imagem, quando um usuário clica em um URL em um Mapa de imagem. |
| TARGET |  | Em visualizadores de zoom direcionados, quando um usuário clica em um destino de zoom para aplicar zoom para parte de uma imagem. |
| SEARCH |  | No ecatalogs, quando um usuário realiza uma pesquisa por palavras. |
| PLAY | **X** (Vídeo) | Nos visualizadores de Vídeo, quando um usuário clica em Reproduzir para iniciar a reprodução de um vídeo.<br><br>**Observação:** Se você estiver usando o relatório de vídeo com base em pulsação do Adobe Analytics, não será necessário mapear variáveis para esse evento do visualizador quando você configurar o Adobe Analytics no Dynamic Media Classic. O Video Heartbeat funciona com visualizadores de vídeo e mixedmedia prontos para Dynamic Media clássica. O player de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo do Adobe Analytics. Consulte [Ativação dos relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| PAUSE | **X** (Vídeo) | Nos visualizadores de Vídeo, quando um usuário clica em Pausar para pausar um vídeo.<br><br>**Observação:** Se você estiver usando o relatório de vídeo com base em pulsação do Adobe Analytics, não será necessário mapear variáveis para esse evento do visualizador quando você configurar o Adobe Analytics no Dynamic Media Classic. O Video Heartbeat funciona com visualizadores de vídeo e mixedmedia prontos para Dynamic Media clássica. O player de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo do Adobe Analytics. Consulte [Ativação dos relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| STOP | **X** (Vídeo) | Nos visualizadores de Vídeo, quando um usuário clica em Parar para parar de reproduzir um vídeo.<br><br>**Observação:** Se você estiver usando o relatório de vídeo com base em pulsação do Adobe Analytics, não será necessário mapear variáveis para esse evento do visualizador quando você configurar o Adobe Analytics no Dynamic Media Classic. O Video Heartbeat funciona com visualizadores de vídeo e mixedmedia prontos para Dynamic Media clássica. O player de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo do Adobe Analytics. Consulte [Ativação dos relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| MILESTONE | **X** (Vídeo) | Nos visualizadores de Vídeo, os eventos de marco são gerados quando o usuário assiste 0, 25, 50, 75 ou 100 % do vídeo.<br><br>**Observação:** Se você estiver usando o relatório de vídeo com base em pulsação do Adobe Analytics, não será necessário mapear variáveis para esse evento do visualizador quando você configurar o Adobe Analytics no Dynamic Media Classic. O Video Heartbeat funciona com visualizadores de vídeo e mixedmedia prontos para Dynamic Media clássica. O player de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo do Adobe Analytics. Consulte [Ativação dos relatórios de vídeo do Adobe Analytics](enabling-analytics-video-reports.md). |
| SWATCH | X (Flyout, Zoom) | Esse evento do visualizador é mapeado para o evento visualizador de página no Sistema de publicação Scene 7. |
| ZOOM | **X** (ecatalog, spinset, Zoom) | Não rastreado pelo Adobe Analytics.<br> |
| PAN | **X** (ecatalog, spinset, Zoom) | Não rastreado pelo Adobe Analytics.<br> |
| SPIN | **X** (spinset) | Não rastreado pelo Adobe Analytics.<br> |


### Variáveis do Dynamic Media Classic {#scene-variables}

Para cada evento do visualizador na tela Configuração do Adobe Analytics, escolha uma variável do Adobe Analytics e uma variável *do Dynamic Media Classic*. As variáveis do Dynamic Media Classic representam os dados que você pode obter para um relatório. Por exemplo, `searchTerm` a variável lista palavras-chave usadas nas pesquisas do ecatalog.

A tabela a seguir descreve as variáveis do Dynamic Media Classic.

| Variável do Dynamic Media Classic | Descrição |
|--- |:--- |
| ativo | ID do ativo do Scene 7 Publishing System ou arquivo de caminho de vídeo. |
| Viewerid | Um número arbitrário atribuído a cada tipo de visualizador diferente. |
| Pagelabel | No ecatalogs, a página que um visualizador exibe. |
| label | O valor do rótulo (uma string). |
| quadro | A página ou referência de página em um conjunto de imagens. |
| rollover_ keyraw | Todo o valor HREF, não apenas qualquer parte processada dele. |
| rollover_ keyproc | A ID de um item referenciado em um Mapa de imagem (válido para eventos href e item). |
| Searchterm | Um termo usado na pesquisa ecatalog. |
| Timestamp | Reproduzir, Parar e Pausar escolhido em visualizadores de vídeo. |
| progress | A porcentagem de um evento de marco concluído. |
| Targetid | O valor da id (um número). |

## Ativação, edição e exclusão de eventos do visualizador {#activating-editing-and-deleting-viewer-events}

Na tela Configuração do Adobe Analytics, você pode ativar, editar e excluir eventos do visualizador:

**Ativar** clique **em Ativar** para ativar ou desativar a desativação de um evento do visualizador selecionado.

**Edição** Selecione um evento do visualizador e clique **no botão Exibir/editar** variáveis. Nas listas suspensas Variável clássica do Dynamic Media e Adobe Analytics, escolha uma variável diferente de cada lista respectiva. Para obter mais informações, consulte Atribuir variáveis do Adobe Analytics aos eventos e variáveis do visualizador do Dynamic Media Classic.

**Excluir** um evento do visualizador e clique em **Exibir/editar** variáveis de exibição de variáveis. Clique **em Excluir**.
