---
title: Exibição, adição e exportação de metadados
description: Saiba como visualização, adicionar e exportar metadados.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '2256'
ht-degree: 0%

---


# Exibição, adição e exportação de metadados{#viewing-adding-and-exporting-metadata}

Você pode armazenar informações específicas para os arquivos com os quais trabalha no Dynamic Media Classic; essas informações são chamadas *metadata*. Você pode usar metadados no Dynamic Media Classic para organizar, pesquisar, filtrar e classificar seus ativos.

Os metadados aparecem em visualização de detalhes junto com as informações geradas pelo Dynamic Media Classic, como data de criação do arquivo, data de publicação e palavras-chave. Para visualização de metadados, abra o ativo na visualização Detalhe e selecione o painel Metadados. Você pode inserir e editar metadados em visualização de detalhes.

Alguns metadados são incorporados diretamente em um arquivo. Se um arquivo contiver esses metadados, o Dynamic Media Classic o carregará automaticamente com o arquivo. Você pode incorporar metadados em ativos de origem no Adobe Photoshop, InDesign, Illustrator e outros aplicativos; O Dynamic Media Classic reconhece esses metadados. Você também pode adicionar metadados a arquivos individuais no painel Metadados na visualização Detalhe. Para garantir a consistência entre ativos, os administradores de empresas criam modelos de Metadados que fornecem os campos de metadados que podem ser preenchidos.

Para obter mais informações sobre metadados incorporados, consulte [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en).

## Metadados de visualização {#view-metadata}

Para visualização dos metadados de um ativo, abra o ativo na visualização Detalhe e clique no painel Metadados. Em seguida, escolha uma opção no menu Visualização de metadados para selecionar um conjunto de campos de metadados. O Dynamic Media Classic oferta essas Visualizações de metadados:

* **Visualização compactaUma lista básica de valores.**


* **Valores**
IPTCVs, definidos pelo Conselho Internacional de Telecomunicações da Imprensa.

* **Valores**
XMPV, conforme definidos pela plataforma de metadados extensível.

Os administradores podem criar Visualizações de metadados. Essas visualizações também aparecem no menu Visualizações de metadados. Para obter informações sobre como criar Visualizações de Metadados, consulte [Visualizações de Metadados](application-setup.md#metadata_views).

## Insira manualmente metadados para um ativo {#manually-enter-metadata-for-an-asset}

1. Abra o ativo na visualização Detalhe.
1. Abra o painel Metadados e execute um dos procedimentos a seguir ou ambos:

   * Escolha uma Visualização de metadados para determinar quais campos de metadados aparecem no painel.
   * Escolha um valor predefinido e clique em Aplicar para preencher campos de metadados com valores predefinidos. Os administradores de empresas criam esses valores predefinidos.

1. Insira valores no painel Metadados.

>[!NOTE]
>
>Para editar os metadados de vários ativos ao mesmo tempo, selecione os ativos e escolha Arquivo > Editar informações. As edições feitas nos metadados na janela Editar informações se aplicam a todos os ativos selecionados.

## Adicionar ou editar palavras-chave {#add-or-edit-keywords}

Além dos metadados, você pode usar palavras-chave para ajudar a pesquisar e gerenciar seus ativos.

Se você tiver adicionado palavras-chave a outros arquivos durante esta sessão, ou se tiver removido palavras-chave da sua lista, elas aparecerão na tabela Sugestões de palavras-chave.

1. Abra o arquivo na Visualização Detalhe.
1. Clique em Palavras-chave.
1. Para adicionar palavras-chave, execute um dos procedimentos a seguir:

   * Digite uma palavra-chave na caixa de texto e clique em Adicionar.
   * Clique em uma palavra-chave na tabela Sugestões de palavra-chave.

1. Para remover uma palavra-chave, selecione-a e clique em Remover. Vai para a tabela Sugestões de palavra-chave.

>[!NOTE]
>
>Você pode adicionar palavras-chave aos arquivos à medida que os carrega para o Dynamic Media Classic. Na caixa de diálogo Carregar opções de trabalho, escolha Metadados adicionais e digite palavras-chave. Consulte [Opções de upload](uploading-files.md#upload_options).

## Importar metadados {#import-metadata}

Em vez de inserir metadados manualmente, um ativo por vez, você pode importar metadados para muitos ativos diferentes de um arquivo XML ou delimitado por tabulação. Digitar os metadados em um arquivo XML ou delimitado por tabulação e importar o arquivo é menos demorado do que inserir metadados em ativos individuais. Na primeira linha do arquivo delimitado por tabulação, digite a ID e os nomes dos campos para os quais deseja registrar metadados. Em cada linha subsequente, insira um nome de ID de ativo seguido de valores de metadados. Os campos que não estão incluídos no arquivo XML ou delimitado por tabulação não são modificados. Para importar metadados de um arquivo XML, verifique se você está em conformidade com o DTD.

>[!NOTE]
>
>Você pode criar um modelo para inserir metadados para que eles possam ser importados corretamente para o Dynamic Media Classic. Depois de criar o modelo, você pode usá-lo para inserir os metadados. Consulte [Crie um modelo para inserir metadados a serem carregados](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Você pode encontrar mais informações sobre propriedades padronizadas em: https://www.adobe.com/devnet/xmp.html

1. No painel Procurar, selecione as imagens às quais deseja adicionar metadados do arquivo XML ou delimitado por tabulação.
1. Clique em **Arquivo** > **Importar metadados**.
1. Na caixa de diálogo **Carregar metadados**, clique em **Procurar**.
1. Na caixa de diálogo **Selecionar arquivos para carregar**, selecione o arquivo delimitado por tabulação ou XML com os metadados.
1. Insira um nome de tarefa.
1. Clique em **Carregar**.

**Identificação de diferentes tipos de metadados na importação**

Lembre-se do seguinte ao identificar diferentes tipos de metadados a serem importados:

* Os Campos Definidos pelo Usuário são identificados pelo nome como criados em Configuração > Configuração do Aplicativo > Metadados > Campos Definidos pelo Usuário. Use a funcionalidade Gerar arquivo para obter uma lista de todos os UDFs definidos no formato de importação correto.
* XMP propriedades de Metadados devem ter o XMP-prefixo relacionado antes do nome (propriedade-). Dois pontos separam o prefixo e o nome. O prefixo XMP pode ser encontrado em Configuração > Configuração do aplicativo > Metadados > Editor de Schemas de metadados. Os nomes técnicos podem ser encontrados na documentação do schema XMP relacionado. Observe que os nomes XMP propriedades não aparecem no recurso Gerar arquivo.
* As propriedades do Schema de metadados devem ter o prefixo relacionado antes do nome (propriedade-). Dois pontos separam o prefixo e o nome. O prefixo e os nomes das propriedades são definidos no editor de Schemas de Metadados. Observe que os nomes das propriedades do Schema Metadados não aparecem no recurso Gerar arquivo.

Por exemplo: A propriedade XMP para palavras-chave é o schema XMP &quot;Dublin Core&quot; com o prefixo &quot;dc&quot; e &quot;subject&quot; é o nome do XMP técnico. O prefixo e o nome do XMP técnico são combinados no nome completo da propriedade &quot;dc:subject&quot;. No formato de importação de metadados XML, &quot;dc.subject&quot; deve ser o nome da propriedade. No formato de importação delimitado por tabulação, ele deve ser o cabeçalho da coluna.

**Importar palavras-chave**

As palavras-chave podem ser importadas como lista separada por vírgulas. Se uma vírgula aparecer em qualquer um dos valores individuais, ela precisa ser escapada por uma barra invertida (\). Uma barra invertida literal é a barra invertida normal do duplo (\\).

Por exemplo, um arquivo de importação de metadados contendo o valor &quot;Hello\, World!,back\\slash,foo&quot; para &quot;dc:subject&quot; define três palavras-chave XMP no ativo: &quot;Olá, Mundo!&quot; &quot;trás\barra&quot; e &quot;foo.&quot;

**Importar arquivos XMP metadados do Schema de XMP e Metadados**

A importação XML aceita somente XML válido. Ao importar XMP ou campos de Schema de Metadados, o prefixo de namespace é adicionado e se comporta aqui como uma namespace XMP. Essa namespace deve ser declarada, por exemplo, na tag de nível superior.

Por exemplo:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

**Importar arquivos delimitados por guia de metadados do Schema de metadados XMP e Metadados**

O prefixo deve ser adicionado ao cabeçalho da coluna relacionada do campo de importação.

## Importar metadados (via FTP) {#import-metadata-via-ftp}

É possível importar metadados para vários arquivos inserindo os metadados em um arquivo XML ou delimitado por tabulação e selecionando a opção Processar arquivos de metadados na tela Carregar (Via FTP).

Verifique se os dados no arquivo delimitado por tabulação ou XML estão no formato correto. Na primeira linha, digite o campo ID seguido dos nomes dos campos de metadados a serem modificados. Em cada linha subsequente, insira um nome de ID de ativo seguido de valores de metadados. Os campos que não estão incluídos no arquivo XML ou delimitado por tabulação não são modificados.

Clique no botão Carregar na barra de navegação global e, na tela Tarefas, selecione a guia Via FTP para importar os metadados. Em seguida, clique em Opções de trabalho. Na caixa de diálogo Carregar opções de trabalho, escolha Processar arquivos de metadados.

## Renomear em lote IDs usando metadados {#batch-rename-ids-using-metadata}

Usando metadados importados de um arquivo delimitado por tabulação ou XML, é possível renomear Dynamic Media Classic IDs. Os metadados importados são aplicados somente às imagens especificadas no próprio arquivo de metadados. Não importa se as imagens estão selecionadas no Painel de navegação.

Para renomear a Dynamic Media Classic ID de uma imagem, adicione uma coluna chamada *newipsid* ao arquivo delimitado por tabulação ou adicione um campo chamado* new_vc_objectname* aos dados XML.

Por exemplo:

| ipsid | newipsid |
|--- |--- |
| jaqueta_1 | Jacket_test_1 |
| jaqueta_azul | Jacket_test_2 |


O log de trabalho do trabalho de Metadados mostrará quais IDs foram renomeadas com êxito e quais não foram.

## Crie um modelo para inserir metadados para carregar {#create-a-template-for-entering-metadata-to-upload}

O Dynamic Media Classic oferta um comando para criar um modelo para a gravação de metadados. O uso do modelo garante que os metadados sejam inseridos no formato correto para que possam ser carregados corretamente no Dynamic Media Classic. Siga estas etapas para criar um modelo para usar na gravação e importação de metadados para o Dynamic Media Classic:

1. Selecione ativos de imagem com campos de metadados que você deseja para o modelo.
1. Escolha Arquivo > Importar metadados.
1. Selecione Imagem para o Tipo de propriedades do ativo.
1. No menu Gerar arquivo, selecione Modelo delimitado por tabulação, Metadados XML do ativo ou DTD XML.
1. Clique em Gerar.
1. Na caixa de diálogo exibida, copie os dados. Use esses dados para construir o modelo.

## Trabalhar com Schemas de metadados {#working-with-metadata-schemas}

Um administrador da empresa pode visualização uma lista de todos os schemas disponíveis. Abra Configuração do aplicativo -> Metadados -> Schema de metadados.

Inicialmente, a lista de schemas padrão globais como XMP está oculta. Eles podem ser exibidos usando a caixa de seleção na parte inferior da lista.

O administrador da empresa pode criar um novo schema personalizado ou editar um schema personalizado existente.

Você pode usar o Editor de Schemas de Metadados para executar as seguintes ações:

| Ação | Descrição |
|--- |--- |
| Adicionar | Adiciona uma nova propriedade ao schema. Uma caixa de diálogo modal coleta as informações: ID, rótulo, estrutura e tipo de dados. |
| Adicionar valor de escolha | Adiciona uma nova opção selecionável a uma propriedade com a estrutura Open Choice ou Closed Choice. Todos os valores de escolha têm o mesmo tipo. Você deve selecionar a propriedade para ativar o botão. |
| Editar | Edite o Rótulo de uma propriedade ou valor de escolha. Você só pode alterar o Rótulo, a ID e as informações de tipo são imutáveis. |
| Mover para cima/Mover para baixo | A ordem no schema é refletida na interface do usuário. Para alterar a ordem, selecione uma propriedade ou um valor de escolha e mova-o com os botões. No momento, não há suporte para arrastar e soltar. |
| Excluir | Exclui uma propriedade ou um valor de escolha do schema. Isso não exclui valores do bloco XMP ou do Banco de Dados. A propriedade não está mais disponível para Visualizações de Metadados e é removida da Visualização Detalhes do Ativo.Se a propriedade foi publicada no Servidor de Metadados, execute uma publicação forçada para remover os dados do Servidor de Metadados voltado para o público. |

O sistema gera automaticamente um schema personalizado para campos definidos pelo usuário com o prefixo &quot;s7udf&quot;. Esses são os campos definidos pelo usuário e são editados em sua própria seção Configuração.

>[!NOTE]
>
>As alterações no schema nunca alteram os próprios metadados do ativo. No entanto, eles não estão visíveis para todas as funcionalidades do Dynamic Media Classic e do Servidor de Metadados e não podem ser acessados após serem alterados. Da mesma forma, se houver metadados para um ativo, a criação do schema correspondente torna os metadados utilizáveis no Dynamic Media Classic e no Servidor de metadados.

O Editor de Schemas de metadados oferta uma forma gráfica para adicionar ou editar um schema de empresa personalizado dentro do Dynamic Media Classic. Um schema é definido por um prefixo, uma namespace e uma lista de propriedades.

* Nome

   UI-Name para o schema. Usado para identificar as propriedades nas Visualizações de metadados e na Pesquisa avançada. Semelhante a XMP seções como Básico, IPTC e PDF.

* Prefixo

   Identificador exclusivo técnico do schema. Limitado às letras a-z e A-Z. O prefixo não é visível na interface do usuário do Dynamic Media Classic, mas é usado quando os metadados de um ativo são armazenados no bloco XMP e em nosso banco de dados. O prefixo é usado para identificar exclusivamente campos de metadados em query de pesquisa de metadados no Servidor de Metadados ou importar.

* Namespace

   Identificador exclusivo técnico do schema, geralmente um URL no formato `https://your.company.com/name/version/`. Consulte a lista de schemas padrão para obter exemplos. A namespace não está visível na interface do usuário do Dynamic Media Classic, mas é usada para armazenar metadados no bloco XMP.

* Descrição

   Descrição do formulário gratuito do schema.

>[!NOTE]
>
>Não é possível editar o prefixo e a namespace. Para alterar essas propriedades, você deve excluir e recriar o schema.

As propriedades descrevem os metadados que podem ser armazenados com esse schema no bloco XMP. Uma propriedade consiste em:

| Propriedade | Descrição |
|--- |--- |
| ID | Identificador técnico desta propriedade. A ID não é visível na interface do usuário do Dynamic Media Classic, mas é usada quando os metadados de um ativo são armazenados no bloco XMP e em nosso banco de dados. A ID é usada para criar query de pesquisa no Servidor de Metadados. A ID tem algumas restrições, como: <ul><li>Sem espaços</li><li>Não &quot;.&quot;, &quot;:&quot;, &quot;$&quot;</li><li>Nenhum número como primeiro caractere</li><li>A prática recomendada é usar a-z ou A-Z como primeiro caractere</li></ul> <br>Depois de criada, a ID não pode ser alterada. |
| Rótulo | UI-Name para esta propriedade. |
| Estrutura | Determina o tipo da propriedade junto com o Tipo de dados. A estrutura pode ser uma das seguintes:<ul><li>Tipo simples: valor único do tipo de dados</li><li>Sequência: uma lista de valores do mesmo tipo de dados</li><li>Opção aberta: selecione um item de uma lista de valores predefinidos ou insira texto livre. Pode ser somente do tipo de dados String ou Integer</li><li>Escolha fechada: selecione um item de uma lista de valores predefinidos (uma caixa pop-up ou combo)</li></ul> |
| Tipo de dados | Selecione um destes tipos disponíveis: <ul><li>String</li><li>Número inteiro</li><li>Flutuar</li><li>Sim/Não (Booliano)</li><li>Data</li></ul> |


Quando a propriedade tem a estrutura Escolha Aberta ou Escolha Fechada, você deve fornecer pelo menos um Valor de Escolha. A opção Abrir pode ser alterada. A opção Fechada não pode ser alterada. Todos os valores de escolha têm o tipo de dados da propriedade.

| Propriedade | Descrição |
|--- |--- |
| ID | Identificador técnico para este valor. A ID não está visível na interface do usuário do Dynamic Media Classic, mas é usada quando os metadados de um ativo são armazenados no bloco XMP e no banco de dados. A ID é usada em query de pesquisa no Servidor de Metadados. A ID não pode conter espaços. Depois de criada, a ID não pode ser alterada. |
| Rótulo | UI-Name para este valor. |

>[!MORELIKETHIS]
>
>* [Predefinições do visualizador](application-setup.md#viewer_presets)
>* [Predefinições de metadados](application-setup.md#metadata_presets)

