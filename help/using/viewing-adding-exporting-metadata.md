---
title: Visualizar, adicionar e exportar metadados
description: Saiba como visualizar, adicionar e exportar metadados no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '2154'
ht-degree: 0%

---

# Visualizar, adicionar e exportar metadados{#viewing-adding-and-exporting-metadata}

Você pode armazenar informações específicas para os arquivos com os quais trabalha no Adobe Dynamic Media Classic; essas informações são chamadas de *metadados*. Você pode usar metadados no Adobe Dynamic Media Classic para organizar, pesquisar, filtrar e classificar seus ativos.

Os metadados são exibidos na Exibição de detalhes. Ela é exibida junto com as informações geradas pela Adobe Dynamic Media Classic. Por exemplo, data de criação do arquivo, data de publicação e palavras-chave. Para exibir metadados, abra o ativo na Exibição de detalhes e selecione o painel Metadados. É possível inserir e editar metadados na Exibição de Detalhes.

Alguns metadados são incorporados diretamente a um arquivo. Se um arquivo contiver esses metadados, o Adobe Dynamic Media Classic fará o upload automaticamente com o arquivo. É possível incorporar metadados em ativos de origem no Adobe Photoshop, InDesign, Illustrator e outros aplicativos; a Adobe Dynamic Media Classic reconhece esses metadados. Você também pode adicionar metadados a arquivos individuais no painel Metadados na Exibição de detalhes. Para garantir a consistência entre os ativos, os administradores da empresa criam modelos de metadados que fornecem os campos de metadados que podem ser preenchidos.

Para obter mais informações sobre metadados incorporados, consulte [Plataforma de metadados extensível](https://www.adobe.com/products/xmp.html).

## Exibir metadados {#view-metadata}

Para exibir os metadados de um ativo, abra o ativo na Exibição de detalhes e toque no painel Metadados. Para selecionar um conjunto de campos de metadados, escolha uma opção no menu Exibição de Metadados. A Adobe Dynamic Media Classic oferece estas Visualizações de metadados:

* **Visualização compacta**: uma lista básica de valores.

* **IPTC**: Valores conforme definidos pelo International Press Telecommunications Council.

* **XMP**: Valores conforme definidos pelo programa de metadados extensíveis.

Os administradores podem criar visualizações de metadados. Essas exibições também aparecem no menu Exibições de metadados.

Consulte [Visualizações de metadados](application-setup.md#metadata_views) para obter informações sobre como criar Exibições de Metadados.

## Inserir metadados manualmente para um ativo {#manually-enter-metadata-for-an-asset}

1. Abra o ativo na Exibição de detalhes.
1. Abra o painel Metadados e execute um ou ambos os procedimentos a seguir:

   * Escolha uma Exibição de metadados para determinar quais campos de metadados aparecem no painel.
   * Escolha um Valor predefinido e selecione **[!UICONTROL Apply]** para preencher campos de metadados com valores predefinidos. Os administradores da empresa criam esses valores predefinidos.

1. Insira os valores no painel Metadados.

>[!NOTE]
>
>Para editar os metadados de vários ativos de uma só vez, selecione os ativos e vá para **[!UICONTROL File]** > **[!UICONTROL Edit Info]**. As edições feitas nos metadados na janela Editar informações se aplicam a todos os ativos selecionados.

## Adicionar ou editar palavras-chave {#add-or-edit-keywords}

Além dos metadados, você pode usar palavras-chave para ajudar a pesquisar e gerenciar seus ativos.

Se você tiver adicionado palavras-chave a outros arquivos durante esta sessão ou se tiver removido palavras-chave da lista, elas aparecerão na tabela Sugestões de palavra-chave.

1. Abra o arquivo na Exibição de detalhes.
1. Selecionar **[!UICONTROL Keywords]**.
1. Para adicionar palavras-chave, siga um destes procedimentos:

   * Digite uma palavra-chave na caixa de texto e selecione **[!UICONTROL Add]**.
   * Selecione uma palavra-chave na **[!UICONTROL Keyword Suggestions]** tabela.

1. Para remover uma palavra-chave, selecione-a e **[!UICONTROL Remove]**. Ele é movido para a tabela Sugestões de palavra-chave.

>[!NOTE]
>
>Você pode adicionar palavras-chave a arquivos enquanto faz upload para o Adobe Dynamic Media Classic. Na caixa de diálogo Fazer Upload das Opções de Job, escolha **[!UICONTROL More Metadata]** e insira palavras-chave.
>Consulte [Opções de upload](uploading-files.md#upload_options).

## Importar metadados {#import-metadata}

Em vez de inserir metadados manualmente um ativo de cada vez, você pode importar metadados de vários ativos diferentes de um arquivo XML ou delimitado por tabulação. Inserir os metadados em um arquivo XML ou delimitado por tabulação e importar o arquivo é menos demorado do que inserir metadados em ativos individuais. Na primeira linha do arquivo delimitado por tabulação, informe o ID e os nomes dos campos para os quais deseja registrar metadados. Em cada linha subsequente, insira um nome de ID de ativo seguido por valores de metadados. Os campos que não estão incluídos no arquivo XML ou delimitado por tabulação não são modificados. Para importar metadados de um arquivo XML, verifique se você está em conformidade com o DTD.

>[!NOTE]
>
>Você pode criar um modelo para inserir metadados, de modo que eles possam ser importados corretamente para o Adobe Dynamic Media Classic. Após criar o template, você pode usá-lo para inserir os metadados.
>Consulte [Crie um modelo para inserir metadados para fazer upload](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Você pode encontrar mais informações sobre propriedades padronizadas no [Centro de desenvolvedores do Adobe XMP](https://www.adobe.com/devnet/xmp.html).

1. No painel Procurar, selecione as imagens às quais deseja adicionar metadados do arquivo XML ou delimitado por tabulação.
1. Ir para **[!UICONTROL File]** > **[!UICONTROL Import Metadata]**.
1. No **[!UICONTROL Upload Metadata]** caixa de diálogo, selecione **[!UICONTROL Browse]**.
1. No **[!UICONTROL Select files to upload]** , selecione o arquivo XML ou delimitado por tabulação com os metadados.
1. Insira um nome de trabalho.
1. Selecionar **[!UICONTROL Upload]**.

### Identificar diferentes tipos de metadados na importação

Lembre-se do seguinte ao identificar diferentes tipos de metadados a serem importados:

* Os nomes dos campos definidos pelo usuário são identificados como criados na **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined fields]**. Use o `Generate file` funcionalidade para obter uma lista de todos os UDFs definidos no formato de importação correto.
* As propriedades de metadados de XMP devem ter o prefixo XMP relacionado antes do nome (property-). Dois pontos separam o prefixo e o nome. O prefixo XMP pode ser encontrado em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Schema]** editor. Os nomes técnicos podem ser encontrados na documentação do schema XMP relacionado. Os nomes de propriedades do XMP não aparecem no `Generate file` recurso.
* As propriedades do esquema de metadados devem ter o prefixo relacionado antes do nome (property-). Dois pontos separam o prefixo e o nome. O prefixo e os nomes de propriedade são definidos no Editor de esquema de metadados. Os nomes das propriedades do esquema de metadados não aparecem no `Generate file` recurso.

Por exemplo: a propriedade XMP para palavras-chave é o schema XMP &quot;Dublin Core&quot; com o prefixo `dc` e `subject` é o nome técnico do XMP. O prefixo e o nome técnico do XMP são combinados no `dc:subject` nome completo da propriedade. No formato de importação de metadados XML, `dc.subject` deve ser o nome da propriedade. No formato de importação delimitado por tabulação, deve ser o cabeçalho da coluna.

### Importar palavras-chave

As palavras-chave podem ser importadas como uma lista separada por vírgulas. Se uma vírgula aparecer em qualquer um dos valores individuais, escape-a usando uma barra invertida (\). Uma barra invertida literal é a barra invertida dupla usual (\\).

Por exemplo, um arquivo de importação de metadados contendo o valor `Hello\, World!,back\\slash,foo` para `dc:subject` O define três palavras-chave XMP no ativo: `Hello, World!,` `back\slash,` e `foo`.

### Importar arquivos XMP e XMP de metadados de esquema de metadados

A importação XML aceita somente XML válido. Ao importar campos de XMP ou Esquema de metadados, o prefixo do namespace é adicionado e se comporta aqui como um namespace XMP. Este namespace deve ser declarado. Por exemplo, na tag de nível superior.

Por exemplo:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### Importar arquivos delimitados por tabulação de metadados de esquema de metadados e XMP

O prefixo deve ser adicionado ao cabeçalho de coluna relacionado do campo de importação.

## Importar metadados (via FTP) {#import-metadata-via-ftp}

É possível importar metadados de vários arquivos. Você insere os metadados em um arquivo XML delimitado por tabulação. Em seguida, selecione **[!UICONTROL Process metadata files]** na página Fazer upload das opções de trabalho (pela guia FTP).

Verifique se os dados no arquivo XML ou delimitado por tabulação estão no formato correto. Na primeira linha, insira o campo ID seguido pelos nomes dos campos de metadados que devem ser modificados. Em cada linha subsequente, insira um nome de ID de ativo seguido por valores de metadados. Os campos que não estão incluídos no arquivo XML ou delimitado por tabulação não são modificados.

Na barra Navegação global, selecione **[!UICONTROL Upload]**. Para importar os metadados, na página Upload, selecione a variável **[!UICONTROL Via FTP]** e selecione **[!UICONTROL Job Options]**. Na caixa de diálogo Fazer Upload das Opções de Job, selecione **[!UICONTROL Job]**, em seguida, selecione a **[!UICONTROL Process metadata files]** caixa de seleção

## Renomear IDs em lote usando metadados {#batch-rename-ids-using-metadata}

Usando metadados importados de um arquivo delimitado por tabulação ou arquivo XML, você pode renomear Adobe Dynamic Media Classic IDs. Os metadados importados são aplicados apenas às imagens especificadas no próprio arquivo de metadados. Não importa se as imagens estão selecionadas no painel Procurar.

Para renomear uma ID do Adobe Dynamic Media Classic de imagem, adicione uma coluna rotulada *newipsid* ao arquivo delimitado por tabulação ou adicione um campo chamado `new_vc_objectname` aos dados XML.

Por exemplo:

| | newipsid |
| --- | --- |
| testcoat_1 | Jacket_test_1 |
| testcoat_blue | Jacket_test_2 |

O log de trabalho para o trabalho de Metadados mostra quais IDs foram renomeadas com êxito e quais não foram.

## Crie um modelo para inserir metadados para fazer upload {#create-a-template-for-entering-metadata-to-upload}

O Adobe Dynamic Media Classic oferece um comando para criar um modelo para gravar metadados. O uso do modelo garante que os metadados sejam inseridos no formato correto para que possam ser carregados corretamente no Adobe Dynamic Media Classic. Para criar um modelo a ser usado na gravação e importação de metadados para o Adobe Dynamic Media Classic, siga estas etapas:

1. Selecione ativos de imagem com campos de metadados que você deseja para o modelo.
1. Ir para **[!UICONTROL File]** > **[!UICONTROL Import Metadata]**.
1. Para o **[!UICONTROL Asset Properties Type]**, selecione **[!UICONTROL Image]**.
1. No **[!UICONTROL `Generate File`]** selecione **[!UICONTROL Tab-delimited Template]**, **[!UICONTROL Asset's XML Metadata]** ou **[!UICONTROL XML DTD]**.
1. Selecionar **[!UICONTROL Generate]**.
1. Na caixa de diálogo exibida, copie os dados. Use esses dados para criar o template.

## Trabalhar com esquemas de metadados {#working-with-metadata-schemas}

Um Administrador de empresa pode exibir uma lista de todos os esquemas disponíveis. Na barra de Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Schema]**.

Inicialmente, a lista de esquemas padrão globais como XMP está oculta. Eles podem ser exibidos usando a caixa de seleção na parte inferior da lista.

O Administrador da empresa pode criar um esquema personalizado ou editar um esquema personalizado existente.

Você pode usar o Editor de esquema de metadados para executar as seguintes ações:

| Ação | Descrição |
| --- | --- |
| Adicionar | Adiciona uma propriedade ao esquema. Uma caixa de diálogo modal coleta as informações: ID, Rótulo, Estrutura e Tipo de dados. |
| Adicionar valor de escolha | Adiciona uma nova opção selecionável a uma propriedade com estrutura Opção aberta ou Opção fechada. Todos os valores de escolha têm o mesmo tipo. Selecione a própria propriedade para ativar o botão. |
| Editar | Edite o Rótulo de uma propriedade ou valor de opção. Você só pode alterar as informações de Rótulo, ID e tipo que são imutáveis. |
| Mover para cima/Mover para baixo | A ordem no esquema é refletida na interface do usuário. Para alterar a ordem, selecione uma propriedade ou um valor de escolha e mova-o com os botões. Arrastar e soltar não é suportado no momento. |
| Excluir | Exclui uma propriedade ou um valor de opção do esquema. Ele não exclui valores do bloco XMP ou do banco de dados. A propriedade não está mais disponível para Exibições de metadados e é removida da Exibição de detalhes do ativo. Se a propriedade tiver sido publicada no Servidor de Metadados, execute uma publicação forçada para remover os dados do Servidor de Metadados voltado para o público. |

O sistema gera automaticamente um esquema personalizado para campos definidos pelo usuário com o prefixo `s7udf`. O esquema consiste em campos existentes definidos pelo usuário que são editados em sua própria seção Configuração.

>[!NOTE]
>
>As alterações no esquema nunca alteram os próprios metadados do ativo. No entanto, elas não estão visíveis para todas as funcionalidades do Adobe Dynamic Media Classic e do Servidor de metadados e não podem ser acessadas após serem alteradas. Da mesma forma, se existirem metadados para um ativo, a criação do esquema correspondente torna os metadados utilizáveis no Adobe Dynamic Media Classic e no Servidor de metadados.

O Editor de esquema de metadados oferece uma maneira gráfica de adicionar ou editar um esquema de empresa personalizado dentro do Adobe Dynamic Media Classic. Um prefixo, um namespace e uma lista de propriedades definem um esquema.

* **[!UICONTROL Name]**: Nome de interface do usuário para o esquema. Usado para identificar as propriedades em Visualizações de metadados e Pesquisa avançada. Semelhante a Seções XMP como Básico, IPTC, PDF.

* **[!UICONTROL Prefix]**: Identificador técnico exclusivo do esquema. Restrito às letras a-z e A-Z. O prefixo não está visível na interface do usuário do Adobe Dynamic Media Classic, mas é usado quando os metadados de um ativo são armazenados no bloco XMP e no banco de dados. O prefixo identifica exclusivamente campos de metadados em consultas de pesquisa de metadados no servidor de metadados ou na importação.

* **[!UICONTROL Namespace]**: Identificador técnico exclusivo para o esquema, normalmente um URL no formulário `https://your.company.com/name/version/`. Consulte a lista de esquemas padrão para ver exemplos. O namespace não está visível na interface do usuário do Adobe Dynamic Media Classic, mas é usado para armazenar metadados no bloco XMP.

* **[!UICONTROL Description]**: Descrição do esquema em formato livre.

>[!NOTE]
>
>O prefixo e o namespace não podem ser editados. Para alterar essas propriedades, você deve excluir e recriar o schema.

As propriedades descrevem os metadados que podem ser armazenados com esse schema no bloco XMP. Uma propriedade consiste em:

| Propriedade | Descrição |
| --- | --- |
| ID | Identificador técnico desta propriedade. A ID não está visível na interface do usuário do Adobe Dynamic Media Classic, mas é usada quando os metadados de um ativo são armazenados no bloco XMP e no banco de dados. A ID é usada para criar consultas de pesquisa no Servidor de metadados. A ID tem algumas restrições, como: `<ul><li>No spaces</li><li>No ".", ":", "$"</li><li>No number as first character</li><li>Best practice is to use a-z or A-Z as first character</li></ul>` <br>Depois de criada, a ID não pode ser alterada. |
| Rótulo | UI-Name para esta propriedade. |
| Estrutura | Determina o tipo da propriedade junto com o Tipo de dados. A estrutura pode ser uma de:<ul><li>Tipo simples: valor único do tipo de dados</li><li>Sequência: uma lista de valores do mesmo tipo de dados</li><li>Abrir Opção: selecione um item de uma lista de valores predefinidos ou informe o texto. Ele só pode ser do tipo de dados String ou Integer</li><li>Opção Fechada: selecione um item em uma lista de valores predefinidos (uma pop-up ou caixa de combinação)</li></ul> |
| Tipo de dados | Selecione um destes tipos disponíveis: <ul><li>String</li><li>Integer</li><li>Flutuante</li><li>Sim/Não (Booleano)</li><li>Data</li></ul> |

Quando a propriedade tiver a estrutura Escolha Aberta ou Escolha Fechada, você deverá fornecer pelo menos um valor de escolha. A opção aberta pode ser alterada. Opção Fechada não pode ser alterada. Todos os valores de escolha têm o Tipo de dados da propriedade.

| Propriedade | Descrição |
| --- | --- |
| ID | Identificador técnico para este valor. A ID não está visível na interface do usuário do Adobe Dynamic Media Classic, mas é usada quando os metadados de um ativo são armazenados no bloco XMP e no banco de dados. A ID é usada em consultas de pesquisa no Servidor de metadados. A ID não pode conter espaços. Depois de criada, a ID não pode ser alterada. |
| Rótulo | UI-Name para este valor. |

>[!MORELIKETHIS]
>
>* [Predefinições do visualizador](application-setup.md#viewer_presets)
>* [Predefinições de metadados](application-setup.md#metadata_presets)
