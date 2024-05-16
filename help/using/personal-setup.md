---
title: Configuração pessoal
description: Todos os usuários podem alterar configurações na tela Configuração pessoal do Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
topic: Administration, Collaboration
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Configuração pessoal {#personal-setup}

Todos os usuários podem alterar configurações na tela Configuração Pessoal. Para abrir a tela Configuração pessoal, vá para **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.

>[!NOTE]
>
>A tela Configuração pessoal lista a função de usuário que você tem no Adobe Dynamic Media Classic: Administrador da empresa, Administrador ou Usuário.

As configurações de Configuração pessoal controlam o comportamento padrão do Painel de navegação, como você recebe configurações de email e senha. Lembre-se de selecionar **[!UICONTROL Save]** depois de alterar essas configurações.

## Informações da Minha conta

Identifica o nome da conta, o nome, o nome de usuário (endereço de email) e a função de usuário atribuída.

## Desktop

* **Limpar cache de imagem**: remove todos os arquivos de imagem em cache do Adobe Dynamic Media do seu computador.
* **Limpar cache de ativos**: remove todos os arquivos de ativos dos caches Adobe Dynamic Media do seu computador.

Além de limpar o cache de imagem e ativos usando o aplicativo de desktop, você pode limpar manualmente o cache diretamente do sistema de arquivos. Com base no seu sistema operacional, navegue até o seguinte:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Extensão do Creative Suite

**Para instalar o Adobe Dynamic Media Creative Suite Extension:**

1. No Adobe Dynamic Media Classic, na barra de ferramentas, acesse **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**, em Extensão do Creative Suite, selecione **[!UICONTROL Download Now]** para baixar o `s7csxs.zxp` arquivo.
1. Selecione o **[!UICONTROL Installation]** e **[!UICONTROL System Requirements]** links para obter informações adicionais sobre a extensão.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li>Select libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, select flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator's package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Navegador

* **[!UICONTROL Thumbnail Size]**: determina o tamanho padrão das imagens em miniatura no Modo de exibição de grade no Painel de navegação.
* **[!UICONTROL Default Asset Library View]**: determina se os ativos na Biblioteca de ativos para conjuntos de builds aparecem como miniaturas ou por nome. Se estiver trabalhando com grandes quantidades de ativos na Biblioteca de ativos, você poderá visualizar os ativos por nome. Por exemplo, se estiver criando um eCatalog grande com muitos arquivos PDF, você pode visualizar os ativos por nome para encurtar a lista.
* **[!UICONTROL Default Browse Sort Order]**: determina a ordem em que os ativos aparecem por padrão no Painel de navegação. Escolha um critério de classificação no menu e se deseja uma classificação crescente ou decrescente.
* **[!UICONTROL Default Browse Location]**: permite definir o local de navegação como padrão, a última pasta pesquisada ou um local específico para o qual você navega e identifica. Você também pode definir o local de navegação para classificar os arquivos e pastas em ordem crescente ou decrescente.
* **[!UICONTROL Default Browse View]**: determina se a Exibição em grade ou em lista é a exibição padrão exibida ao abrir o painel Procurar pela primeira vez.
* **[!UICONTROL Splash Screen Display]**: determina se você verá alguma tela inicial, incluindo a tela inicial de boas-vindas.
* **[!UICONTROL Show ToolTips]**: determina se as dicas de ferramentas aparecem ao mover o ponteiro sobre botões, menus e links de navegação. As dicas de ferramentas descrevem itens da interface do usuário na tela.
* **[!UICONTROL Checkerboard Background]**: exibe uma camada xadrez atrás das imagens, permitindo que você veja facilmente as áreas transparentes de uma imagem que tem um canal alfa.
* **[!UICONTROL Show File Size]**: exibe o tamanho do arquivo de um ativo quando você está navegando.
* **[!UICONTROL Include UDFs in Search]**: Para melhorar o desempenho do sistema para a maioria das pesquisas de metadados executadas, desmarque (padrão).

  Se a maioria das pesquisas de metadados se beneficiar da inclusão de campos definidos pelo usuário, é possível selecionar essa opção para ativá-la. Como alternativa, use a Pesquisa avançada para oferecer uma experiência de pesquisa mais direcionada e rápida do que a inclusão de campos definidos pelo usuário.

  Consulte [Realização de uma pesquisa avançada](searching-assets.md#conducting_an_advanced_search).

  Consulte também [Campos definidos pelo usuário](application-setup.md#user_defined_fields).

* **[!UICONTROL Basic Search Type]**: é possível selecionar entre duas opções: **[!UICONTROL Contains]** pesquisa a string inteira para o valor especificado; **[!UICONTROL StartsWith]** pesquisa desde o início da string e retorna resultados mais rapidamente do que **[!UICONTROL Contains]**. Ambas as opções substituem o padrão definido em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Application General Settings]** pelo Administrador.
* **[!UICONTROL Show Command Feedback]**: selecione para ativar a exibição de solicitações de comando para o servidor; desmarque para desativar.
* **[!UICONTROL Show Dialog During Export]**: selecione para mostrar uma caixa de diálogo pop-up durante uma exportação. Se você desmarcar (desativar) essa opção, ainda poderá ir para a página Trabalhos para recuperar os resultados da exportação.

## E-mail

* **[!UICONTROL Email Options]**: escolha como você deseja que o Adobe Dynamic Media Classic informe você por email quando os trabalhos de upload e publicação forem concluídos. Você pode receber avisos de conclusão de tarefas somente se ocorrerem avisos ou erros.
* **[!UICONTROL Email Scope]**: determina se você recebe todos os e-mails de job da sua empresa ou apenas e-mails sobre os jobs de upload e publicação que você iniciou.
* **[!UICONTROL Email Types]**: determina se você será informado quando os trabalhos de upload e os trabalhos de publicação forem concluídos.

## Idioma

* **[!UICONTROL Preferred Language]**: determina o idioma que você deseja usar para a interface.

## Senha

* **[!UICONTROL Current Password]**: digite a senha atual.
* **[!UICONTROL New Password]**: digite uma senha nova e válida. Sua senha deve atender aos seguintes requisitos:
   * Ter entre 8 e 25 caracteres.
   * Contêm pelo menos uma letra minúscula.
   * Contêm pelo menos uma letra maiúscula.
   * Ter pelo menos um número.
   * Conter pelo menos um dos seguintes caracteres especiais: `# $ &: _ : { }`
* **[!UICONTROL Re-Type Password]**: digite novamente a nova senha para confirmar que você a está inserindo corretamente.
* **[!UICONTROL Password Expiration]**: determina se a senha expira após 72 dias como uma medida de segurança. Se você selecionou Sim, será solicitado que você crie uma senha após 72 dias.
