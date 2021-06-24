---
title: Compartilhamento de alterações de ativos com colegas em tempo real
description: Saiba como compartilhar alterações de ativos com colegas em tempo real.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic,Gerenciamento de ativos,Colaboração
role: Administrator,Business Practitioner
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
source-git-commit: 9d73e74ffc4a1e7e31c84720a9bae105b6afb1ae
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Compartilhamento de alterações de ativos com colegas em tempo real{#sharing-asset-changes-with-peers-in-real-time}

Com várias cópias do Dynamic Media Classic em execução em um ou mais computadores na mesma empresa, as seguintes ações de qualquer cliente Dynamic Media Classic são atualizadas em tempo real com todos os clientes pares:

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
