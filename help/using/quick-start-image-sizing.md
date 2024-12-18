---
title: 'Início rápido: dimensionamento de imagem'
description: Uma introdução e o Início rápido do dimensionamento de imagem para ajudar você a começar a usar rapidamente as técnicas de dimensionamento de imagem no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
topic: Content Management
level: Beginner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# Início rápido: dimensionamento de imagem{#quick-start-image-sizing}

Dimensionamento de imagem refere-se à capacidade do Adobe Dynamic Media Classic de criar várias imagens derivadas com base em uma única imagem de alta resolução. Em vez de criar manualmente várias imagens (por exemplo, uma miniatura e uma imagem ampliada) para seu site ou aplicativo, você fornece uma única imagem principal. O Adobe Dynamic Media Classic gera todas as imagens modificadas da mesma maneira que você as solicita. A capacidade de fornecer imagens dinamicamente a partir de uma única imagem principal tem muitas vantagens:

* Não é necessário criar manualmente várias cópias da imagem em tamanhos diferentes. Você fornece uma imagem principal para o Adobe Dynamic Media Classic, e o Adobe Dynamic Media Classic gera derivados de tamanhos diferentes da imagem principal.
* Você pode alterar rapidamente o tamanho de um tipo de imagem em todo o site ou aplicativo. Por exemplo, para alterar todas as imagens em miniatura, é possível modificar a Predefinição de imagem da &quot;miniatura&quot;. Uma predefinição de imagem é semelhante a uma macro, uma coleção de atributos de tamanho e formatação. É possível modificar a predefinição de imagem em &quot;miniatura&quot; para alterar o tamanho de todas as imagens em miniatura em todo o site ou aplicativo.
* Não é necessário gerenciar os arquivos principais e todos os vários derivados em nenhum de seus sistemas de gerenciamento de conteúdo ou ativos interna ou externamente.

![Você pode criar várias imagens derivadas em tamanhos diferentes do mesmo arquivo primário de alta resolução.](/help/using/assets/is_derivative_sizes_popup.png)

Consulte [Dimensionamento de imagem: vídeo de treinamento Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS).

O seguinte Início rápido de dimensionamento de imagem foi projetado para ajudar você a começar a trabalhar rapidamente com técnicas de dimensionamento de imagem no Adobe Dynamic Media Classic. Siga as etapas de 1 a 5. Após cada etapa, há uma referência cruzada em que você pode encontrar mais informações, se necessário.

## 1. Fazer upload de imagens principais

Comece fazendo upload das imagens principais no Adobe Dynamic Media Classic. Quanto ao tamanho, a Adobe Dynamic Media Classic recomenda usar imagens que sejam do maior tamanho que você prevê usar em seu site ou aplicativo. Por exemplo, se você quiser que os visualizadores ampliem imagens, carregue imagens com pelo menos 2000 pixels de tamanho maior. O Adobe Dynamic Media Classic é compatível com muitos formatos de arquivo de imagem, mas são recomendados TIFF sem perdas e imagens PNG.

Na barra Navegação global, selecione **[!UICONTROL Upload]** para carregar arquivos do seu computador para uma pasta no Adobe Dynamic Media Classic. Consulte [Carregar imagens principais](uploading-master-images.md#uploading_master_images).

## 2. Configurar predefinições da imagem

Como uma macro, uma Predefinição de imagem é uma coleção de comandos de tamanho e formatação predefinidos salvos com um nome. Uma Predefinição de imagem controla o tamanho e a formatação com que as imagens são entregues dos Servidores de imagem da Dynamic Media. Você pode configurar as Predefinições de imagem por conta própria, caso tenha o status de Administrador da empresa. É possível fornecer imagens dinamicamente usando as Predefinições de imagem padrão que já vêm com o Adobe Dynamic Media Classic.

Para criar uma Predefinição de imagem (se você for um administrador), na barra de Navegação Global, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Image Presets]**. Em seguida, selecione **[!UICONTROL Add]** para criar uma Predefinição de imagem ou selecione **[!UICONTROL Edit]** para alterar uma Predefinição de imagem existente.

A Predefinição de imagem criada é adicionada ao menu Predefinição de imagem na página Visualizar. Você pode usar sua nova Predefinição de imagem para exibir imagens dinamicamente em seus sites e aplicativos. Consulte [Configurar predefinições de imagem](setting-image-presets.md#setting_up_image_presets).

## 3. Visualizar predefinições da imagem

A próxima etapa é visualizar as Predefinições de imagem que o administrador configurou em tamanhos de predefinição diferentes.

Para explorar Predefinições de Imagem, na barra Navegação Global, vá para **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]** e navegue até uma Predefinição de Imagem.

Experimente com as diferentes Predefinições de imagem. Descubra como a imagem é exibida quando é entregue dinamicamente ao seu site ou aplicativo em tamanhos diferentes.

Consulte [Visualizar um ativo de imagem com base em sua Predefinição de imagem](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Publish suas imagens principais

A publicação dos arquivos de imagem principais tem dois objetivos essenciais:

* Publicar suas imagens principais nos servidores de imagens da Dynamic Media para que as imagens possam ser entregues dinamicamente ao seu site e aplicativo.
* A publicação ativa as cadeias de caracteres de URL para chamar imagens dos Dynamic Media Image Servers para seu site ou aplicativo. Após a publicação, você pode copiar e colocar os URLs gerados pela Adobe Dynamic Media Classic onde necessário no site ou aplicativo.

Na barra Navegação Global, selecione **[!UICONTROL Publish]** para iniciar um trabalho de publicação. Na caixa de diálogo Publicação, selecione **[!UICONTROL Submit Publish]**. Consulte [imagens principais do Publish](publishing-master-images.md#publishing_master_images).

## 5. Vincular URLs à sua aplicação web

O Adobe Dynamic Media Classic cria strings de texto explicativo de URL para imagens. Ao publicar imagens nos Dynamic Media Image Servers, os URLs ficam ativos. Você pode copiar essas cadeias de caracteres de URL do painel Procurar (na Exibição de detalhes) ou da tela Visualização. Após copiar as cadeias de caracteres de URL, é possível usá-las no site e nos aplicativos. O URL para dimensionamento de imagem substitui a referência a um nome de imagem estática no código da página da Web. O URL faz referência a um nome de imagem principal que o banco de dados substitui para cada nova imagem a ser exibida.

As cadeias de caracteres de URL geradas com Predefinições de imagem contêm o nome de uma Predefinição de imagem. Este nome está entre cifrões (`$`). Por exemplo, `$thumbnail$` pode ser a Predefinição de imagem projetada para mostrar as imagens principais no tamanho de miniatura. Consulte [Vincular URLs ao aplicativo Web](linking-urls-web-application.md#linking_urls_to_your_web_application).
