---
title: Fazer logon no Adobe Analytics
description: Saiba como fazer logon no Adobe Analytics a partir do Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
topic: Integrations, Development
level: Experienced
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Fazer logon no Adobe Analytics{#log-in-to-adobe-analytics}

Antes de fazer logon para configurar relatórios do Adobe Analytics e corresponder variáveis de relatório do Adobe Analytics a eventos do Adobe Dynamic Media Classic, verifique se você é membro do grupo de Acesso ao serviço da Web no Adobe Analytics. Os membros deste grupo podem acessar todos os relatórios nos conjuntos de relatórios especificados por meio da API de serviços da Web do Experience Cloud, independentemente das permissões definidas na interface. Para adicionar um membro ao grupo, no Adobe Analytics, vá para **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]**.

Ao fazer logon, você tem a opção de inserir a ID da organização do Experience Cloud para usar a implementação de análise de vídeo mais recente. Se você optar por não inserir sua ID, o relatório de vídeo ainda funcionará. No entanto, isso pode fazer com que os dados não se integrem corretamente com outros dados para esse cliente de fora do Adobe Dynamic Media Classic.

>[!NOTE]
>
>Se sua conta do Adobe Analytics tiver sido migrada para a autenticação baseada no Adobe IMS (Identity Management System) para logon, inserir credenciais diretas não funcionará.

## Fazer logon no Adobe Analytics a partir do Adobe Dynamic Media Classic {#log-in-to-analytics-from-dmc}

Comece integrando o Dynamic Media Classic com o Adobe Analytics OAuth. Normalmente, a integração do Adobe Analytics OAuth com o Dynamic Media Classic é feita apenas uma vez por usuário.

1. Access [Console do Adobe Developer](https://developer.adobe.com/console). Verifique se sua conta tem permissões de administrador para a organização para a qual a integração é necessária.
1. Próximo ao canto superior direito da Home page, na lista suspensa, selecione a empresa apropriada. (A captura de tela abaixo é apenas para fins de informação; o nome real da empresa que você selecionar pode variar.)

   ![Criar um novo projeto](assets/analytics-oauth1.png)

1. Siga um destes procedimentos:

   * Na parte superior da página, no **[!UICONTROL Home]** selecione **[!UICONTROL Create new project]**.
   * Na parte superior da página, no **[!UICONTROL Projects]** guia. Próximo ao canto direito da página, selecione **[!UICONTROL Create new project]**.

1. Na página do projeto, selecione **[!UICONTROL Add API]**.
1. No **[!UICONTROL Add an API]** selecione **[!UICONTROL Adobe Analytics]**.
1. Próximo ao canto inferior direito da página, selecione **[!UICONTROL Next]**.

   ![Adicionar uma API](assets/analytics-oauth2.png)

1. No **[!UICONTROL Configure API]** selecione **[!UICONTROL USER AUTHENTICATION OAuth]**.
1. Próximo ao canto inferior direito da página, selecione **[!UICONTROL Next]**.
1. No **[!UICONTROL Configure API]** selecione **[!UICONTROL OAUTH 2.0 Web]**.
1. No **[!UICONTROL Default redirect URI]** digite o seguinte caminho exatamente como mostrado:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. No **[!UICONTROL Redirect URI pattern]** digite o seguinte caminho exatamente como mostrado:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. No canto inferior direito da página, selecione **[!UICONTROL Save configured API]**.
1. No painel de navegação, no lado esquerdo da página do Adobe Analytics, em **[!UICONTROL Credentials]**, selecione **[!UICONTROL OAuth Web]**.
1. Em **[!UICONTROL Credential details]**, faça o seguinte:
   * Em **[!UICONTROL Client ID]**, selecione **[!UICONTROL Copy]** para copiar o valor. Esse valor é necessário para a configuração subsequente do Analytics no aplicativo de desktop do Dynamic Media Classic que será seguido.
   * Em **[!UICONTROL Client Secret]**, selecione **[!UICONTROL Retrieve client secret]** para revelar o valor associado. Selecionar **[!UICONTROL Copy]** para copiar o valor. Esse valor é necessário para a configuração subsequente do Adobe Analytics no aplicativo de desktop do Dynamic Media Classic que será seguido.

## Configurar o Adobe Analytics no Adobe Dynamic Media Classic {#configure-analytics-in-dmc}

>[!NOTE]
>
>Após a configuração inicial do Adobe Analytics no Dynamic Media Classic, a única vez que você deve refazer a configuração é nos seguintes casos:
>
>* Um novo relatório é adicionado no Analytics e o usuário deseja começar a enviar dados para esse novo relatório.
>* O servidor de rastreamento é atualizado no Adobe Analytics.
>* Uma nova variável de rastreamento é introduzida em um relatório e você deseja vincular uma variável específica do Visualizador na interface do Dynamic Media Classic a essa nova variável do Analytics.
>

1. Próximo ao canto superior direito do aplicativo de desktop Adobe Dynamic Media Classic, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**.
1. No painel esquerdo, em **[!UICONTROL Application Setup]**, selecione **[!UICONTROL Adobe Analytics]**.
1. No **[!UICONTROL Adobe Analytics Configuration]** selecione **[!UICONTROL Adobe Analytics Login]**.
1. No **[!UICONTROL Adobe Analytics Login]** caixa de diálogo, no campo **[!UICONTROL CLIENT ID]** e o campo **[!UICONTROL CLIENT SECRET]** cole os respectivos valores que você copiou anteriormente.
1. No canto inferior direito da caixa de diálogo, selecione **[!UICONTROL Login]** e faça logon no Adobe IMS (Identity Management Services).

   Ao fazer logon com êxito, a caixa de diálogo Logon do Adobe Analytics será exibida novamente junto com a tag **[!UICONTROL COMPANIES]** lista suspensa, iniciada pelas empresas que estão disponíveis para você.

1. No **[!UICONTROL COMPANIES]** selecione uma empresa.

   Depois de selecionar uma empresa, a variável **[!UICONTROL SUITES]** A lista suspensa, iniciada pelos Conjuntos de relatórios disponíveis para a empresa selecionada, fica visível.

1. No **[!UICONTROL SUITES]** escolha um conjunto de relatórios.

   >[!NOTE]
   >
   >Por padrão, o usuário deve estar ciente de que ambos **[!UICONTROL COMPANIES]** e **[!UICONTROL SUITES]** as listas suspensas estão vazias. Dessa forma, o usuário deve selecionar um valor em cada lista.

1. Selecionar **[!UICONTROL OK]** para poder salvar a configuração.

   >[!NOTE]
   >
   >A variável **[!UICONTROL Adobe Analytics Server]** o campo é preenchido com um servidor de rastreamento de terceiros sugerido que corresponde ao namespace do analytics quando você seleciona **[!UICONTROL OK]**. Se você usar um servidor de rastreamento diferente, atualize-o neste campo para evitar perda de dados.

1. No canto inferior esquerdo da página Configuração do Adobe Analytics, selecione **[!UICONTROL Save]** para garantir que a configuração da sua conta do Adobe Analytics seja atualizada.

>[!MORELIKETHIS]
>
>* [Configurar relatórios do Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
