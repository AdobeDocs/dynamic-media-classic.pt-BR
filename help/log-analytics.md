---
title: Faça logon no Adobe Analytics
description: Saiba como fazer logon no Adobe Analytics.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---


# Faça logon no Adobe Analytics{#log-in-to-adobe-analytics}

Antes de fazer logon para configurar relatórios do Adobe Analytics e corresponder as variáveis de relatório do Adobe Analytics aos eventos do Dynamic Media Classic, verifique se você foi adicionado como membro do grupo Acesso ao serviço da Web no Adobe Analytics. Os membros deste grupo podem acessar todos os relatórios nos conjuntos de relatórios especificados por meio da API de serviços da Web do Marketing Cloud, independentemente das permissões definidas na interface. Para adicionar um membro ao grupo, no Adobe Analytics, clique em **Ferramentas administrativas** > **Gerenciamento de usuários** > **Editar grupos**.

Ao fazer logon, você tem a opção de inserir a ID de organização do Marketing Cloud para usar a implementação mais recente da análise de vídeo. Se você optar por não inserir sua ID, o relatórios de vídeo ainda funcionará. No entanto, pode fazer com que os dados não se integrem corretamente com outros dados desse cliente de fora do Dynamic Media Classic.

>[!NOTE]
>
>Se a sua conta Adobe Analytics tiver sido migrada para a autenticação baseada no Adobe IMS (Identity Management System) para logon, a inserção de credenciais diretas não funcionará.

**Para fazer logon no Adobe Analytics**

1. Próximo ao canto superior direito da página do Dynamic Media Classic, toque em **[!UICONTROL Setup > Application Setup]**.
1. No painel esquerdo, em **[!UICONTROL Application Setup]**, toque em **[!UICONTROL Adobe Analytics]**.
1. Na página Configuração do Adobe Analytics, toque em **[!UICONTROL Adobe Analytics Login]**.
1. Na caixa de diálogo **[!UICONTROL Adobe Analytics Login]**, digite o nome da empresa, a ID de organização do Marketing Cloud (opcional), o nome de usuário e a chave *shared secret* no campo de texto **[!UICONTROL Password]**.

   Você pode recuperar a chave *shared secret* do console de administração do Analytics. Consulte [Como obter credenciais de API para contas de usuário](https://helpx.adobe.com/analytics/kb/how-to-get-api-credentials-for-user-accounts-.html).

1. Clique em **[!UICONTROL Login]**.
1. No menu suspenso **[!UICONTROL Report Suite]**, escolha um conjunto de relatórios e clique em **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Na primeira vez que você fizer logon no Adobe Analytics, a lista suspensa Report Suite estará em branco. Você não escolhe um conjunto de relatórios na primeira vez que faz logon. Depois de fazer logon pela primeira vez, faça logout e volte à tela do Adobe Analytics. Faça logon novamente para poder escolher um conjunto de relatórios.

>[!MORELIKETHIS]
>
>* [Configuração de relatórios da Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

