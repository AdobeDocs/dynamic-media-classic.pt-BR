---
title: Instrumentação de um visualizador usando o Adobe Analytics Instrumentation Kit
seo-title: Instrumentação de um visualizador usando o Adobe Analytics Instrumentation Kit
description: nulo
seo-description: Saiba como instrumentar um visualizador usando o Adobe Analytics Instrumentation Kit.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# Instrumentação de um visualizador usando o Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Você pode usar o Adobe Analytics Instrumentation Kit para integrar um visualizador HTML5 ao Adobe Analytics.

Se você usar qualquer uma das predefinições predefinidas do visualizador HTML5 do Dynamic Media Classic, esteja ciente de que elas já contêm todo o código de implementação necessário para enviar dados para a Adobe Analytics, nenhuma instrumentação adicional é necessária para você.

## Configurar o rastreamento do Adobe Analytics do Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Para todos os visualizadores HTML5, adicione o seguinte JavaScript ao container HTML, geralmente no elemento &lt;head>:

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

`Company` está definida como o nome da empresa do Dynamic Media Classic. `&preset` é opcional, a menos que o nome predefinido da empresa não seja `companypreset`. Nesses casos, poderia ser `companypreset-1, companypreset-2`, e assim por diante. O número mais alto é uma instância mais recente da predefinição. Para determinar o nome correto do valor predefinido de empresa, clique em **Copiar URL** e procure o `preset=`parâmetro para localizar o nome predefinido de empresa.

Continuando, agora você adicionará uma função que transmite o evento do visualizador ao código de rastreamento do Adobe Analytics.

Adicione a `s7ComponentEvent()` função ao HTML do container (ou JSP, ou ASPX ou outro):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

O nome da função faz distinção entre maiúsculas e minúsculas. O único parâmetro passado para `s7componentEvent`isso é obrigatório é o último: `eventData`. `s7track()` está definido em s_code.jsp incluído acima. `s7track` lida com todo o rastreamento por cada evento. (Para personalizar ainda mais os dados transmitidos à Adobe Analytics, essa área é o local para fazer isso.)

## Habilitar eventos HREF e ITEM {#enabling-href-and-item-events}

Você pode ativar eventos HREF (sobreposição) e ITEM (cliques do mouse/toque) nos visualizadores por meio da edição do Mapa de imagem. Defina os identificadores para HREF e ITEM no Mapa de imagem que está associado ao conteúdo do visualizador. Adicione um `&rolloverKey=` parâmetro ao valor HREF no Mapa de imagem.
