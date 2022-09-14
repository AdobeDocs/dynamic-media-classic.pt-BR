---
title: "Início rápido: Dimensionamento de imagem"
description: Uma introdução e o início rápido do dimensionamento de imagem para ajudá-lo a ativar e executar rapidamente com as técnicas de dimensionamento de imagem no Adobe Dynamic Media Classic.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 0%

---

# Início rápido: Dimensionamento de imagem{#quick-start-image-sizing}

Dimensionamento de imagem refere-se à capacidade do Adobe Dynamic Media Classic de criar várias imagens derivadas com base em uma única imagem de alta resolução. Em vez de criar manualmente várias imagens (por exemplo, uma miniatura e uma imagem de exibição ampliada) para seu site ou aplicativo, você fornece uma única imagem primária. O Adobe Dynamic Media Classic gera todas as imagens modificadas da mesma maneira que você as solicita. Ser capaz de fornecer imagens dinamicamente de uma única imagem primária tem muitas vantagens:

* Não é necessário criar manualmente várias cópias da imagem em tamanhos diferentes. Você fornece uma imagem primária para a Adobe Dynamic Media Classic, e a Adobe Dynamic Media Classic gera derivados de tamanhos diferentes da imagem principal.
* Você pode alterar rapidamente o tamanho de um tipo de imagem em todo o site ou aplicativo. Por exemplo, para alterar todas as imagens em miniatura, você pode modificar a predefinição de imagem em &quot;miniatura&quot;. Uma Predefinição de imagem — é semelhante a uma macro — é uma coleção de atributos de tamanho e formatação. Você pode modificar a predefinição de imagem de &quot;miniatura&quot; para alterar o tamanho de todas as imagens em miniatura em seu site ou aplicativo.
* Não é necessário gerenciar os arquivos principais e todos os vários derivados em qualquer um dos sistemas de gerenciamento de conteúdo ou ativos internamente ou externamente.

![Você pode criar várias imagens derivadas em diferentes tamanhos do mesmo arquivo principal de alta resolução.](/help/assets/is_derivative_sizes_popup.png)

Consulte [Tamanho da imagem: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) vídeo de treinamento.

O seguinte Início rápido de dimensionamento de imagem foi projetado para ajudar você a ativar e executar rapidamente com as técnicas de dimensionamento de imagem no Adobe Dynamic Media Classic. Siga as etapas de 1 a 5. Após cada etapa, há uma referência cruzada onde você pode encontrar mais informações, se precisar.

## 1. Fazer upload das imagens primárias

Comece carregando suas imagens principais no Adobe Dynamic Media Classic. Quanto ao tamanho, a Adobe Dynamic Media Classic recomenda usar imagens que são o maior tamanho que você espera usar em seu site ou aplicativo. Por exemplo, se você quiser que os visualizadores ampliem imagens, carregue imagens que tenham pelo menos 2000 pixels no tamanho maior. O Adobe Dynamic Media Classic suporta muitos formatos de arquivo de imagem, mas são recomendadas imagens de TIFF e PNG sem perdas.

Na barra Navegação global, selecione **[!UICONTROL Upload]** para carregar arquivos do seu computador para uma pasta no Adobe Dynamic Media Classic. Consulte [Upload das imagens primárias](uploading-master-images.md#uploading_master_images).

## 2. Configurar predefinições da imagem

Como uma macro, uma Predefinição de imagem é uma coleção de comandos predefinidos de tamanho e formatação salvos em um nome. Uma predefinição de imagem governa o tamanho e a formatação com que as imagens são entregues dos servidores de imagem da Dynamic Media. Você pode configurar as Predefinições de imagem por conta própria, se tiver o status de administrador da empresa. O Adobe Dynamic Media Classic também vem com Predefinições de imagem padrão, e você pode usá-las para fornecer imagens dinamicamente.

Para criar uma Predefinição de imagem (se você for um administrador), na barra Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Image Presets]**. Em seguida, selecione **[!UICONTROL Add]** para criar uma predefinição de imagem ou selecione **[!UICONTROL Edit]** para alterar uma predefinição de imagem existente.

A Predefinição de imagem criada é adicionada ao menu Predefinição de imagem na página Visualizar. Você pode usar sua nova Predefinição de imagem para exibir imagens dinamicamente em seus sites e aplicativos. Consulte [Configurar predefinições da imagem](setting-image-presets.md#setting_up_image_presets).

## 3. Visualizar predefinições da imagem

A próxima etapa é visualizar as Predefinições de imagem que seu administrador configurou nos diferentes tamanhos predefinidos.

Para explorar as Predefinições de imagem, na barra Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]** e navegue até uma predefinição de imagem.

Experimente com diferentes predefinições de imagem. Descubra como sua imagem aparece quando é entregue dinamicamente em seu site ou aplicativo em diferentes tamanhos.

Consulte [Visualizar um ativo de imagem com base em sua Predefinição de imagem](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Publicar as imagens principais

A publicação dos arquivos de imagem principais tem dois objetivos essenciais:

* Publique suas imagens principais nos Servidores de Imagem da Dynamic Media para que as imagens possam ser entregues dinamicamente ao seu site e aplicativo.
* A publicação ativa as cadeias de caracteres do URL para chamar imagens dos Servidores de Imagem da Dynamic Media para o site ou aplicativo. Após a publicação, você pode copiar e colocar os URLs gerados pela Adobe Dynamic Media Classic, conforme necessário, em seu site ou aplicativo.

Na barra Navegação global, selecione **[!UICONTROL Publish]** para iniciar um trabalho de publicação. Na caixa de diálogo Publicar , selecione **[!UICONTROL Submit Publish]**. Consulte [Publicar imagens primárias](publishing-master-images.md#publishing_master_images).

## 5. Vincular URLs ao aplicativo da Web

O Adobe Dynamic Media Classic cria cadeias de caracteres de chamada de URL para imagens. Ao publicar imagens nos Servidores de imagem da Dynamic Media, os URLs ficam ativos. Você pode copiar essas cadeias de caracteres do URL no Painel de navegação (na Exibição de detalhes) ou na tela de Visualização. Depois de copiar as cadeias de caracteres do URL, você pode usá-las em seu site e aplicativos. O URL para dimensionamento de imagem substitui a referência a um nome de imagem estática no código da página da Web. O URL faz referência a um nome de imagem principal, que é substituído pelo seu banco de dados para cada nova imagem ser exibida.

As cadeias de caracteres de URL geradas com predefinições de imagem contêm o nome de uma predefinição de imagem. Este nome está incluso em cifrão (`$`). Por exemplo, `$thumbnail$` pode ser a Predefinição de imagem criada para mostrar as imagens primárias em tamanho de miniatura. Consulte [Vincular URLs ao aplicativo da Web](linking-urls-web-application.md#linking_urls_to_your_web_application).
