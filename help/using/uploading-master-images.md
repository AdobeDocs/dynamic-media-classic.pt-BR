---
title: Fazer upload de imagens principais
description: Saiba como fazer upload de imagens principais no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Fazer upload de imagens principais{#uploading-master-images}

Antes de carregar imagens no Adobe Dynamic Media Classic, verifique se elas têm o tamanho e o formato da mais alta qualidade. A Adobe Dynamic Media Classic recomenda o upload de imagens de alta qualidade com uma contagem de pixels suficiente (de 1500 a 2000 pixels no tamanho longo). Esse dimensionamento permite qualquer Dynamic Imaging necessário.

Para obter detalhes sobre como carregar imagens, consulte [Carregar arquivos](uploading-files.md#uploading_files).

**Preparar suas imagens principais para carregamento:**

Prepare seus arquivos de imagem principais antes de carregá-los no Adobe Dynamic Media Classic:

* **Tamanho da imagem**: crie as imagens de maior tamanho que você prevê usar. Os tamanhos de imagem típicos variam de 1500 a 2500 pixels no tamanho mais longo. Se você pretende usar o recurso Zoom, a Adobe Dynamic Media Classic recomenda usar imagens com pelo menos 2000 pixels no tamanho mais longo para obter o detalhe de zoom ideal. O Adobe Dynamic Media Classic pode renderizar imagens de até 25 megapixels cada. Por exemplo, você pode usar uma imagem de 5000 × 5000 MP ou qualquer outra combinação de tamanho até 25 MP.

* **Formatos de arquivo**: o Adobe Dynamic Media Classic oferece suporte a todos os formatos de arquivo de imagem padrão. Esses formatos incluem TIFF, BMP, JPEG, PSD, GIF e EPS. Formatos de imagem sem perda - TIFF e PNG - são recomendados. Se você estiver usando uma imagem de JPEG, use as configurações de mais alta qualidade.

* **Espaço de cores**: RGB é o espaço de cores para apresentações de imagens da Web; imagens CMYK usadas normalmente para impressão são convertidas automaticamente em RGB ao carregá-las. É recomendado fazer upload de imagens CMYK que tenham um perfil de cores ICC (International Color Consortium) incorporado para conversão em RGB. Consulte também [perfis de ICC (International Color Consortium)](/help/using/icc-profiles.md).
