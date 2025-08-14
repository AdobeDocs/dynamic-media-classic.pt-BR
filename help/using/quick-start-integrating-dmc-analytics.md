---
title: 'Início rápido: integrar o Adobe Dynamic Media Classic e o Adobe Analytics'
description: Uma introdução e um Início rápido sobre como integrar o Adobe Dynamic Media Classic e o Adobe Analytics.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Início rápido: integrar o Adobe Dynamic Media Classic e o Adobe Analytics {#quick-start-integrating-dmc-analytics}

O Adobe Analytics é o produto líder do setor e fornece aos profissionais de marketing um local onde eles podem medir, analisar e otimizar dados integrados de todas as iniciativas online em vários canais de marketing.

Depois de integrar o Adobe Analytics com o Adobe Dynamic Media Classic, você pode obter relatórios sobre o comportamento dos visitantes do site usando visualizadores do Adobe Dynamic Media Classic em seu site. Por exemplo, quando um visitante do site seleciona um destino de zoom em um Visualizador de zoom do Adobe Dynamic Media Classic, o Adobe Analytics registra essa ação. Os relatórios do Adobe Analytics podem coletar informações cumulativas sobre a atividade do usuário em visualizadores do Adobe Dynamic Media Classic.

Usando os relatórios do Adobe Analytics, você pode obter uma visão clara da atividade dos clientes em seu site. É possível determinar quais apresentações de produto levam à conversão e quais não atraem o interesse do cliente.

Consulte também [Medir vídeo no Adobe Analytics](https://experienceleague.adobe.com/pt-br/docs/media-analytics/using/media-overview).

>[!NOTE]
>
>É necessária uma conta válida do Adobe Analytics para integrar o Analytics ao Adobe Dynamic Media Classic e gerar relatórios do Analytics.

Esse Quick Start foi projetado para colocar suas operações em funcionamento rapidamente com o Adobe Analytics Instrumentation Kit.

## &#x200B;1. Faça logon no Adobe Analytics por meio do Adobe Dynamic Media Classic e baixe as variáveis de relatório do Adobe Analytics

>[!NOTE]
>
>Verifique se você foi adicionado como membro do grupo de Acesso ao serviço da Web no Adobe Analytics. Faça essa verificação antes de configurar os relatórios do Adobe Analytics. E antes de vincular as variáveis de relatório do Adobe Analytics aos eventos do Adobe Dynamic Media Classic. Os membros deste grupo podem acessar todos os relatórios nos conjuntos de relatórios especificados. Você pode fazer isso usando a API de serviços da Web do Experience Cloud, independentemente das permissões definidas na interface. Para adicionar um membro ao grupo, no Adobe Analytics, vá para **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]**.

Depois de verificar que você é membro do grupo de Acesso ao Serviço Web, no Adobe Dynamic Media Classic, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Adobe Analytics]**. Na página Configuração do Adobe Analytics, selecione **[!UICONTROL Adobe Analytics Login]**.

Consulte [Fazer logon no Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Na caixa de diálogo Logon do Adobe Analytics, digite sua ID da Organização do Experience Cloud (opcional) e suas credenciais completas e, em seguida, selecione **[!UICONTROL Login]**. No menu suspenso Conjunto de relatórios, selecione o nome do conjunto de relatórios que deseja usar.

## &#x200B;2. Atribuir variáveis de relatório do Adobe Analytics a eventos do visualizador do Adobe Dynamic Media Classic e variáveis do Adobe Dynamic Media Classic

Na página Configuração do Adobe Analytics, especifique as informações desejadas nos relatórios do Adobe Analytics. Para cada evento do visualizador do Adobe Dynamic Media Classic sobre o qual você deseja obter informações, escolha uma variável do Adobe Analytics (no conjunto de relatórios) e uma variável do Adobe Dynamic Media Classic.

* Os eventos do visualizador descrevem a atividade do usuário que você deseja medir nos relatórios.
* As variáveis do Adobe Dynamic Media Classic descrevem os dados sobre eventos de usuário que você deseja que os relatórios forneçam.

A Configuração do Adobe Analytics também oferece ferramentas para ativar, editar e excluir eventos do visualizador.

Depois de selecionar **[!UICONTROL Save]** na página Configuração do Adobe Analytics, um código de rastreamento personalizado para medir a atividade do usuário é inserido nos visualizadores do Adobe Dynamic Media Classic. Essa funcionalidade permite rastrear a atividade do usuário nos relatórios do Adobe Analytics.

Consulte [Configurar relatórios do Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## &#x200B;3. Publicar seus visualizadores do Adobe Dynamic Media Classic

Publique seus visualizadores do Adobe Dynamic Media Classic para que os visualizadores (com código para rastrear a atividade do usuário nos relatórios do Adobe Analytics) sejam carregados nos servidores da Adobe Dynamic Media Classic. Após a publicação, essas informações são incluídas nos visualizadores. Use-o para análise pelo Adobe Analytics.

Consulte [Publicar informações de configuração](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## &#x200B;4. Coloque visualizadores do Adobe Dynamic Media Classic em seu site

Coloque os visualizadores do Adobe Dynamic Media Classic com o código de rastreamento do Adobe Analytics em seu site.

## &#x200B;5. Teste a integração do Adobe Analytics visualizando um relatório do Adobe Analytics

Para exibir os relatórios do Adobe Analytics, vá para o site da Adobe Analytics. A página Geração de relatórios permite exibir dados e gerar gráficos para medir a atividade do usuário com visualizadores diferentes.

Consulte [Testar a integração do Adobe Analytics exibindo um relatório do Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
