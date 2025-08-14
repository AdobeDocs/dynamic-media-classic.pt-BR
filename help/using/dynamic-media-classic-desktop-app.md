---
title: desktop Adobe Dynamic Media Classic
description: Saiba mais sobre o aplicativo de desktop do Adobe Dynamic Media Classic disponível.
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
topic: Administration
level: Intermediate
source-git-commit: afc347201b13c3b91ec5e1bd3ac5304442772f8d
workflow-type: tm+mt
source-wordcount: '1903'
ht-degree: 0%

---

# Disponível agora: aplicativo de desktop do Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Os usuários do Adobe Dynamic Media Classic agora têm acesso a uma nova experiência de aplicativo de desktop que não depende mais da tecnologia Adobe Flash no navegador.

Este novo aplicativo agora está disponível para Windows® e macOS.

>[!IMPORTANT]
>
>A Adobe recomenda que você instale o novo aplicativo de desktop Adobe Dynamic Media Classic até 1º de outubro de 2020. Isso garantirá uma transição suave antes da desativação do Adobe Flash Player em 31 de dezembro de 2020. Após essa data, não será possível fazer logon na versão do navegador da interface do usuário do Adobe Dynamic Media Classic rotulada como Adobe Dynamic Media Classic no produto.

Consulte as Perguntas Frequentes do [Novo logon do Adobe Dynamic Media Classic agora disponível.](/help/using/new-ui-2020.md)

## Requisitos de sistema para o aplicativo de desktop do Adobe Dynamic Media Classic {#system-requirements-dmc-app}

O aplicativo de desktop do Adobe Dynamic Media Classic é compatível com os seguintes sistemas operacionais:

* macOS 10.10 ou mais recente.
* Windows® 7 ou mais recente.

Consulte os requisitos completos do sistema em [Requisitos do sistema para o aplicativo de desktop do Adobe Dynamic Media Classic](/help/using/system-requirements.md).

A notificação de atualização no aplicativo de desktop do Adobe Dynamic Media Classic não é gerada para versões *secundárias*. Os clientes que se beneficiam de correções em uma versão secundária podem atualizar o.

## Corrigido somente na versão mais recente (20.22.2) do macOS {#release-feb2022}

* macOS Monterey: a página de upload de arquivos congela nos envios subsequentes. <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## Correções na versão mais recente (20.22.1) {#release-jan2022}

* Ao editar uma imagem, os botões **[!UICONTROL Save]** não funcionavam.
* Nos editores de Conjunto, os botões **[!UICONTROL Close]**, **[!UICONTROL Save]** e **[!UICONTROL Save As]** ficam desabilitados após rolar ativos no painel **[!UICONTROL Add Assets]**.
* O botão **[!UICONTROL Play]** na exibição de Detalhes do vídeo não funcionou.
* Não foi possível inserir `d` e `e` nos campos **[!UICONTROL Username]** e **[!UICONTROL Password]** ao executar o macOS Monterey.
* As APIs restantes do Analytics foram movidas para a versão 2.0.

## Correções na versão 20.21.3 {#release-sept2021}

* Miniaturas quebradas de ativos vistos após um período de inatividade no aplicativo de desktop.
* O aplicativo de desktop para de responder, normalmente após as operações Set.
* Solicitar Ofuscação e Modo de Bloqueio habilitado automaticamente em **[!UICONTROL Test Image Serving]**.

  Consulte [O serviço de Teste Seguro](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Mecanismo de autenticação atualizado com o Adobe Analytics. Relevante para novas integrações ou se algumas variáveis do Analytics precisam ser atualizadas no aplicativo de desktop do Dynamic Media Classic.

  Consulte [Fazer logon no Adobe Analytics](/help/using/log-analytics.md) para ver as etapas atualizadas.

## Correções na versão 20.21.2 {#minor-release}

* Limitação conhecida no 20.21.1: a lista suspensa **[!UICONTROL Server]** na tela de entrada estava vazia.
* Em **[!UICONTROL Upload Job Options]**, o valor de nome de Camada padrão em **[!UICONTROL Photoshop Options]**, agora é **[!UICONTROL Photoshop and Layer Name]**. As camadas no arquivo PSD são carregadas como imagens separadas.
   * O padrão anterior de **[!UICONTROL Layer name]**, nomeava as imagens após seu nome de camada ou número de camada no arquivo PSD. O número da camada era usado se os nomes das camadas no arquivo do PSD fossem nomes de camadas padrão do Photoshop.
   * O novo padrão de **[!UICONTROL Photoshop and Layer Name]**, nomeia as imagens após o arquivo PSD seguido pelo nome ou número da camada. O número da camada é usado se os nomes das camadas no arquivo do PSD forem nomes de camadas padrão do Photoshop.
   * Considerando que as imagens de camada no Adobe Dynamic Media Classic agora têm nomes exclusivos, não ocorrerá nenhuma atualização no PSD ou nos modelos existentes (quais nomes de camada compartilhados nos arquivos originais do PSD).
* Miniaturas de ativos quebradas.

## Correções na versão 20.21.1 {#latest-fixes-desktop-app}

* Problemas de entrada devido ao tempo limite que resultam na seguinte mensagem: *Este usuário pode ser atribuído ao grupo ou grupos sem permissão. Contate o administrador.*
* As predefinições do visualizador são duplicadas a cada tentativa de senha incorreta.
* O aplicativo de desktop não responde devido a muitos ativos na pasta raiz. (Corrigido no Windows®; funcionando conforme desejado no macOS.)

## Correções na versão 20.20.2 {#previous-version-fixes-desktop-app}

* Sem limitação no número de arquivos que você pode carregar por meio da interface do usuário do aplicativo de desktop para macOS e Windows®.
* Não é necessário sair do aplicativo de desktop para alternar entre empresas.
* A operação de colar com as teclas Ctrl+V agora funciona no Windows®.
* No futuro, quando uma nova versão do aplicativo de desktop for lançada, os usuários serão notificados no próprio aplicativo de desktop.

## Baixe e instale o aplicativo de desktop Adobe Dynamic Media Classic mais recente no macOS ou no Windows® {#installation-dmc-app}

Consulte também:

* [Baixe e instale silenciosamente o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Mac](#install-silent-mac-dmc-app)
* [Baixe e instale silenciosamente o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Windows](#install-silent-windows-dmc-app)

1. Desinstale todas as versões mais antigas do aplicativo de desktop do Adobe Dynamic Media Classic no sistema.

1. Baixe o instalador mais recente para o aplicativo de desktop do Adobe Dynamic Media Classic.

   * A versão mais recente está disponível no site a seguir:

      * [macOS (.DMG): Baixar](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows (.EXE): Baixar](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * A versão anterior está disponível no link a seguir:

      * [macOS (.DMG): Baixar](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® (.EXE): Baixar](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--         * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Siga um destes procedimentos com base no instalador que você baixou.

   * **macOS** -Na caixa de diálogo **[!UICONTROL Drag & drop to install]**, arraste **[!UICONTROL Adobe Dynamic Media Classic]** e solte-a em **[!UICONTROL Applications]**.

     ![Arraste e solte a instalação no macOS](/help/using/assets/dragondrop-install1.png)

   * Na pasta **[!UICONTROL Applications]**, toque no ícone Adobe Dynamic Media Classic.
   * Na caixa de diálogo, toque em **[!UICONTROL Open]** para abrir o aplicativo de desktop do Adobe Dynamic Media Classic.

     ![Abrir aplicativo baixado](/help/using/assets/open-dmclassicapp1.png)

   * **Windows** - Execute o binário do instalador e siga as instruções na tela para instalar o aplicativo de desktop.

1. Quando você abre o aplicativo, a nova página de Logon do Adobe Dynamic Media Classic é exibida:

   ![entrada no Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Para fazer logon no aplicativo de desktop do Adobe Dynamic Media Classic, use as mesmas credenciais usadas para fazer logon no Adobe Dynamic Media Classic no navegador.

   Para que o **[!UICONTROL Server]** use, consulte o seguinte mapeamento para o ambiente de produção:

   | Servidor | URL do navegador |
   | --- | --- |
   | Produção de NA (América do Norte) | https://s7sps1.scene7.com/ |
   | Produção na EMEA (Europa, Oriente Médio e África) | https://s7sps3.scene7.com/ |
   | Produção da APAC (Ásia-Pacífico) | https://s7sps5.scene7.com/ |

1. Após fazer logon, observe a experiência familiar da interface do usuário do navegador. Você pode continuar sua atividade diária do Adobe Dynamic Media Classic como de costume no aplicativo de desktop.

## Baixe e *instale silenciosamente* o aplicativo de desktop mais recente do Adobe Dynamic Media Classic no macOS {#install-silent-mac-dmc-app}

Consulte também:

* [Baixe e instale o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Mac ou no Windows](#installation-dmc-app)
* [Baixe e instale silenciosamente o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Windows](#install-silent-windows-dmc-app)

Para baixar e *instalar silenciosamente* a versão mais recente do aplicativo de desktop do Adobe Dynamic Media Classic no macOS:

1. Desinstale todas as versões mais antigas do aplicativo de desktop do Adobe Dynamic Media Classic no sistema.

1. Baixe o instalador mais recente do aplicativo de desktop do Adobe Dynamic Media Classic para macOS.

   * [macOS (.DMG): Baixar](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. Monte a imagem de disco baixada (.DMG) em um local de ponto de montagem usando o seguinte comando:

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. Copie o arquivo .APP para **[!UICONTROL Applications]** usando o seguinte comando:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG: hdiutil detach <mount_point_path>
   ```

1. Quando você abre o aplicativo, a nova página de Logon do Adobe Dynamic Media Classic é exibida:

   ![entrada no Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Para fazer logon no aplicativo de desktop do Adobe Dynamic Media Classic, use as mesmas credenciais usadas para fazer logon no Adobe Dynamic Media Classic no navegador.

   Para que o **[!UICONTROL Server]** use, consulte o seguinte mapeamento para o ambiente de produção:

   | Servidor | URL do navegador |
   | --- | --- |
   | Produção de NA (América do Norte) | https://s7sps1.scene7.com/ |
   | Produção na EMEA (Europa, Oriente Médio e África) | https://s7sps3.scene7.com/ |
   | Produção da APAC (Ásia-Pacífico) | https://s7sps5.scene7.com/ |

## Baixe e *instale silenciosamente* o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Windows® {#install-silent-windows-dmc-app}

O comando usado é para uma instalação silenciosa básica do MSI. No entanto, o instalador do aplicativo de desktop do Adobe Dynamic Media Classic é um instalador MSI do InstallScript criado com o InstallShield. Quando você executa o instalador no modo de registro, qualquer interação do usuário é registrada em um arquivo de resposta. Esse arquivo de resposta é então usado para uma instalação silenciosa, conforme descrito em [Executando instalações no modo silencioso](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

Consulte também:

* [Baixe e instale o aplicativo de desktop Adobe Dynamic Media Classic mais recente no Mac ou no Windows](#installation-dmc-app)

* [Baixe e instale silenciosamente o aplicativo de desktop Adobe Dynamic Media Classic mais recente no macOS](#install-silent-mac-dmc-app)

Para baixar e *instalar silenciosamente* a versão mais recente do aplicativo de desktop da Adobe Dynamic Media Classic no Windows®:

1. Desinstale todas as versões mais antigas do aplicativo de desktop do Adobe Dynamic Media Classic no sistema.

1. Baixe o instalador mais recente para o aplicativo de desktop do Adobe Dynamic Media Classic.

   * [Windows® (.EXE): Baixar](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Execute o instalador no modo de registro usando o seguinte comando:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. Na janela do instalador da GUI, siga as etapas para instalar para que as interações/entradas, como o local de instalação, sejam gravadas no arquivo `Setup.iss`.

1. Copie o arquivo `Setup.iss` e `adobe-dynamic-media-classic-20.22.1.exe` criados em outro computador.

1. Execute o seguinte comando para uma instalação silenciosa:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   Detalhes sobre parâmetros de linha de comando estão disponíveis em [Setup.exe e Update.exe nos parâmetros de linha de comando](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. Quando você abre o aplicativo, a nova página de Logon do Adobe Dynamic Media Classic é exibida:

   ![entrada no Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Para fazer logon no aplicativo de desktop do Adobe Dynamic Media Classic, use as mesmas credenciais usadas para fazer logon no Adobe Dynamic Media Classic no navegador.

   Para que o **[!UICONTROL Server]** use, consulte o seguinte mapeamento para o ambiente de produção:

   | Servidor | URL do navegador |
   | --- | --- |
   | Produção de NA (América do Norte) | https://s7sps1.scene7.com/ |
   | Produção na EMEA (Europa, Oriente Médio e África) | https://s7sps3.scene7.com/ |
   | Produção da APAC (Ásia-Pacífico) | https://s7sps5.scene7.com/ |

## Apresentação em vídeo sobre como usar o aplicativo de desktop do Adobe Dynamic Media Classic {#dmc-app-video-walk-through}

Assista a uma [apresentação em vídeo sobre como usar o Aplicativo de Desktop da Adobe Dynamic Media Classic](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media) (Duração: 2 minutos e 36 segundos).

## Limpeza do cache de imagens e de ativos no computador usando o aplicativo de desktop {#clear-cache}

1. No aplicativo de desktop do Adobe Dynamic Media Classic, próximo ao canto superior direito, toque em **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Na página **[!UICONTROL Personal Setup]**, no cabeçalho **[!UICONTROL Desktop]**, siga um destes procedimentos:
   * Para remover todos os arquivos de imagem em cache do Adobe Dynamic Media do seu computador, toque em **[!UICONTROL Clear Image Cache]** e, em seguida, em **[!UICONTROL OK]**.
   * Para remover todos os arquivos de ativos em cache do Adobe Dynamic Media do computador, toque em **[!UICONTROL Clear Asset Cache]** e em **[!UICONTROL OK]**.
1. No canto inferior direito da página, toque em **[!UICONTROL Close]**.

### Limpeza manual do cache de imagens e de ativos

Além de limpar o cache de imagem e ativos usando o aplicativo de desktop, você pode limpar manualmente o cache diretamente do sistema de arquivos.

1. Com base no seu sistema operacional, navegue até o seguinte:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limitações conhecidas do Adobe Dynamic Media Classic 20.21.1

* A lista suspensa **[!UICONTROL Server]** fica vazia após a atualização para o aplicativo de desktop do Adobe Dynamic Media Classic 20.21.1: Cenário: você instala e entra no Adobe Dynamic Media Classic 20.20.1 ou 20.20.2 e, em seguida, fecha o aplicativo. Em seguida, atualize para o Adobe Dynamic Media Classic 20.21.1. Quando você tenta entrar, a lista suspensa **[!UICONTROL Server]** na caixa de diálogo **[!UICONTROL Sign-in to your account]** fica vazia. Para contornar esse problema, você deve [limpar manualmente o cache](#clear-cache) (veja as etapas acima).

## Limitações conhecidas no Adobe Dynamic Media Classic 20.20.1 (corrigidas na versão 20.20.2)

**_Aplica-se somente ao Windows® - Há uma limitação no número de arquivos que podem ser carregados por meio da interface do usuário do aplicativo de desktop?_**<br>Sim, é possível carregar no máximo 150 arquivos de cada vez usando a interface do usuário do aplicativo de desktop.

**_Aplica-se ao Windows® e à macOS - Como alterno entre empresas?_**<br>Para alternar entre empresas, faça o seguinte:

* No aplicativo Adobe Dynamic Media Classic, selecione a nova empresa na lista suspensa empresa.
* Quando a janela pop-up for exibida, toque em **[!UICONTROL OK]** para sair e fechar o aplicativo.

  ![Para usar a nova empresa, reinicie o aplicativo](/help/using/assets/dmclassic-new-company1.png)

* Reinicie o Adobe Dynamic Media Classic e entre como de costume para trabalhar com a nova empresa.

## Dicas e truques

**_Não consigo ver o painel Carrinho de Mídia na página de aterrissagem do Adobe Dynamic Media Classic._**<br>No Adobe Dynamic Media Classic, toque em **[!UICONTROL Setup > Personal Setup]**. Na seção Navegador, verifique se **[!UICONTROL Show MediaPortal Features]**está selecionado (marcado). Toque em **[!UICONTROL Save > Close]**.

**_O estado de publicação (indicador verde) de um ativo não é refletido corretamente._**<br>Na interface do usuário do navegador, foi necessário fazer logon novamente na interface do usuário para ver o estado de publicação correto dos ativos. No aplicativo de desktop, o Adobe introduziu um ícone do **[!UICONTROL Refresh]**na barra de ferramentas, à direita do botão **[!UICONTROL Select None]**. Toque no ícone **[!UICONTROL Refresh]**para ver o status mais recente de todos os ativos na página especificada. Não é necessário fazer logon novamente como na interface do usuário do navegador.

![Ícone Atualizar](/help/using/assets/refresh-icon1.png)
*Ícone Atualizar*

**_Não vejo predefinições de conjunto de lotes funcionando no aplicativo de desktop._**<br>Toque em **[!UICONTROL Upload > Job Options > Batch Set Presets]**. Verifique se o relevante **[!UICONTROL Batch Set Preset]**está habilitado. Clique em **[!UICONTROL Save and Submit upload]**.
