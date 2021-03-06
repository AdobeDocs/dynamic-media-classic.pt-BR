---
title: Personalizar a tela do Media Portal
description: Saiba como personalizar a tela do Media Portal no Adobe Dynamic Media Classic.
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Personalizar a tela do Media Portal{#customizing-the-media-portal-screen}

As configurações de estilo do Media Portal permitem que você atribua uma marca à tela do Media Portal com o logotipo e as cores de sua empresa. Use as configurações de estilo para colocar a marca da sua empresa no Media Portal.

Para acessar as configurações de estilo, vá para **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Style Settings]**. Certifique-se de selecionar **[!UICONTROL Save]** para salvar suas configurações depois de marcá-las. Você pode selecionar **[!UICONTROL Restore]** para retornar as configurações padrão. Conforme você faz suas escolhas, o painel Visualização mostra como elas são exibidas.

* **[!UICONTROL Logo]** - Selecione  **[!UICONTROL Browse]** e escolha um gráfico na janela Selecionar imagem do logotipo.

* **[!UICONTROL Application]** - Crie uma mistura de cores de gradiente fazendo escolhas nos menus Cores do gradiente de plano de fundo .

* **[!UICONTROL Tree]** - Escolha uma cor de sobreposição (a cor que aparece quando você move o ponteiro sobre um item) e a cor da seleção (a cor que aparece quando você seleciona um item).

* **[!UICONTROL Accordion]** - Escolha as cores de plano de fundo, um estilo de borda e as cores de rolagem e selecionadas para a opção que aparece no lado direito da tela na exibição Detalhes.

* **[!UICONTROL Accordion Header]** - Escolha se deseja fazer texto na face do cabeçalho acordeão.

* **[!UICONTROL Datagrid]** - Escolha as cores da linha de cabeçalho nas grades de dados.

* **[!UICONTROL Alert]** - Escolha uma cor de plano de fundo para caixas de mensagem de alerta.

* **[!UICONTROL Progress Bar]** - Escolha uma cor para a barra que indique o progresso dos uploads e downloads.

Para que os usuários do Media Portal vejam as configurações de estilo que você escolheu, eles devem anexar `?company=(company name)` ao URL com o qual acessam o Media Portal. Por exemplo, para ver as configurações de estilo, os usuários do Media Portal que acessam a empresa PortalCo no seguinte endereço:

`https://s7sps1.scene7.com/MediaPortal`

Em vez disso, use o seguinte URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

Incluir o nome da empresa no URL permite que o Media Portal reconheça a empresa que um usuário deseja acessar e aplique as configurações de estilo da empresa de acordo.

Você pode saber mais sobre como comunicar alterações de URL a usuários do Media Portal e configurar uma mensagem de email de boas-vindas para que novos usuários recebam o URL correto do Media Portal.

Consulte [Configurar a mensagem de email de boas-vindas para usuários do Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
