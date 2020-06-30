---
title: Aplicativo Adobe Dynamic Media Classic para desktop - Agora disponível
seo-title: Aplicativo Adobe Dynamic Media Classic para desktop - Agora disponível
description: nulo
seo-description: Saiba mais sobre o aplicativo Dynamic Media Classic para desktop.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
translation-type: tm+mt
source-git-commit: 8858ca1482b8a33e3294df345bc2e5fc34483e07
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---


# Agora disponível: Aplicativo de desktop Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Os usuários do Dynamic Media Classic agora têm acesso a uma nova experiência de aplicativo de desktop que não depende mais da tecnologia Adobe Flash no navegador.

Este novo aplicativo está disponível para Windows e MacOS.

>[!IMPORTANT]
>
>Recomendamos que você instale o novo aplicativo Adobe Dynamic Media Classic para desktop até 1º de outubro de 2020. Isso garantirá uma transição suave antes de o Adobe Flash Player ser descontinuado em 31 de dezembro de 2020. Nessa data, você não poderá mais fazer logon na versão do navegador da interface do usuário do Adobe Dynamic Media Classic, rotulada como Scene7 Publishing System no produto.

Consulte as Perguntas frequentes sobre a experiência de logon do [novo Dynamic Media Classic disponível.](/help/new-ui-2020.md)

## Requisitos de sistema para o aplicativo Adobe Dynamic Media Classic para desktop {#system-requirements-dmc-app}

O aplicativo Adobe Dynamic Media Classic para desktop é compatível com os seguintes sistemas operacionais:
* macOS X 10.10 ou mais recente.
* Windows 7 ou mais recente.

## Baixar e instalar o aplicativo Adobe Dynamic Media Classic para desktop {#installation-dmc-app}

1. Desinstale versões mais antigas do aplicativo Dynamic Media Classic para desktop no seu sistema.

1. Baixe o instalador mais recente do aplicativo Adobe Dynamic Media Classic para desktop.

   * [macOS (.dmg) - Download.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)
   * [Windows (.exe) - Download.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)

1. Execute um dos procedimentos a seguir com base no instalador que você baixou.

   * **Para macOS** - Na caixa de **[!UICONTROL Drag & drop to install]** diálogo, arraste **[!UICONTROL Adobe Dynamic Media Classic]** e solte-o **[!UICONTROL Applications]**.

      ![Arraste e solte a instalação no macOS](/help/assets/dragondrop-install1.png)

   * Na **[!UICONTROL Applications]** pasta, toque no ícone Adobe Dynamic Media Classic.
   * Na caixa de diálogo, toque em **[!UICONTROL Open]** para abrir o aplicativo Adobe Dynamic Media Classic para desktop.

      ![Abrir aplicativo baixado](/help/assets/open-dmclassicapp1.png)

   * **No Windows** - execute o binário do instalador e siga as instruções na tela para instalar o aplicativo de desktop.

1. Quando você abre o aplicativo, a nova página de logon do Adobe Dynamic Media Classic é exibida:

   ![Logon no Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Use as mesmas credenciais do navegador para fazer logon no Adobe Dynamic Media Classic.

   Para **[!UICONTROL Server]** usar o, consulte o seguinte mapeamento para o ambiente de produção:

   | URL do navegador | Nome do servidor do aplicativo de desktop |
   |---|---|
   | https://s7sps1.scene7.com/ | Produção de NA (América do Norte) |
   | https://s7sps3.scene7.com/ | Produção da EMEA (Europa, Oriente Médio e África) |
   | https://s7sps5.scene7.com/ | Produção de APAC (Ásia-Pacífico) |

1. Após a interface de usuário de logon, você observará a experiência familiar da interface de usuário do navegador. Você pode carregar sua atividade do dia a dia como de costume na interface do usuário do aplicativo para desktop.

## Limitações conhecidas no Dynamic Media Classic

**_Aplica-se somente ao Windows - há uma limitação no número de arquivos que podem ser carregados por meio da interface do usuário do aplicativo para desktop?_**<br> Sim, um máximo de 150 arquivos pode ser carregado de cada vez por meio da interface do usuário do aplicativo para desktop.

**_Aplica-se ao Windows e macOS - Como alterno entre o empresa?_**<br> Para alternar entre empresas, faça o seguinte:
* No aplicativo Dynamic Media Classic, selecione a nova empresa na lista suspensa empresa.
* Quando o pop-up for exibido, toque em **[!UICONTROL OK]** para sair e fechar o aplicativo.

   ![Reinicie o aplicativo para usar a nova empresa](/help/assets/dmclassic-new-company1.png)
* Reinicie o Dynamic Media Classic e faça logon como de costume para trabalhar com a nova empresa.

## Dicas e truques

**_Não consigo ver o painel Carrinho de mídia na landing page do Dynamic Media Classic._**<br> No Dynamic Media Classic, toque em **[!UICONTROL Setup > Personal Setup]**. Na seção Navegador, verifique se **[!UICONTROL Show MediaPortal Features]** está selecionado (marcado). Toque em **[!UICONTROL Save > Close]**.

**_O estado de publicação (indicador verde) de um ativo não é refletido corretamente._**<br> Na interface do usuário do navegador, um novo logon na interface era necessário para ver o estado correto de publicação dos ativos. No aplicativo de desktop, apresentamos um **[!UICONTROL Refresh]** ícone na barra de ferramentas, à direita do **[!UICONTROL Select None]** botão. Toque no **[!UICONTROL Refresh]** ícone para ver o status mais recente de todos os ativos em uma determinada página. Não é necessário refazer o logon como com a interface do navegador.

![Ícone](/help/assets/refresh-icon1.png)Atualizar ícone *Atualizar*

**_Não vejo predefinições de conjuntos de lotes funcionando no aplicativo de desktop._**<br> Toque em **[!UICONTROL Upload > Job Options > Batch Set Presets]**. Verifique se o relevante **[!UICONTROL Batch Set Preset]** está ativado. Clique em **[!UICONTROL Save and Submit upload]**.
