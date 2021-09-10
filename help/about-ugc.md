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
source-git-commit: 30f1aa8c30c0a1f7cf0f4298530e1e80597d7c3e
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# Sobre conteúdo gerado pelo usuário no Adobe Dynamic Media Classic {#about-user-generated-content}

O uso de UGC (conteúdo gerado pelo usuário) consiste em carregar ativos em um repositório de armazenamento dedicado do Adobe Dynamic Media Classic e executar operações relacionadas.

O UGC oferece suporte aos seguintes formatos de arquivo:

* Rastreamento: JPG, PNG, TIFF
* Vetor: AI, EPS (arquivos EPS do Adobe Illustrator 2018 não são compatíveis), PDF (somente quando o arquivo PDF é aberto e salvo anteriormente no Adobe Illustrator CS6)

>[!IMPORTANT]
>
>O suporte para ativos de imagem vetorial UGC novos ou existentes no Adobe Dynamic Media Classic será encerrado em 30 de setembro de 2021.

Antes de fazer upload de ativos, você obtém uma chave secreta compartilhada. Use essa chave para recuperar um token de upload. Você envia o token de upload quando carrega ativos e executa outras tarefas UGC.

Depois de recuperar uma chave secreta compartilhada e um token de upload, você pode executar as seguintes operações para o conteúdo gerado pelo usuário:

* Faça upload de um ativo.
* Obter metadados de ativos de imagem.
* Exclua um ativo carregado.
* Obtenha informações sobre o uso de espaço em disco de uma empresa.
