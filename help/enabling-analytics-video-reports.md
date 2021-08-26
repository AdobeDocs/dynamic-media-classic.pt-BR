---
title: Ativar os relatórios de vídeo do Adobe Analytics
description: Saiba como habilitar relatórios de vídeo do Adobe Analytics no Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: 20a5e54a9f3fa442d3a993afae07aa5b1b13e9c3
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Ativar os relatórios de vídeo do Adobe Analytics{#enabling-adobe-analytics-video-reports}

Usando o relatório de vídeo baseado em pulsação do Adobe Analytics, você não deve mais habilitar os quatro eventos do visualizador de vídeo (Reproduzir, Pausar, Parar, Marco) ao configurar o Adobe Analytics no Dynamic Media Classic. O Video Heartbeat funciona com os visualizadores de vídeo HTML5 do Dynamic Media Classic e de mídia mista prontos para uso. O reprodutor de vídeo gera dados de rastreamento para visualização nos Relatórios de vídeo do Adobe Analytics.

* Para obter uma introdução à mídia de transmissão e à &quot;medição de pulsação&quot;, consulte [Sobre o Adobe Analytics para mídia de transmissão](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* A integração dos relatórios de vídeo do Adobe Analytics com o Dynamic Media Classic é compatível com variáveis de solução, mas não com variáveis personalizadas.

   Consulte [Parâmetros de áudio e vídeo](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) para obter mais informações sobre variáveis de solução e variáveis personalizadas.

* Segmentos prontos para uso de incrementos de um minuto são compatíveis. No entanto, o relatório de segmento personalizado, como marcos definidos pelo cliente com base em incrementos de tempo, em % de marco ou marcos de deslocamento, não é suportado.

   Para obter mais informações sobre os requisitos e a configuração da mídia de transmissão, consulte [Medir mídia de transmissão em Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Para obter informações sobre variáveis personalizadas e de solução, consulte [Ativação de relatórios de mídia](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Se a solução licenciada do Adobe Analytics não incluir o Video Heartbeat, você deve continuar usando as etapas descritas neste capítulo para atribuir variáveis do Adobe Analytics aos eventos e variáveis do visualizador Dynamic Media Classic.
