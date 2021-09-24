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
source-git-commit: d18dbbf89a1bfe4df46cbe7d56cdf6f442595ddb
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Faça logon no Adobe Analytics{#log-in-to-adobe-analytics}

Antes de fazer logon para configurar relatórios do Adobe Analytics e corresponder as variáveis de relatório do Adobe Analytics aos eventos do Adobe Dynamic Media Classic, verifique se você é membro do grupo Acesso ao serviço da Web no Adobe Analytics. Os membros deste grupo podem acessar todos os relatórios nos conjuntos de relatórios especificados por meio da API de serviços da Web do Experience Cloud, independentemente das permissões definidas na interface. Para adicionar um membro ao grupo, no Adobe Analytics, vá para **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]**.

Ao fazer logon, você tem a opção de inserir a ID de organização do Experience Cloud para usar a implementação de análise de vídeo mais recente. Se você optar por não inserir sua ID, o relatório de vídeo ainda funcionará. No entanto, pode fazer com que os dados não sejam integrados corretamente com outros dados para esse cliente de fora do Adobe Dynamic Media Classic.

>[!NOTE]
>
>Se sua conta do Adobe Analytics tiver sido migrada para a autenticação baseada no Adobe IMS (Identity Management System) para logon, a inserção de credenciais diretas não funcionará.

**Para fazer logon no Adobe Analytics a partir do Adobe Dynamic Media Classic:**

Comece integrando o Dynamic Media Classic ao Adobe Analytics OAuth. A integração do Adobe Analytics OAuth com o Dynamic Media Classic geralmente é feita apenas uma vez por usuário.

1. Acesse [Console do Desenvolvedor do Adobe](https://developer.adobe.com/console). Certifique-se de que sua conta tenha permissões de administrador para a organização para a qual a integração é necessária.
1. Próximo ao canto superior direito da Página inicial, na lista suspensa, selecione a empresa apropriada. (A captura de tela abaixo é apenas para fins informativos; o nome real da empresa selecionado pode variar.)

   ![Criar um novo projeto](assets/analytics-oauth1.png)

1. Siga um destes procedimentos:

   * Na parte superior da página, na guia **[!UICONTROL Home]**, selecione **[!UICONTROL Create new project]**.
   * Na parte superior da página, na guia **[!UICONTROL Projects]** . Próximo ao canto direito da página, selecione **[!UICONTROL Create new project]**.

1. Na página do projeto, selecione **[!UICONTROL Add API]**.
1. Na página **[!UICONTROL Add an API]**, selecione **[!UICONTROL Adobe Analytics]**.
1. Próximo ao canto inferior direito da página, selecione **[!UICONTROL Next]**.

   ![Adicionar uma API](assets/analytics-oauth2.png)

1. Na página **[!UICONTROL Configure API]**, selecione **[!UICONTROL USER AUTHENTICATION OAuth]**.
1. Próximo ao canto inferior direito da página, selecione **[!UICONTROL Next]**.
1. Na página **[!UICONTROL Configure API]**, selecione **[!UICONTROL OAUTH 2.0 Web]**.
1. No campo de texto **[!UICONTROL Default redirect URI]**, insira o seguinte caminho exatamente como mostrado:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. No campo de texto **[!UICONTROL Redirect URI pattern]**, insira o seguinte caminho exatamente como mostrado:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. No canto inferior direito da página, selecione **[!UICONTROL Save configured API]**.
1. No painel de navegação, no lado esquerdo da página do Adobe Analytics, em **[!UICONTROL Credentials]**, selecione **[!UICONTROL OAuth Web]**.
1. Em **[!UICONTROL Credential details]**, faça o seguinte:
   * Em **[!UICONTROL Client ID]**, selecione **[!UICONTROL Copy]** para copiar o valor. Você precisa desse valor para a configuração subsequente do Analytics no aplicativo de desktop do Dynamic Media Classic que deve ser seguida.
   * Em **[!UICONTROL Client Secret]**, selecione **[!UICONTROL Retrieve client secret]** para revelar o valor associado. Selecione **[!UICONTROL Copy]** para copiar o valor. Você precisa desse valor para a configuração subsequente do Adobe Analytics no aplicativo de desktop Dynamic Media Classic que deve ser seguida.

**Configurar o Adobe Analytics no aplicativo de desktop Dynamic Media Classic**

>[!NOTE]
>
>Após a configuração inicial do Adobe Analytics no Dynamic Media Classic, as únicas vezes que você deve refazer a configuração são os seguintes casos:
>
>* Um novo relatório é adicionado ao Analytics e o usuário deseja começar a enviar dados para esse novo relatório.
>* O servidor de rastreamento é atualizado no Adobe Analytics.
>* Uma nova variável de rastreamento é introduzida em um relatório e você deseja vincular uma variável de Visualizador específica na interface do usuário do Dynamic Media Classic a essa nova variável do Analytics.

>


1. Próximo ao canto superior direito do aplicativo de desktop Adobe Dynamic Media Classic, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**.
1. No painel esquerdo, em **[!UICONTROL Application Setup]**, selecione **[!UICONTROL Adobe Analytics]**.
1. Na página **[!UICONTROL Adobe Analytics Configuration]**, selecione **[!UICONTROL Adobe Analytics Login]**.
1. Na caixa de diálogo **[!UICONTROL Adobe Analytics Login]**, no campo ID do cliente e no campo Segredo do cliente , cole os respectivos valores que você copiou anteriormente.
1. Faça logon do IMS.

   Quando você está conectado com êxito, a lista suspensa **[!UICONTROL COMPANIES]**, iniciada pelas empresas disponíveis para você, fica visível.

1. Na lista suspensa **[!UICONTROL COMPANIES]**, escolha uma empresa.

   Após selecionar uma empresa, a lista suspensa **[!UICONTROL SUITES]**, iniciada pelos Conjuntos de relatórios disponíveis para a empresa selecionada, torna-se visível.

1. Na lista suspensa **[!UICONTROL SUITES]**, escolha um conjunto de relatórios.

   >[!NOTE]
   >
   >Por padrão, o usuário deve estar ciente do fato de que as listas suspensas **[!UICONTROL COMPANIES]** e **[!UICONTROL SUITES]** estão vazias. Dessa forma, o usuário deve selecionar um valor em cada lista. —>

1. Selecione **[!UICONTROL OK]** para salvar a configuração.

>[!MORELIKETHIS]
>
>* [Configurar relatórios do Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

