---
title: Instrumentação de um visualizador usando o Kit de instrumentação do Adobe Analytics
description: Saiba como instrumentar um visualizador usando o Adobe Analytics Instrumentation Kit.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Engenheiro de dados,Administrador,Profissional de negócios
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Instrumentação de um visualizador usando o Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Você pode usar o Kit de instrumentação do Adobe Analytics para integrar um visualizador de HTML5 ao Adobe Analytics.

Se você usar qualquer uma das predefinições do visualizador HTML5 do Dynamic Media Classic, esteja ciente de que elas já contêm todo o código de implementação necessário para enviar dados para o Adobe Analytics — nenhuma instrumentação adicional é necessária para você.

## Configurar o rastreamento do Adobe Analytics no Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Para todos os visualizadores HTML5, adicione o seguinte JavaScript ao contêiner HTML, normalmente no elemento &lt;head> :

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

`Company` é definida como o nome da empresa do Dynamic Media Classic. `&preset` é opcional, a menos que o nome predefinido da empresa não seja  `companypreset`. Nesses casos, pode ser `companypreset-1, companypreset-2` e assim por diante. O número mais alto é uma instância mais recente da predefinição. Para determinar o nome correto do valor predefinido da empresa, clique em **Copiar URL** e olhe para o parâmetro `preset=`para encontrar o nome predefinido da empresa.

Continuando, agora você adicionará uma função que transmite o evento do visualizador ao código de rastreamento do Adobe Analytics.

Adicione a função `s7ComponentEvent()` ao HTML do contêiner (ou JSP, ou ASPX ou outro):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

O nome da função diferencia maiúsculas de minúsculas. O único parâmetro passado para `s7componentEvent`que é necessário é o último: `eventData`. `s7track()` é definido em s_code.jsp incluído acima. `s7track` O lida com todo o rastreamento por cada evento. (Para personalizar ainda mais os dados transmitidos ao Adobe Analytics, essa área é o lugar para fazer isso.)

## Ativar eventos HREF e ITEM {#enabling-href-and-item-events}

Você pode ativar eventos HREF (sobreposição) e ITEM (cliques/toque do mouse) nos visualizadores por meio da edição do Mapa de imagem. Defina os identificadores para o HREF e o ITEM no Mapa de imagem que está associado ao conteúdo do visualizador. Adicione um parâmetro `&rolloverKey=` ao valor HREF no Mapa de imagem.
