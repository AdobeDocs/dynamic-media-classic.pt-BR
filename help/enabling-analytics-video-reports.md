---
title: Ativação dos relatórios de vídeo da Adobe Analytics
description: Saiba como ativar relatórios de vídeo do Adobe Analytics.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# Habilitar relatórios de vídeo do Adobe Analytics{#enabling-adobe-analytics-video-reports}

Usando o relatórios de vídeo baseado em pulsação do Adobe Analytics, não é mais necessário ativar os quatro eventos do visualizador de vídeo (Reproduzir, Pausar, Parar, Etapa) ao configurar o Adobe Analytics no Dynamic Media Classic. O Video Heartbeat funciona com visualizadores Dynamic Media Classic HTML5 e MixedMedia prontos para uso. O player de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo da Adobe Analytics.

* Para obter uma introdução à mídia de streaming e à ‘medição de pulsação’, consulte [Sobre o Adobe Analytics para Streaming Media](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* A integração dos relatórios de vídeo do Adobe Analytics com o Dynamic Media Classic oferece suporte a variáveis de solução, mas não a variáveis personalizadas.

   Consulte [Parâmetros de áudio e vídeo](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) para obter mais informações sobre variáveis de solução e variáveis personalizadas.

* Segmentos predefinidos de incrementos de um minuto são suportados. No entanto, o relatórios de segmento personalizado, como marcos definidos pelo cliente com base em incrementos de tempo, marcos de % ou marcos de deslocamento, não é suportado.

   Para obter mais informações sobre os requisitos e a configuração da mídia de streaming, consulte [Medição da mídia de Steaming no Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Para obter informações sobre variáveis personalizadas e de solução, consulte [Ativação de relatórios de mídia](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Se sua solução licenciada do Adobe Analytics não incluir o Video Heartbeat, será necessário continuar usando as etapas descritas neste capítulo para atribuir variáveis do Adobe Analytics aos eventos e variáveis do visualizador Dynamic Media Classic.

