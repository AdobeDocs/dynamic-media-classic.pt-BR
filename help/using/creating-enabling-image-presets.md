---
title: Criar e ativar predefinições de imagem
description: Saiba como criar e ativar predefinições de imagens no Adobe Dynamic Media Classic.
uuid: 62cfc6fa-da91-4c42-a3ed-10956384d633
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 84257b2a-681c-4fe9-a6e5-3633c1d61d8c
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Criar e ativar predefinições de imagem{#creating-and-enabling-image-presets}

Quando os usuários exportam ativos de imagem usando o Media Portal, eles podem escolher uma Predefinição de imagem na caixa de diálogo Exportar ativos selecionados. Uma predefinição de imagem é uma coleção de configurações predefinidas que alteram o tamanho, a qualidade da imagem, o formato, a resolução e outros aspectos da aparência de uma imagem quando ela é exportada.

Os administradores do Portal de mídia podem criar Predefinições de imagem para controlar como as imagens são reformatadas quando são exportadas. As Predefinições de imagem reformatam imagens de acordo com as especificações da sua empresa quando os usuários exportam imagens do Adobe Dynamic Media Classic. Em vez de reformatar imagens por conta própria, os usuários as exportam para as especificações precisas de uma Predefinição de imagem.

As seguintes restrições se aplicam quando você exporta ativos de imagem:

* A largura × altura deve ser inferior ou igual a 100 MB por imagem. Por exemplo, a imagem não pode exceder 10 K × 10 K, ou qualquer variação de aspecto abaixo, como 8 K × 12 K.
* Há um tamanho máximo total de 1 GB por trabalho de exportação.
* Você pode ter um máximo de 500 ativos totais por trabalho de exportação.

>[!NOTE]
>
>Essas restrições se aplicam apenas à exportação de ativos de imagem derivados, não à exportação de arquivos principais.

Para criar Predefinições de imagem, consulte [Predefinições da imagem](application-setup.md#image_presets).

Para permitir que os usuários escolham Predefinições de imagem ao exportar arquivos, consulte [Especificação de opções de exportação disponíveis para usuários do Portal de mídia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

Para escolher quais Predefinições de Imagem estão disponíveis para os membros de um grupo, consulte [Escolher permissões de acesso de Predefinição de imagem para um grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).
