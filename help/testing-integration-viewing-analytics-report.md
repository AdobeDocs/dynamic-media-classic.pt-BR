---
title: Teste da integração ao visualizar um relatório da Adobe Analytics
seo-title: Teste da integração ao visualizar um relatório da Adobe Analytics
description: nulo
seo-description: Saiba como testar a integração ao exibir um relatório da Adobe Analytics.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---


# Teste da integração ao visualizar um relatório da Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Depois de criar as variáveis necessárias no Adobe Analytics, vinculá-las aos eventos do Dynamic Media Classic e concluir as etapas de implementação necessárias, teste a configuração. Você pode testar e verificar se os dados estão sendo capturados, dentro da própria Adobe Analytics. Se a configuração funcionar aqui, não serão necessárias mais etapas. Supondo que você tenha seguido as etapas acima e vinculado seus dados de evento do Dynamic Media Classic a uma ou mais variáveis de tráfego personalizadas, siga este fluxo de trabalho para testar seus dados no Adobe Analytics.

**Para testar a integração exibindo um relatório da Adobe Analytics**

1. Inicie um visualizador do Dynamic Media Classic de sua conta, particularmente um que transmite a métrica que você deseja capturar, e interaja com ele para criar alguns dados de evento.

   Por exemplo, se você quiser medir as visualizações alternativas mais populares em um Conjunto de imagens, pré-visualização um Conjunto de imagens e clique em diferentes imagens em miniaturas.

1. No Adobe Analytics, vá até Tráfego personalizado > Tráfego personalizado 1-10 > [Nome da prop], selecionando o nome da prop de tráfego nas opções de menu.

   Por exemplo, para acessar a propriedade LoadAsset em nossa conta de amostra, a opção de menu adequada seria Tráfego personalizado > Tráfego personalizado 1-10 > LoadAsset. Se você tiver mais de dez props personalizados, você também poderá ver outras opções de menu.

1. Visualização no gráfico produzido pela Adobe Analytics. Observe que esses são normalmente apenas os dados de uma única métrica. Se você também quiser saber com qual ativo esses dados estão associados (por exemplo, qual vídeo está sendo assistido a apenas 50% ou qual imagem em um conjunto é mais popular), certifique-se de capturar os dados de ativos desse evento também.

>[!NOTE]
>
>Todos os dados do visualizador do Dynamic Media Classic são exibidos e reportados nos relatórios de Tráfego personalizado ou nos relatórios de Conversão personalizada do Adobe Analytics.

Para obter mais informações, consulte [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
