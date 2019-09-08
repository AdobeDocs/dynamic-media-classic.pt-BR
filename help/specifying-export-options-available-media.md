---
title: Especificação das opções de exportação disponíveis para usuários do Media Portal
seo-title: Especificação das opções de exportação disponíveis para usuários do Media Portal
description: 'null'
seo-description: Saiba como especificar opções de exportação que estão disponíveis para usuários do Media Portal.
uuid: 5258 b 8 a 4-0704-43 cd -97 d 1-c 9 af 2 e 4 e 298 b
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 9 bfd 95 da -3714-4 e 38-98 af -331 a 04 c 685 f 5
translation-type: tm+mt
source-git-commit: 0f6c8e6ac69e29aab7a48425aab76c10170d9ddf

---


# Especificação das opções de exportação disponíveis para usuários do Media Portal {#specifying-export-options-available-to-media-portal-users}

Se o administrador lhes conceder permissão, os usuários do Media Portal poderão reformatar as imagens à medida que elas os exportarem. Por exemplo, eles podem alterar o tamanho, o formato do arquivo e a qualidade da imagem. Reformatar automaticamente imagens conforme elas são exportadas economiza tempo, pois não precisa reformatar as imagens separadamente. Além disso, os administradores podem criar uma seleção pré-estabelecida de configurações de formato de imagem. Você pode usar uma predefinição ao exportar imagens para reformá-las para as especificações de sua empresa.

As duas restrições a seguir se aplicam se você exportar ativos de imagem por meio de uma conversão definida pelo usuário ou se exportar imagens mestre originais:

* O arquivo de exportação compactado compactado tem um tamanho máximo de arquivo de 1 GB para o trabalho de exportação.
* Você pode ter no máximo 500 ativos por tarefa de exportação.

Consulte [também Exportar ativos do Sistema de publicação Scene 7](exporting-assets-scene7-publishing-system.md#exporting_assets_from_scene7_publishing_system).

**Especificação das opções de exportação disponíveis para usuários do Media Portal**

1. Clique **em Configuração** &gt; **Predefinições de imagens**.
1. Na janela Predefinições de imagens, selecione um dos seguintes:

   **Habilitar conversão definida pelo usuário** quando selecionada, essa opção permite que os usuários escolham outros na lista suspensa Tamanho na janela Exportar ativos selecionados. Os usuários podem escolher uma unidade de medida, como pixels ou centímetros, e especificar a largura e a altura desejadas. Quando eles exportam ou baixam esses arquivos, os arquivos de imagem são reformatados.

   Quando **os pixels** são escolhidos na lista suspensa **Tamanho** , a largura da imagem resultante x altura não pode exceder 100 milhões de pixels. Esse tamanho equivale a 10,000 x 10,000 pixels de uma imagem quadrada, ou aproximadamente 8,000 x 12,000 pixels para uma imagem de proporção de 2 x 3. Essa limitação de tamanho não se aplica se você exportar imagens mestre originais.

   Desmarque essa opção se desejar que os usuários baixem arquivos sem reformatá-los à medida que são baixados.

   **Habilitar Exportação original** Permite exportar imagens mestre originais. No painel Exportar ativos selecionados, os usuários podem abrir o menu suspenso Conversão e escolher Exportar original para exportar arquivos originais. Desmarque essa opção se quiser forçar os usuários a escolher uma Predefinição de imagem ou escolher opções de conversão ao exportar imagens.

>[!MORELIKETHIS]
>
>* [Predefinições de imagens](application-setup.md#image_presets)
>* [Escolher permissões de acesso a predefinição de imagem para um grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

