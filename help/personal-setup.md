---
title: Configuração pessoal
description: Todos os usuários podem alterar as configurações na tela Configuração pessoal do Dynamic Media Classic.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1197'
ht-degree: 1%

---


# Configuração pessoal {#personal-setup}

Todos os usuários podem alterar as configurações na tela Configuração pessoal. Para abrir a tela Configuração pessoal, clique em Configuração > Configuração pessoal.

>[!NOTE]
>
>A tela Configuração pessoal lista qual função de usuário você tem no Dynamic Media Classic: Administrador, Administrador ou Usuário da Empresa.

As configurações de Configuração pessoal controlam o comportamento padrão do Painel de navegação, como você recebe e-mail e as configurações de senha. Lembre-se de clicar em Salvar depois de alterar essas configurações.

## Informações da Minha Conta

Identifica o nome da conta, o nome, o nome de usuário (endereço de email) e a função de usuário atribuída.

### Versão da área de trabalho

Clique em Instalar agora para instalar a versão para desktop do Dynamic Media Classic no disco rígido local. Ou clique em Reinstalar agora para instalar a versão da área de trabalho novamente.

## Para instalar o plug-in no disco rígido local

1. Na página Configuração pessoal no Dynamic Media Classic, em Plug-in do Illustrator para Web-to-Print, clique em **Baixar agora** para baixar o **Plug-in do Illustrator para Web-to-Print.zip** arquivo.
1. Descompacte o arquivo ZIP em uma pasta temporária.

   Um arquivo readme é incluído na raiz do arquivo descompactado para fornecer informações adicionais sobre o plug-in.

1. Dependendo do sistema operacional instalado, execute um dos seguintes procedimentos:

### Windows

| Se você estiver executando | Faça isso |
|--- |--- |
| Adobe Illustrator 18 no Adobe Creative Cloud 2014 | <ul><li>Na raiz da pasta descompactada, clique em CC-2014.</li><li>Dependendo da versão de bits do Adobe Illustrator que você estiver usando, clique em win32 ou win64.</li><li>Clique em bibliotecas > chama e copie `aflame.dll` para a pasta executável do Adobe Illustrator. Por exemplo, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Observação**: Este caminho de exemplo é para o local de 64 bits; em vez disso, o local de 32 bits pode estar sob Arquivos de Programas (x86).  <br/><ul><li>Retorne à mesma pasta de bibliotecas, clique em flamingo e copie `aflamingo.dll` para a mesma pasta executável do Adobe Illustrator que você usou na etapa anterior. </li><li>Retorne para a pasta win32 ou win64 selecionada na etapa 2 e, em seguida, copie `AdobeS7FXGFileFormat.aip` para a pasta de plug-ins do Adobe Illustrator. Por exemplo, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Observação**: Este caminho de exemplo é para o local de 64 bits; em vez disso, o local de 32 bits pode estar sob Arquivos de Programas (x86). |
| Adobe Illustrator 17 no Adobe Creative Cloud | <ul><li>Na raiz da pasta descompactada, clique em CC. </li><li>Dependendo da versão de bits do Adobe Illustrator que você estiver usando, clique em win32 ou win64.</li><li> Copie `AdobeS7FXGFileFormat.aip` para a pasta de plug-ins do Adobe Illustrator. Por exemplo, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Observação**: Este caminho de exemplo é para o local de 64 bits; em vez disso, o local de 32 bits pode estar sob Arquivos de Programas (x86). |
| Adobe Illustrator 16 no Adobe Creative Suite 6 | <ul><li>Na raiz da pasta descompactada, clique em 6.0. </li><li>Dependendo da versão de bits do Adobe Illustrator que você estiver usando, clique em win32 ou win64. </li><li>Copie Adobe7FXGFileFormat.aip para a pasta de plug-ins do Adobe Illustrator. Por exemplo, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Observação**: Este caminho de exemplo é para o local de 64 bits; em vez disso, o local de 32 bits pode estar sob Arquivos de Programas (x86). |

### Mac

| Se você estiver executando | Faça isso |
|--- |--- |
| Adobe Illustrator 18 no Adobe Creative Cloud 2014 | <ul><li>Na raiz da pasta descompactada, clique em CC-2014 > mac64.</li><li>Clique em bibliotecas > chama e copie a pasta `aflame.framework` para a pasta de conteúdo do pacote Adobe Illustrator. Por exemplo, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (Para abrir a pasta de conteúdo do pacote do Adobe Illustrator, clique com o botão direito do mouse no ícone Adobe Illustrator CC 2014 e clique em Mostrar conteúdo do pacote no menu de contexto).</li><li>Retorne à mesma pasta de bibliotecas, clique em `flamingo` e copie a pasta `aflamingo.framework` para a mesma pasta de conteúdo do pacote Adobe Illustrator que você usou na etapa anterior.</li><li>Retorne à pasta mac64 selecionada na etapa 1 e copie a pasta `AdobeS7FXGFileFormat.aip` para a pasta de plug-in do Adobe Illustrator. Por exemplo, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 17 no Adobe Creative Cloud | <ul><li>Na raiz da pasta descompactada, clique em CC > mac64</li><li>Copie a pasta `AdobeS7FXGFileFormat.aip` para a pasta de plug-in do Adobe Illustrator. Por exemplo, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 16 no Adobe Creative Suite 6 | <ul><li>Na raiz da pasta descompactada, clique em 6.0 > mac64</li><li>Copie a pasta `AdobeS7FXGFileFormat.aip` para a pasta de plug-in do Adobe Illustrator. Por exemplo, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul> |

O plug-in agora está disponível para você usar no Adobe Illustrator.

### Navegador

* **Tamanho da miniatura**
   * Determina o tamanho padrão das imagens em miniatura na exibição em Grade no Painel de navegação.
* **Exibição da biblioteca de ativos padrão**
   * Determina se os ativos na Biblioteca de ativos para conjuntos de build aparecem como miniaturas ou por nome. Se você estiver trabalhando com grandes quantidades de ativos na Biblioteca de ativos, é possível visualizar os ativos por nome. Por exemplo, se você estiver criando um grande eCatalog com muitos arquivos PDF, poderá exibir os ativos por nome para tornar a lista mais curta.
* **Ordem de classificação de navegação padrão**
   * Determina a ordem na qual os ativos aparecem por padrão no Painel de navegação. Escolha um critério de classificação no menu e se deseja uma classificação crescente ou decrescente.
* **Local de navegação padrão**
   * Permite definir o local do navegador para o padrão, a última pasta navegada ou para um local específico no qual você navega e identifica. Você também pode definir o local do navegador para classificar os arquivos e pastas em ordem crescente ou decrescente.
* **Exibição de navegação padrão**
   * Determina se a exibição de Grade ou de Lista é a exibição padrão que você vê ao abrir o Painel de navegação pela primeira vez.
* **Exibição da tela de apresentação**
   * Determina se você vê alguma tela inicial, incluindo a tela inicial de Boas-vindas.
* **Mostrar dicas de ferramentas**
   * Determina se as dicas de ferramenta aparecem quando você move o ponteiro sobre botões, menus e links de navegação. Dicas de ferramentas descrevem itens na tela.
* **Fundo do quadro de verificação**
   * Exibe uma camada de tabuleiro atrás de imagens, permitindo que você veja facilmente as áreas transparentes de uma imagem que tem um canal alfa.
* **Mostrar tamanho do arquivo**
   * Exibe o tamanho do arquivo de um ativo durante a navegação.
* **Incluir UDFs na Pesquisa**
   * Desmarcada (padrão) para melhorar o desempenho do sistema para a maioria das pesquisas de metadados executadas.

Se a maioria de suas pesquisas de metadados se beneficiar da inclusão de campos definidos pelo usuário, você poderá selecionar essa opção para ativá-los. Como alternativa, use a Pesquisa avançada para fornecer uma experiência de pesquisa mais direcionada e mais rápida do que incluir campos definidos pelo usuário.

Consulte [Realização de uma pesquisa avançada](searching-assets.md#conducting_an_advanced_search).

Consulte também [Campos definidos pelo usuário](application-setup.md#user_defined_fields).

* **Tipo de pesquisa básica**
   * Escolha um tipo de pesquisa padrão, Contém ou Começa com.
* **Mostrar recursos do Media Portal**
   * Selecione essa opção para acessar recursos do Media Portal, como Carrinho de mídia.
* **Mostrar Feedback de Comando**
   * Mostrar solicitações de comando para o servidor.
* **Mostrar caixa de diálogo durante a exportação**
   * Exibe uma caixa de diálogo quando você executa uma exportação. Se você desmarcar essa opção, ainda poderá acessar a página Trabalhos para recuperar os resultados da exportação.

## Email

* **Opções de email**
   * Escolha como deseja que o Dynamic Media Classic o informe por e-mail quando os trabalhos de upload e publicação forem concluídos. Você pode receber avisos de conclusão de trabalho somente se ocorrerem avisos ou erros.
* **Escopo de email**
   * Determina se você recebe todo o email de trabalho da sua empresa ou apenas o email sobre trabalhos de upload e publicação iniciados.
* **Tipos de email**
   * Determina se você é informado quando trabalhos de upload e publicação são concluídos.
* **Idioma**
* **Idioma preferencial**
   * Determina o idioma da interface.
* **Senha**
* **Nova senha**
   * Digite uma senha nova e válida. Sua senha deve atender aos seguintes requisitos:
      * Ter entre 8 e 25 caracteres
      * Ter pelo menos uma letra minúscula
      * Ter pelo menos uma letra maiúscula
      * Ter pelo menos um número
      * Ter pelo menos um dos seguintes caracteres especiais: #$&amp;-_:{}
* **Digite novamente a senha**
   * Insira novamente a nova senha para confirmar que está digitando corretamente.
* **Expiração da senha**
   * Determina se a senha expira após 72 dias como medida de segurança. Se você selecionar Sim, será solicitado a criar uma nova senha após 72 dias.
