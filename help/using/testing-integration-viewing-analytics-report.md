---
title: Testar a integração visualizando um relatório do Adobe Analytics
description: Saiba como testar a integração no Adobe Dynamic Media Classic visualizando um relatório do Adobe Analytics.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T20:14:40.601Z'
TQID: 'https://experienceleague.adobe.com/BwQe9AuhBfi-bLCuO-j48kE-3gw9rgtz5GEI9nIBRjE'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 331
ht-degree: 0%

---

# Testar a integração visualizando um relatório do Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Depois de criar as variáveis necessárias no Adobe Analytics, vinculá-las aos eventos do Adobe Dynamic Media Classic e concluir as etapas de implementação necessárias, você pode testar a configuração. Você pode testar e verificar se os dados estão sendo capturados dentro do próprio Adobe Analytics. Se a configuração funcionar aqui, nenhuma outra etapa será necessária. Supondo que você tenha seguido as etapas acima e vinculado seus dados de evento do Adobe Dynamic Media Classic a uma ou mais variáveis de Tráfego personalizado, siga esse fluxo de trabalho para testar seus dados dentro do Adobe Analytics.

**Para testar a integração exibindo um relatório do Adobe Analytics:**

1. Inicie um visualizador do Adobe Dynamic Media Classic na sua conta, especialmente um que transmita a métrica que deseja obter, e interaja com ele para criar alguns dados do evento.

   Por exemplo, se você deseja medir visualizações alternativas populares em um Conjunto de imagens, visualize um Conjunto de imagens e clique nas diferentes imagens de miniaturas.

1. No Adobe Analytics, vá para **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > [Nome da prop], selecionando o nome da prop de tráfego nas opções de menu.

   Por exemplo, para acessar a prop **[!UICONTROL LoadAsset]** na conta de exemplo, a escolha de menu adequada é **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > **[!UICONTROL LoadAsset]**. Se você tiver mais de dez props personalizadas, também verá outras opções de menu.

1. Visualize o gráfico produzido pela Adobe Analytics. Normalmente, esse gráfico é apenas os dados de uma única métrica. Se você também quiser saber a qual ativo esses dados estão associados, obtenha os dados de ativo desse evento. Por exemplo, geralmente é útil saber qual vídeo é assistido apenas 50% ou qual imagem em um conjunto é popular.

>[!NOTE]
>
>Todos os dados do visualizador do Adobe Dynamic Media Classic são exibidos e relatados nos relatórios Tráfego personalizado ou Conversão personalizada do Adobe Analytics.

Para obter mais informações, consulte [Tutoriais do Analytics](https://experienceleague.adobe.com/en/docs/analytics-learn/tutorials/overview).