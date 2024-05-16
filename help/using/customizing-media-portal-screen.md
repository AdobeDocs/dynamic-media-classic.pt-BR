---
title: Personalizar a tela do Portal de mídia
description: Saiba como personalizar a tela do Portal de mídia no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Personalizar a tela do Portal de mídia{#customizing-the-media-portal-screen}

As configurações de estilo do Portal de mídia permitem que você marque a tela Portal de mídia com o logotipo e as cores da sua empresa. Use as configurações de estilo para colocar a marca da sua empresa no Portal de mídia.

Para acessar as configurações de estilo, vá para **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Style Settings]**. Certifique-se de selecionar **[!UICONTROL Save]** para salvar suas configurações depois de criá-las. É possível selecionar **[!UICONTROL Restore]** para retornar às configurações padrão. À medida que você faz suas escolhas, o painel Visualização mostra como elas são exibidas.

* **[!UICONTROL Logo]**: Selecionar **[!UICONTROL Browse]** e escolha um gráfico na janela Selecionar imagem de logotipo.

* **[!UICONTROL Application]**: crie uma mistura de cores de gradiente fazendo escolhas nos menus das Cores de gradiente de plano de fundo.

* **[!UICONTROL Tree]**: escolha uma cor de rolagem (a cor que aparece quando você move o ponteiro sobre um item) e a cor de seleção (a cor que aparece quando você seleciona um item).

* **[!UICONTROL Accordion]**: escolha as cores do plano de fundo, um estilo de borda, a sobreposição e as cores selecionadas para o acordeão exibido no lado direito da tela na exibição de Detalhes.

* **[!UICONTROL Accordion Header]**: escolha se o texto deve ficar em negrito no cabeçalho do acordeão.

* **[!UICONTROL Datagrid]**: escolha as cores para a linha de cabeçalho nas grades de dados.

* **[!UICONTROL Alert]**: Escolha uma cor de fundo para as caixas de mensagem de alerta.

* **[!UICONTROL Progress Bar]**: escolha uma cor para a barra que indica o progresso dos uploads e downloads.

Para que os usuários do Media Portal vejam as configurações de estilo escolhidas, eles devem anexar `?company=(company name)` ao URL com o qual acessam o Media Portal. Por exemplo, para ver as configurações de estilo, os usuários do Portal de mídia que acessam a empresa PortalCo no seguinte endereço:

`https://s7sps1.scene7.com/MediaPortal`

Em vez disso, use o seguinte URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

A inclusão do nome da empresa no URL permite que o Media Portal reconheça a empresa que um usuário deseja acessar e aplique as configurações de estilo da empresa de acordo.

Você pode saber mais sobre como comunicar alterações de URL aos usuários do Media Portal e configurar uma mensagem de email de boas-vindas para que novos usuários recebam o URL correto do Media Portal.

Consulte [Configure a mensagem de e-mail de boas-vindas para os usuários do Portal de mídia](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
