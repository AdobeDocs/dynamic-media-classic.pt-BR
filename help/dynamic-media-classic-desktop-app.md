---
title: Aplicativo de desktop do Adobe Dynamic Media Classic - Agora disponível
description: Saiba mais sobre o aplicativo de desktop do Adobe Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: 92c3cccbd03f8e159ca6e1ae90558826a5b1443b
workflow-type: tm+mt
source-wordcount: '1904'
ht-degree: 0%

---

# Agora disponível: Aplicativo de desktop do Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Os usuários da Adobe Dynamic Media Classic agora têm acesso a uma nova experiência de aplicativo de desktop que não depende mais da tecnologia de Flash no navegador.

Este novo aplicativo está agora disponível para Windows® e macOS.

>[!IMPORTANT]
>
>O Adobe recomenda instalar o novo aplicativo de desktop do Adobe Dynamic Media Classic até 1º de outubro de 2020. Isso garantirá uma transição suave para que o Adobe Flash Player seja descontinuado em 31 de dezembro de 2020. Após essa data, você não poderá fazer logon na versão do navegador da interface do usuário do Adobe Dynamic Media Classic, identificada como Adobe Dynamic Media Classic no produto.

Consulte as Perguntas frequentes da [A nova experiência de logon do Adobe Dynamic Media Classic está disponível.](/help/new-ui-2020.md)

## Requisitos de sistema para o aplicativo de desktop Adobe Dynamic Media Classic {#system-requirements-dmc-app}

O aplicativo de desktop do Adobe Dynamic Media Classic é compatível com os seguintes sistemas operacionais:

* macOS 10.10 ou mais recente.
* Windows® 7 ou mais recente.

>[!NOTE]
>
>A notificação de atualização no aplicativo de desktop do Adobe Dynamic Media Classic não é gerada para *menor* versões. Os clientes que se beneficiam de correções em uma versão secundária podem atualizar.

## Correções na versão mais recente (20.22.1) {#release-jan2022}

* Edição de imagem **[!UICONTROL Save]** os botões não funcionavam.
* Nos editores do Conjunto, a variável **[!UICONTROL Close]**, **[!UICONTROL Save]** e **[!UICONTROL Save As]** os botões ficam desativados depois de rolar os ativos no **[!UICONTROL Add Assets]** painel.
* **[!UICONTROL Play]** na exibição Detalhes do vídeo não funcionava.
* Não foi possível inserir `d` e `e` em **[!UICONTROL Username]** e **[!UICONTROL Password]** ao executar o macOS Monterey.
* As APIs de análise restantes foram movidas para a versão 2.0.

## Correções na versão 20.21.3 {#release-sept2021}

* Miniaturas quebradas para ativos vistos após um período de inatividade no aplicativo de desktop.
* O aplicativo de desktop para de responder, normalmente após as operações Definir.
* Solicitar ofuscação e modo de bloqueio ativado automaticamente em **[!UICONTROL Test Image Serving]**.

   Consulte [Testar o serviço de teste seguro](/help/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Atualização do mecanismo de autenticação com o Adobe Analytics. Relevante para novas integrações ou se algumas variáveis do Analytics devem ser atualizadas no aplicativo de desktop do Dynamic Media Classic.

   Consulte [Faça logon no Adobe Analytics](/help/log-analytics.md) para etapas atualizadas.

## Correções na versão 20.21.2 {#minor-release}

* Limitação conhecida na versão 20.21.1: o **[!UICONTROL Server]** a lista suspensa na tela de Logon estava vazia.
* Em **[!UICONTROL Upload Job Options]**, Valor padrão de nomeação de camada em **[!UICONTROL Photoshop Options]**, agora é **[!UICONTROL Photoshop and Layer Name]**. As camadas no arquivo PSD são carregadas como imagens separadas.
   * O padrão anterior de **[!UICONTROL Layer name]**, nomeie as imagens após o nome da camada ou o número da camada no arquivo PSD. O número da camada foi usado se os nomes da camada no arquivo PSD fossem nomes padrão da camada Photoshop.
   * O novo padrão de **[!UICONTROL Photoshop and Layer Name]**, nomeia as imagens após o PSD, seguido do nome da camada ou do número da camada. O número da camada é usado se os nomes da camada no arquivo PSD forem nomes padrão da camada do Photoshop.
   * Considerando que as imagens de camada no Adobe Dynamic Media Classic agora têm nomes exclusivos, nenhuma atualização no PSD ou Modelos existentes acontecerá (que compartilhou nomes de camada nos arquivos PSD originais).
* Miniaturas de ativos quebradas.

## Correções na versão 20.21.1 {#latest-fixes-desktop-app}

* Problemas de logon devido ao tempo limite que resultam na seguinte mensagem: *Esse usuário pode ser atribuído ao grupo ou grupos sem permissão. Entre em contato com o administrador.*
* As predefinições do visualizador são duplicadas a cada tentativa incorreta de senha.
* O aplicativo de desktop fica sem resposta devido a muitos ativos na pasta raiz. (Fixo no Windows®; funcionando como desejado no macOS.)

## Correções na versão 20.20.2 {#previous-version-fixes-desktop-app}

* Nenhuma limitação no número de arquivos que você pode fazer upload por meio da interface do usuário do aplicativo de desktop para macOS e Windows®.
* Não é necessário sair do aplicativo de desktop para alternar entre empresas.
* Ctrl+V para a operação de colar agora funciona no Windows®.
* Futuramente, quando uma nova versão do aplicativo de desktop for lançada, os usuários serão notificados dentro do próprio aplicativo de desktop.

## Baixe e instale o aplicativo de desktop Adobe Dynamic Media Classic mais recente no macOS ou Windows® {#installation-dmc-app}

Consulte também:

* [Baixe e instale silenciosamente o aplicativo de desktop do Adobe Dynamic Media Classic mais recente no Mac](#install-silent-mac-dmc-app)
* [Baixe e instale silenciosamente o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Windows®](#install-silent-windows-dmc-app)

1. Desinstale as versões mais antigas do aplicativo de desktop do Adobe Dynamic Media Classic no seu sistema.

1. Baixe o instalador mais recente para o aplicativo de desktop do Adobe Dynamic Media Classic.

   * A versão mais recente (20.22.1) está disponível no seguinte endereço:

      * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)
   * A versão anterior (20.21.3) está disponível em:

      * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg)
      * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)


<!--    * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Siga um destes procedimentos com base no instalador baixado.

   * **macOS** -No **[!UICONTROL Drag & drop to install]** caixa de diálogo, arrastar **[!UICONTROL Adobe Dynamic Media Classic]** e solte-o em **[!UICONTROL Applications]**.

      ![Arrastar e soltar instalação no macOS](/help/assets/dragondrop-install1.png)

   * No **[!UICONTROL Applications]** toque no ícone Adobe Dynamic Media Classic .
   * Na caixa de diálogo, toque em **[!UICONTROL Open]** para abrir o aplicativo de desktop do Adobe Dynamic Media Classic.

      ![Abrir aplicativo baixado](/help/assets/open-dmclassicapp1.png)

   * **Windows** - Execute o binário do instalador e siga as instruções na tela para instalar o aplicativo de desktop.

1. Ao abrir o aplicativo, a nova página de Logon do Adobe Dynamic Media Classic é exibida:

   ![Logon no Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Para fazer logon no aplicativo de desktop do Adobe Dynamic Media Classic, use as mesmas credenciais usadas para fazer logon no Adobe Dynamic Media Classic no navegador.

   Para o **[!UICONTROL Server]** para usar, consulte o seguinte mapeamento para o ambiente de produção:

   | Servidor | URL do navegador |
   | --- | --- |
   | Produção de NA (América do Norte) | https://s7sps1.scene7.com/ |
   | Produção da EMEA (Europa, Oriente Médio e África) | https://s7sps3.scene7.com/ |
   | Produção de APAC (Ásia-Pacífico) | https://s7sps5.scene7.com/ |

1. Após fazer logon, observe a experiência familiar da interface do usuário do navegador. Você pode continuar sua atividade diária do Adobe Dynamic Media Classic como de costume no aplicativo de desktop.

## Baixe e *silencioso* instale o aplicativo de desktop mais recente do Adobe Dynamic Media Classic no macOS {#install-silent-mac-dmc-app}

Consulte também:

* [Baixe e instale o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Mac ou Windows®](#installation-dmc-app)
* [Baixe e instale silenciosamente o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Windows®](#install-silent-windows-dmc-app)

Para baixar e *silencioso* instale a versão mais recente do aplicativo de desktop do Adobe Dynamic Media Classic no macOS:

1. Desinstale as versões mais antigas do aplicativo de desktop do Adobe Dynamic Media Classic no seu sistema.

1. Baixe o instalador mais recente do aplicativo de desktop do Adobe Dynamic Media Classic para macOS.

   * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)

1. Monte a Imagem de Disco baixada (.DMG) em um local de ponto de montagem usando o seguinte comando:

   `hdiutil attach adobe-dynamic-media-classic-20.22.1.dmg -mountpoint <mount_point_path>`

1. Copie o arquivo .APP para **[!UICONTROL Applications]** usando o seguinte comando:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. Ao abrir o aplicativo, a nova página de Logon do Adobe Dynamic Media Classic é exibida:

   ![Logon no Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Para fazer logon no aplicativo de desktop do Adobe Dynamic Media Classic, use as mesmas credenciais usadas para fazer logon no Adobe Dynamic Media Classic no navegador.

   Para o **[!UICONTROL Server]** para usar, consulte o seguinte mapeamento para o ambiente de produção:

   | Servidor | URL do navegador |
   | --- | --- |
   | Produção de NA (América do Norte) | https://s7sps1.scene7.com/ |
   | Produção da EMEA (Europa, Oriente Médio e África) | https://s7sps3.scene7.com/ |
   | Produção de APAC (Ásia-Pacífico) | https://s7sps5.scene7.com/ |

## Baixe e *silencioso* instale o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Windows® {#install-silent-windows-dmc-app}

O comando usado é para uma instalação silenciosa MSI básica. No entanto, o instalador do aplicativo de desktop do Adobe Dynamic Media Classic é um instalador do InstallScript MSI criado com o InstallShield. Quando você executa o instalador no modo de registro, qualquer interação do usuário é registrada em um arquivo de resposta. Esse arquivo de resposta é então usado para uma instalação silenciosa conforme descrito em [Executando instalações no modo silencioso.](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Consulte também:

* [Baixe e instale o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Mac ou Windows®](#installation-dmc-app)
* [Baixe e instale silenciosamente o aplicativo de desktop do Adobe Dynamic Media Classic mais recente no macOS](#install-silent-mac-dmc-app)

Para baixar e *silencioso* instale a versão mais recente do aplicativo de desktop Adobe Dynamic Media Classic no Windows®:

1. Desinstale as versões mais antigas do aplicativo de desktop do Adobe Dynamic Media Classic no seu sistema.

1. Baixe o instalador mais recente para o aplicativo de desktop do Adobe Dynamic Media Classic.

   * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Execute o instalador no modo de registro usando o seguinte comando:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. Na janela do instalador da GUI, siga as etapas para instalar para que as interações/entradas, como o local de instalação, sejam registradas em `Setup.iss` arquivo.

1. Copie os `Setup.iss` e `adobe-dynamic-media-classic-20.22.1.exe` para outro computador.

1. Execute o seguinte comando para uma instalação silenciosa:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   Detalhes sobre os parâmetros da linha de comando estão disponíveis em [Parâmetros de linha de comando Setup.exe e Update.exe.](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. Ao abrir o aplicativo, a nova página de Logon do Adobe Dynamic Media Classic é exibida:

   ![Logon no Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Para fazer logon no aplicativo de desktop do Adobe Dynamic Media Classic, use as mesmas credenciais usadas para fazer logon no Adobe Dynamic Media Classic no navegador.

   Para o **[!UICONTROL Server]** para usar, consulte o seguinte mapeamento para o ambiente de produção:

   | Servidor | URL do navegador |
   | --- | --- |
   | Produção de NA (América do Norte) | https://s7sps1.scene7.com/ |
   | Produção da EMEA (Europa, Oriente Médio e África) | https://s7sps3.scene7.com/ |
   | Produção de APAC (Ásia-Pacífico) | https://s7sps5.scene7.com/ |

## Vídeo de apresentação sobre o uso do aplicativo de desktop do Adobe Dynamic Media Classic {#dmc-app-video-walk-through}

Assista a [apresentação de vídeo sobre o uso do aplicativo de desktop do Adobe Dynamic Media Classic](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (Comprimento: 2 minutos (36 segundos).

## Limpar o cache de imagem e o cache de ativos no computador usando o aplicativo de desktop {#clear-cache}

1. No aplicativo de desktop do Adobe Dynamic Media Classic, próximo ao canto superior direito, toque em **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. No **[!UICONTROL Personal Setup]** na página **[!UICONTROL Desktop]** , execute um dos seguintes procedimentos:
   * Para remover todos os arquivos de imagem em cache do Adobe Dynamic Media de seu computador, toque em **[!UICONTROL Clear Image Cache]** e toque em **[!UICONTROL OK]**.
   * Para remover todos os arquivos de ativos em cache do Adobe Dynamic Media de seu computador, toque em **[!UICONTROL Clear Asset Cache]** e toque em **[!UICONTROL OK]**.
1. No canto inferior direito da página, toque em **[!UICONTROL Close]**.

### Limpar manualmente o cache de imagens e o cache de ativos

Além de limpar o cache de imagem e ativos usando o aplicativo de desktop, você pode limpar manualmente o cache diretamente do sistema de arquivos.

1. Com base no seu sistema operacional, navegue até o seguinte:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limitação conhecida no Adobe Dynamic Media Classic 20.21.1

* O **[!UICONTROL Server]** a lista suspensa fica vazia após a atualização para o aplicativo de desktop do Adobe Dynamic Media Classic 20.21.1 - Cenário: Você instala e faz logon no Adobe Dynamic Media Classic 20.20.1 ou 20.20.2 e então fecha o aplicativo. Em seguida, atualize para o Adobe Dynamic Media Classic 20.21.1. Ao tentar fazer logon, a variável **[!UICONTROL Server]** na lista suspensa na **[!UICONTROL Sign in to your account]** A caixa de diálogo está vazia. Para contornar esse problema, você deve [limpar manualmente o cache](#clear-cache) (consulte as etapas acima).

## Limitações conhecidas do Adobe Dynamic Media Classic 20.20.1 (corrigidas na versão 20.20.2)

**_Aplica-se somente ao Windows® - Existe uma limitação no número de arquivos que podem ser carregados por meio da interface do usuário do aplicativo de desktop?_**<br>Sim, um máximo de 150 arquivos pode ser carregado de cada vez por meio da interface do usuário do aplicativo de desktop.

**_Aplica-se ao Windows® e macOS - Como faço para alternar entre empresas?_**<br>Para alternar entre empresas, faça o seguinte:

* No aplicativo Adobe Dynamic Media Classic, selecione a nova empresa na lista suspensa da empresa.
* Quando a janela pop-up for exibida, toque em **[!UICONTROL OK]** para sair e fechar o aplicativo.

   ![Para usar a nova empresa, reinicie o aplicativo](/help/assets/dmclassic-new-company1.png)

* Reinicie o Adobe Dynamic Media Classic e faça logon como de costume para trabalhar com a nova empresa.

## Dicas e truques

**_Não consigo ver o painel Carrinho de mídia na página de aterrissagem do Adobe Dynamic Media Classic._**<br>No Adobe Dynamic Media Classic, toque em **[!UICONTROL Setup > Personal Setup]**. Na seção Navegador , verifique se **[!UICONTROL Show MediaPortal Features]**está selecionada (marcada). Toque **[!UICONTROL Save > Close]**.

**_O estado de publicação (indicador verde) de um ativo não é refletido corretamente._**<br>Na interface do usuário do navegador, era necessário fazer logon novamente na interface do usuário para visualizar o estado de publicação correto dos ativos. No aplicativo de desktop, o Adobe apresentou um **[!UICONTROL Refresh]**ícone na barra de ferramentas, à direita do **[!UICONTROL Select None]**botão. Toque no **[!UICONTROL Refresh]**para ver o status mais recente de todos os ativos na determinada página. Não é necessário fazer logon novamente como na interface do usuário do navegador.

![Ícone Atualizar](/help/assets/refresh-icon1.png)
*Ícone Atualizar*

**_Não vejo predefinições de conjuntos em lotes que funcionam no aplicativo de desktop._**<br>Toque **[!UICONTROL Upload > Job Options > Batch Set Presets]**. Assegure a **[!UICONTROL Batch Set Preset]**estiver ativado. Clique em **[!UICONTROL Save and Submit upload]**.
