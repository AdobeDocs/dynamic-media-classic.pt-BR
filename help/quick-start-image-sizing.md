---
title: '" Início rápido: Dimensionamento da imagem "'
seo-title: '" Início rápido: Dimensionamento da imagem "'
description: 'null'
seo-description: Uma introdução e uma Introdução rápida ao dimensionamento da imagem para ajudá-lo a começar a usar rapidamente as técnicas de dimensionamento de imagem.
uuid: 6 c 4 ad 4 b 7-549 d -4 daa-b 6 b 9-5997 a 8427 af 8
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/image_ sizing
discoiquuid: dcaa 9 b 21-b 925-4 dbb -865 e -7918 cdbda 50 c
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Início rápido: Dimensionamento da imagem{#quick-start-image-sizing}

Dimensionamento de imagem refere-se à capacidade do Dynamic Media Classic de criar várias imagens derivadas com base em uma única imagem de alta resolução. Em vez de criar manualmente várias imagens (por exemplo, uma miniatura e uma imagem ampliada) para seu site ou aplicativo, você fornece uma única imagem mestra. O Dynamic Media Classic gera todas as imagens modificadas da mesma maneira que você solicita. A capacidade de fornecer imagens dinamicamente a partir de uma única imagem mestra tem muitas vantagens:

* Não é necessário criar manualmente várias cópias da imagem em tamanhos diferentes. Você fornece uma imagem mestre ao Dynamic Media Classic e o Dynamic Media Classic gera derivados diferentes de tamanho da imagem mestre.
* É possível alterar rapidamente o tamanho de um tipo de imagem em todo o seu site ou aplicativo. Por exemplo, para alterar todas as imagens em miniatura, é possível modificar a Predefinição de imagem «miniatura». Uma predefinição de imagem— é semelhante a uma macro— é uma coleção de atributos de tamanho e formatação. É possível modificar a predefinição de imagem «miniatura» para alterar o tamanho de todas as imagens em miniatura em todo o site ou aplicativo.
* Você não precisa gerenciar os mestres e todos os diversos derivados em nenhum dos sistemas de conteúdo ou gerenciamento de ativos internamente ou externamente.

![É possível criar várias imagens derivadas em tamanho diferente do mesmo arquivo mestre de alta resolução.](/help/assets/is_derivative_sizes_popup.png)

**Início rápido**

Este Início rápido de Dimensionamento de imagem foi projetado para ajudá-lo a começar a usar rapidamente as técnicas de dimensionamento de imagem no Sistema de publicação Scene 7. Siga as etapas 1-5. Depois de cada etapa, é uma referência cruzada onde você pode encontrar mais informações, se necessário.

**1. Upload de imagens mestre**

Comece carregando suas imagens mestre no Sistema de publicação Scene 7. Como o tamanho, o Dynamic Media Classic recomenda usar imagens que são o maior tamanho que você prevê usando em seu site ou aplicativo. Por exemplo, se você quiser que os visualizadores aumentem o zoom de imagens, carregue imagens com pelo menos 2000 pixels na maior dimensão. O Dynamic Media Classic oferece suporte a muitos formatos de arquivo de imagem, mas imagens TIFF e PNG sem perdas são recomendadas.

Selecione o botão Carregar na barra Navegação global para carregar arquivos de seu computador para uma pasta no Sistema de publicação Scene 7. Consulte [Upload de imagens mestre](uploading-master-images.md#uploading_master_images).

**2. Configuração de predefinições de imagens**

Como uma macro, uma predefinição de imagem é uma coleção de comandos predefinidos de tamanho e formatação salvos com um nome. Uma predefinição de imagem rege o tamanho e a formatação com as quais as imagens são entregues dos servidores de imagem do Dynamic Media. Você pode configurar as Predefinições de imagens por conta própria se tiver status de administrador da empresa. O Dynamic Media Classic também vem com as predefinições de imagens padrão, e você pode usá-las para fornecer imagens dinamicamente.

Para criar uma predefinição de imagem (se for um administrador), escolha Configuração &gt; Configuração do aplicativo. Na tela Configuração, exiba as opções de Configuração de aplicativo e escolha Predefinições de imagens. Em seguida, clique **em Adicionar** ou **Editar** para criar uma predefinição de imagem.

A Predefinição de imagem criada é adicionada ao menu Predefinição de imagem na tela Visualizar. Você pode usar a nova Predefinição de imagem para exibir imagens dinamicamente em seus sites e aplicativos. Consulte [Configuração de predefinições de imagens](setting-image-presets.md#setting_up_image_presets).

**3. Visualizar predefinições de imagens**

A próxima etapa é visualizar as predefinições de imagens que seu administrador configura em tamanhos predefinidos diferentes.

Para explorar Predefinições de imagens, clique **em Configuração** &gt; **Predefinições** de imagens e procure uma Predefinição de imagem.

Experimente com as diferentes predefinições de imagens. Descubra a aparência da imagem quando ela é entregue dinamicamente em seu site ou aplicativo de tamanhos diferentes.

Consulte [Visualizar um ativo de imagem com base na predefinição de imagem](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

**4. Publicar imagens mestre**

A publicação de arquivos de imagem mestre fornece dois objetivos essenciais:

* Publique suas imagens mestras nos servidores de imagem do Dynamic Media para que as imagens possam ser enviadas dinamicamente em seu site e aplicativo.
* A publicação ativa as sequências de caracteres de URL para chamar imagens de Servidores de imagem do Dynamic Media a seu site ou aplicativo. Após a publicação, você pode copiar e colocar os urls gerados por Digital Media Classic, onde necessário em seu site ou aplicativo.

Selecione o botão Publicar na barra Navegação global para iniciar uma publicação. Na tela Publicar, selecione o botão Iniciar publicação. Consulte [Publicar imagens mestre](publishing-master-images.md#publishing_master_images).

**5. Vincular urls ao aplicativo da Web**

O Dynamic Media Classic cria strings de retorno de URL para imagens. Quando você publica imagens nos servidores de imagem do Dynamic Media, os urls ficam ativos. Você pode copiar essas sequências de URL do Painel Procurar (na exibição Detalhe) ou da tela Visualizar. Depois de copiar as strings de URL, você pode usá-las em seu site e aplicativos. O URL para dimensionamento de imagem substitui a referência a um nome de imagem estática no código da página da Web. O URL faz referência a um nome de imagem mestre, que é substituído pelo banco de dados para cada nova imagem exibida.

As sequências de caracteres de URL geradas com Predefinições de imagens contêm o nome de uma Predefinição de imagem. Esse nome é incluído em cifrão (`$`). Por exemplo, `$thumbnail$` pode ser a Predefinição de imagem projetada para mostrar imagens mestre no tamanho da miniatura. Consulte [Vincular urls ao aplicativo da Web](linking-urls-web-application.md#linking_urls_to_your_web_application).
