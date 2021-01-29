---
title: Compartilhar alterações de ativos com colegas em tempo real
description: Saiba como compartilhar alterações de ativos com colegas em tempo real.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---


# Compartilhar alterações de ativos com colegas em tempo real{#sharing-asset-changes-with-peers-in-real-time}

Com várias cópias do Dynamic Media Classic em execução em um ou mais computadores na mesma empresa, as seguintes ações de qualquer cliente Dynamic Media Classic são atualizadas em tempo real com todos os clientes peer:

* Editar um ativo (construtor, editor de imagens etc.)
* Renomear um ativo
* Excluir um ativo
* Mover um ativo
* Carregar um ou mais ativos (desktop e FTP)
* Criar, excluir ou renomear uma pasta

Depois que uma alteração é feita no cliente de origem, todos os clientes de mesmo nível conectados à mesma empresa são atualizados com a alteração. As alterações são feitas em pares sem notificação, a menos que o par esteja editando um ativo em alteração em qualquer um dos editores ou construtores de imagem.

Ao fazer logon, você será solicitado a permitir ou negar atualizações de mesmo nível. Você pode &quot;lembrar&quot; a escolha para que seja solicitado apenas uma vez. Para limpar sua escolha, exclua o site apropriado do painel Rede de pares no Global Settings.

Se você estiver editando um ativo que é alterado por um par, será solicitado a assimilar a alteração no construtor ou editor. Se você escolher Sim, o construtor ou editor descartará quaisquer alterações feitas no ativo e importará o ativo atualizado. Se você escolher Não, o ativo permanecerá inalterado no construtor ou editor e quaisquer alterações feitas persistirão nessa sessão.

Ao salvar o ativo, você é notificado de que existe uma versão mais recente e perguntado se deseja sobrescrever o ativo com suas alterações.
