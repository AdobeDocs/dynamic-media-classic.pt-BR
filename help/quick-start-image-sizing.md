---
title: '"Início rápido: Dimensionamento de imagem"'
description: Uma introdução e o início rápido do dimensionamento de imagem para ajudá-lo a ativar e executar rapidamente com as técnicas de dimensionamento de imagem.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Gerenciamento de ativos
role: Business Practitioner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Início rápido: Dimensionamento de imagem{#quick-start-image-sizing}

O Dimensionamento de imagem refere-se à capacidade do Dynamic Media Classic de criar várias imagens derivadas com base em uma única imagem de alta resolução. Em vez de criar manualmente várias imagens, por exemplo, uma miniatura e uma imagem ampliada, para seu site ou aplicativo, você fornece uma única imagem principal. O Dynamic Media Classic gera todas as imagens modificadas da mesma maneira que você as solicita. Ser capaz de fornecer imagens dinamicamente de uma única imagem principal tem muitas vantagens:

* Não é necessário criar manualmente várias cópias da imagem em tamanhos diferentes. Você fornece uma imagem principal para o Dynamic Media Classic, e o Dynamic Media Classic gera derivados de tamanhos diferentes da imagem principal.
* Você pode alterar rapidamente o tamanho de um tipo de imagem em todo o site ou aplicativo. Por exemplo, para alterar todas as imagens em miniatura, você pode modificar a predefinição de imagem em &quot;miniatura&quot;. Uma Predefinição de imagem — é semelhante a uma macro — é uma coleção de atributos de tamanho e formatação. Você pode modificar a predefinição de imagem de &quot;miniatura&quot; para alterar o tamanho de todas as imagens em miniatura em seu site ou aplicativo.
* Não é necessário gerenciar os mestres e todos os vários derivados em qualquer um dos sistemas de gerenciamento de conteúdo ou ativos internamente ou externamente.

![Você pode criar várias imagens derivadas em diferentes tamanhos do mesmo arquivo principal de alta resolução.](/help/assets/is_derivative_sizes_popup.png)

**Início rápido**

Este Início rápido de dimensionamento de imagem foi projetado para ajudar você a ativar e executar rapidamente com as técnicas de dimensionamento de imagem no Dynamic Media Classic. Siga as etapas de 1 a 5. Depois de cada etapa é uma referência cruzada onde você pode encontrar mais informações, se precisar.

**1. Upload de imagens principais**

Comece carregando suas imagens principais no Dynamic Media Classic. Quanto ao tamanho, o Dynamic Media Classic recomenda o uso de imagens que são o maior tamanho que você prevê usar em seu site ou aplicativo. Por exemplo, se você quiser que os visualizadores ampliem imagens, carregue imagens que tenham pelo menos 2000 pixels na maior dimensão. O Dynamic Media Classic é compatível com muitos formatos de arquivo de imagem, mas imagens TIFF e PNG sem perdas são recomendadas.

Selecione o botão Fazer upload na barra Navegação global para fazer upload de arquivos do seu computador para uma pasta no Dynamic Media Classic. Consulte [Upload de imagens principais](uploading-master-images.md#uploading_master_images).

**2. Configuração de predefinições de imagens**

Como uma macro, uma Predefinição de imagem é uma coleção de comandos predefinidos de tamanho e formatação salvos em um nome. Uma predefinição de imagem governa o tamanho e a formatação com que as imagens são entregues dos servidores de imagem da Dynamic Media. Você pode configurar as Predefinições de imagem por conta própria, se tiver o status de administrador da empresa. O Dynamic Media Classic também vem com Predefinições de imagem padrão, e você pode usá-las para fornecer imagens dinamicamente.

Para criar uma Predefinição de imagem (se você for um administrador), escolha Configuração > Configuração do aplicativo. Na tela Configuração, exiba as opções de Configuração do aplicativo e escolha Predefinições de imagem. Em seguida, clique em **Adicionar** ou **Editar** para criar uma Predefinição de imagem.

A Predefinição de imagem criada é adicionada ao menu Predefinição de imagem na tela Visualização. Você pode usar sua nova Predefinição de imagem para exibir imagens dinamicamente em seus sites e aplicativos. Consulte [Configuração de predefinições de imagem](setting-image-presets.md#setting_up_image_presets).

**3. Visualização de predefinições de imagem**

A próxima etapa é visualizar as Predefinições de imagem que seu administrador configurou nos diferentes tamanhos predefinidos.

Para explorar Predefinições de imagem, clique em **Configurar** > **Predefinições de imagem** e navegue até uma Predefinição de imagem.

Experimente com diferentes predefinições de imagem. Descubra a aparência da imagem quando ela é entregue dinamicamente ao seu site ou aplicativo em diferentes tamanhos.

Consulte [Visualização de um ativo de imagem com base em sua Predefinição de imagem](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

**4. Publicar suas imagens principais**

A publicação dos arquivos de imagem principais tem dois objetivos essenciais:

* Publique suas imagens principais nos Servidores de Imagem da Dynamic Media para que as imagens possam ser entregues dinamicamente ao seu site e aplicativo.
* A publicação ativa as cadeias de caracteres do URL para chamar imagens dos Servidores de Imagem da Dynamic Media para o site ou aplicativo. Após a publicação, você pode copiar e colocar os URLs gerados pelo Dynamic Media Classic, conforme necessário, em seu site ou aplicativo.

Selecione o botão Publicar na barra Navegação global para iniciar uma publicação. Na caixa de diálogo Publicar , clique em **[!UICONTROL Submit Publish]**. Consulte [Publicação de imagens principais](publishing-master-images.md#publishing_master_images).

**5. Vincular URLs ao aplicativo da Web:**

O Dynamic Media Classic cria sequências de chamada de URL para imagens. Ao publicar imagens nos Servidores de imagem da Dynamic Media, os URLs ficam ativos. Você pode copiar essas cadeias de caracteres do URL no Painel de navegação (na Exibição de detalhes) ou na tela de Visualização. Depois de copiar as cadeias de caracteres do URL, você pode usá-las em seu site e aplicativos. O URL para dimensionamento de imagem substitui a referência a um nome de imagem estática no código da página da Web. O URL faz referência a um nome de imagem principal, que é substituído pelo seu banco de dados para cada nova imagem ser exibida.

As cadeias de caracteres de URL geradas com predefinições de imagem contêm o nome de uma predefinição de imagem. Esse nome é incluído nos sinais de dólar (`$`). Por exemplo, `$thumbnail$` pode ser a Predefinição de imagem projetada para mostrar imagens principais no tamanho da miniatura. Consulte [Vincular URLs ao aplicativo Web](linking-urls-web-application.md#linking_urls_to_your_web_application).
