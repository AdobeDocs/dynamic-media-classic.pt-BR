---
title: Aplicativo Adobe Dynamic Media Classic para desktop - Agora disponível
description: Saiba mais sobre o aplicativo Dynamic Media Classic para desktop.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
translation-type: tm+mt
source-git-commit: 556deae011dd82e847b72c00981a84190f9a5805
workflow-type: tm+mt
source-wordcount: '1601'
ht-degree: 0%

---


# Agora disponível: Aplicativo Adobe Dynamic Media Classic para desktop {#dynamic-media-classic-desktop-app}

Os usuários do Dynamic Media Classic agora têm acesso a uma nova experiência de aplicativo de desktop que não depende mais da tecnologia de Flash no navegador.

Este novo aplicativo está disponível para Windows e MacOS.

>[!IMPORTANT]
>
>O Adobe recomenda que você instale o novo aplicativo Adobe Classic para desktop até 1º de outubro de 2020. Ao fazer isso, você terá uma transição suave antes que o Flash Player do Adobe seja substituído em 31 de dezembro de 2020. Após essa data, não é possível fazer logon na versão do navegador da interface do usuário do Adobe Dynamic Media Classic, rotulada como Dynamic Media Classic no produto.

Consulte as Perguntas frequentes da nova experiência de logon do Dynamic Media Classic disponível.](/help/new-ui-2020.md)[

## Requisitos de sistema para o aplicativo Adobe Dynamic Media Classic para desktop {#system-requirements-dmc-app}

O aplicativo Adobe Dynamic Media Classic para desktop é compatível com os seguintes sistemas operacionais:

* macOS 10.10 ou mais recente.
* Windows 7 ou mais recente.

## Correções na versão mais recente (20.21.1) {#latest-fixes-desktop-app}

* Problemas de logon devido ao tempo limite resultando na seguinte mensagem: *Este utilizador pode ser atribuído ao grupo ou grupos sem permissão. Entre em contato com o administrador.*
* As predefinições do visualizador são duplicadas com cada tentativa incorreta de senha.
* O aplicativo de desktop não responde devido a muitos ativos na pasta raiz. (Corrigido no Windows; trabalhando conforme desejado no macOS.)
* jlkjlkj

## Correções na versão anterior (20.20.2) {#previous-version-fixes-desktop-app}

* Nenhuma limitação no número de arquivos que você pode carregar por meio da interface do usuário do aplicativo de desktop para MacOS e Windows.
* Não é necessário sair do aplicativo de desktop para alternar entre o empresa.
* A operação Ctrl+V para colar agora funciona no Windows.
* No futuro, quando uma nova versão do aplicativo desktop for lançada, os usuários serão notificados dentro do próprio aplicativo desktop. —>

## Baixe e instale o aplicativo Adobe Classic para desktop mais recente no macOS ou no Windows {#installation-dmc-app}

Consulte também:

* [Baixe e instale silenciosamente o aplicativo Adobe Classic para desktop mais recente no Mac](#install-silent-mac-dmc-app)
* [Baixe e instale silenciosamente o aplicativo Adobe Classic para desktop mais recente no Windows](#install-silent-windows-dmc-app)

1. Desinstale versões mais antigas do aplicativo Dynamic Media Classic para desktop no seu sistema.

1. Baixe o instalador mais recente para o aplicativo Adobe Dynamic Media Classic para desktop.

   * A versão mais recente (20.21.1) está disponível em:

      * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.dmg)
      * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.exe)
   * A versão anterior (20.20.2) está disponível em:

      * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
      * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe)



1. Execute um dos procedimentos a seguir com base no instalador que você baixou.

   * **Para macOS**  - Na caixa  **[!UICONTROL Drag & drop to install]** de diálogo, arraste  **[!UICONTROL Adobe Dynamic Media Classic]** e solte-o  **[!UICONTROL Applications]**.

      ![Arraste e solte a instalação no macOS](/help/assets/dragondrop-install1.png)

   * Na pasta **[!UICONTROL Applications]**, toque no ícone do Adobe Dynamic Media Classic.
   * Na caixa de diálogo, toque em **[!UICONTROL Open]** para abrir o aplicativo de desktop Adobe Dynamic Media Classic.

      ![Abrir aplicativo baixado](/help/assets/open-dmclassicapp1.png)

   * **No Windows**  - execute o binário do instalador e siga as instruções na tela para instalar o aplicativo de desktop.

1. Quando você abrir o aplicativo, a nova página de Login do Adobe Dynamic Media Classic será exibida:

   ![Logon no Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Para fazer logon no aplicativo Adobe Dynamic Media Classic para desktop, use as mesmas credenciais usadas para fazer logon no Dynamic Media Classic no navegador.

   Para usar o **[!UICONTROL Server]**, consulte o seguinte mapeamento para o ambiente de produção:

   | URL do navegador | Nome do servidor do aplicativo de desktop |
   |---|---|
   | https://s7sps1.scene7.com/ | Produção de NA (América do Norte) |
   | https://s7sps3.scene7.com/ | Produção da EMEA (Europa, Oriente Médio e África) |
   | https://s7sps5.scene7.com/ | Produção de APAC (Ásia-Pacífico) |

1. Após o logon, observe a experiência familiar da interface do usuário do navegador. Você pode continuar a sua atividade do dia a dia do Dynamic Media Classic, como de costume, no aplicativo de desktop.

## Baixe e *silent* instale o aplicativo Adobe Classic para desktop mais recente no macOS {#install-silent-mac-dmc-app}

Consulte também:

* [Baixe e instale o aplicativo Adobe Classic para desktop mais recente no Mac ou no Windows](#installation-dmc-app)
* [Baixe e instale silenciosamente o aplicativo Adobe Classic para desktop mais recente no Windows](#install-silent-windows-dmc-app)

Para baixar e *silent* instalar a versão mais recente do aplicativo Adobe Dynamic Media Classic para desktop no macOS:

1. Desinstale versões mais antigas do aplicativo Dynamic Media Classic para desktop no seu sistema.

1. Baixe o instalador mais recente do aplicativo Adobe Dynamic Media Classic para desktop para macOS.

   * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.dmg)

1. Monte a imagem de disco baixada (.DMG) em um local de ponto de montagem usando o seguinte comando:

   `hdiutil attach adobe-dynamic-media-classic-20.21.1.dmg -mountpoint <mount_point_path>`

1. Copie o arquivo .APP para **[!UICONTROL Applications]** usando o seguinte comando:

   `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. Quando você abrir o aplicativo, a nova página de Login do Adobe Dynamic Media Classic será exibida:

   ![Logon no Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Para fazer logon no aplicativo Adobe Dynamic Media Classic para desktop, use as mesmas credenciais usadas para fazer logon no Dynamic Media Classic no navegador.

   Para usar o **[!UICONTROL Server]**, consulte o seguinte mapeamento para o ambiente de produção:

   | URL do navegador | Nome do servidor do aplicativo de desktop |
   |---|---|
   | https://s7sps1.scene7.com/ | Produção de NA (América do Norte) |
   | https://s7sps3.scene7.com/ | Produção da EMEA (Europa, Oriente Médio e África) |
   | https://s7sps5.scene7.com/ | Produção de APAC (Ásia-Pacífico) |

## Baixe e *silent* instale o aplicativo Adobe Classic para desktop mais recente no Windows {#install-silent-windows-dmc-app}

O comando usado é para uma instalação silenciosa MSI básica. Entretanto, o instalador do aplicativo Dynamic Media Classic para desktop é um instalador InstallScript MSI criado usando o InstallShield. Quando você executa o instalador no modo de registro, qualquer interação do usuário é registrada em um arquivo de resposta. Este arquivo de resposta é então usado para uma instalação silenciosa, conforme descrito em [Executando Instalações no Modo Silencioso.](https://docs.flexera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Consulte também:

* [Baixe e instale o aplicativo Adobe Classic para desktop mais recente no Mac ou no Windows](#installation-dmc-app)
* [Baixe e instale silenciosamente o aplicativo Adobe Classic para desktop mais recente no macOS](#install-silent-mac-dmc-app)

Para baixar e *silent* instalar a versão mais recente do aplicativo Adobe Dynamic Media Classic para desktop no Windows:

1. Desinstale versões mais antigas do aplicativo Dynamic Media Classic para desktop no seu sistema.

1. Baixe o instalador mais recente para o aplicativo Adobe Dynamic Media Classic para desktop.

   * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.exe)

1. Execute o instalador no modo de registro usando o seguinte comando:

   `adobe-dynamic-media-classic-20.21.1.exe /r /f1"C:\Setup.iss"`

1. Na janela do instalador da GUI, siga as etapas para instalar de modo que as interações/entradas, como o local de instalação, sejam gravadas no arquivo `Setup.iss`.

1. Copie o arquivo `Setup.iss` criado e `adobe-dynamic-media-classic-20.21.1.exe` para outro computador.

1. Execute o seguinte comando para uma instalação silenciosa:

   `adobe-dynamic-media-classic-20.21.1.exe /s /f1"C:\Setup.iss"`

   Detalhes sobre os parâmetros da linha de comando estão disponíveis em [Setup.exe e Update.exe Command-Line Parameters.](https://docs.flexera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. Quando você abrir o aplicativo, a nova página de Login do Adobe Dynamic Media Classic será exibida:

   ![Logon no Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Para fazer logon no aplicativo Adobe Dynamic Media Classic para desktop, use as mesmas credenciais usadas para fazer logon no Dynamic Media Classic no navegador.

   Para usar o **[!UICONTROL Server]**, consulte o seguinte mapeamento para o ambiente de produção:

   | URL do navegador | Nome do servidor do aplicativo de desktop |
   |---|---|
   | https://s7sps1.scene7.com/ | Produção de NA (América do Norte) |
   | https://s7sps3.scene7.com/ | Produção da EMEA (Europa, Oriente Médio e África) |
   | https://s7sps5.scene7.com/ | Produção de APAC (Ásia-Pacífico) |


## Vídeo sobre como usar o aplicativo Dynamic Media Classic Desktop {#dmc-app-video-walk-through}

Assista a [uma apresentação de vídeo sobre como usar o aplicativo Dynamic Media Classic Desktop](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (Duração: 2 minutos (36 segundos).

## Limpar o cache de imagens e o cache de ativos no computador usando o aplicativo de desktop {#clear-cache}

1. No aplicativo Dynamic Media Classic para desktop, próximo ao canto superior direito, toque em **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Na página **[!UICONTROL Personal Setup]**, sob o cabeçalho **[!UICONTROL Desktop]**, execute um dos procedimentos a seguir:
   * Para remover todos os arquivos de imagem em cache do Adobe Dynamic Media de seu computador, toque **[!UICONTROL Clear Image Cache]** e em **[!UICONTROL OK]**.
   * Para remover todos os arquivos de ativos em cache do Adobe Dynamic Media do seu computador, toque **[!UICONTROL Clear Asset Cache]** e em **[!UICONTROL OK]**.
1. No canto inferior direito da página, toque em **[!UICONTROL Close]**.

### Limpar manualmente o cache de imagens e o cache de ativos

Além de limpar o cache de imagem e ativos usando o aplicativo de desktop, você pode limpar manualmente o cache diretamente do sistema de arquivos.

1. Com base no seu sistema operacional, navegue até o seguinte:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limitação conhecida no Dynamic Media Classic 2021.1

* A lista suspensa **[!UICONTROL Server]** fica vazia após a atualização para o aplicativo de desktop Dynamic Media Classic 20.21.1 - Cenário: Instale e faça logon no Dynamic Media Classic 20.20.1 ou 20.20.2 e feche o aplicativo. Em seguida, você atualiza para o Dynamic Media Classic 20.21.1. Quando você tenta fazer logon, a lista suspensa **[!UICONTROL Server]** na caixa de diálogo **[!UICONTROL Sign in to your account]** fica vazia. Para contornar esse problema, você deve [limpar manualmente o cache](#clear-cache) (consulte as etapas acima).

## Limitações conhecidas no Dynamic Media Classic 20.20.1 (corrigidas em 20.20.2)

**_Aplica-se somente ao Windows - há uma limitação no número de arquivos que podem ser carregados por meio da interface do usuário do aplicativo para desktop?_**<br>Sim, um máximo de 150 arquivos pode ser carregado de cada vez por meio da interface do usuário do aplicativo para desktop.

**_Aplica-se ao Windows e macOS - Como alterno entre o empresa?_**<br>Para alternar entre empresas, faça o seguinte:
* No aplicativo Dynamic Media Classic, selecione a nova empresa na lista suspensa empresa.
* Quando a janela pop-up for exibida, toque em **[!UICONTROL OK]** para sair e fechar o aplicativo.

   ![Para usar a nova empresa, reinicie o aplicativo](/help/assets/dmclassic-new-company1.png)

* Reinicie o Dynamic Media Classic e faça logon como de costume para trabalhar com a nova empresa.

## Dicas e truques

**_Não consigo ver o painel Carrinho de mídia na landing page do Dynamic Media Classic._**<br>No Dynamic Media Classic, toque em **[!UICONTROL Setup > Personal Setup]**. Na seção Navegador, verifique se **[!UICONTROL Show MediaPortal Features]**está selecionado (marcado). Toque em **[!UICONTROL Save > Close]**.

**_O estado de publicação (indicador verde) de um ativo não é refletido corretamente._**<br>Na interface do usuário do navegador, um novo logon na interface do usuário era necessário para ver o estado de publicação correto dos ativos. No aplicativo de desktop, o Adobe introduziu um ícone **[!UICONTROL Refresh]**na barra de ferramentas, à direita do botão **[!UICONTROL Select None]**. Toque no ícone **[!UICONTROL Refresh]**para ver o status mais recente de todos os ativos em uma determinada página. Não é necessário refazer o logon como com a interface do usuário do navegador.

![Ícone ](/help/assets/refresh-icon1.png)
*Atualizar íconeÍcone Atualizar*

**_Não vejo predefinições de conjuntos de lotes funcionando no aplicativo de desktop._**<br>Toque em **[!UICONTROL Upload > Job Options > Batch Set Presets]**. Verifique se o **[!UICONTROL Batch Set Preset]**relevante está ativado. Clique em **[!UICONTROL Save and Submit upload]**.
