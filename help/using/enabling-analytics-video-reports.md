---
title: Ativar relatórios de vídeo do Adobe Analytics
description: Saiba como habilitar relatórios de vídeo do Adobe Analytics no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
autotag-review: '2026-05-13T19:47:00.853Z'
TQID: 'https://experienceleague.adobe.com/bXlrGU0zMEyfa-E-x-29-biChC17GJTEViBP8GoouTU'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 270
ht-degree: 0%

---

# Ativar relatórios de vídeo do Adobe Analytics{#enabling-adobe-analytics-video-reports}

Usando o relatório de vídeo baseado em pulsação do Adobe Analytics, você não deve mais ativar os quatro eventos do visualizador de vídeo (Reproduzir, Pausar, Parar, Marco) ao configurar o Adobe Analytics no Adobe Dynamic Media Classic. O Video Heartbeat funciona com visualizadores integrados de vídeo e mídia mista do Adobe Dynamic Media Classic HTML5. O reprodutor de vídeo gera dados de rastreamento para exibição nos relatórios de vídeo do Adobe Analytics.

* Para obter uma introdução à mídia de transmissão e à &quot;medição de pulsação&quot;, consulte [Sobre o Adobe Analytics para mídia de transmissão](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* A integração dos relatórios de vídeo do Adobe Analytics com o Adobe Dynamic Media Classic é compatível com variáveis da solução, mas não com variáveis personalizadas.

  Consulte [Parâmetros de áudio e vídeo](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters) para obter mais informações sobre variáveis de solução e variáveis personalizadas.

* Segmentos prontos para uso com incrementos de um minuto são compatíveis. No entanto, os relatórios de segmento personalizados, como marcos definidos pelo cliente com base em incrementos de tempo, % de marcos ou marcos de compensação, não são compatíveis.

  Para obter mais informações sobre os requisitos e a configuração da mídia de streaming, consulte [Medir mídia de streaming no Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Para obter informações sobre variáveis personalizadas e de solução, consulte [Habilitação de relatórios de mídia](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Se sua solução licenciada do Adobe Analytics não incluir o Video Heartbeat, continue usando as etapas descritas neste capítulo para atribuir variáveis do Adobe Analytics a eventos e variáveis do visualizador do Adobe Dynamic Media Classic.
