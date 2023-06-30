---
title: Integrar o Adobe Dynamic Media Classic com o Adobe Target Standard/Premium
description: Saiba como integrar o Adobe Dynamic Media Classic ao Adobe Target Standard/Premium.
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# Integrar o Adobe Dynamic Media Classic com o Adobe Target Standard/Premium {#integrating-dmc-with-target}

Antes de integrar [!DNL Adobe Dynamic Media Classic] com [!DNL Target Standard/Premium], você deve inserir seu URL do Target no [!DNL Adobe Dynamic Media Classic] tela Configurações gerais do aplicativo. Para obter o URL do Target e inseri-lo na página Configurações Gerais da Aplicação, faça o seguinte:

1. Entrada [!DNL Adobe Experience Cloud], faça logon no [!DNL Target Standard/Premium] conta.
1. Depois de fazer logon, na barra de endereços do navegador, copie o URL para e incluindo `.com`.

   Por exemplo, se a variável *ficcional* O URL (caminhos de URLs sempre contêm barras, não barras invertidas, como neste exemplo) na barra de endereços é `https:\\www.myfictionalsite.com/categories/admin/home.do`, copie somente esta parte do *ficcional* URL: `https:\\www.myfictionalsite.com`.

1. Entrada [!DNL Adobe Dynamic Media Classic], vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**.
1. Na página Definições Gerais da Aplicação, no campo **[!UICONTROL Test&Target Server Name]** cole o URL copiado na etapa 2.
1. Selecionar **[!UICONTROL Close]**.
