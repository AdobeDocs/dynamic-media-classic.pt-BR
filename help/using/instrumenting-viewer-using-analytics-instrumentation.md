---
title: Instrumentar um visualizador usando o kit de instrumentação do Adobe Analytics
description: Saiba como instrumentar um visualizador usando o Kit de instrumentação do Adobe Analytics no Adobe Dynamic Media Classic.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
source-git-commit: a9bd472705bce32f63a5710c3266e51256d17a00
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# Instrumentar um visualizador usando o kit de instrumentação do Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Você pode usar o kit de instrumentação do Adobe Analytics para integrar um visualizador de HTML 5 com o Adobe Analytics.

Se você usar qualquer uma das predefinições do visualizador do Adobe Dynamic Media Classic HTML5 predefinidas, elas já conterão todo o código de implementação para enviar dados para o Adobe Analytics. Nenhuma outra instrumentação será necessária.

## Configurar o rastreamento do Adobe Analytics no Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Para todos os visualizadores de HTML, adicione o seguinte JavaScript ao contêiner de HTML, geralmente no &lt;head> elemento:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Onde `Adobe Dynamic Media Classic Company ID` é definido como o nome da empresa do Adobe Dynamic Media Classic. E `&preset` é opcional, a menos que o nome da predefinição da empresa não seja `companypreset`. Nesses casos, poderia ser `companypreset-1, companypreset-2`e assim por diante. O número mais alto é uma instância mais recente da predefinição. Para determinar o nome correto do valor predefinido da empresa, selecione **[!UICONTROL Copy URL]** e, em seguida, observe o `preset=`para localizar o nome da predefinição da empresa.

Continuando, adicione uma função que transmite o evento do visualizador para o código de rastreamento do Adobe Analytics.

Adicione o `s7ComponentEvent()` para o HTML do contêiner (ou JSP, ou ASPX ou outro):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

O nome da função diferencia maiúsculas de minúsculas. O único parâmetro passado para `s7componentEvent`que é obrigatório é o último: `eventData`. Onde `s7track()` é definido no s_code.jsp incluído acima. E `s7track` O lida com todo o rastreamento de cada evento. (Para personalizar ainda mais os dados transmitidos para o Adobe Analytics, essa área é o local para fazer isso.)

## Ativar eventos HREF e ITEM {#enabling-href-and-item-events}

Você pode ativar eventos HREF (rolagem) e ITEM (cliques do mouse/toque) nos visualizadores por meio da edição do Mapa de imagem. Defina os identificadores para HREF e ITEM no Mapa de imagem associado ao conteúdo do visualizador. Adicionar um `&rolloverKey=` para o valor HREF no Mapa de imagem.
