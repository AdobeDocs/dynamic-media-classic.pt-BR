---
title: Prática recomendada para usar o visualizador de vídeo do HTML5
description: Saiba mais sobre as práticas recomendadas para usar o visualizador de vídeo do HTML5.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# Práticas recomendadas para usar o visualizador de vídeo do HTML5{#best-practice-using-the-html-video-viewer}

As Predefinições do visualizador de vídeo Adobe Dynamic Media Classic HTML5 são players de vídeo robustos. No lado do design do reprodutor, é possível criar toda a funcionalidade dele usando as ferramentas padrão de desenvolvimento para Web. Por exemplo, você pode projetar os botões, os controles e o plano de fundo personalizado da imagem de pôster usando o HTML5 e o CSS para ajudar você a alcançar seus clientes com uma aparência personalizada.

No lado da reprodução do visualizador, ele detecta automaticamente o recurso de vídeo do navegador. Em seguida, ele serve o vídeo usando o HLS (HTTP Live Streaming), também conhecido como transmissão de vídeo adaptável. Ou, se esse método de delivery não estiver presente, será usado o HTML5 progressive.

Ao combinar em um único jogador as seguintes habilidades:

* Componentes de reprodução criados com HTML5 e CSS
* Reprodução incorporada
* Uso de transmissão adaptável e progressiva com base na capacidade do navegador

Você estende o alcance do seu conteúdo de mídia avançada para usuários de desktop e dispositivos móveis. Você também garante uma experiência de vídeo otimizada.

Consulte também [Sobre HTML5 Viewers](https://experienceleague.adobe.com/pt-br/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) no Guia de Referência do Adobe Viewers.

Consulte também o vídeo de treinamento [Predefinições do visualizador](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS).

## Reprodução de vídeo em computadores desktop e dispositivos móveis usando o Adobe Dynamic Media Classic Video Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Para streaming de vídeo adaptável de desktop e móvel, os vídeos usados para a alternância da taxa de bits são baseados em todos os vídeos MP4 no Conjunto de vídeos adaptados.

A reprodução de vídeo ocorre usando HLS ou vídeo progressivo. O HLS (HTTP Live Streaming) é um padrão da Apple para transmissão de vídeo adaptável que ajusta automaticamente a reprodução com base na capacidade de largura de banda da rede. Ele também permite que o cliente &quot;procure&quot; qualquer ponto do vídeo, sem a necessidade de aguardar o download do restante do vídeo. Consulte também [HTTP Live Streaming](https://developer.apple.com/streaming/). O vídeo progressivo é fornecido ao baixar e armazenar o vídeo localmente na tela de desktop de um usuário ou no dispositivo móvel.

A tabela a seguir descreve o dispositivo, o navegador e o método de reprodução de vídeos em computadores desktop e dispositivos móveis que usam o Adobe Dynamic Media Classic Video Viewer.

| Dispositivo | Navegador | Modo de reprodução de vídeo |
|--- |--- |--- |
| Desktop | Internet Explorer 9 e 10 | Download progressivo. |
| Desktop | Internet Explorer 11+ | Transmissão contínua de vídeo do HLS. |
| Desktop | Firefox 23-44 | Download progressivo. |
| Desktop | Firefox 45 ou posterior | Transmissão contínua de vídeo do HLS. |
| Desktop | Chrome | Transmissão contínua de vídeo do HLS. |
| Desktop | Safari (Mac) | Transmissão contínua de vídeo do HLS. |
| Dispositivo móvel | Chrome (Android™ 6 ou anterior) | Download progressivo. |
| Dispositivo móvel | Chrome (Android™ 7 ou posterior) | Transmissão contínua de vídeo do HLS. |
| Dispositivo móvel | Android™ (navegador padrão) | Download progressivo. |
| Dispositivo móvel | Safari (iOS) | Transmissão contínua de vídeo do HLS. |
| Dispositivo móvel | Chrome (iOS) | Transmissão contínua de vídeo do HLS. |
| Dispositivo móvel | BlackBerry® | Transmissão contínua de vídeo do HLS. |
