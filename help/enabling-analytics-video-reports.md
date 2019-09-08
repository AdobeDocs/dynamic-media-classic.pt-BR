---
title: Ativação dos relatórios de vídeo do Adobe Analytics
seo-title: Ativação dos relatórios de vídeo do Adobe Analytics
description: 'null'
seo-description: Saiba como ativar os relatórios de vídeo do Adobe Analytics.
uuid: 078594 b 2-7 d 53-4714-8128-ff 3 b 5 c 3 a 5 e 36
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/adobe_ analytics_ instrumentation_ kit
discoiquuid: 18644 a 53-92 da -40 ab-b 961-318 d 8332 c 54 d
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Ativação dos relatórios de vídeo do Adobe Analytics{#enabling-adobe-analytics-video-reports}

Com o relatório de vídeo com base no Adobe Analytics, não é mais necessário ativar os quatro eventos do visualizador de vídeo (Reproduzir, Pausar, Parar, Marco) quando você configura o Adobe Analytics no Dynamic Media Classic. O Video Heartbeat funciona com visualizadores de vídeo e mixedmedia prontos para Dynamic Media clássica. O player de vídeo gera dados de rastreamento para exibição nos Relatórios de vídeo do Adobe Analytics.

* A integração dos relatórios de vídeo do Adobe Analytics com o Dynamic Media Classic oferece suporte a variáveis de solução, mas não a variáveis personalizadas.

   Consulte [Configurar relatórios de vídeo do Analytics](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) para obter mais informações sobre variáveis de solução e variáveis personalizadas.

* Segmentos prontos para uso de incrementos de um minuto são suportados. No entanto, relatórios de segmento personalizados, como marcos definidos pelo cliente com base em incrementos de tempo, % marco ou marcos de offset, não são suportados.

Para obter mais informações sobre os requisitos e a configuração do Video Heartbeat, consulte [Medição de vídeo no Adobe Analytics usando heartbeat de vídeo](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Se a solução licenciada do Adobe Analytics não incluir o Video Heartbeat, será necessário continuar a usar as etapas descritas neste capítulo para atribuir variáveis do Adobe Analytics aos eventos e variáveis do visualizador do Dynamic Media Classic.

