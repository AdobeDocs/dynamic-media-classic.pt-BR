---
title: '"Melhores práticas: Usar o visualizador de vídeo HTML5"'
seo-title: '"Melhores práticas: Usar o visualizador de vídeo HTML5"'
description: nulo
seo-description: Saiba mais sobre as práticas recomendadas para o uso do visualizador de vídeo HTML5.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---


# Melhores práticas: Uso do visualizador de vídeo HTML5{#best-practice-using-the-html-video-viewer}

As predefinições do visualizador de vídeo HTML5 do Dynamic Media Classic são players de vídeo robustos. No lado de design do player, é possível criar toda a funcionalidade do player de vídeo usando ferramentas padrão de desenvolvimento da Web. Por exemplo, você pode projetar botões, controles e imagens de fundo de pôster personalizadas usando HTML5 e CSS para ajudá-lo a alcançar seus clientes com uma aparência personalizada.

No lado da reprodução do visualizador, ele detecta automaticamente a capacidade de vídeo do navegador. Em seguida, ele serve o vídeo usando HLS (streaming de vídeo adaptável). Ou, se esse método de delivery não estiver presente, então o HTML5 progressivo será usado.

Ao combinar em um único player a capacidade de projetar os componentes de reprodução usando HTML5 e CSS, ter reprodução integrada e usar streaming adaptável e progressivo dependendo da capacidade do navegador, você estende o alcance do conteúdo de mídia avançada para usuários de desktop e móveis e garante uma experiência de vídeo otimizada.

Consulte também [Sobre Visualizadores HTML5](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html) no Guia de Referência de Visualizadores de Adobe.

## Reprodução de vídeo em computadores desktop e dispositivos móveis usando o Dynamic Media Classic Video Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Para streaming de vídeo adaptável para desktop e dispositivos móveis, os vídeos usados para switching de taxa de bits são baseados em todos os vídeos MP4 no Conjunto de vídeos adaptáveis.

A reprodução do vídeo ocorre usando HLS ou vídeo progressivo. HLS (HTTP Live Streaming) é um padrão da Apple para streaming de vídeo adaptável que ajusta automaticamente a reprodução com base na capacidade de largura de banda da rede. Ele também permite que o cliente &quot;procure&quot; qualquer ponto do vídeo, sem precisar aguardar o download do restante do vídeo. Consulte também [HTTP Live Streaming](https://developer.apple.com/streaming/). O vídeo progressivo é fornecido por meio do download e armazenamento local do vídeo na tela do desktop do usuário ou dispositivo móvel.

A tabela a seguir descreve o dispositivo, o navegador e o método de reprodução de vídeos em computadores desktop e dispositivos móveis usando o Dynamic Media Classic Video Viewer.

| Dispositivo | Navegador | Modo de reprodução de vídeo |
|--- |--- |--- |
| Desktop | Internet Explorer 9 e 10 | Download progressivo. |
| Desktop | Internet Explorer 11+ | Transmissão de vídeo HLS. |
| Desktop | Firefox 23-44 | Download progressivo. |
| Desktop | Firefox 45 ou posterior | Transmissão de vídeo HLS. |
| Desktop | Cromo | Transmissão de vídeo HLS. |
| Desktop | Safari (Mac) | Transmissão de vídeo HLS. |
| Dispositivo móvel | Chrome (Android 6 ou anterior) | Download progressivo. |
| Dispositivo móvel | Chrome (Android 7 ou posterior) | Transmissão de vídeo HLS. |
| Dispositivo móvel | Android (navegador padrão) | Download progressivo. |
| Dispositivo móvel | Safari (iOS) | Transmissão de vídeo HLS. |
| Dispositivo móvel | Chrome (iOS) | Transmissão de vídeo HLS. |
| Dispositivo móvel | Blackberry | Transmissão de vídeo HLS. |
