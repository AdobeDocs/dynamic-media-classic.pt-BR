---
title: Prática recomendada para usar o visualizador de vídeo HTML5
description: Saiba mais sobre as práticas recomendadas para usar o visualizador de vídeo do HTML5.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Práticas recomendadas para usar o visualizador de vídeo HTML5{#best-practice-using-the-html-video-viewer}

As predefinições do visualizador de vídeo do Adobe Dynamic Media Classic HTML5 são players de vídeo robustos. No lado de design do reprodutor, é possível criar a funcionalidade inteira do reprodutor de vídeo usando ferramentas de desenvolvimento da Web padrão. Por exemplo, você pode projetar botões, controles e imagens de fundo de pôster personalizadas usando HTML5 e CSS para ajudá-lo a alcançar seus clientes com uma aparência personalizada.

No lado da reprodução do visualizador, ele detecta automaticamente o recurso de vídeo do navegador. Em seguida, ele serve o vídeo usando HLS (HTTP Live Streaming), também conhecido como streaming de vídeo adaptável. Ou, se esse método de delivery não estiver presente, HTML5 progressivo será usado.

Ao combinar em um único reprodutor as seguintes capacidades:

* Componentes de reprodução projetados com HTML5 e CSS
* Reprodução incorporada
* Uso de streaming adaptável e progressivo com base na capacidade do navegador

Você estende o alcance do seu conteúdo de mídia avançada para usuários de desktop e de dispositivos móveis. Você também garante uma experiência em vídeo simplificada.

Consulte também [Sobre visualizadores do HTML5](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) no Guia de referência de visualizadores do Adobe.

Consulte também [Vídeo de treinamento de predefinições do visualizador](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS).

## Reprodução de vídeo em computadores desktop e dispositivos móveis usando o Adobe Dynamic Media Classic Video Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Para streaming de vídeo adaptável para desktop e dispositivos móveis, os vídeos usados para alternância de taxa de bits são baseados em todos os vídeos MP4 no Adaptive Video Set.

A reprodução de vídeo ocorre usando HLS ou vídeo progressivo. O HLS (HTTP Live Streaming) é um padrão Apple para streaming de vídeo adaptável que ajusta automaticamente a reprodução com base na capacidade da largura de banda da rede. Ele também permite que o cliente &quot;procure&quot; em qualquer ponto do vídeo, sem precisar aguardar o download do restante do vídeo. Consulte também [HTTP Live Streaming](https://developer.apple.com/streaming/). O vídeo progressivo é fornecido pelo download e armazenamento local do vídeo na tela de desktop de um usuário ou no dispositivo móvel.

A tabela a seguir descreve o dispositivo, o navegador e o método de reprodução de vídeos em computadores desktop e dispositivos móveis usando o Adobe Dynamic Media Classic Video Viewer.

| Dispositivo | Navegador | Modo de reprodução de vídeo |
|--- |--- |--- |
| Desktop | Internet Explorer 9 e 10 | Download progressivo. |
| Desktop | Internet Explorer 11+ | Transmissão de vídeo HLS. |
| Desktop | Firefox 23-44 | Download progressivo. |
| Desktop | Firefox 45 ou superior | Transmissão de vídeo HLS. |
| Desktop | Cromo | Transmissão de vídeo HLS. |
| Desktop | Safari (Mac) | Transmissão de vídeo HLS. |
| Celular | Chrome (Android™ 6 ou anterior) | Download progressivo. |
| Celular | Chrome (Android™ 7 ou posterior) | Transmissão de vídeo HLS. |
| Celular | Android™ (Navegador padrão) | Download progressivo. |
| Celular | Safari (iOS) | Transmissão de vídeo HLS. |
| Celular | Chrome (iOS) | Transmissão de vídeo HLS. |
| Celular | BlackBerry® | Transmissão de vídeo HLS. |
