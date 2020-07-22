---
title: Especificação de opções de exportação disponíveis para usuários do Media Portal
seo-title: Especificação de opções de exportação disponíveis para usuários do Media Portal
description: nulo
seo-description: Saiba como especificar opções de exportação que estão disponíveis para usuários do Portal de mídia.
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
translation-type: tm+mt
source-git-commit: 38f5cf5264f9775a225d354ed9dc2f6caee236f2
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---


# Especificação de opções de exportação disponíveis para usuários do Media Portal {#specifying-export-options-available-to-media-portal-users}

Se o administrador conceder a eles permissão, os usuários do Portal de mídia poderão reformatar as imagens à medida que as exportarem. Por exemplo, eles podem alterar o tamanho, o formato de arquivo e a qualidade da imagem. A reformatação automática de imagens à medida que são exportadas economiza tempo ao não precisar reformatar imagens separadamente. Além disso, os administradores podem criar uma predefinição — uma seleção preestabelecida das configurações de formato de imagem. Você pode usar uma predefinição ao exportar imagens para reformatá-las de acordo com as especificações da sua empresa.

As duas restrições a seguir se aplicam se você exportar ativos de imagem por meio de uma conversão definida pelo usuário ou se exportar imagens principais originais:

* O arquivo compactado de exportação do Zip tem um tamanho máximo de arquivo de 1 GB para o trabalho de exportação.
* É possível ter no máximo 500 ativos por trabalho de exportação.

Consulte também [Exportar ativos do Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**Especificação de opções de exportação disponíveis para usuários do Media Portal**

1. Clique em **Configuração** > Predefinições **de imagem**.
1. Na janela Predefinições de imagem, selecione uma das seguintes opções:

   * **Ativar conversão definida pelo usuário** Quando selecionada, essa opção permite que os usuários escolham outro na lista suspensa Tamanho na janela Exportar ativos selecionados. Os usuários podem escolher uma unidade de medida, como pixels ou centímetros, e especificar a largura e a altura desejadas. Quando eles exportam ou baixam esses arquivos, os arquivos de imagem são reformatados.

      Quando **os pixels** são escolhidos na lista **suspensa Tamanho**, a largura x altura da imagem resultante não pode exceder 100 milhões de pixels. Esse tamanho equivale a 10.000 x 10.000 pixels para uma imagem quadrada, ou aproximadamente 8.000 x 12.000 pixels para uma imagem com proporção de tela 2x3. Essa limitação de tamanho não se aplica se você exportar imagens principais originais.

      Desmarque essa opção se desejar que os usuários baixem arquivos sem reformatá-los durante o download.

   * **Ativar Exportar original** permite exportar imagens principais originais. No painel Exportar ativos selecionados, os usuários podem abrir o menu suspenso Conversão e escolher Exportar original para exportar arquivos originais. Desmarque essa opção se desejar forçar os usuários a escolher uma Predefinição de imagem ou escolher opções de conversão ao exportar imagens.

>[!MORELIKETHIS]
>
>* [Predefinições de imagem](application-setup.md#image_presets)
>* [Escolher permissões de acesso à predefinição de imagem para um grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

