---
title: Upload de arquivos de modelo
description: Saiba como fazer upload de arquivos de modelo no Adobe Dynamic Media Classic.
uuid: e19979b5-3f41-49c5-99aa-107ede3be98c
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 75658717-5c39-473e-9d32-718d00706310
feature: Dynamic Media Classic
role: User
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
source-git-commit: 8bc49ae3704f0551c70d68a0ddd63725bdcc645c
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Upload de arquivos de modelo{#uploading-template-files}

Faça upload dos arquivos necessários para seu modelo no Adobe Dynamic Media Classic antes de começar a criar o modelo. Você pode criar modelos a partir de um Adobe® Photoshop® PSD ou um arquivo de imagem. Imagens TIFF e PNG são recomendadas porque permitem transparência.

>[!NOTE]
>
>O Adobe Dynamic Media Classic recomenda o uso de imagens TIFF ou PSD transparentes em seus modelos com o tamanho exato que você deseja que sejam exibidas em seu site. Ao publicar o modelo, chame a imagem com uma predefinição de imagem que também tenha o mesmo tamanho. Prestar atenção ao tamanho garante que o modelo não seja redimensionado (refeito) em um tamanho maior ou menor do que o tamanho em que foi projetado.

Os modelos podem ser criados a partir de arquivos Adobe Photoshop PSD ou arquivos de imagem.

Para obter instruções detalhadas sobre como fazer upload de arquivos, consulte [Fazer upload de arquivos](uploading-files.md#uploading_files). Lembre-se do seguinte ao carregar arquivos de modelo:

* Se você estiver carregando um arquivo PSD, poderá criar um modelo a partir dele. O Adobe Dynamic Media Classic cria uma imagem separada para cada camada no PSD. Na caixa de diálogo Upload Job Options , selecione **[!UICONTROL Photoshop Options]** e selecione **[!UICONTROL Maintain Layers]** e **[!UICONTROL Create Template]**. Em seguida, escolha uma opção na lista suspensa **[!UICONTROL Layer Naming]** para nomear as imagens que o Adobe Dynamic Media Classic cria das camadas no PSD.
Consulte [Opções de carregamento de PSD](psd-files.md#psd_upload_options).

<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [Fazer upload de seus arquivos](uploading-files.md#uploading_your_files)
>* [Trabalhar com arquivos PSD](psd-files.md#working_with_psd_files)

