---
title: '"Start rápido: Dimensionamento da imagem"'
seo-title: '"Start rápido: Dimensionamento da imagem"'
description: nulo
seo-description: Uma introdução e um Start rápido para o Dimensionamento de imagens para ajudá-lo a começar a trabalhar rapidamente com as técnicas de Dimensionamento de imagens.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 0%

---


# Start rápido: Dimensionamento da imagem{#quick-start-image-sizing}

O dimensionamento de imagem refere-se à capacidade do Dynamic Media Classic de criar várias imagens derivadas com base em uma única imagem de alta resolução. Em vez de criar manualmente várias imagens (por exemplo, uma miniatura e imagem de visualização ampliada) para seu site ou aplicativo, você fornece uma única imagem principal. O Dynamic Media Classic gera todas as imagens modificadas exatamente como você as solicita. Ser capaz de fornecer imagens dinamicamente a partir de uma única imagem principal tem muitas vantagens:

* Não é necessário criar manualmente várias cópias da imagem em tamanhos diferentes. Você fornece uma imagem principal ao Dynamic Media Classic, e o Dynamic Media Classic gera derivados de tamanhos diferentes da imagem principal.
* Você pode alterar rapidamente o tamanho de um tipo de imagem em todo o site ou aplicativo. Por exemplo, para alterar todas as imagens em miniatura, é possível modificar a predefinição de imagem &quot;em miniatura&quot;. Uma predefinição de imagem, semelhante a uma macro, é uma coleção de atributos de tamanho e formatação. Você pode modificar a predefinição de imagem &quot;miniatura&quot; para alterar o tamanho de todas as imagens em miniatura em todo o site ou aplicativo.
* Você não precisa gerenciar os principais e todos os diversos derivados em qualquer um dos seus sistemas de gerenciamento de conteúdo ou ativos, interna ou externamente.

![É possível criar várias imagens derivadas em tamanhos diferentes do mesmo arquivo principal de alta resolução.](/help/assets/is_derivative_sizes_popup.png)

**Start rápido**

Este Start rápido de dimensionamento de imagem foi projetado para ajudá-lo a começar a usar rapidamente as técnicas de dimensionamento de imagem no Dynamic Media Classic. Siga as etapas de 1 a 5. Após cada etapa é uma referência cruzada na qual você pode encontrar mais informações, se necessário.

**1. Upload de imagens principais**

Start carregando suas imagens principais no Dynamic Media Classic. Quanto ao tamanho, o Dynamic Media Classic recomenda o uso de imagens com o maior tamanho que você espera que sejam usadas em seu site ou aplicativo. Por exemplo, se você quiser que os visualizadores ampliem imagens, carregue imagens que tenham pelo menos 2000 pixels na maior dimensão. O Dynamic Media Classic é compatível com vários formatos de arquivo de imagem, mas imagens TIFF e PNG sem perdas são recomendadas.

Selecione o botão Carregar na barra Navegação global para fazer upload de arquivos do seu computador para uma pasta no Dynamic Media Classic. Consulte [Carregando imagens principais](uploading-master-images.md#uploading_master_images).

**2. Configuração de predefinições de imagens**

Como uma macro, uma predefinição de imagem é uma coleção de comandos de tamanho e formatação predefinidos salvos com um nome. Uma predefinição de imagem governa o tamanho e a formatação com os quais as imagens são entregues pelos servidores de imagem Dynamic Media. Você pode configurar as predefinições de imagens por conta própria se tiver o status de administrador da empresa. O Dynamic Media Classic também é fornecido com as predefinições de imagem padrão e você pode usá-las para fornecer imagens dinamicamente.

Para criar uma predefinição de imagem (se você for um administrador), escolha Configuração > Configuração do aplicativo. Na tela Configuração, exiba as opções de Configuração do aplicativo e escolha Predefinições de imagem. Em seguida, clique em **Adicionar** ou **Editar** para criar uma predefinição de imagem.

A predefinição de imagem que você cria é adicionada ao menu Predefinição de imagem na tela de Pré-visualização. Você pode usar sua nova predefinição de imagem para exibir imagens dinamicamente em seus sites e aplicativos. Consulte [Configuração de predefinições de imagens](setting-image-presets.md#setting_up_image_presets).

**3. Pré-visualização de Predefinições de Imagem**

A próxima etapa é pré-visualização das predefinições de imagem configuradas pelo administrador com tamanhos predefinidos diferentes.

Para explorar as predefinições de imagens, clique em **Configuração** > **Predefinições de imagens** e navegue até uma predefinição de imagens.

Experimente as diferentes predefinições de imagens. Descubra a aparência da imagem quando ela é fornecida dinamicamente para o seu site ou aplicativo em tamanhos diferentes.

Consulte [Visualizar um ativo de imagem com base em sua predefinição de imagem](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

**4. Publicar suas imagens principais**

A publicação dos arquivos de imagem principais tem dois objetivos essenciais:

* Publique suas imagens principais nos Dynamic Media Image Servers para que as imagens possam ser distribuídas dinamicamente para seu site e aplicativo.
* A publicação ativa as sequências de caracteres de URL para chamar imagens dos Servidores de Imagens da Dynamic Media para seu site ou aplicativo. Após a publicação, você pode copiar e colocar os URLs gerados pelo Dynamic Media Classic, onde necessário, em seu site ou aplicativo.

Selecione o botão Publicar na barra Navegação global para iniciar uma publicação. Na tela Publicar, selecione o botão Publicar Start. Consulte [Publicar imagens principais](publishing-master-images.md#publishing_master_images).

**5. Vincular URLs ao aplicativo da Web**

O Dynamic Media Classic cria sequências de chamada de URL para imagens. Quando você publica imagens nos Dynamic Media Image Servers, os URLs ficam ativos. É possível copiar essas sequências de caracteres de URL do Painel de navegação (em visualização detalhada) ou da tela de Pré-visualização. Depois de copiar as sequências de caracteres do URL, você pode usá-las no site e nos aplicativos. O URL para dimensionamento de imagem substitui a referência a um nome de imagem estática no código da página da Web. O URL faz referência a um nome de imagem principal, que é substituído pelo banco de dados para que cada nova imagem seja exibida.

As sequências de caracteres de URL geradas com predefinições de imagem contêm o nome de uma predefinição de imagem. Este nome está incluído nos sinais em dólar (`$`). Por exemplo, `$thumbnail$` pode ser a predefinição de imagem projetada para mostrar imagens principais em tamanho de miniatura. Consulte [Vincular URLs ao seu aplicativo da Web](linking-urls-web-application.md#linking_urls_to_your_web_application).
