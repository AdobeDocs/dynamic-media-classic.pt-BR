---
title: Configuração pessoal
description: Todos os usuários podem alterar as configurações na tela Configuração pessoal do Dynamic Media Classic.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 1%

---


# Configuração pessoal {#personal-setup}

Todos os usuários podem alterar as configurações na tela Configuração pessoal. Para abrir a tela Configuração pessoal, clique em Configuração > Configuração pessoal.

>[!NOTE]
>
>A tela Configuração pessoal lista qual função de usuário você tem no Dynamic Media Classic: Administrador, Administrador ou Usuário da empresa.

As configurações de configuração pessoal controlam o comportamento padrão do Painel de navegação, como você recebe e-mails e as configurações de senha. Lembre-se de clicar em Salvar depois de alterar essas configurações.

## Informações da minha conta

Identifica o nome da sua conta, o nome, o nome de usuário (endereço de email) e a função de usuário atribuída.

### Versão do desktop

Clique em Instalar agora para instalar a versão para desktop do Dynamic Media Classic no disco rígido local. Ou clique em Reinstalar agora para instalar a versão da área de trabalho novamente.

## Para instalar o plug-in no disco rígido local

1. Na página Instalação pessoal no Dynamic Media Classic, em Illustrator Plug-in for Web-to-Print, clique em **Baixar agora** para baixar o arquivo **Illustrator Plug-in for Web-to-Print.zip**.
1. Descompacte o arquivo ZIP em uma pasta temporária.

   Um arquivo readme é incluído na raiz do arquivo descompactado para fornecer informações adicionais sobre o plug-in.

1. Dependendo do sistema operacional instalado, execute um dos procedimentos a seguir:

### Windows

| Se você estiver executando | Faça isso |
|--- |--- |
| Adobe Illustrator 18 no Adobe Creative Cloud 2014 | <ul><li>Na raiz da pasta descompactada, clique em CC-2014.</li><li>Dependendo da versão bit do Adobe Illustrator que você estiver usando, clique em win32 ou win64.</li><li>Clique em bibliotecas > chama e copie `aflame.dll` para a pasta executável do Adobe Illustrator. Por exemplo, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Observação**: Este caminho de exemplo é para o local de 64 bits; o local de 32 bits pode estar em Arquivos de Programa (x86).  <br/><ul><li>Retorne à mesma pasta de bibliotecas, clique em flamingo e copie `aflamingo.dll` para a mesma pasta executável do Adobe Illustrator que você usou na etapa anterior. </li><li>Retorne à pasta win32 ou win64 selecionada na etapa 2 e copie `AdobeS7FXGFileFormat.aip` para a pasta de plug-ins Adobe Illustrator. Por exemplo, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Observação**: Este caminho de exemplo é para o local de 64 bits; o local de 32 bits pode estar em Arquivos de Programa (x86). |
| Adobe Illustrator 17 no Adobe Creative Cloud | <ul><li>Na raiz da pasta descompactada, clique em CC. </li><li>Dependendo da versão bit do Adobe Illustrator que você estiver usando, clique em win32 ou win64.</li><li> Copie `AdobeS7FXGFileFormat.aip` para a pasta de plug-ins do Adobe Illustrator. Por exemplo, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Observação**: Este caminho de exemplo é para o local de 64 bits; o local de 32 bits pode estar em Arquivos de Programa (x86). |
| Adobe Illustrator 16 no Creative Suite 6 | <ul><li>Na raiz da pasta descompactada, clique em 6.0. </li><li>Dependendo da versão bit do Adobe Illustrator que você estiver usando, clique em win32 ou win64. </li><li>Copie Adobe7FXGFileFormat.aip para a pasta de plug-ins Adobe Illustrator. Por exemplo, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Observação**: Este caminho de exemplo é para o local de 64 bits; o local de 32 bits pode estar em Arquivos de Programa (x86). |

### Mac

| Se você estiver executando | Faça isso |
|--- |--- |
| Adobe Illustrator 18 no Adobe Creative Cloud 2014 | <ul><li>Na raiz da pasta descompactada, clique em CC-2014 > mac64.</li><li>Clique em bibliotecas > chama e copie a pasta `aflame.framework` para a pasta de conteúdo do pacote Adobe Illustrator. Por exemplo, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (Para abrir a pasta de conteúdo do pacote da Adobe Illustrator, clique com o botão direito do mouse no ícone Adobe illustrator CC 2014 e clique em Mostrar conteúdo do pacote no menu de contexto).</li><li>Retorne à mesma pasta de bibliotecas, clique em `flamingo` e copie a pasta `aflamingo.framework` para a mesma pasta de conteúdo do pacote Adobe Illustrator que você usou na etapa anterior.</li><li>Retorne à pasta mac64 selecionada na etapa 1 e copie a pasta `AdobeS7FXGFileFormat.aip` para a pasta de plug-in da Adobe Illustrator. Por exemplo, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 17 no Adobe Creative Cloud | <ul><li>Na raiz da pasta descompactada, clique em CC > mac64</li><li>Copie a pasta `AdobeS7FXGFileFormat.aip` para a pasta de plug-in da Adobe Illustrator. Por exemplo, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 16 no Creative Suite 6 | <ul><li>Na raiz da pasta descompactada, clique em 6.0 > mac64</li><li>Copie a pasta `AdobeS7FXGFileFormat.aip` para a pasta de plug-in da Adobe Illustrator. Por exemplo, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul> |

O plug-in agora está disponível para você usar no Adobe Illustrator.

### Navegador

* **Tamanho da miniatura**
   * Determina o tamanho padrão das imagens em miniatura na visualização de grade no painel Procurar.
* **Visualização da Biblioteca de ativos padrão**
   * Determina se os ativos na Biblioteca de ativos para conjuntos de compilação aparecem como miniaturas ou por nome. Se você estiver trabalhando com grandes quantidades de ativos na Biblioteca de ativos, poderá visualização os ativos por nome. Por exemplo, se você estiver criando um eCatalog grande com muitos arquivos PDF, poderá visualização os ativos por nome para diminuir a lista.
* **Ordem de classificação de navegação padrão**
   * Determina a ordem na qual os ativos aparecem por padrão no Painel de navegação. Escolha um critério de classificação no menu e se deseja uma classificação crescente ou decrescente.
* **Local de navegação padrão**
   * Permite que você defina o local de navegação como padrão, a última pasta navegada ou para um local específico para o qual você navega e identifica. Você também pode definir o local de navegação para classificar os arquivos e pastas em ordem crescente ou decrescente.
* **Visualização de navegação padrão**
   * Determina se a visualização de grade ou a visualização de Lista é a visualização padrão que você vê ao abrir o painel Procurar.
* **Exibição da tela de apresentação**
   * Determina se você vê alguma tela inicial, incluindo a tela inicial Bem-vindo.
* **Mostrar dicas de ferramentas**
   * Determina se as dicas de ferramenta aparecem quando você move o ponteiro sobre botões, menus e links de navegação. Dicas de ferramentas descrevem itens na tela.
* **Plano de fundo do xadrez**
   * Exibe uma camada de tabuleiro de xadrez atrás de imagens, permitindo que você veja facilmente as áreas transparentes de uma imagem que tem um canal alfa.
* **Mostrar tamanho do arquivo**
   * Exibe o tamanho de arquivo de um ativo quando você está navegando.
* **Incluir UDFs na pesquisa**
   * Desmarcada (padrão) para melhorar o desempenho do sistema para a maioria das pesquisas de metadados que você executa.

Se a maioria das suas pesquisas de metadados beneficiar-se da inclusão de campos definidos pelo usuário, é possível selecionar essa opção para ativá-la. Como alternativa, use a Pesquisa avançada para fornecer uma experiência de pesquisa mais direcionada e rápida do que incluindo campos definidos pelo usuário.

Consulte [Realizando uma pesquisa avançada](searching-assets.md#conducting_an_advanced_search).

Consulte também [Campos Definidos pelo Usuário](application-setup.md#user_defined_fields).

* **Tipo de pesquisa básica**
   * Escolha um tipo de pesquisa padrão, Contém ou Start com.
* **Mostrar recursos do Portal de mídia**
   * Selecione essa opção para acessar os recursos do Portal de mídia, como o Carrinho de mídia.
* **Mostrar feedback de comando**
   * Mostrar solicitações de comando para o servidor.
* **Mostrar caixa de diálogo durante a exportação**
   * Exibe uma caixa de diálogo quando você executa uma exportação. Se desmarcar essa opção, você ainda poderá ir para a página Tarefas para recuperar os resultados da exportação.

## Email

* **Opções de e-mail**
   * Escolha como deseja que o Dynamic Media Classic informe você por email quando os trabalhos de upload e publicação forem concluídos. Você pode receber avisos de conclusão de trabalhos somente se ocorrerem avisos ou erros.
* **Escopo de email**
   * Determina se você recebe todos os emails de trabalho para sua empresa ou somente emails sobre upload e publicação de trabalhos iniciados.
* **Tipos de email**
   * Determina se você é informado quando trabalhos de upload e publicação são concluídos.
* **Idioma**
* **Idioma preferencial**
   * Determina o idioma da interface.
* **Senha**
* **Nova senha**
   * Digite uma nova senha válida. Sua senha deve atender aos seguintes requisitos:
      * Ter entre 8 e 25 caracteres
      * Contém pelo menos uma letra minúscula
      * Contém pelo menos uma letra maiúscula
      * Contém pelo menos um número
      * Contenha pelo menos um dos seguintes caracteres especiais: #$&amp;-_:{}
* **Digite novamente a senha**
   * Digite novamente a nova senha para confirmar que você a está inserindo corretamente.
* **Expiração da senha**
   * Determina se a senha expira após 72 dias como medida de segurança. Se você selecionar Sim, será solicitado que você crie uma nova senha após 72 dias.
