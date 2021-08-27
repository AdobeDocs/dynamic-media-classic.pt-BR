---
title: Configuração pessoal
description: Todos os usuários podem alterar as configurações na tela Configuração pessoal do Adobe Dynamic Media Classic.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
source-git-commit: 3185824deca4d4b3c5549bda2e47f179094110e7
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---

# Configuração pessoal {#personal-setup}

Todos os usuários podem alterar as configurações na tela Configuração pessoal. Para abrir a tela Configuração pessoal, vá para **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.

>[!NOTE]
>
>A tela Configuração pessoal lista qual função de usuário você tem no Adobe Dynamic Media Classic: Administrador, Administrador ou Usuário da Empresa.

As configurações de Configuração pessoal controlam o comportamento padrão do Painel de navegação, como você recebe e-mail e as configurações de senha. Lembre-se de selecionar **[!UICONTROL Save]** depois de alterar essas configurações.

## Informações da Minha Conta

Identifica o nome da conta, o nome, o nome de usuário (endereço de email) e a função de usuário atribuída.

## Desktop

* **Limpar cache de imagem**  - Remove todos os arquivos de imagem em cache do Adobe Dynamic Media do seu computador.
* **Limpar cache de ativos**  - Remove todos os arquivos de ativos do Adobe Dynamic Media em cache do seu computador.

Além de limpar o cache de imagem e ativos usando o aplicativo de desktop, você pode limpar manualmente o cache diretamente do sistema de arquivos. Com base no seu sistema operacional, navegue até o seguinte:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Extensão Creative Suite

**Para instalar a extensão Adobe Dynamic Media Creative Suite:**

1. No Adobe Dynamic Media Classic, na barra de ferramentas, vá para **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**, em Creative Suite Extension, selecione **[!UICONTROL Download Now]** para baixar o arquivo `s7csxs.zxp`.
1. Selecione os links **[!UICONTROL Installation]** e **[!UICONTROL System Requirements]** para obter informações adicionais sobre a extensão.

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
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Navegador

* **[!UICONTROL Thumbnail Size]** - Determina o tamanho padrão de imagens em miniatura na Exibição de grade no Painel de navegação.
* **[!UICONTROL Default Asset Library View]** - Determina se os ativos na Biblioteca de ativos para conjuntos de build aparecem como miniaturas ou por nome. Se você estiver trabalhando com grandes quantidades de ativos na Biblioteca de ativos, é possível visualizar os ativos por nome. Por exemplo, se você estiver criando um grande eCatalog com muitos arquivos PDF, poderá exibir os ativos por nome para tornar a lista mais curta.
* **[!UICONTROL Default Browse Sort Order]** - Determina a ordem em que os ativos aparecem por padrão no Painel de navegação. Escolha um critério de classificação no menu e se deseja uma classificação crescente ou decrescente.
* **[!UICONTROL Default Browse Location]** - Permite definir o local do navegador para o padrão, a última pasta navegada ou para um local específico no qual você navega e identifica. Você também pode definir o local do navegador para classificar os arquivos e pastas em ordem crescente ou decrescente.
* **[!UICONTROL Default Browse View]** - Determina se a Exibição de Grade ou de Lista é a exibição padrão que você vê ao abrir o painel Procurar pela primeira vez.
* **[!UICONTROL Splash Screen Display]** - Determina se você vê alguma tela inicial, incluindo a tela inicial de Boas-vindas.
* **[!UICONTROL Show ToolTips]** - Determina se as dicas de ferramentas aparecem quando você move o ponteiro sobre botões, menus e links de navegação. As dicas de ferramentas descrevem os itens da interface do usuário na tela.
* **[!UICONTROL Checkerboard Background]** - Exibe uma camada de tabuleiro atrás de imagens, permitindo que você veja facilmente as áreas transparentes de uma imagem que tem um canal alfa.
* **[!UICONTROL Show File Size]** - Exibe o tamanho do arquivo de um ativo durante a navegação.
* **[!UICONTROL Include UDFs in Search]** - Para melhorar o desempenho do sistema para a maioria das pesquisas de metadados executadas, desmarcado (padrão).

   Se a maioria de suas pesquisas de metadados se beneficiar da inclusão de campos definidos pelo usuário, você poderá selecionar essa opção para ativá-los. Como alternativa, use a Pesquisa avançada para fornecer uma experiência de pesquisa mais direcionada e mais rápida do que incluir campos definidos pelo usuário.

   Consulte [Realização de uma pesquisa avançada](searching-assets.md#conducting_an_advanced_search).

   Consulte também [Campos definidos pelo usuário](application-setup.md#user_defined_fields).

* **[!UICONTROL Basic Search Type]** - É possível selecionar entre duas opções:  **[!UICONTROL Contains]** pesquisa a string completa para o valor especificado;  **[!UICONTROL StartsWith]** pesquisa a partir do início da string e retorna os resultados mais rapidamente do que  **[!UICONTROL Contains]**. Qualquer opção substitui o padrão definido em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Application General Settings]** pelo Administrador.
* **[!UICONTROL Show Command Feedback]** - Selecione para ativar a exibição de solicitações de comando para o servidor; desmarque para desligar.
* **[!UICONTROL Show Dialog During Export]** - Selecione para mostrar uma caixa de diálogo pop-up durante uma exportação. Se você desmarcar (desativar) essa opção, ainda poderá acessar a página Trabalhos para recuperar os resultados da exportação.

## Email

* ****[!UICONTROL Email Options]**** - Escolha como deseja que o Adobe Dynamic Media Classic o informe por e-mail quando os trabalhos de upload e publicação forem concluídos. Você pode receber avisos de conclusão de trabalho somente se ocorrerem avisos ou erros.
* ****[!UICONTROL Email Scope]**** - Determina se você recebe todo o email de trabalho da sua empresa ou apenas o email sobre trabalhos de upload e publicação iniciados.
* ****[!UICONTROL Email Types]**** - Determina se você é informado quando trabalhos de upload e publicação são concluídos.

## Idioma

* **[!UICONTROL Preferred Language]** - Determina o idioma que deseja usar na interface.

## Senha

* **[!UICONTROL Current Password]** - Digite a senha da sua senha atual.
* **[!UICONTROL New Password]** - Digite uma senha nova e válida. Sua senha deve atender aos seguintes requisitos:
   * Ter entre 8 e 25 caracteres.
   * Ter pelo menos uma letra minúscula.
   * Ter pelo menos uma letra maiúscula.
   * Ter pelo menos um número.
   * Ter pelo menos um dos seguintes caracteres especiais: `# $ & - _ : { }`
* **[!UICONTROL Re-Type Password]** - Insira novamente a nova senha para confirmar que está digitando corretamente.
* **[!UICONTROL Password Expiration]** - Determina se a senha expira após 72 dias como medida de segurança. Se você selecionar Sim, será solicitado a criar uma senha após 72 dias.
