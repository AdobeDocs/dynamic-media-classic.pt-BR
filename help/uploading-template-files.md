---
title: Fazer upload de arquivos de modelo
description: Saiba como carregar arquivos de modelo no Adobe Dynamic Media Classic.
uuid: e19979b5-3f41-49c5-99aa-107ede3be98c
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 75658717-5c39-473e-9d32-718d00706310
feature: Dynamic Media Classic
role: User
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Fazer upload de arquivos de modelo{#uploading-template-files}

Faça upload dos arquivos necessários para o modelo no Adobe Dynamic Media Classic antes de começar a criar o modelo. Você pode criar modelos a partir de um PSD Adobe® Photoshop® ou de um arquivo de imagem. Imagens TIFF e PNG são recomendadas porque permitem transparência.

>[!NOTE]
>
>A Adobe Dynamic Media Classic recomenda usar imagens de TIFF ou PSD transparentes em seus modelos no tamanho exato que você deseja exibir em seu site. Ao publicar o modelo, chame a imagem com uma Predefinição de imagem que também seja do mesmo tamanho. Prestar atenção ao tamanho garante que o modelo não seja redimensionado (reamostragem) em um tamanho maior ou menor do que o tamanho em que foi projetado.

Os modelos podem ser criados a partir de arquivos PSD ou arquivos de imagem do Adobe Photoshop.

Para obter instruções detalhadas sobre o upload de arquivos, consulte [Fazer upload de arquivos](uploading-files.md#uploading_files). Lembre-se do seguinte ao fazer upload de arquivos de modelo:

* Se você estiver carregando um arquivo PSD, é possível criar um modelo a partir dele. O Adobe Dynamic Media Classic cria uma imagem separada para cada camada no PSD. Na caixa de diálogo Fazer Upload das Opções de Job, selecione **[!UICONTROL Photoshop Options]** e selecione **[!UICONTROL Maintain Layers]** e **[!UICONTROL Create Template]**. Em seguida, escolha uma opção no **[!UICONTROL Layer Naming]** lista suspensa para nomear as imagens que o Adobe Dynamic Media Classic cria a partir de camadas no PSD.
Consulte [opções de upload de PSD](psd-files.md#psd_upload_options).

<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [Fazer upload dos arquivos](uploading-files.md#uploading_your_files)
>* [Trabalhar com arquivos PSD](psd-files.md#working_with_psd_files)

