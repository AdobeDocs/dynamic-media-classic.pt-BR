---
title: Ativar os relatórios de vídeo do Adobe Analytics
description: Saiba como habilitar relatórios de vídeo do Adobe Analytics no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Ativar os relatórios de vídeo do Adobe Analytics{#enabling-adobe-analytics-video-reports}

Com os relatórios de vídeo baseados em pulsação do Adobe Analytics, não é mais necessário habilitar os quatro eventos do visualizador de vídeo (Reproduzir, Pausar, Parar, Marco) ao configurar o Adobe Analytics no Adobe Dynamic Media Classic. O Video Heartbeat funciona com os visualizadores de vídeo e mídia mista prontos para uso do Adobe Dynamic Media Classic HTML 5. O reprodutor de vídeo gera dados de rastreamento para visualização nos Relatórios de vídeo do Adobe Analytics.

* Para obter uma introdução à mídia de streaming e à &quot;medição de pulsação&quot;, consulte [Sobre o Adobe Analytics para mídia de streaming](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* A integração dos relatórios de vídeo do Adobe Analytics com o Adobe Dynamic Media Classic é compatível com variáveis de solução, mas não com variáveis personalizadas.

   Consulte [Parâmetros de áudio e vídeo](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) para obter mais informações sobre variáveis da solução e variáveis personalizadas.

* Segmentos prontos para uso de incrementos de um minuto são compatíveis. No entanto, o relatório de segmento personalizado, como marcos definidos pelo cliente com base em incrementos de tempo, em % de marco ou marcos de deslocamento, não é suportado.

   Para obter mais informações sobre os requisitos e a configuração da mídia de streaming, consulte [Meça a mídia de streaming no Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Para obter informações sobre variáveis personalizadas e de solução, consulte [Ativação de relatórios de mídia](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Se a solução licenciada do Adobe Analytics não incluir o Video Heartbeat, você deve continuar usando as etapas descritas neste capítulo para atribuir variáveis do Adobe Analytics aos eventos e variáveis do visualizador Adobe Dynamic Media Classic.
