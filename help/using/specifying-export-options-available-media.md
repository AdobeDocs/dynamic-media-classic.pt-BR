---
title: Especifique as opções de exportação disponíveis para os usuários do Portal de mídia
description: Saiba como especificar opções de exportação que estão disponíveis para usuários do Portal de mídia no Adobe Dynamic Media Classic.
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Especifique as opções de exportação disponíveis para os usuários do Portal de mídia {#specifying-export-options-available-to-media-portal-users}

Se o administrador conceder permissão, os usuários do Portal de mídia poderão reformatar as imagens à medida que forem exportadas. Por exemplo, eles podem alterar o tamanho, o formato do arquivo e a qualidade da imagem. A reformatação automática de imagens à medida que são exportadas economiza tempo, pois não é necessário reformatar as imagens separadamente. Além disso, os administradores podem criar uma predefinição, uma seleção preestabelecida de configurações de formato de imagem. É possível usar uma predefinição ao exportar imagens para reformatá-las de acordo com as especificações da sua empresa.

As duas restrições a seguir se aplicam se você exportar ativos de imagem por meio de uma conversão definida pelo usuário ou se exportar imagens primárias originais:

* O arquivo de exportação compactado Zip tem um tamanho máximo de arquivo de 1 GB para o trabalho de exportação.
* Você pode ter um máximo de 500 ativos totais por trabalho de exportação.

Consulte também [Exportar ativos do Adobe Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**Para especificar opções de exportação disponíveis para usuários do Portal de mídia:**

1. Na barra de Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.
1. Na janela Predefinições de imagem, selecione qualquer uma das seguintes opções:

   * **Ativar conversão definida pelo usuário** - Quando selecionada, essa opção permite que os usuários escolham outras opções na **[!UICONTROL Size]** na janela Exportar ativos selecionados. Os usuários podem então escolher uma unidade de medida, como pixels ou centímetros, e especificar a largura e a altura desejadas. Quando eles exportam ou baixam esses arquivos, os arquivos de imagem são reformatados.

      Quando **[!UICONTROL pixels]** são escolhidos entre os **[!UICONTROL Size]** lista suspensa, a largura x altura da imagem resultante não pode exceder 100 milhões de pixels. Esse tamanho equivale a 10.000 x 10.000 pixels para uma imagem quadrada, ou aproximadamente 8.000 x 12.000 pixels para uma imagem com proporção 2x3. Essa limitação de tamanho não se aplica se você exportar imagens primárias originais.

      Desmarque essa opção se desejar que os usuários baixem os arquivos sem reformatar a maneira como eles são baixados.

   * **Ativar exportação original** - Permite exportar as imagens principais originais. No **[!UICONTROL Export Selected Assets]** , os usuários podem abrir a **[!UICONTROL Conversion]** menu suspenso e escolha **[!UICONTROL Export Original]** para exportar arquivos originais. Desmarque essa opção se quiser forçar os usuários a escolher uma predefinição de imagem ou escolher opções de conversão ao exportar imagens.

>[!MORELIKETHIS]
>
>* [Predefinições da imagem](application-setup.md#image_presets)
>* [Escolher permissões de acesso de Predefinição de imagem para um grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

