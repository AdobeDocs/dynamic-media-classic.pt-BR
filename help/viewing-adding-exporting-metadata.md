---
title: Exibição, adição e exportação de metadados
seo-title: Exibição, adição e exportação de metadados
description: 'null'
seo-description: Saiba como exibir, adicionar e exportar metadados.
uuid: a 5254 c 51-9 e 04-45 ae -8236-3 eab 2925 e 5 fc
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/managing_ assets
discoiquuid: 5414 b 4 f 5-6 e 05-468 c -8725-385423596342
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Exibição, adição e exportação de metadados{#viewing-adding-and-exporting-metadata}

É possível armazenar informações específicas aos arquivos com os quais você trabalha no Sistema de publicação Scene 7; essas informações são chamadas *de metadados*. Você pode usar metadados no Dynamic Media Classic para organizar, pesquisar, filtrar e classificar seus ativos.

Os metadados aparecem na exibição Detalhe junto com informações geradas pelo Dynamic Media Classic, como data de criação de arquivos, data de publicação e palavras-chave. Para exibir metadados, abra o ativo na exibição Detalhe e selecione o painel Metadados. Você pode inserir e editar metadados na exibição Detalhe.

Alguns metadados são incorporados diretamente em um arquivo. Se um arquivo contiver esses metadados, o Dynamic Media Classic o carregará automaticamente com o arquivo. Você pode incorporar metadados em itens de origem no Adobe Photoshop, indesign, Illustrator e outros aplicativos; O Dynamic Media Classic reconhece esses metadados. Você também pode adicionar metadados a arquivos individuais no painel Metadados na exibição Detalhe. Para garantir a consistência entre os ativos, os administradores da empresa criam modelos de metadados que fornecem os campos de metadados que podem ser preenchidos.

Para obter mais informações sobre metadados incorporados, consulte [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en).

## Exibir metadados {#view-metadata}

Para exibir os metadados de um ativo, abra o ativo na exibição Detalhe e clique no painel Metadados. Em seguida, escolha uma opção no menu Exibição de metadados para selecionar um conjunto de campos de metadados. O Dynamic Media Classic oferece essas Exibições de metadados:

**Exibição compacta** Uma lista básica de valores.

**Valores IPTC** , conforme definido pelo International Press Telecommunications Council.

**Valores XMP** , conforme definido pela plataforma de metadados extensível.

Os administradores podem criar exibições de metadados. Essas exibições também aparecem no menu Exibições de metadados. Para obter informações sobre como criar exibições de metadados, consulte [Exibições de metadados](application-setup.md#metadata_views).

## Inserir metadados manualmente para um ativo {#manually-enter-metadata-for-an-asset}

1. Abra o ativo na exibição Detalhe.
1. Abra o painel Metadados e execute um dos procedimentos a seguir:

   * Escolha uma Exibição de metadados para determinar quais campos de metadados aparecem no painel.
   * Escolha um Valor predefinido e clique em Aplicar para preencher campos de metadados com valores predefinidos. Os administradores de empresa criam esses valores predefinidos.

1. Insira valores no painel Metadados.

>[!NOTE]
>
>Para editar os metadados de vários ativos de uma vez, selecione os ativos e escolha Arquivo &gt; Editar informações. As edições feitas aos metadados na janela Editar informações se aplicam a todos os ativos selecionados.

## Adicionar ou editar palavras-chave {#add-or-edit-keywords}

Além dos metadados, você pode usar palavras-chave para auxiliar na pesquisa e no gerenciamento de ativos.

Se você tiver adicionado palavras-chave a outros arquivos durante esta sessão, ou se tiver removido palavras-chave da lista, elas aparecerão na tabela Sugestões de palavra-chave.

1. Abra o arquivo na Exibição de detalhes.
1. Clique em Palavras-chave.
1. Para adicionar palavras-chave, execute um dos seguintes procedimentos:

   * Digite uma palavra-chave na caixa de texto e clique em Adicionar.
   * Clique em uma palavra-chave na tabela Sugestões de palavra-chave.

1. Para remover uma palavra-chave, selecione-a e clique em Remover. Ele move para a tabela Sugestões de palavras-chave.

>[!NOTE]
É possível adicionar palavras-chave a arquivos quando você os carrega no Dynamic Media Classic. Na caixa de diálogo Carregar opções de trabalho, escolha Metadados adicionais e insira palavras-chave. Consulte [Opções de upload](uploading-files.md#upload_options).

## Importar metadados {#import-metadata}

Em vez de inserir manualmente metadados um ativo por vez, você pode importar metadados para muitos ativos diferentes de um arquivo delimitado por tabulação ou XML. Inserir os metadados em um arquivo delimitado por tabulação ou XML e importar o arquivo é menos demorado do que inserir metadados em ativos individuais. Na primeira linha do arquivo delimitado por tabulação, insira a ID e os nomes dos campos cujos metadados você deseja gravar. Em cada linha subsequente, insira um nome de ID de ativo seguido por valores de metadados. Os campos não incluídos no arquivo delimitado por tabulação ou XML não são modificados. Para importar metadados de um arquivo XML, verifique se você está em conformidade com o DTD.

>[!NOTE]
Você pode criar um modelo para inserir metadados para que possa ser importado corretamente para o Sistema de publicação Scene 7. Depois de criar o modelo, você pode usá-lo para inserir os metadados. Consulte [Criar um modelo para inserir metadados para fazer upload](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Você pode encontrar mais informações sobre propriedades padronizadas em: https://www.adobe.com/devnet/xmp.html

1. No Painel Procurar, selecione as imagens nas quais deseja adicionar metadados a partir do arquivo delimitado por tabulações ou XML.
1. Clique **em Arquivo** &gt; **Importar metadados**.
1. Na caixa de diálogo **Carregar metadados** , clique em **Procurar**.
1. Na **caixa de** diálogo Selecionar arquivos para carregar, selecione o arquivo delimitado por tabulação ou XML com os metadados.
1. Insira um nome de serviço.
1. Clique em **Carregar**.

**Identificação de tipos de metadados diferentes na importação**

Lembre-se do seguinte ao identificar diferentes tipos de metadados a serem importados:

* Os campos definidos pelo usuário são identificados pelo nome criado em Configuração &gt; Configuração do aplicativo &gt; Metadados &gt; Campos definidos pelo usuário. Use a funcionalidade Gerar arquivo para obter uma lista de todas as udfs definidas no formato de importação correto.
* As propriedades de metadados XMP devem ter o prefixo XMP relacionado antes do nome (property-). Um sinal de dois pontos separa o prefixo e o nome. O prefixo XMP pode ser encontrado em Configuração &gt; Configuração do aplicativo &gt; Metadados &gt; Editor de esquema de metadados. Os nomes técnicos podem ser encontrados na documentação do esquema XMP relacionado. Observe que os nomes das propriedades XMP não aparecem no recurso Gerar arquivo.
* As propriedades do esquema de metadados devem ter o prefixo relacionado antes do nome (property-). Um sinal de dois pontos separa o prefixo e o nome. O prefixo e os nomes de propriedades são definidos no editor de Esquema de metadados. Observe que os nomes das propriedades do Esquema de metadados não aparecem no recurso Gerar arquivo.

Por exemplo: A propriedade XMP das palavras-chave é o esquema XMP "Dublin Core" com o prefixo "dc" e "sujeito" é o nome técnico XMP. O prefixo e o nome técnico XMP são combinados no "dc: " nome da propriedade inteira ". No formato de importação de metadados XML, "dc. subject" deve ser o nome da propriedade. No formato de importação delimitado por tabulação, deve ser o cabeçalho da coluna.

**Importar palavras-chave**

As palavras-chave podem ser importadas como uma lista separada por vírgulas. Se uma vírgula aparecer em qualquer valor individual, ela precisará ser escapada por uma barra invertida (\). Uma barra invertida literal é a barra invertida comum (\\).

Por exemplo, um arquivo de importação de metadados contendo o valor "Hello\, World! , voltar\\ barra, foo "para" dc: " define três palavras-chave XMP no ativo: " Hello, World! , "voltar\ barra," e "foo."

**Importar arquivos XMP de metadados XMP e metadados**

A importação XML aceita somente XML válido. Ao importar campos XMP ou Esquema de metadados, o prefixo do namespace é adicionado e se comporta aqui como um namespace XMP. Esse namespace deve ser declarado por exemplo na tag de nível superior.

Por exemplo:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

**Importar metadados delimitados por XMP e metadados de metadados de importação**

O prefixo deve ser adicionado ao cabeçalho da coluna relacionada do campo de importação.

## Importar metadados (via FTP) {#import-metadata-via-ftp}

É possível importar metadados para vários arquivos inserindo os metadados em um arquivo delimitado por tabulação ou XML e selecionando a opção Processar arquivos de metadados no upload (Via FTP).

Verifique se os dados no arquivo delimitado por tabulação ou XML estão no formato correto. Na primeira linha, insira o campo ID seguido pelos nomes dos campos de metadados a serem modificados. Em cada linha subsequente, insira um nome de ID de ativo seguido por valores de metadados. Os campos não incluídos no arquivo delimitado por tabulação ou XML não são modificados.

Clique no botão Carregar na barra de navegação global e, na tela Tarefas, selecione a guia Via FTP para importar os metadados. Em seguida, clique em Opções de trabalho. Na caixa de diálogo Fazer upload das opções de trabalho, escolha Processar arquivos de metadados.

## Renomear IDs em lote usando metadados {#batch-rename-ids-using-metadata}

Usando metadados importados de um arquivo delimitado por tabulação ou um arquivo XML, você pode renomear as IDs do sistema de publicação Scene 7. Os metadados importados são aplicados somente às imagens especificadas no próprio arquivo de metadados. Não importa se as imagens estão selecionadas no Painel Procurar.

Para renomear a ID do sistema de publicação do Scene 7 de uma imagem, adicione uma coluna chamada *newipsid* ao arquivo delimitado por tabulação ou adicione um campo chamado * new_ vc_ objectname * aos dados XML.

Por exemplo:

| ipsid | newipsid |
|--- |--- |
| testjacket_ 1 | Jacket_ test_ 1 |
| testjacket_ blue | Jacket_ test_ 2 |


O log de tarefas para o trabalho de metadados mostrará quais IDs foram renomeadas com sucesso e quais não estavam.

## Criar um modelo para inserir metadados para fazer upload {#create-a-template-for-entering-metadata-to-upload}

O Dynamic Media Classic oferece um comando para a criação de um modelo para a gravação de metadados. O uso do modelo garante que os metadados sejam inseridos no formato correto para que possam ser carregados corretamente no Sistema de publicação Scene 7. Siga estas etapas para criar um modelo para uso na gravação e importação de metadados para o Sistema de publicação Scene 7:

1. Selecione ativos de imagem com campos de metadados que deseja para o modelo.
1. Escolha Arquivo &gt; Importar metadados.
1. Selecione Imagem para o Tipo de propriedades do ativo.
1. No menu Gerar arquivo, selecione Delimitado por tabulação, Metadados XML do ativo ou DTD XML.
1. Clique em Gerar.
1. Na caixa de diálogo exibida, copie os dados. Use esses dados para criar o modelo.

## Trabalhar com esquemas de metadados {#working-with-metadata-schemas}

Um administrador da empresa pode exibir uma lista de todos os esquemas disponíveis. Abra Configuração do aplicativo -&gt; Metadados -&gt; Esquema de metadados.

Inicialmente, a lista de esquemas padrão globais como XMP ficava oculta. Eles podem ser exibidos usando a caixa de seleção na parte inferior da lista.

O administrador da empresa pode criar um novo esquema personalizado ou editar um esquema personalizado existente.

Você pode usar o Editor de esquema de metadados para executar as seguintes ações:

| Ação | Descrição |
|--- |--- |
| Adicionar | Adiciona uma nova propriedade ao esquema. Uma caixa de diálogo modal coleta as informações: ID, Rótulo, Estrutura e Tipo de dados. |
| Adicionar valor de escolha | Adiciona uma nova escolha selecionável a uma propriedade com estrutura Aberta ou Opção fechada. Todos os valores de escolha têm o mesmo tipo. Você deve selecionar a propriedade para ativar o botão. |
| Editar | Edite o rótulo de uma propriedade ou valor de escolha. Você pode alterar somente o rótulo, a ID e as informações de digitação. |
| Mover para cima/Mover para baixo | A ordem no esquema é refletida na interface do usuário. Para alterar a ordem, selecione uma propriedade ou valor de escolha e mova-o com os botões. Arrastar e soltar não é suportado no momento. |
| Excluir | Exclui uma propriedade ou um valor de escolha do esquema. Isso não exclui valores do bloco XMP ou do banco de dados. A propriedade não está mais disponível para Exibições de metadados e é removida da Exibição de detalhes do ativo. Se a propriedade foi publicada no Servidor de metadados, execute uma publicação para remover os dados do servidor de metadados voltado ao público. |

O sistema gera automaticamente um esquema personalizado para campos definidos pelo usuário com o prefixo "s 7 udf". Esses são campos definidos pelo usuário e são editados em sua própria seção Configuração.

>[!NOTE]
As alterações no esquema nunca alteram os metadados do ativo em si. No entanto, eles não estão visíveis para toda a funcionalidade SPS e de metadados e não podem ser acessados após serem alterados. Da mesma forma, se os metadados de um ativo existir, a criação do esquema correspondente tornará os metadados utilizáveis no SPS e no Servidor de metadados.

O Editor de esquema de metadados oferece uma forma gráfica de adicionar ou editar um esquema de empresa personalizado dentro do SPS. Um esquema é definido por um prefixo, um namespace e uma lista de propriedades.

* Nome

   Nome da interface do usuário para o esquema. Usado para identificar as propriedades nas Exibições de metadados e Pesquisa avançada. Semelhante a Seções XMP como Básico, IPTC, PDF.

* Prefixo

   Identificador técnico exclusivo para o esquema. Limitado às letras a-z e A-Z. O prefixo não está visível na interface do usuário do SPS, mas é usado quando os metadados de um ativo são armazenados no bloco XMP e no nosso banco de dados. O prefixo é usado para identificar unicamente os campos de metadados nas consultas de pesquisa de metadados no Servidor de metadados ou na importação.

* Namespace

   Identificador técnico exclusivo para o esquema, geralmente um URL no formulário `https://your.company.com/name/version/`. Consulte a lista de esquemas padrão para obter exemplos. O namespace não está visível na interface do usuário do SPS, mas é usado para armazenar metadados no bloco XMP.

* Descrição

   Descrição de forma gratuita do esquema.

>[!NOTE]
O prefixo e o namespace não podem ser editados. Para alterar essas propriedades, você deve excluir e recriar o esquema.

As propriedades descrevem os metadados que podem ser armazenados com esse esquema no bloco XMP. Uma propriedade consiste em:

| Propriedade | Descrição |
|--- |--- |
| ID | Identificador técnico para essa propriedade. A ID não é visível na interface do usuário do SPS, mas usada, quando os metadados de um ativo são armazenados no bloco XMP e no nosso banco de dados. A ID é usada para criar consultas de pesquisa no servidor de metadados. A ID tem algumas restrições como: <ul><li>Sem espaços</li><li>Não ". ", ": ", " $"</li><li>Nenhum número como o primeiro caractere</li><li>A prática recomendada é usar a-z ou A-Z como primeiro caractere</li></ul> <br>Depois de criada, a ID não pode ser alterada. |
| Rótulo | UI-Name para esta propriedade. |
| Estrutura | Determina o tipo de propriedade juntamente com o Tipo de dados. A estrutura pode ser:<ul><li>Tipo simples: valor único de tipo de dados</li><li>Sequência: uma lista de valores do mesmo tipo de dados</li><li>Abrir escolha: selecione um item de uma lista de valores predefinidos ou insira texto gratuito. Pode ser somente de tipo de dados String ou Integer</li><li>Escolha fechada: selecionar um item de uma lista de valores predefinidos (um pop-up ou uma caixa de combinação)</li></ul> |
| Tipo de dados | Selecione dentre esses tipos disponíveis: <ul><li>String</li><li>Número inteiro</li><li>Flutuar</li><li>Sim/Não (Booliano)</li><li>Data</li></ul> |


Quando a propriedade tem a estrutura Abrir escolha ou Escolha fechada, você deve fornecer pelo menos um Valor de escolha. A opção Abrir escolha pode ser alterada. A opção Escolha fechada não pode ser alterada. Todos os Valores de escolha têm o tipo de dados da propriedade.

| Propriedade | Descrição |
|--- |--- |
| ID | Identificador técnico para esse valor. A ID não é visível na interface do usuário do SPS, mas é usada quando os metadados de um ativo são armazenados no bloco XMP e no banco de dados. A ID é usada nas consultas de pesquisa no servidor de metadados. A ID não pode conter espaços. Depois de criada, a ID não pode ser alterada. |
| Rótulo | UI-Name para este valor. |

>[!MORELIKETHIS]
* [Predefinições do visualizador](application-setup.md#viewer_presets)
* [Predefinições de metadados](application-setup.md#metadata_presets)

