---
title: '" Início rápido: Integração do Dynamic Media Classic e do Adobe Analytics "'
seo-title: '" Início rápido: Integração do Dynamic Media Classic e do Adobe Analytics "'
description: 'null'
seo-description: Uma introdução e uma Introdução rápida à integração do Dynamic Media Classic e do Adobe Analytics para ajudá-lo a começar a usar rapidamente.
uuid: 3 f 9 e 2 c 91-15 d 4-4 b 53-8220-9 b 1 ca 57 c 0 b 1 d
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/adobe_ analytics_ instrumentation_ kit
discoiquuid: abec 9 a 85-013 c -4030-b 129-bf 27 a 89 cb 464
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Início rápido: Integração do Dynamic Media Classic e do Adobe Analytics {#quick-start-integrating-scene-and-adobe-analytics}

O Adobe Analytics é o produto líder do setor que fornece aos profissionais de marketing um local onde eles podem medir, analisar e otimizar dados integrados de todas as iniciativas online em vários canais de marketing.

Depois de integrar o Adobe Analytics com o Sistema de publicação Scene 7, você pode obter relatórios sobre o comportamento dos visitantes do site usando visualizadores do Dynamic Media Classic em seu site. Por exemplo, quando um visitante do site clica em um destino de zoom em um Visualizador de zoom clássico do Media Media, o Adobe Analytics registra essa ação. Os relatórios do Adobe Analytics podem coletar informações cumulativas sobre a atividade do usuário nos visualizadores do Dynamic Media Classic.

Com os relatórios do Adobe Analytics, você pode obter uma imagem clara da atividade dos clientes em seu site. Você pode determinar quais apresentações de produto levam à conversão e que não desenham os interesses do cliente.

Consulte [também Medição de vídeo no Adobe Analytics](https://marketing.adobe.com/resources/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Uma conta válida do Adobe Analytics é necessária para integrar o Analytics com o Sistema de publicação Scene 7 e gerar relatórios do Analytics.

**Início rápido**

Este Início rápido foi projetado para agilizar o processo com o Kit de instrumentação do Adobe Analytics.

**1. Faça logon no Adobe Analytics por meio do Dynamic Media Classic e baixe as variáveis de relatório do Adobe Analytics**

>[!NOTE]
>
>Antes de configurar os relatórios do Adobe Analytics e corresponder as variáveis de relatório do Adobe Analytics aos eventos clássicos de Dynamic Media, verifique se você foi adicionado como membro do grupo Acesso ao serviço da Web no Adobe Analytics. Os membros deste grupo podem acessar todos os relatórios nos conjuntos de relatórios especificados por meio da API de serviços da Web da Marketing Cloud, independentemente das permissões definidas na interface. Para adicionar um membro ao grupo, no Adobe Analytics, clique em Ferramentas **administrativas** &gt; **Gerenciamento de usuários** &gt; **Editar grupos**.

Depois de verificar se você é membro do grupo Acesso ao serviço da Web, no Dynamic Media Classic, clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Adobe Analytics**. Na página Configuração do Adobe Analytics, clique **em Logon do Adobe Analytics**.

Consulte [Logon no Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Na caixa de diálogo Logon do Adobe Analytics, digite a ID organizacional da Marketing Cloud (opcional) e suas credenciais completas, em seguida, clique **em Logon**. No menu suspenso Conjunto de relatórios, selecione o nome do conjunto de relatórios que deseja usar.

**2. Atribuir variáveis de relatório do Adobe Analytics aos eventos do visualizador do Dynamic Media Classic e variáveis do Dynamic Media Classic**

Na página Configuração do Adobe Analytics, especifique as informações desejadas nos relatórios do Adobe Analytics. Para cada evento do visualizador do Dynamic Media Classic que você deseja obter informações, escolha uma variável do Adobe Analytics (de seu conjunto de relatórios) e uma variável do Dynamic Media Classic.

* Os eventos do visualizador descrevem a atividade do usuário que você deseja avaliar nos relatórios.
* As variáveis do Dynamic Media Classic descrevem os dados sobre os eventos de usuário que você deseja que os relatórios forneçam.

A Configuração do Adobe Analytics também oferece ferramentas para ativar, editar e excluir eventos do visualizador.

Depois de clicar em Salvar na tela Configuração do Adobe Analytics, o código de rastreamento personalizado para medir a atividade do usuário será inserido nos visualizadores do Dynamic Media Classic. Essa funcionalidade permite rastrear a atividade do usuário nos relatórios do Adobe Analytics.

Consulte [Configuração dos relatórios do Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

**3. Publicar os visualizadores do Dynamic Media Classic**

Publique os visualizadores do Dynamic Media Classic para que os visualizadores (com código para rastrear a atividade do usuário nos relatórios do Adobe Analytics) sejam carregados nos servidores do Dynamic Media Classic. Depois de publicar, essas informações serão incluídas nos visualizadores e poderão ser usadas para análises pelo Adobe Analytics.

Consulte [Publicar informações](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)de configuração.

**4. Colocar visualizadores do Dynamic Media Classic em seu site**

Coloque os visualizadores do Dynamic Media Classic com o código de rastreamento do Adobe Analytics em seu site.

**5. Teste a integração do Adobe Analytics visualizando um relatório do Adobe Analytics**

Para exibir os relatórios do Adobe Analytics, acesse o site do Adobe Analytics. A página Relatório permite exibir dados e gerar gráficos e gráficos para medir a atividade do usuário com visualizadores diferentes.

Consulte [Teste da integração do Adobe Analytics visualizando um relatório do Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
