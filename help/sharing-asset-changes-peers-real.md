---
title: Compartilhar alterações de ativos com colegas em tempo real
description: Saiba como compartilhar alterações de ativos com colegas em tempo real no Adobe Dynamic Media Classic.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Compartilhar alterações de ativos com colegas em tempo real{#sharing-asset-changes-with-peers-in-real-time}

Com várias cópias do Adobe Dynamic Media Classic em execução em vários computadores na mesma empresa, as seguintes ações de qualquer cliente Adobe Dynamic Media Classic são atualizadas em tempo real com todos os clientes peer:

* Editar um ativo (construtor, editor de imagens e assim por diante)
* Renomear um ativo
* Excluir um ativo
* Mover um ativo
* Fazer upload de um ou mais ativos (desktop e FTP)
* Criar, excluir ou renomear uma pasta

Depois que uma alteração é feita no cliente de origem, todos os clientes peer que entraram na mesma empresa são atualizados com a alteração. As alterações são feitas a pares sem notificação, a menos que o par edite um ativo em alteração em qualquer um dos editores ou construtores de imagem.

Ao fazer logon, você será solicitado a permitir ou negar atualizações de peer. Você pode &quot;lembrar&quot; a escolha para ser solicitado apenas uma vez. Para limpar sua escolha, exclua o site apropriado do painel Peer Assisted Networking nas Configurações globais.

Se você estiver editando um ativo que é alterado por um par, será solicitado a assimilar a alteração no construtor ou editor. Se você escolher **[!UICONTROL Yes]**, o construtor ou editor descarta qualquer alteração feita no ativo e importa o ativo atualizado. Se você escolher **[!UICONTROL No]**, o ativo permanece inalterado no construtor ou editor e quaisquer alterações feitas persistem nessa sessão.

Ao salvar o ativo, você é notificado de que existe uma versão mais recente e perguntado se deseja substituir o ativo por suas alterações.
