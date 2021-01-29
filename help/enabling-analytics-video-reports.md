---
title: Ativação dos relatórios de vídeo da Adobe Analytics
description: Saiba como ativar relatórios de vídeo do Adobe Analytics.
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---


# Habilitar relatórios de vídeo do Adobe Analytics{#enabling-adobe-analytics-video-reports}

Usando o relatórios de vídeo baseado em pulsação do Adobe Analytics, não é mais necessário ativar os quatro eventos do visualizador de vídeo (Reproduzir, Pausar, Parar, Etapa) ao configurar o Adobe Analytics no Dynamic Media Classic. O Video Heartbeat funciona com visualizadores Dynamic Media Classic HTML5 e MixedMedia prontos para uso. O player de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo da Adobe Analytics.

* A integração dos relatórios de vídeo do Adobe Analytics com o Dynamic Media Classic oferece suporte a variáveis de solução, mas não a variáveis personalizadas.

   Consulte [Configurar o Relatórios de vídeo do Analytics](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) para obter mais informações sobre variáveis de solução e variáveis personalizadas.

* Segmentos predefinidos de incrementos de um minuto são suportados. No entanto, o relatórios de segmento personalizado, como marcos definidos pelo cliente com base em incrementos de tempo, marcos de % ou marcos de deslocamento, não é suportado.

Para obter mais informações sobre os requisitos e a configuração do Video Heartbeat, consulte [Medição de vídeo no Adobe Analytics usando o Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Se sua solução licenciada do Adobe Analytics não incluir o Video Heartbeat, será necessário continuar usando as etapas descritas neste capítulo para atribuir variáveis do Adobe Analytics aos eventos e variáveis do visualizador Dynamic Media Classic.

