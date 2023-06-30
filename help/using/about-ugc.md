---
title: Sobre conteúdo gerado pelo usuário no Adobe Dynamic Media Classic
description: Uma introdução ao conteúdo gerado pelo usuário.
uuid: ba867a6a-84a4-4968-9a77-712f3ce5dad5
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
discoiquuid: c1594abf-8cc2-46dd-88bf-af93db7db607
feature: Dynamic Media Classic
role: Admin,User
exl-id: 14729192-7b9d-4f42-99da-6564a3f35959
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Sobre conteúdo gerado pelo usuário no Adobe Dynamic Media Classic {#about-user-generated-content}

O uso do UGC (conteúdo gerado pelo usuário) consiste em fazer upload de ativos para um repositório de armazenamento dedicado do Adobe Dynamic Media Classic e executar operações relacionadas.

O UGC suporta formatos de arquivos de imagem rasterizada BMP, GIF, JPG, PNG, PSD, TIFF.

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
