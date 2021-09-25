---
title: Faça logon no Adobe Analytics
description: Saiba como fazer logon no Adobe Analytics pelo Adobe Dynamic Media Classic.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: e3c2dcaa245e486ada62edd554db5a39d495483e
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Faça logon no Adobe Analytics{#log-in-to-adobe-analytics}

Antes de fazer logon para configurar relatórios do Adobe Analytics e corresponder as variáveis de relatório do Adobe Analytics aos eventos do Adobe Dynamic Media Classic, verifique se você é membro do grupo Acesso ao serviço da Web no Adobe Analytics. Os membros deste grupo podem acessar todos os relatórios nos conjuntos de relatórios especificados por meio da API de serviços da Web do Experience Cloud, independentemente das permissões definidas na interface. Para adicionar um membro ao grupo, no Adobe Analytics, vá para **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]**.

Ao fazer logon, você tem a opção de inserir a ID de organização do Experience Cloud para usar a implementação de análise de vídeo mais recente. Se você optar por não inserir sua ID, o relatório de vídeo ainda funcionará. No entanto, pode fazer com que os dados não sejam integrados corretamente com outros dados para esse cliente de fora do Adobe Dynamic Media Classic.

>[!NOTE]
>
>Se sua conta do Adobe Analytics tiver sido migrada para a autenticação baseada no Adobe IMS (Identity Management System) para logon, a inserção de credenciais diretas não funcionará.

**Para fazer logon no Adobe Analytics:**

1. Próximo ao canto superior direito da página do Adobe Dynamic Media Classic, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**.
1. No painel esquerdo, em **[!UICONTROL Application Setup]**, toque em **[!UICONTROL Adobe Analytics]**.
1. Na página Configuração do Adobe Analytics , toque em **[!UICONTROL Adobe Analytics Login]**.
1. Na caixa de diálogo **[!UICONTROL Adobe Analytics Login]**, digite o nome da empresa, a ID de organização do Experience Cloud (opcional), o nome de usuário e a chave *segredo compartilhado* no campo de texto **[!UICONTROL Password]**.

   Você pode recuperar a chave *shared secret* do Admin Console do Analytics. Consulte [Como obter credenciais de API para contas de usuário](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md).

1. Selecione **[!UICONTROL Login]**.
1. No menu suspenso **[!UICONTROL Report Suite]**, escolha um conjunto de relatórios e selecione **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Na primeira vez que você faz logon no Adobe Analytics, a lista suspensa Conjunto de relatórios fica em branco. Você não escolhe um conjunto de relatórios na primeira vez que faz logon. Depois de fazer logon pela primeira vez, faça logoff e retorne à tela Adobe Analytics. Faça logon novamente para poder escolher um conjunto de relatórios.

>[!MORELIKETHIS]
>
>* [Configurar relatórios do Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

