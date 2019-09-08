---
title: Configuração pessoal
seo-title: Configuração pessoal
description: 'null'
seo-description: Todos os usuários podem alterar as configurações na tela Configuração pessoal do Dynamic Media Classic.
uuid: 29 cb 825 a-f 158-4 a 1 e -9 d 5 f -7636 ee 411 b 6 e
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/configuração
discoiquuid: 6314 e 7 b 7-5 bde -4 fe 2-8674-e 4 fc 5fc 5 d 4 d 1 c
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Configuração pessoal {#personal-setup}

Todos os usuários podem alterar as configurações na tela Configuração pessoal. Para abrir a tela de Configuração pessoal, clique em Configuração &gt; Configuração pessoal.

>[!NOTE]
>
>A tela de Configuração pessoal lista a função do usuário no Sistema de publicação Scene 7: Administrador da empresa, administrador ou usuário.

As configurações de Configuração pessoal controlam o comportamento padrão do Painel Procurar, como você recebe as configurações de email e senha. Lembre-se de clicar em Salvar depois de alterar essas configurações.

## Minhas informações de conta

Identifica o nome da conta, o nome, o nome de usuário (endereço de email) e a função de usuário atribuída.

### Versão da área de trabalho

Clique em Instalar agora para instalar a versão da área de trabalho do Sistema de publicação Scene 7 no disco rígido local. Ou clique em Reinstalar agora para instalar a versão da área de trabalho novamente.

### Illustator Plug-in para Web-to-Print

Em computadores executando o Windows 7 ou 8, você deve ter privilégios de administrador e fazer logon como um administrador no Windows para instalar o Plug-in do Adobe Illustrator para a Web para impressão. Depois de instalar o plug-in, ele estará disponível no Adobe Illustrator.

O plug-in é compatível com as seguintes versões do Adobe Illustrator:

* Adobe Illustrator 18 na Adobe Creative Cloud 2014.
* Adobe Illustrator 17 na Adobe Creative Cloud.
* Adobe Illustrator 16 na Adobe Creative Suite 6.

As plataformas suportadas do Adobe Illustrator incluem o seguinte:

* Apple Mac OS X 10.7 ou superior.
* Windows 8, 32 bits e 64 bits.
* Windows 7, 32 bits e 64 bits.
* Windows XP, 32 bits e 64 bits (para Adobe Illustrator 16 apenas no Adobe Creative Suite 6).

Consulte também [Publicação de modelo](quick-start-template-publishing.md).

## Instalação do plug-in no disco rígido local

1. Na página Configuração pessoal no Sistema de publicação Scene 7, em Plug-in do Illustrator para Web-to-Print, clique **em Baixar agora** para baixar o **plug-in do Illustrator para Web-to-Print.zip** .
1. Descompacte o arquivo ZIP em uma pasta temporária.

   Um arquivo readme é incluído na raiz do arquivo descompactado para fornecer informações adicionais sobre o plug-in.

1. Dependendo do sistema operacional instalado, execute um dos procedimentos a seguir:

### Windows

| Se estiver executando | Fazer isso |
|--- |--- |
| Adobe Illustrator 18 na Adobe Creative Cloud 2014 | <ul><li>Na raiz da pasta descompactada, clique em CC -2014.</li><li>Dependendo da versão de bits do Adobe Illustrator que você está usando, clique em win 32 ou win 64.</li><li>Clique em bibliotecas &gt; flame e copie `aflame.dll` para a pasta executável do Adobe Illustrator. Por exemplo `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Observação**: Este caminho de exemplo é para o local de 64 bits; o local de 32 bits pode ser enquadrado em Arquivos de programas (x 86). <br/><ul><li>Retorne à mesma pasta de bibliotecas, clique em flamingo e copie `aflamingo.dll` para a mesma pasta executável do Adobe Illustrator que você usou na etapa anterior. </li><li>Retorne à pasta win 32 ou win 64 que você selecionou na etapa 2 e copie `AdobeS7FXGFileFormat.aip` para a pasta de plug-ins do Adobe Illustrator. Por exemplo `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Observação**: Este caminho de exemplo é para o local de 64 bits; o local de 32 bits pode ser enquadrado em Arquivos de programas (x 86). |
| Adobe Illustrator 17 na Adobe Creative Cloud | <ul><li>Na raiz da pasta descompactada, clique em CC. </li><li>Dependendo da versão de bits do Adobe Illustrator que você está usando, clique em win 32 ou win 64.</li><li> Copie `AdobeS7FXGFileFormat.aip` para a pasta de plug-ins do Adobe Illustrator. Por exemplo `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Observação**: Este caminho de exemplo é para o local de 64 bits; o local de 32 bits pode ser enquadrado em Arquivos de programas (x 86). |
| Adobe Illustrator 16 na Adobe Creative Suite 6 | <ul><li>Na raiz da pasta descompactada, clique em 6.0. </li><li>Dependendo da versão de bits do Adobe Illustrator que você está usando, clique em win 32 ou win 64. </li><li>Copie o adobes 7 fxgfileformat. aip para a pasta de plug-ins do Adobe Illustrator. Por exemplo `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Observação**: Este caminho de exemplo é para o local de 64 bits; o local de 32 bits pode ser enquadrado em Arquivos de programas (x 86). |

### Mac

| Se estiver executando | Fazer isso |
|--- |--- |
| Adobe Illustrator 18 na Adobe Creative Cloud 2014 | <ul><li>Na raiz da pasta descompactada, clique em CC -2014 &gt; mac 64.</li><li>Clique em bibliotecas &gt; flame e copie a `aflame.framework` pasta para a pasta do conteúdo do pacote do Adobe Illustrator. Por exemplo `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (Para abrir a pasta de conteúdo do pacote do Adobe Illustrator, clique com o botão direito do mouse no ícone Adobe illustrator CC 2014 e clique em Mostrar conteúdo do pacote no menu de contexto).</li><li>Retorne à mesma pasta de bibliotecas, clique `flamingo`em e copie a `aflamingo.framework` pasta para a mesma pasta de conteúdo do pacote do Adobe Illustrator que você usou na etapa anterior.</li><li>Retorne à pasta mac 64 selecionada na etapa 1 e copie a `AdobeS7FXGFileFormat.aip` pasta para a pasta de plug-in do Adobe Illustrator. Por exemplo `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 17 na Adobe Creative Cloud | <ul><li>Na raiz da pasta descompactada, clique em CC &gt; mac 64</li><li>Copie a `AdobeS7FXGFileFormat.aip` pasta para a pasta de plug-in do Adobe Illustrator. Por exemplo `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 16 na Adobe Creative Suite 6 | <ul><li>Na raiz da pasta descompactada, clique em 6.0 &gt; mac 64</li><li>Copie a `AdobeS7FXGFileFormat.aip` pasta para a pasta de plug-in do Adobe Illustrator. Por exemplo `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul> |

O plug-in agora está disponível para uso no Adobe Illustrator.

### Navegador

* **Tamanho da miniatura**
   * Determina o tamanho padrão das imagens em miniatura na exibição de Grade no Painel Procurar.
* **Exibição padrão da biblioteca de ativos**
   * Determina se os ativos na Biblioteca de ativos para conjuntos de criação aparecem como miniaturas ou por nome. Se estiver trabalhando com grandes quantidades de ativos na Biblioteca de ativos, você pode visualizar os ativos por nome. Por exemplo, se você estiver criando um ecatalog grande com muitos arquivos PDF, poderá exibir os ativos por nome para tornar a lista mais curta.
* **Ordem de classificação padrão de navegação**
   * Determina a ordem em que os ativos aparecem por padrão no Painel Procurar. Escolha um critério de classificação no menu e se deseja uma classificação crescente ou decrescente.
* **Local de navegação padrão**
   * Permite definir o local de navegação para o padrão, a última pasta navegada ou a localização específica que você navega e identifica. Você também pode definir o local da navegação para classificar os arquivos e pastas em ordem crescente ou decrescente.
* **Exibição de navegação padrão**
   * Determina se a exibição de Grade ou a Exibição de lista é a exibição padrão que você vê quando abre o Painel de navegação.
* **Exibição de tela de apresentação**
   * Determina se você verá telas de apresentação, incluindo a tela de apresentação de Boas-vindas.
* **Mostrar dicas de ferramentas**
   * Determina se dicas de ferramentas aparecem quando você move o ponteiro sobre botões, menus e links de navegação. Dicas de ferramentas descrevem itens na tela.
* **Plano de fundo do quadriculado**
   * Exibe uma camada de quadriculado atrás das imagens, permitindo ver facilmente as áreas transparentes de uma imagem com um canal alfa.
* **Mostrar tamanho de arquivo**
   * Exibe o tamanho de arquivo de um ativo ao navegar.
* **Confirmar ao sair do SPS**
   * Exibe uma janela de confirmação antes de sair do Sistema de publicação Scene 7.
* **Incluir udfs na pesquisa**
   * Desmarcado (padrão) para melhorar o desempenho do sistema na maioria das buscas de metadados que você executa.

Se a maioria dos seus metadados se beneficiar de incluir campos definidos pelo usuário, você pode selecionar essa opção para ativá-la. Como alternativa, use a Pesquisa avançada para fornecer uma experiência de pesquisa mais direcionada e mais rápida do que incluir campos definidos pelo usuário.

Consulte [Realizar uma pesquisa avançada](searching-assets.md#conducting_an_advanced_search).

Consulte também [Campos definidos pelo usuário](application-setup.md#user_defined_fields).

* **Tipo de pesquisa básica**
   * Escolha um tipo de pesquisa padrão, Contém ou Começa com.
* **Mostrar recursos do portal de mídia**
   * Selecione esta opção para acessar recursos do Media Portal, como o Media Carrt.
* **Mostrar feedback de comando**
   * Mostrar solicitações de comando para o servidor.
* **Mostrar caixa de diálogo durante a exportação**
   * Exibe uma caixa de diálogo quando você realiza uma exportação. Se desmarcar essa opção, você ainda poderá acessar a página Tarefas para recuperar os resultados da exportação.

## Email

* **Opções de e-mail**
   * Escolha como você deseja que o Dynamic Media Classic informe por email quando carregar e publicar trabalhos. Você pode receber avisos de conclusão de tarefas somente se houver avisos ou erros.
* **Escopo do email**
   * Determina se você recebe todo o serviço de email para sua empresa ou somente email sobre carregar e publicar trabalhos que você inicia.
* **Tipos de e-mail**
   * Determina se você é informado quando as tarefas de upload e publicação de tarefas são concluídas.
* **Idioma**
* **Idioma preferencial**
   * Determina o idioma da interface.
* **Senha**
* **Nova senha**
   * Insira uma nova senha válida. Sua senha deve atender aos seguintes requisitos:
      * Tenha entre 8a 25 caracteres
      * Conter pelo menos uma letra minúscula
      * Conter pelo menos uma letra maiúscula
      * Conter pelo menos um número
      * Contiver pelo menos um dos seguintes caracteres especiais: # $ &amp;-_: {}

* **Redigitar senha**
   * Insira novamente a nova senha para confirmar que você o está inserindo corretamente.
* **Expiração da senha**
   * Determina se a senha expira após 72 dias como uma medida de segurança. Se você selecionar Sim, será solicitado a criar uma nova senha após 72 dias.
