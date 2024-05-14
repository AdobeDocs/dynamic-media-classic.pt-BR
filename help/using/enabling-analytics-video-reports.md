---
title: Ativar relatórios de vídeo do Adobe Analytics
description: Saiba como habilitar relatórios de vídeo do Adobe Analytics no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Ativar relatórios de vídeo do Adobe Analytics{#enabling-adobe-analytics-video-reports}

Usando o relatório de vídeo baseado em pulsação do Adobe Analytics, você não deve mais ativar os quatro eventos do visualizador de vídeo (Reproduzir, Pausar, Parar, Marco) ao configurar o Adobe Analytics no Adobe Dynamic Media Classic. O Video Heartbeat funciona com visualizadores integrados de HTML5 de vídeo e mídia mista do Adobe Dynamic Media Classic. O reprodutor de vídeo gera dados de rastreamento para exibição nos relatórios de vídeo do Adobe Analytics.

* Para obter uma introdução à mídia de transmissão e à &quot;medição de heartbeat&quot;, consulte [Sobre o Adobe Analytics para mídia de streaming](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* A integração dos relatórios de vídeo do Adobe Analytics com o Adobe Dynamic Media Classic é compatível com variáveis da solução, mas não com variáveis personalizadas.

  Consulte [Parâmetros de áudio e vídeo](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters) para obter mais informações sobre variáveis de solução e variáveis personalizadas.

* Segmentos prontos para uso com incrementos de um minuto são compatíveis. No entanto, os relatórios de segmento personalizados, como marcos definidos pelo cliente com base em incrementos de tempo, % de marcos ou marcos de compensação, não são compatíveis.

  Para obter mais informações sobre os requisitos e a configuração da mídia de transmissão, consulte [Meça a mídia de streaming no Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Para obter informações sobre variáveis personalizadas e de soluções, consulte [Ativação de relatórios de mídia](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Se sua solução licenciada do Adobe Analytics não incluir o Video Heartbeat, continue usando as etapas descritas neste capítulo para atribuir variáveis do Adobe Analytics a eventos e variáveis do visualizador do Adobe Dynamic Media Classic.
