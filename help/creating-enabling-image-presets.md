---
title: Criação e ativação de predefinições de imagens
description: Saiba como criar e ativar predefinições de imagens.
uuid: 62cfc6fa-da91-4c42-a3ed-10956384d633
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 84257b2a-681c-4fe9-a6e5-3633c1d61d8c
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Criação e ativação de predefinições de imagens{#creating-and-enabling-image-presets}

Quando os usuários exportam ativos de imagem usando o Media Portal, eles podem escolher uma Predefinição de imagem na caixa de diálogo Exportar ativos selecionados. Uma predefinição de imagem é uma coleção de configurações predefinidas que mudam o tamanho, a qualidade da imagem, o formato, a resolução e outros aspectos da aparência de uma imagem quando ela é exportada.

Os administradores do Portal de mídia podem criar predefinições de imagens para controlar como as imagens são reformatadas quando são exportadas. As predefinições de imagens reformatam imagens de acordo com as especificações da sua empresa quando os usuários exportam imagens do Dynamic Media Classic. Em vez de reformatar imagens sozinhas, os usuários as exportam para as especificações precisas de uma predefinição de imagem.

As seguintes restrições se aplicam quando você exporta ativos de imagem:

* A largura x altura deve ser menor ou igual a 100 MB por imagem. Por exemplo, a imagem não pode exceder 10K x 10K, ou qualquer variação de aspecto abaixo, como 8K x 12K.
* Existe um tamanho de arquivo total máximo de 1 GB por trabalho de exportação.
* É possível ter no máximo 500 ativos por trabalho de exportação.

>[!NOTE]
>
>Essas restrições se aplicam apenas à exportação de ativos de imagem derivados, não à exportação de arquivos principais.

Para criar predefinições de imagens, consulte [Predefinições de imagens](application-setup.md#image_presets).

Para permitir que os usuários escolham Predefinições de imagem quando exportam arquivos, consulte [Especificar opções de exportação disponíveis para os usuários do Portal de mídia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

Para escolher quais predefinições de imagens estão disponíveis para os membros de um grupo, consulte [Escolher permissões de acesso à predefinição de imagens para um grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).
