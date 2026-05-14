---
title: Sobre conteúdo gerado pelo usuário no Adobe Dynamic Media Classic
description: Uma introdução ao conteúdo gerado pelo usuário.
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
feature: Dynamic Media Classic
role: Admin,User
exl-id: 14729192-7b9d-4f42-99da-6564a3f35959
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:34:44.287Z'
TQID: 'https://experienceleague.adobe.com/SwNEO6U33qx45AECK79nff9f9kABWuOdq91d4X8SHd0'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 179
ht-degree: 0%

---

# Sobre conteúdo gerado pelo usuário no Adobe Dynamic Media Classic {#about-user-generated-content}

O uso do UGC (conteúdo gerado pelo usuário) consiste em fazer upload de ativos para um repositório de armazenamento dedicado do Adobe Dynamic Media Classic e executar operações relacionadas.

O UGC é compatível com formatos de arquivo de imagem rasterizada BMP, GIF, JPG, PNG, PSD, TIFF.

>[!IMPORTANT]
>
>A partir de 1 de maio de 2023, os ativos UGC no Dynamic Media estarão disponíveis para uso por até 60 dias a partir da data do upload. Após 60 dias, os ativos serão removidos.

<!-- * Vector: AI, EPS (EPS files from Adobe Illustrator 2018 are not supported), PDF (only when the PDF file is previously opened and saved in Adobe Illustrator CS6) -->

>[!NOTE]
>
>O suporte a ativos de imagem vetorial UGC novos ou existentes no Adobe Dynamic Media Classic terminou em 30 de setembro de 2021.

Antes de carregar ativos, você obtém uma chave de segredo compartilhado. Você usa essa chave para recuperar um token de upload. Você envia o token de upload ao fazer upload de ativos e executar outras tarefas de UGC.

Depois de recuperar uma chave de segredo compartilhado e fazer upload do token, você pode executar as seguintes operações para o conteúdo gerado pelo usuário:

* Fazer upload de um ativo.
* Obter metadados de ativos de imagem.
* Exclua um ativo carregado.
* Obter informações sobre o uso de espaço em disco de uma empresa.
