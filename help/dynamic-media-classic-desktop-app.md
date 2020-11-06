---
title: Aplicativo de desktop Adobe Dynamic Media Classic - Agora disponível
seo-title: Aplicativo de desktop Adobe Dynamic Media Classic - Agora disponível
description: nulo
seo-description: Saiba mais sobre o aplicativo de desktop do Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
translation-type: tm+mt
source-git-commit: 9e7955b2311496e58e9e973c8f579b2f256c55cb
workflow-type: tm+mt
source-wordcount: '1500'
ht-degree: 0%

---


# Agora disponível: aplicativo de desktop Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Os usuários do Dynamic Media Classic agora têm acesso a uma nova experiência de aplicativo de desktop que não depende mais da tecnologia de Flash do Adobe no navegador.

Este novo aplicativo está disponível para Windows e MacOS.

>[!IMPORTANT]
>
>Recomendamos que você instale o novo aplicativo de desktop Adobe Dynamic Media Classic até 1º de outubro de 2020. Ao fazer isso, você terá uma transição suave antes que o Flash Player do Adobe seja substituído em 31 de dezembro de 2020. Nessa data, você não poderá mais fazer logon na versão do navegador da interface do usuário do Adobe Dynamic Media Classic, rotulada como Dynamic Media Classic no produto.

Consulte as Perguntas frequentes sobre a experiência de logon do [Novo Dynamic Media Classic disponível.](/help/new-ui-2020.md)

## Requisitos de sistema para o aplicativo de desktop Adobe Dynamic Media Classic {#system-requirements-dmc-app}

O aplicativo de desktop Adobe Dynamic Media Classic é compatível com os seguintes sistemas operacionais:
* macOS X 10.10 ou mais recente.
* Windows 7 ou mais recente.

## Correções na versão mais recente 20.20.2 {#latest-fixes-desktop-app}

* Nenhuma limitação no número de arquivos que você pode carregar por meio da interface do usuário do aplicativo de desktop para MacOS e Windows.
* Não é necessário sair do aplicativo de desktop para alternar entre o empresa.
* A operação Ctrl+V para colar agora funciona no Windows.
* No futuro, quando uma nova versão do aplicativo desktop for lançada, os usuários serão notificados dentro do próprio aplicativo desktop.

## Baixe e instale o aplicativo de desktop Adobe Dynamic Media Classic mais recente no macOS ou Windows {#installation-dmc-app}

Consulte também:

* [Baixe e instale silenciosamente o aplicativo Adobe Dynamic Media Classic para desktop mais recente no Mac](#install-silent-mac-dmc-app)
* [Baixe e instale silenciosamente o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Windows](#install-silent-windows-dmc-app)

1. Desinstale as versões mais antigas do aplicativo para desktop Dynamic Media Classic no sistema.

1. Baixe o instalador mais recente para o aplicativo de desktop Adobe Dynamic Media Classic.

   >[!NOTE]
   >
   >O usuário que já instalou a versão do GA deve *desinstalá* -la do sistema Windows local antes de instalar a versão mais recente. Ou os usuários podem simplesmente *substituir* a versão do GA instalada em seu sistema macOS local pela versão mais recente. Os novos usuários devem instalar diretamente a versão mais recente 20.20.2.

   A versão mais recente é 20.20.2, disponível no seguinte endereço:

   * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
   * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe)

   A versão GA (General Availability) era 20.20.1, disponível no seguinte endereço:

   * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)
   * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)




1. Execute um dos procedimentos a seguir com base no instalador que você baixou.

   * **Para macOS** - Na caixa de **[!UICONTROL Drag & drop to install]** diálogo, arraste **[!UICONTROL Adobe Dynamic Media Classic]** e solte-o **[!UICONTROL Applications]**.

      ![Arraste e solte a instalação no macOS](/help/assets/dragondrop-install1.png)

   * Na **[!UICONTROL Applications]** pasta, toque no ícone Adobe Dynamic Media Classic.
   * Na caixa de diálogo, toque em **[!UICONTROL Open]** para abrir o aplicativo de desktop Adobe Dynamic Media Classic.

      ![Abrir aplicativo baixado](/help/assets/open-dmclassicapp1.png)

   * **No Windows** - execute o binário do instalador e siga as instruções na tela para instalar o aplicativo de desktop.

1. Quando você abrir o aplicativo, a nova página de logon do Adobe Dynamic Media Classic será exibida:

   ![Login no Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Use as mesmas credenciais do navegador para fazer logon no Adobe Dynamic Media Classic.

   Para **[!UICONTROL Server]** usar o, consulte o seguinte mapeamento para o ambiente de produção:

   | URL do navegador | Nome do servidor do aplicativo de desktop |
   |---|---|
   | https://s7sps1.scene7.com/ | Produção de NA (América do Norte) |
   | https://s7sps3.scene7.com/ | Produção da EMEA (Europa, Oriente Médio e África) |
   | https://s7sps5.scene7.com/ | Produção de APAC (Ásia-Pacífico) |

1. Após a interface de usuário de logon, você observará a experiência familiar da interface de usuário do navegador. Você pode carregar sua atividade do dia a dia como de costume na interface do usuário do aplicativo para desktop.

## Baixe e instale *silenciosamente* o aplicativo de desktop Adobe Dynamic Media Classic mais recente no macOS {#install-silent-mac-dmc-app}

Consulte também:

* [Baixe e instale o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Mac ou no Windows](#installation-dmc-app)
* [Baixe e instale silenciosamente o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Windows](#install-silent-windows-dmc-app)

Para baixar e instalar *silenciosamente* a versão mais recente do aplicativo de desktop Adobe Dynamic Media Classic no macOS:

1. Desinstale as versões mais antigas do aplicativo para desktop Dynamic Media Classic no sistema.

1. Baixe o instalador mais recente para o aplicativo de desktop Adobe Dynamic Media Classic para macOS.

   * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)

1. Monte a imagem de disco baixada (.DMG) em um local de ponto de montagem usando o seguinte comando:

   `hdiutil attach adobe-dynamic-media-classic-20.20.2.dmg -mountpoint <mount_point_path>`

1. Copie o arquivo .APP para **[!UICONTROL Applications]** usar o seguinte comando:

   `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. Quando você abrir o aplicativo, a nova página de logon do Adobe Dynamic Media Classic será exibida:

   ![Login no Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Use as mesmas credenciais do navegador para fazer logon no Adobe Dynamic Media Classic.

   Para **[!UICONTROL Server]** usar o, consulte o seguinte mapeamento para o ambiente de produção:

   | URL do navegador | Nome do servidor do aplicativo de desktop |
   |---|---|
   | https://s7sps1.scene7.com/ | Produção de NA (América do Norte) |
   | https://s7sps3.scene7.com/ | Produção da EMEA (Europa, Oriente Médio e África) |
   | https://s7sps5.scene7.com/ | Produção de APAC (Ásia-Pacífico) |

## Baixe e instale *silenciosamente* o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Windows {#install-silent-windows-dmc-app}

O comando usado é para uma instalação silenciosa MSI básica. Entretanto, o instalador do aplicativo para desktop Dynamic Media Classic é um instalador MSI InstallScript criado usando o InstallShield. Quando você executa o instalador no modo de registro, qualquer interação do usuário é registrada em um arquivo de resposta. Esse arquivo de resposta é então usado para uma instalação silenciosa, conforme descrito em [Execução de instalações no modo silencioso.](https://docs.flexera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Consulte também:

* [Baixe e instale o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Mac ou no Windows](#installation-dmc-app)
* [Baixe e instale silenciosamente o aplicativo de desktop Adobe Dynamic Media Classic mais recente no macOS](#install-silent-mac-dmc-app)

Para baixar e instalar *silenciosamente* a versão mais recente do aplicativo de desktop Adobe Dynamic Media Classic no Windows:

1. Desinstale as versões mais antigas do aplicativo para desktop Dynamic Media Classic no sistema.

1. Baixe o instalador mais recente para o aplicativo de desktop Adobe Dynamic Media Classic.

   * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe)

1. Execute o instalador no modo de registro usando o seguinte comando:

   `adobe-dynamic-media-classic-20.20.2.exe /r /f1"C:\Setup.iss"`

1. Na janela do instalador da GUI, siga as etapas para instalar para que as interações/entradas, como o local de instalação, sejam gravadas no `Setup.iss` arquivo.

1. Copie o arquivo criado `Setup.iss` e `adobe-dynamic-media-classic-20.20.2.exe` para outro computador.

1. Execute o seguinte comando para uma instalação silenciosa:

   `adobe-dynamic-media-classic-20.20.2.exe /s /f1"C:\Setup.iss"`

   Detalhes sobre os parâmetros da linha de comando estão disponíveis em [Setup.exe e Update.exe Command-Line Parameters.](https://docs.flexera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. Quando você abrir o aplicativo, a nova página de logon do Adobe Dynamic Media Classic será exibida:

   ![Login no Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Use as mesmas credenciais do navegador para fazer logon no Adobe Dynamic Media Classic.

   Para **[!UICONTROL Server]** usar o, consulte o seguinte mapeamento para o ambiente de produção:

   | URL do navegador | Nome do servidor do aplicativo de desktop |
   |---|---|
   | https://s7sps1.scene7.com/ | Produção de NA (América do Norte) |
   | https://s7sps3.scene7.com/ | Produção da EMEA (Europa, Oriente Médio e África) |
   | https://s7sps5.scene7.com/ | Produção de APAC (Ásia-Pacífico) |


## Vídeo sobre como usar o aplicativo de desktop do Dynamic Media Classic {#dmc-app-video-walk-through}

Assista a uma apresentação de [vídeo sobre como usar o aplicativo](https://docs.adobe.com/content/help/en/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html) Dynamic Media Classic Desktop (Duração: 2 minutos (36 segundos).

## Limpar o cache de imagens e o cache de ativos no computador usando o aplicativo de desktop

1. No aplicativo de desktop Dynamic Media Classic, próximo ao canto superior direito, toque em **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Na **[!UICONTROL Personal Setup]** página, sob o **[!UICONTROL Desktop]** cabeçalho, execute um dos procedimentos a seguir:
   * Toque em **[!UICONTROL Clear Image Cache]** para remover todos os arquivos de imagem em cache do Adobe Dynamic Media do computador. Toque em **[!UICONTROL OK]**.
   * Toque em **[!UICONTROL Clear Asset Cache]** para remover todos os arquivos de ativos em cache do Adobe Dynamic Media do computador. Toque em **[!UICONTROL OK]**.
1. In the lower-right corner of the page, tap **[!UICONTROL Close]**.

### Limpar manualmente o cache de imagens e o cache de ativos

Além de limpar o cache de imagem e ativos usando o aplicativo de desktop, você também pode realizar essa tarefa manualmente limpando o cache diretamente do sistema de arquivos.

1. Com base no seu sistema operacional, navegue até o seguinte:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limitações conhecidas no Dynamic Media Classic 20.20.1 (corrigido em 20.20.2)

**_Aplica-se somente ao Windows - há uma limitação no número de arquivos que podem ser carregados por meio da interface do usuário do aplicativo para desktop?_**<br>Sim, um máximo de 150 arquivos pode ser carregado de cada vez por meio da interface do usuário do aplicativo para desktop.

**_Aplica-se ao Windows e macOS - Como alterno entre o empresa?_**<br>Para alternar entre empresas, faça o seguinte:
* No aplicativo Dynamic Media Classic, selecione a nova empresa na lista suspensa empresa.
* Quando o pop-up for exibido, toque em **[!UICONTROL OK]** para sair e fechar o aplicativo.

   ![Reinicie o aplicativo para usar a nova empresa](/help/assets/dmclassic-new-company1.png)
* Reinicie o Dynamic Media Classic e faça logon como de costume para trabalhar com a nova empresa.

## Dicas e truques

**_Não consigo ver o painel Carrinho de mídia na landing page do Dynamic Media Classic._**<br>No Dynamic Media Classic, toque **[!UICONTROL Setup > Personal Setup]**. Na seção Navegador, verifique se **[!UICONTROL Show MediaPortal Features]**está selecionado (marcado). Toque em **[!UICONTROL Save > Close]**.

**_O estado de publicação (indicador verde) de um ativo não é refletido corretamente._**<br>Na interface do usuário do navegador, um novo logon na interface do usuário era necessário para ver o estado correto de publicação dos ativos. No aplicativo de desktop, apresentamos um **[!UICONTROL Refresh]**ícone na barra de ferramentas, à direita do **[!UICONTROL Select None]**botão. Toque no **[!UICONTROL Refresh]**ícone para ver o status mais recente de todos os ativos em uma determinada página. Não é necessário refazer o logon como com a interface do navegador.

![Ícone](/help/assets/refresh-icon1.png)Atualizar ícone *Atualizar*

**_Não vejo predefinições de conjuntos de lotes funcionando no aplicativo de desktop._**<br>Toque em **[!UICONTROL Upload > Job Options > Batch Set Presets]**. Verifique se o relevante **[!UICONTROL Batch Set Preset]**está ativado. Clique em **[!UICONTROL Save and Submit upload]**.
