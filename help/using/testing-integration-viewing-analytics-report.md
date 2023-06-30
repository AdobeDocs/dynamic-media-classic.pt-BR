---
title: Testar a integração visualizando um relatório do Adobe Analytics
description: Saiba como testar a integração no Adobe Dynamic Media Classic visualizando um relatório do Adobe Analytics.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Testar a integração visualizando um relatório do Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Depois de criar as variáveis necessárias no Adobe Analytics, vinculá-las aos eventos do Adobe Dynamic Media Classic e concluir as etapas de implementação necessárias, você pode testar a configuração. Você pode testar e verificar se os dados estão sendo capturados, dentro do próprio Adobe Analytics. Se a configuração funcionar aqui, nenhuma outra etapa será necessária. Supondo que você tenha seguido as etapas acima e vinculado seus dados de evento do Adobe Dynamic Media Classic a uma ou mais variáveis de tráfego personalizadas, siga esse fluxo de trabalho para testar seus dados dentro do Adobe Analytics.

**Para testar a integração visualizando um relatório do Adobe Analytics:**

1. Inicie um visualizador do Adobe Dynamic Media Classic na sua conta, especialmente um que transmita a métrica que deseja obter, e interaja com ele para criar alguns dados do evento.

   Por exemplo, se você deseja medir visualizações alternativas populares em um Conjunto de imagens, visualize um Conjunto de imagens e clique nas diferentes imagens de miniaturas.

1. No Adobe Analytics, acesse **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > [Nome da prop], selecionando o nome da prop de tráfego nas opções de menu.

   Por exemplo, para acessar o **[!UICONTROL LoadAsset]** prop na conta de exemplo, a opção de menu adequada é **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > **[!UICONTROL LoadAsset]**. Se você tiver mais de dez props personalizadas, também verá outras opções de menu.

1. Visualize o gráfico produzido pela Adobe Analytics. Normalmente, esse gráfico é apenas os dados de uma única métrica. Se você também quiser saber a qual ativo esses dados estão associados, obtenha os dados de ativo desse evento. Por exemplo, geralmente é útil saber qual vídeo é assistido a apenas 50% ou qual imagem em um conjunto é popular.

>[!NOTE]
>
>Todos os dados do visualizador do Adobe Dynamic Media Classic são exibidos e relatados nos relatórios Tráfego personalizado ou Conversão personalizada do Adobe Analytics.

Para obter mais informações, consulte [Tutorials do Analytics](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html).