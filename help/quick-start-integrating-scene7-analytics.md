---
title: '"Start rápido: Integração do Dynamic Media Classic e do Adobe Analytics "'
seo-title: '"Start rápido: Integração do Dynamic Media Classic e do Adobe Analytics "'
description: nulo
seo-description: Uma introdução e um Start rápido para integrar o Dynamic Media Classic e o Adobe Analytics para ajudá-lo a começar a funcionar rapidamente.
uuid: 3f9e2c91-15d4-4b53-8220-9b1ca57c0b1d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: abec9a85-013c-4030-b129-bf27a89cb464
translation-type: tm+mt
source-git-commit: 2fb7e34b734dba1e0bd1d150580d7d6c74ee1b79
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 0%

---


# Start rápido: Integração do Dynamic Media Classic e do Adobe Analytics {#quick-start-integrating-scene-and-adobe-analytics}

O Adobe Analytics é o produto líder do setor que fornece aos profissionais de marketing um local onde eles podem medir, analisar e otimizar dados integrados de todas as iniciativas online em vários canais de marketing.

Depois de integrar o Adobe Analytics ao Scene7 Publishing System, você pode obter relatórios sobre o comportamento dos visitantes do site usando visualizadores do Dynamic Media Classic em seu site. Por exemplo, quando um visitante de site clica em um público alvo de zoom em um visualizador de zoom do Dynamic Media Classic, o Adobe Analytics registra essa ação. Os relatórios do Adobe Analytics podem coletar informações cumulativas sobre a atividade do usuário nos visualizadores do Dynamic Media Classic.

Usando os relatórios da Adobe Analytics, você pode obter uma imagem clara da atividade de clientes em seu site. Você pode determinar quais apresentações de produtos levam à conversão e quais não atraem o interesse do cliente.

Consulte também [Avaliação de vídeo no Adobe Analytics](https://docs.adobe.com/content/help/en/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Uma conta válida do Adobe Analytics é necessária para integrar o Analytics ao Scene7 Publishing System e gerar relatórios do Analytics.

**Start rápido**

Este Start rápido foi projetado para colocar você em operação rapidamente com o Adobe Analytics Instrumentation Kit.

**1. Faça logon no Adobe Analytics por meio do Dynamic Media Classic e baixe as variáveis de relatório do Adobe Analytics**

>[!NOTE]
>
>Antes de configurar os relatórios do Adobe Analytics e corresponder as variáveis de relatório do Adobe Analytics aos eventos do Dynamic Media Classic, verifique se você foi adicionado como membro do grupo Acesso ao serviço da Web no Adobe Analytics. Os membros deste grupo podem acessar todos os relatórios nos conjuntos de relatórios especificados por meio da API de serviços da Web da Marketing Cloud, independentemente das permissões definidas na interface. Para adicionar um membro ao grupo, no Adobe Analytics, clique em **Ferramentas** administrativas > Gerenciamento **** do usuário > **Editar grupos**.

Depois de verificar se você é membro do grupo Acesso ao serviço da Web, no Dynamic Media Classic, clique em **Configuração** > Configuração **** do aplicativo > **Adobe Analytics**. Na página Configuração do Adobe Analytics, clique em Logon **do** Adobe Analytics.

Consulte [Fazer logon no Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Na caixa de diálogo Logon do Adobe Analytics, digite a ID de empresa da Marketing Cloud (opcional) e as credenciais completas, em seguida, clique em **Logon**. No menu suspenso Conjunto de relatórios, selecione o nome do conjunto de relatórios que deseja usar.

**2. Atribuir variáveis de relatório do Adobe Analytics a eventos do visualizador Dynamic Media Classic e variáveis do Dynamic Media Classic**

Na página Configuração do Adobe Analytics, especifique as informações desejadas nos relatórios do Adobe Analytics. Para cada evento do visualizador do Dynamic Media Classic sobre o qual você deseja obter informações, escolha uma variável do Adobe Analytics (do conjunto de relatórios) e uma variável do Dynamic Media Classic.

* Os eventos do visualizador descrevem a atividade do usuário que você deseja medir nos relatórios.
* As variáveis do Dynamic Media Classic descrevem os dados sobre eventos de usuário que você deseja que os relatórios forneçam.

A Configuração do Adobe Analytics também oferta ferramentas para ativar, editar e excluir eventos do visualizador.

Após clicar em Salvar na tela Configuração do Adobe Analytics, o código de rastreamento personalizado para medir a atividade do usuário é inserido nos visualizadores do Dynamic Media Classic. Essa funcionalidade permite rastrear a atividade do usuário nos relatórios do Adobe Analytics.

Consulte [Configuração de relatórios](configuring-analytics-reports.md#configuring_adobe_analytics_reports)do Adobe Analytics.

**3. Publicar seus visualizadores do Dynamic Media Classic**

Publique os visualizadores do Dynamic Media Classic para que os visualizadores (com código para rastrear a atividade do usuário nos relatórios do Adobe Analytics) sejam carregados nos servidores Dynamic Media Classic. Após a publicação, essas informações são incluídas nos visualizadores e podem ser usadas para análises pela Adobe Analytics.

Consulte [Publicação de informações](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)de configuração.

**4. Colocar visualizadores do Dynamic Media Classic em seu site**

Coloque os visualizadores do Dynamic Media Classic com o código de rastreamento do Adobe Analytics em seu site.

**5. Teste a integração do Adobe Analytics exibindo um relatório da Adobe Analytics**

Para visualização dos relatórios do Adobe Analytics, acesse o site da Adobe Analytics. A página Relatórios permite que você visualização dados e gere gráficos e gráficos para medir a atividade do usuário com visualizadores diferentes.

Consulte [Testar a integração do Adobe Analytics exibindo um relatório](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)do Adobe Analytics.
