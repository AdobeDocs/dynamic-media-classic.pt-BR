---
title: Instrumentando um visualizador usando o Kit de instrumentação do Adobe Analytics
seo-title: Instrumentando um visualizador usando o Kit de instrumentação do Adobe Analytics
description: 'null'
seo-description: Saiba como preparar um visualizador usando o Kit de instrumentação do Adobe Analytics.
uuid: cf 9 a 4002-966 d -4641-9 cd 0-2 ee 8 b 5454 f 60
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/adobe_ analytics_ instrumentation_ kit
discoiquuid: a 2824244-1755-42 de-a 167-42 af 117 cf 038
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Instrumentando um visualizador usando o Kit de instrumentação do Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Você pode usar o Kit de instrumentação do Adobe Analytics para integrar um visualizador HTML 5 com o Adobe Analytics.

Se você usar qualquer uma das predefinições predefinidas do visualizador do Dynamic Media clássica, esteja ciente de que já contém todo o código de implementação necessário para enviar dados para o Adobe Analytics—não é necessária outra instrumentação.

## Configurar o rastreamento do Adobe Analytics do Sistema de publicação Scene 7 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Para todos os visualizadores HTML 5, adicione o seguinte javascript ao contêiner HTML, normalmente no elemento &lt; head &gt;:

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<SPS Company ID>&preset=companypreset-1"></script>
```

`Company` é definido como o nome da empresa SPS. `&preset` é opcional, a não ser que o nome da predefinição da empresa `companypreset`não seja. Nesses casos, pode ser `companypreset-1, companypreset-2`, e assim por diante. O número mais alto é uma instância mais nova da predefinição. Para determinar o nome correto do valor predefinido da empresa, clique **em Copiar URL** e olhe o `preset=`parâmetro para encontrar o nome da predefinição da empresa.

Continuando, você adicionará uma função que transmite o evento do visualizador ao código de rastreamento do Adobe Analytics.

Adicione `s7ComponentEvent()` a função ao HTML do contêiner (ou JSP ou ASPX ou outro):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

O nome da função diferencia maiúsculas e minúsculas. O único parâmetro transmitido `s7componentEvent`a esse é o último: `eventData`. `s7track()` é definido em s_ code. jsp incluído acima. `s7track` trata todo o rastreamento por cada evento. (Para personalizar ainda mais os dados transmitidos para o Adobe Analytics, essa área é o local para fazer isso.)

## Ativar eventos HREF e ITEM {#enabling-href-and-item-events}

Você pode ativar os eventos HREF (rollover) e ITEM (cliques/toque do mouse) nos visualizadores por meio da edição do Mapa de imagens. Defina os identificadores para HREF e ITEM no Mapa de imagem que está associado ao conteúdo do visualizador. Adicione um `&rolloverKey=` parâmetro ao valor HREF no Mapa de imagem.
