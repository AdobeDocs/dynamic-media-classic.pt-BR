---
title: '" Prática recomendada: Como usar o visualizador de vídeo HTML 5'
seo-title: '" Prática recomendada: Como usar o visualizador de vídeo HTML 5'
description: 'null'
seo-description: Saiba mais sobre as práticas recomendadas para usar o visualizador de vídeo HTML 5.
uuid: 3 c 8924 dc -7 bea -4 c 25-b 77 b -005 f 57 b 71 b 64
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/vídeo
discoiquuid: 4 b 11 cab 7-88 cf -42 dd -8554-2 eea 530753 bb
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Prática recomendada: Uso do visualizador de vídeo HTML 5{#best-practice-using-the-html-video-viewer}

As predefinições do visualizador de vídeo HTML 5 de Dynamic Media clássica são players de vídeo robustos. No design do player, você pode criar toda a funcionalidade do player de vídeo usando ferramentas padrão de desenvolvimento na Web. Por exemplo, você pode criar os botões, controles e o fundo de imagem de pôster personalizado usando HTML 5 e CSS para ajudar você a atingir seus clientes com uma aparência personalizada.

Na reprodução do visualizador, detecta automaticamente o recurso de vídeo do navegador. Em seguida, fornece o vídeo usando HLS (streaming de vídeo adaptável). Ou, se esse método de entrega não estiver presente, o HTML 5 progressivo será usado em vez disso.

Ao combinar em um único player a capacidade de projetar os componentes de reprodução usando HTML 5 e CSS, ter reprodução incorporada e usar streaming adaptável e progressivo, dependendo do recurso do navegador, você estende o alcance do conteúdo de mídia avançada para os usuários de desktop e móveis e garante uma experiência de vídeo simplificada.

Consulte [também Sobre visualizadores](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) HTML 5 no Guia de referência de visualizadores da Adobe.

## Reprodução de vídeo em computadores desktop e dispositivos móveis usando o Visualizador de vídeo clássico do Dynamic Media {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Para streaming de vídeo adaptável para desktop e móvel, os vídeos usados para troca de taxa de bits são baseados em todos os vídeos MP 4 no Conjunto de vídeos adaptativos.

A reprodução de vídeo ocorre usando HLS ou vídeo progressivo. HLS (HTTP Live Streaming) é um padrão da Apple para streaming de vídeo adaptável que ajusta a reprodução automaticamente com base na capacidade de banda de rede. Também permite que o cliente «procure» em qualquer ponto no vídeo sem precisar aguardar o download do restante do vídeo (consulte também [HTTP Live Streaming](#UnresolvedLink-https://developer.apple.com/streaming/)). O vídeo progressivo é entregue baixando e armazenando o vídeo localmente em uma tela de desktop ou dispositivo móvel do usuário.

A tabela a seguir descreve o dispositivo, navegador e método de reprodução de vídeos em computadores desktop e dispositivos móveis usando o Visualizador de vídeo clássico do Dynamic Media.

| Dispositivo | Navegador | Modo de reprodução de vídeo |
|--- |--- |--- |
| Desktop | Internet Explorer 9 e 10 | Download progressivo. |
| Área de trabalho | Internet Explorer 11 + | Streaming de vídeo HLS. |
| Área de trabalho | Firefox 23-44 | Download progressivo. |
| Área de trabalho | Firefox 45 ou posterior | Streaming de vídeo HLS. |
| Área de trabalho | Chrome | Streaming de vídeo HLS. |
| Área de trabalho | Safari (Mac) | Streaming de vídeo HLS. |
| Dispositivo móvel | Chrome (Android 6 ou anterior) | Download progressivo. |
| Dispositivo móvel | Chrome (Android 7 ou posterior) | Streaming de vídeo HLS. |
| Dispositivo móvel | Android (Navegador padrão) | Download progressivo. |
| Dispositivo móvel | Safari (iOS) | Streaming de vídeo HLS. |
| Dispositivo móvel | Chrome (iOS) | Streaming de vídeo HLS. |
| Dispositivo móvel | Blackberry | Streaming de vídeo HLS. |
