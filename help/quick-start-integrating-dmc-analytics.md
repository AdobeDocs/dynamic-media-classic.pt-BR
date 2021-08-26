---
title: '"Início rápido: Integração do Adobe Dynamic Media Classic e Adobe Analytics"'
description: Uma introdução e o Início rápido para integrar o Adobe Dynamic Media Classic e o Adobe Analytics, para ajudá-lo a ativar e executar rapidamente.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Início rápido: Integração do Adobe Dynamic Media Classic e Adobe Analytics {#quick-start-integrating-dmc-analytics}

O Adobe Analytics é o produto líder do setor que fornece aos profissionais de marketing um único local onde podem medir, analisar e otimizar dados integrados de todas as iniciativas online em vários canais de marketing.

Após integrar o Adobe Analytics com o Adobe Dynamic Media Classic, você pode obter relatórios sobre o comportamento dos visitantes do site usando visualizadores Adobe Dynamic Media Classic em seu site da Web. Por exemplo, quando um visitante de um site clica em um direcionamento de zoom em um Visualizador de zoom do Adobe Dynamic Media Classic, o Adobe Analytics registra essa ação. Os relatórios do Adobe Analytics podem coletar informações cumulativas sobre a atividade do usuário nos visualizadores do Adobe Dynamic Media Classic.

Com os relatórios do Adobe Analytics, você pode obter uma imagem clara da atividade dos clientes no seu site. Você pode determinar quais apresentações de produtos levam à conversão e quais não atraem o interesse do cliente.

Consulte também [Medição de vídeo no Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

>[!NOTE]
>
>É necessária uma conta válida do Adobe Analytics para integrar o Analytics com o Adobe Dynamic Media Classic e gerar relatórios do Analytics.

Este Início Rápido foi projetado para ajudá-lo a ativar e executar rapidamente com o Kit de Instrumentação do Adobe Analytics.

## 1. Faça logon no Adobe Analytics por meio do Adobe Dynamic Media Classic e baixe as variáveis de relatório do Adobe Analytics

>[!NOTE]
>
>Antes de configurar os relatórios do Adobe Analytics e corresponder as variáveis de relatório do Adobe Analytics aos eventos do Adobe Dynamic Media Classic, verifique se você foi adicionado como membro do grupo Acesso ao serviço da Web no Adobe Analytics. Os membros deste grupo podem acessar todos os relatórios nos conjuntos de relatórios especificados por meio da API de Serviços da Web do Marketing Cloud, independentemente das permissões definidas na interface. Para adicionar um membro ao grupo, no Adobe Analytics, clique em **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]**.

Depois de verificar que você é membro do grupo Acesso ao serviço da Web, no Adobe Dynamic Media Classic, clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Adobe Analytics]**. Na página Configuração do Adobe Analytics , clique em **[!UICONTROL Adobe Analytics Login]**.

Consulte [Fazer logon no Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Na caixa de diálogo Logon do Adobe Analytics, digite a ID da organização do Marketing Cloud (opcional) e as credenciais completas, em seguida, clique em **[!UICONTROL Login]**. No menu suspenso Conjunto de relatórios , selecione o nome do conjunto de relatórios que deseja usar.

## 2. Atribua variáveis de relatório do Adobe Analytics aos eventos do visualizador do Adobe Dynamic Media Classic e às variáveis do Adobe Dynamic Media Classic

Na página Configuração do Adobe Analytics , especifique as informações desejadas nos relatórios do Adobe Analytics . Para cada Adobe do visualizador do Dynamic Media Classic sobre o qual você deseja obter informações, escolha uma variável do Adobe Analytics (no conjunto de relatórios) e uma variável do Adobe Dynamic Media Classic.

* Os eventos do visualizador descrevem a atividade do usuário que você deseja medir nos relatórios.
* As variáveis do Adobe Dynamic Media Classic descrevem os dados sobre os eventos do usuário que você deseja que os relatórios entreguem.

A Configuração do Adobe Analytics também oferece ferramentas para ativar, editar e excluir eventos do visualizador.

Depois de clicar em **[!UICONTROL Save]** na página Configuração do Adobe Analytics, o código de rastreamento personalizado para medir a atividade do usuário é inserido nos visualizadores do Adobe Dynamic Media Classic. Essa funcionalidade permite rastrear a atividade do usuário nos relatórios do Adobe Analytics.

Consulte [Configuração de relatórios Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Publicar seus visualizadores Adobe Dynamic Media Classic

Publique seus visualizadores Adobe Dynamic Media Classic para que os visualizadores (com código para rastrear a atividade do usuário em relatórios do Adobe Analytics) sejam carregados nos servidores Adobe Dynamic Media Classic. Após a publicação, essas informações são incluídas nos visualizadores e podem ser usadas para análises pelo Adobe Analytics.

Consulte [Informações de configuração de publicação](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Coloque os visualizadores do Adobe Dynamic Media Classic no seu site

Coloque os visualizadores do Adobe Dynamic Media Classic com o código de rastreamento do Adobe Analytics no seu site.

## 5. Teste a integração do Adobe Analytics exibindo um relatório do Adobe Analytics

Para exibir relatórios do Adobe Analytics, vá para o site do Adobe Analytics. A página Relatório permite que você visualize dados e gere gráficos e tabelas para medir a atividade do usuário com visualizadores diferentes.

Consulte [Testar a integração do Adobe Analytics exibindo um relatório do Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
