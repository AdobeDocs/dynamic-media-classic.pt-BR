---
title: Compartilhar alterações de ativos com clientes de mesmo nível em tempo real
description: Saiba como compartilhar alterações de ativos com colegas em tempo real no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
autotag-review: '2026-05-13T20:12:54.992Z'
TQID: 'https://experienceleague.adobe.com/Yn5GsnQ4cM3Byk18iEB8Z4uGsTt9FjEZOBP17Yt-K8M'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 4c8d0e861708e8931bbefe55260c7704c43e0ce6
workflow-type: tm+mt
source-wordcount: 283
ht-degree: 0%

---

# Compartilhar alterações de ativos com clientes de mesmo nível em tempo real{#sharing-asset-changes-with-peers-in-real-time}

Há várias instâncias do Adobe Dynamic Media Classic em execução em computadores na mesma organização. Nesse cenário, as seguintes ações de qualquer cliente do Dynamic Media Classic são atualizadas em tempo real em todos os clientes de mesmo nível:

* Editar um ativo (construtor, editor de imagens etc.)
* Renomear um ativo
* Excluir um ativo
* Mover um ativo
* Fazer upload de um ou mais ativos (desktop e FTP)
* Criar, excluir ou renomear uma pasta

Depois que uma alteração é feita no cliente de origem, todos os clientes de mesmo nível conectados à mesma empresa são atualizados com a alteração. As alterações são aplicadas aos colegas automaticamente, desde que o par não esteja editando o ativo em nenhum dos editores ou construtores de imagem.

Ao fazer logon, você será solicitado a permitir ou negar atualizações de colegas. Você pode salvar a escolha para que seja solicitado apenas uma vez. Para limpar sua escolha, exclua o site apropriado do painel Rede assistida entre parceiros em Configurações globais.

Se você estava editando um ativo alterado por um item de mesmo nível, será solicitado a assimilar a alteração no construtor ou editor. Se você escolher **[!UICONTROL Yes]**, o construtor ou editor descartará todas as alterações feitas no ativo e importará o ativo atualizado. Se você escolher **[!UICONTROL No]**, o ativo não será alterado no construtor ou editor e todas as alterações feitas persistirão nessa sessão.

Ao salvar o ativo, você é notificado de que existe uma versão mais recente. Em seguida, será solicitado que você confirme se deseja substituir o ativo pelas alterações.
