---
title: Ativar relatórios de vídeo do Adobe Analytics
description: Saiba como ativar os relatórios de vídeo do Adobe Analytics.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: 3def4a02eda8dc36f2811b3d4f0e870fff1994e4
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---


# Ativar relatórios de vídeo do Adobe Analytics{#enabling-adobe-analytics-video-reports}

Usando o relatório de vídeo baseado em pulsação do Adobe Analytics, você não deve mais habilitar os quatro eventos do visualizador de vídeo (Reproduzir, Pausar, Parar, Marco) ao configurar o Adobe Analytics no Dynamic Media Classic. O Video Heartbeat funciona com os visualizadores Dynamic Media Classic HTML5 e MixedMedia prontos para uso. O reprodutor de vídeo gera dados de rastreamento para visualização nos Relatórios de vídeo do Adobe Analytics.

* Para obter uma introdução à mídia de transmissão e à &quot;medição de pulsação&quot;, consulte [Sobre o Adobe Analytics para mídia de transmissão](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* A integração dos relatórios de vídeo do Adobe Analytics com o Dynamic Media Classic é compatível com variáveis de solução, mas não com variáveis personalizadas.

   Consulte [Parâmetros de áudio e vídeo](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) para obter mais informações sobre variáveis de solução e variáveis personalizadas.

* Segmentos prontos para uso de incrementos de um minuto são compatíveis. No entanto, o relatório de segmento personalizado, como marcos definidos pelo cliente com base em incrementos de tempo, em % de marco ou marcos de deslocamento, não é suportado.

   Para obter mais informações sobre os requisitos e a configuração da mídia de transmissão, consulte [Medição da mídia de transmissão no Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Para obter informações sobre variáveis personalizadas e de solução, consulte [Ativação de relatórios de mídia](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Se a solução licenciada do Adobe Analytics não incluir o Video Heartbeat, você deve continuar usando as etapas descritas neste capítulo para atribuir variáveis do Adobe Analytics aos eventos e variáveis do visualizador Dynamic Media Classic.

