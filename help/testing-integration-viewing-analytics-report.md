---
title: Teste da integração exibindo um relatório do Adobe Analytics
description: Saiba como testar a integração exibindo um relatório do Adobe Analytics.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Engenheiro de dados,Administrador,Profissional de negócios
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---


# Teste da integração exibindo um relatório do Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Depois de criar as variáveis necessárias no Adobe Analytics, vinculá-las aos eventos do Dynamic Media Classic e concluir as etapas de implementação necessárias, teste a configuração. Você pode testar e verificar se os dados estão sendo capturados, dentro do próprio Adobe Analytics. Se a configuração funcionar aqui, nenhuma etapa adicional será necessária. Supondo que você tenha seguido as etapas acima e vinculado os dados do evento do Dynamic Media Classic a uma ou mais variáveis de tráfego personalizadas, siga este fluxo de trabalho para testar seus dados no Adobe Analytics.

**Para testar a integração exibindo um relatório do Adobe Analytics**

1. Inicie um visualizador do Dynamic Media Classic de sua conta, especialmente um que transmita a métrica que você deseja capturar, e interaja com ele para criar alguns dados de evento.

   Por exemplo, se você quiser medir as exibições alternativas mais populares em um Conjunto de imagens, visualize um Conjunto de imagens e clique nas diferentes imagens de miniaturas.

1. No Adobe Analytics, vá para Tráfego personalizado > Tráfego personalizado 1-10 > [Nome de prop], selecionando o nome da prop de tráfego nas opções do menu.

   Por exemplo, para acessar a propriedade LoadAsset em nossa conta de exemplo, a escolha adequada do menu seria Tráfego personalizado > Tráfego personalizado 1-10 > LoadAsset. Se você tiver mais de dez props personalizados, poderá ver opções de menu adicionais também.

1. Visualize o gráfico produzido pela Adobe Analytics. Observe que isso normalmente são apenas os dados de uma única métrica. Se também quiser saber com qual ativo esses dados estão associados (por exemplo, qual vídeo está sendo assistido a apenas 50% ou qual imagem em um conjunto é mais popular), certifique-se de capturar os dados de ativo desse evento também.

>[!NOTE]
>
>Todos os dados do visualizador do Dynamic Media Classic são exibidos e relatados nos relatórios de Tráfego personalizado ou nos relatórios de Conversão personalizada do Adobe Analytics.

Para obter mais informações, consulte [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
