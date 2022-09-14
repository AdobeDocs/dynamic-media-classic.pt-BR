---
title: Especificar opções de exportação disponíveis para usuários do Media Portal
description: Saiba como especificar opções de exportação que estão disponíveis para usuários do Media Portal no Adobe Dynamic Media Classic.
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Especificar opções de exportação disponíveis para usuários do Media Portal {#specifying-export-options-available-to-media-portal-users}

Se o administrador conceder permissão, os usuários do Media Portal poderão reformatar imagens à medida que as exportarem. Por exemplo, eles podem alterar o tamanho, o formato de arquivo e a qualidade da imagem. A reformatação automática de imagens conforme são exportadas economiza tempo, não sendo necessário reformatar as imagens separadamente. Além disso, os administradores podem criar uma predefinição — uma seleção preestabelecida de configurações de formato de imagem. Você pode usar uma predefinição ao exportar imagens para reformatá-las de acordo com as especificações da sua empresa.

As duas restrições a seguir se aplicam se você exportar ativos de imagem por meio de uma conversão definida pelo usuário ou se exportar as imagens primárias originais:

* O arquivo de exportação Zip compactado tem um tamanho máximo de arquivo de 1 GB para o trabalho de exportação.
* Você pode ter no máximo 500 ativos totais por trabalho de exportação.

Consulte também [Exportar ativos do Adobe Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**Para especificar opções de exportação disponíveis para usuários do Media Portal:**

1. Na barra Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.
1. Na janela Predefinições de imagem, selecione uma das opções a seguir:

   * **Habilitar conversão definida pelo usuário** - Quando selecionada, essa opção permite que os usuários escolham outro na variável **[!UICONTROL Size]** lista suspensa na janela Exportar ativos selecionados . Em seguida, os usuários podem escolher uma unidade de medida, como pixels ou centímetros, e especificar a largura e a altura desejadas. Quando eles exportam ou baixam esses arquivos, os arquivos de imagem são reformatados.

      When **[!UICONTROL pixels]** são escolhidos de entre **[!UICONTROL Size]** na lista suspensa, a largura x altura da imagem resultante não pode exceder 100 milhões de pixels. Esse tamanho equivale a 10.000 x 10.000 pixels para uma imagem quadrada, ou aproximadamente 8.000 x 12.000 pixels para uma imagem com relação de aspecto 2x3. Essa limitação de tamanho não se aplica se você exportar as imagens primárias originais.

      Desmarque essa opção se desejar que os usuários baixem arquivos sem reformatá-los à medida que forem baixados.

   * **Ativar Exportação Original** - Permite exportar as imagens primárias originais. No **[!UICONTROL Export Selected Assets]** , os usuários podem abrir o **[!UICONTROL Conversion]** e escolha **[!UICONTROL Export Original]** para exportar arquivos originais. Desmarque essa opção se desejar forçar os usuários a escolher uma predefinição de imagem ou escolher opções de conversão ao exportar imagens.

>[!MORELIKETHIS]
>
>* [Predefinições de imagem](application-setup.md#image_presets)
>* [Escolher permissões de acesso à predefinição de imagem para um grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

