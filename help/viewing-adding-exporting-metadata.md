---
title: Exibição, adição e exportação de metadados
description: Saiba como visualizar, adicionar e exportar metadados.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '2198'
ht-degree: 0%

---

# Exibição, adição e exportação de metadados{#viewing-adding-and-exporting-metadata}

Você pode armazenar informações específicas para os arquivos com os quais trabalha no Adobe Dynamic Media Classic; essas informações são chamadas de *metadata*. Você pode usar metadados no Adobe Dynamic Media Classic para organizar, pesquisar, filtrar e classificar seus ativos.

Os metadados aparecem na Exibição de detalhes junto com as informações geradas pelo Adobe Dynamic Media Classic, como a data de criação do arquivo, a data de publicação e as palavras-chave. Para exibir metadados, abra o ativo na Exibição de detalhes e selecione o painel Metadados . Você pode inserir e editar metadados na Exibição de detalhes.

Alguns metadados são incorporados diretamente em um arquivo. Se um arquivo contiver esses metadados, o Adobe Dynamic Media Classic o carregará automaticamente com o arquivo . Você pode incorporar metadados em ativos de origem no Adobe Photoshop, InDesign, Illustrator e outros aplicativos; O Adobe Dynamic Media Classic reconhece esses metadados. Você também pode adicionar metadados a arquivos individuais no painel Metadados na Exibição de detalhes. Para garantir a consistência entre os ativos, os administradores da empresa criam modelos de metadados que fornecem os campos de metadados que podem ser preenchidos.

Para obter mais informações sobre metadados incorporados, consulte [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en).

## Exibir metadados {#view-metadata}

Para exibir os metadados de um ativo, abra o ativo na Exibição de detalhes e toque no painel Metadados . Para selecionar um conjunto de campos de metadados, escolha uma opção no menu Exibição de metadados . O Adobe Dynamic Media Classic oferece estas Exibições de metadados:

* **Exibição compacta**  - Uma lista básica de valores.

* **IPTC**  - Valores tal como definidos pelo Conselho Internacional de Telecomunicações de Imprensa.

* **XMP**  - Valores como definidos pelo programa de metadados extensíveis.

Os administradores podem criar Exibições de metadados. Essas exibições também são exibidas no menu Visualizações de metadados .

Consulte [Exibições de metadados](application-setup.md#metadata_views) para obter informações sobre como criar Exibições de metadados.

## Inserir manualmente metadados para um ativo {#manually-enter-metadata-for-an-asset}

1. Abra o ativo na Exibição de detalhes.
1. Abra o painel Metadados e execute um ou ambos os procedimentos a seguir:

   * Escolha uma Exibição de metadados para determinar quais campos de metadados aparecem no painel.
   * Escolha um valor predefinido e clique em **[!UICONTROL Apply]** para preencher campos de metadados com valores predefinidos. Os administradores da empresa criam esses valores predefinidos.

1. Insira valores no painel Metadados.

>[!NOTE]
>
>Para editar os metadados de vários ativos de uma só vez, selecione os ativos e clique em **[!UICONTROL File]** > **[!UICONTROL Edit Info]**. As edições feitas nos metadados na janela Editar informações se aplicam a todos os ativos selecionados.

## Adicionar ou editar palavras-chave {#add-or-edit-keywords}

Além dos metadados, você pode usar palavras-chave para ajudar a pesquisar e gerenciar os ativos.

Se você adicionou palavras-chave a outros arquivos durante esta sessão, ou se removeu palavras-chave de sua lista, elas são exibidas na tabela Sugestões de Palavra-Chave.

1. Abra o arquivo na Exibição de detalhes.
1. Clique em **[!UICONTROL Keywords]**.
1. Para adicionar palavras-chave, siga um destes procedimentos:

   * Digite uma palavra-chave na caixa de texto e clique em **[!UICONTROL Add]**.
   * Clique em uma palavra-chave na tabela **[!UICONTROL Keyword Suggestions]**.

1. Para remover uma palavra-chave, selecione-a e clique em **[!UICONTROL Remove]**. Ela é movida para a tabela de Sugestões de Palavras-Chave.

>[!NOTE]
>
>Você pode adicionar palavras-chave a arquivos à medida que você as carrega no Adobe Dynamic Media Classic. Na caixa de diálogo Upload Job Options , escolha **[!UICONTROL Additional Metadata]** e insira palavras-chave.
>Consulte [Opções de upload](uploading-files.md#upload_options).

## Importar metadados {#import-metadata}

Em vez de inserir metadados manualmente em um ativo por vez, você pode importar metadados para muitos ativos diferentes de um arquivo XML ou delimitado por tabulação. Inserir os metadados em um arquivo delimitado por tabulação ou XML e importar o arquivo é menos demorado do que inserir metadados em ativos individuais. Na primeira linha do arquivo delimitado por tabulação, insira a ID e os nomes dos campos nos quais deseja registrar os metadados. Em cada linha subsequente, insira um nome de ID de ativo seguido de valores de metadados. Os campos que não estão incluídos no arquivo delimitado por tabulação ou XML não são modificados. Para importar metadados de um arquivo XML, verifique se você está em conformidade com o DTD.

>[!NOTE]
>
>Você pode criar um modelo para inserir metadados, de modo que ele possa ser importado corretamente para o Adobe Dynamic Media Classic. Depois de criar o modelo, você pode usá-lo para inserir os metadados.
>Consulte [Criar um modelo para inserir metadados a serem carregados](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Você pode encontrar mais informações sobre propriedades padronizadas em [Adobe XMP Developer Center](https://www.adobe.com/devnet/xmp.html).

1. No painel Procurar, selecione as imagens às quais deseja adicionar metadados do arquivo delimitado por tabulação ou XML.
1. Clique em **[!UICONTROL File]** > **[!UICONTROL Import Metadata]**.
1. Na caixa de diálogo **[!UICONTROL Upload Metadata]**, clique em **[!UICONTROL Browse]**.
1. Na caixa de diálogo **[!UICONTROL Select files to upload]**, selecione o arquivo delimitado por tabulação ou XML com os metadados.
1. Insira um nome de trabalho.
1. Clique em **[!UICONTROL Upload]**.

### Identificação de diferentes tipos de metadados na importação

Lembre-se do seguinte ao identificar diferentes tipos de metadados a serem importados:

* Os campos definidos pelo usuário são identificados pelo nome, conforme criado em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined fields]**. Use a funcionalidade Gerar arquivo para obter uma lista de todos os UDFs definidos no formato de importação correto.
* XMP As propriedades de metadados devem ter o prefixo XMP relacionado antes do nome (property-). Um sinal de dois pontos separa o prefixo e o nome. O prefixo XMP pode ser encontrado em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Schema]** editor. Os nomes técnicos podem ser encontrados na documentação do schema de XMP relacionado. XMP nomes de propriedades não aparecem no recurso Gerar arquivo .
* As propriedades do Esquema de metadados devem ter o prefixo relacionado antes do nome (propriedade-). Um sinal de dois pontos separa o prefixo e o nome. O prefixo e os nomes das propriedades são definidos no editor de Esquema de metadados. Os nomes das propriedades do Esquema de metadados não aparecem no recurso Gerar arquivo .

Por exemplo: A propriedade XMP de palavras-chave é o schema XMP &quot;Dublin Core&quot; com o prefixo `dc` e `subject` é o nome do XMP técnico. O prefixo e o nome do XMP técnico são combinados no nome completo da propriedade `dc:subject`. No formato de importação de metadados XML, `dc.subject` deve ser o nome da propriedade. No formato de importação delimitado por tabulação, ele deve ser o cabeçalho da coluna.

### Importar Palavras-Chave

As palavras-chave podem ser importadas como uma lista separada por vírgulas. Se uma vírgula for exibida em qualquer um dos valores individuais, ela deverá ser escapada por uma barra invertida (\). Uma barra invertida literal é a barra invertida dupla normal (\\).

Por exemplo, um arquivo de importação de metadados contendo o valor &quot;Hello\, World!,back\\slash,foo&quot; para `dc:subject` define três palavras-chave XMP no ativo: &quot;Olá, Mundo!&quot;, &quot;trás\barra&quot; e &quot;foo.&quot;

### Importar XMP e arquivos de XMP de metadados do Esquema de Metadados

A importação XML aceita apenas XML válido. Ao importar XMP ou campos de Esquema de metadados, o prefixo do namespace é adicionado e se comporta aqui como um namespace XMP. Este namespace deve ser declarado. Por exemplo, na tag de nível superior.

Por exemplo:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### Importar XMP e arquivos delimitados por tabulação de metadados do esquema de metadados

O prefixo deve ser adicionado ao cabeçalho da coluna relacionada do campo de importação.

## Importar metadados (via FTP) {#import-metadata-via-ftp}

Você pode importar metadados para vários arquivos inserindo os metadados em um arquivo XML ou delimitado por tabulação e selecionando **[!UICONTROL Process metadata files]** na página Upload Job Options (Via FTP tab) .

Verifique se os dados no arquivo delimitado por tabulação ou XML estão no formato correto. Na primeira linha, insira o campo ID seguido dos nomes dos campos de metadados que serão modificados. Em cada linha subsequente, insira um nome de ID de ativo seguido de valores de metadados. Os campos que não estão incluídos no arquivo delimitado por tabulação ou XML não são modificados.

Na barra Navegação global, clique em **[!UICONTROL Upload]**. Para importar os metadados, na página Upload , clique na guia **[!UICONTROL Via FTP]** e, em seguida, clique em **[!UICONTROL Job Options]**. Na caixa de diálogo Upload Job Options , clique em **[!UICONTROL Job]** e marque a caixa de seleção **[!UICONTROL Process metadata files]**.

## Renomear IDs em lote usando metadados {#batch-rename-ids-using-metadata}

Com os metadados importados de um arquivo delimitado por tabulação ou XML, é possível renomear as IDs clássicas do Adobe Dynamic Media. Os metadados importados são aplicados somente às imagens especificadas no próprio arquivo de metadados. Não importa se as imagens estão selecionadas no Painel de navegação.

Para renomear uma ID Adobe do Dynamic Media Classic de uma imagem, adicione uma coluna rotulada *newipsid* ao arquivo delimitado por tabulação ou adicione um campo chamado `new_vc_objectname` aos dados XML.

Por exemplo:

| ipsid | newipsid |
|--- |--- |
| jaqueta_1 | Jacket_test_1 |
| jaqueta_azul | Jacket_test_2 |

O log de trabalho do trabalho de Metadados mostra quais IDs foram renomeadas com êxito e quais não foram.

## Criar um modelo para inserir metadados para upload {#create-a-template-for-entering-metadata-to-upload}

O Adobe Dynamic Media Classic oferece um comando para criar um modelo para registrar metadados. Usar o modelo garante que os metadados sejam inseridos no formato correto para que possam ser carregados corretamente no Adobe Dynamic Media Classic. Para criar um modelo para usar na gravação e importação de metadados para o Adobe Dynamic Media Classic, siga estas etapas:

1. Selecione ativos de imagem com campos de metadados que você deseja para seu modelo.
1. Clique em **[!UICONTROL File]** > **[!UICONTROL Import Metadata]**.
1. Para o **[!UICONTROL Asset Properties Type]**, selecione **[!UICONTROL Image]**.
1. Na lista suspensa **[!UICONTROL Generate File]**, escolha **[!UICONTROL Tab delimited Template]**, **[!UICONTROL Asset's XML Metadata]** ou **[!UICONTROL XML DTD]**.
1. Clique em **[!UICONTROL Generate]**.
1. Na caixa de diálogo exibida, copie os dados. Use esses dados para construir o template.

## Trabalhar com esquemas de metadados {#working-with-metadata-schemas}

Um administrador da empresa pode exibir uma lista de todos os esquemas disponíveis. Na barra Navegação global, clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Schema]**.

Inicialmente, a lista de esquemas padrão globais como XMP está oculta. Eles podem ser exibidos usando a caixa de seleção na parte inferior da lista.

O administrador da empresa pode criar um esquema personalizado ou editar um esquema personalizado existente.

Você pode usar o Editor de esquema de metadados para executar as seguintes ações:

| Ação | Descrição |
|--- |--- |
| Adicionar | Adiciona uma propriedade ao esquema. Uma caixa de diálogo modal coleta as informações: ID, rótulo, estrutura e tipo de dados. |
| Adicionar valor de escolha | Adiciona uma nova opção selecionável a uma propriedade com estrutura de escolha aberta ou escolha fechada. Todos os valores de escolha têm o mesmo tipo. Selecione a própria propriedade para ativar o botão. |
| Editar | Edite o Label de uma propriedade ou valor de escolha. Você só pode alterar o Rótulo, a ID e as informações do tipo são imutáveis. |
| Mover para cima/Mover para baixo | A ordem no schema é refletida na interface do usuário. Para alterar a ordem, selecione uma propriedade ou um valor de escolha e mova-o com os botões. Atualmente, não há suporte para arrastar e soltar. |
| Excluir | Exclui uma propriedade ou um valor de escolha do esquema. Ele não exclui valores do bloco XMP ou do Banco de Dados. A propriedade não está mais disponível para Exibições de metadados e é removida da Exibição de detalhes do ativo. Se a propriedade foi publicada no Servidor de Metadados, execute uma publicação forçada para remover os dados do Servidor de Metadados voltado para o público. |

O sistema gera automaticamente um esquema personalizado para campos definidos pelo usuário com o prefixo `s7udf`. São campos definidos pelo usuário existentes e são editados na própria seção Configuração .

>[!NOTE]
>
>Alterações no schema nunca alteram os próprios metadados do ativo. No entanto, elas não estão visíveis para todas as funcionalidades do Adobe Dynamic Media Classic e do Servidor de Metadados e não podem ser acessadas após serem alteradas. Da mesma forma, se houver metadados para um ativo, a criação do schema correspondente torna os metadados utilizáveis no Adobe Dynamic Media Classic e no Servidor de metadados.

O Editor de esquema de metadados oferece uma maneira gráfica de adicionar ou editar um esquema de empresa personalizado dentro do Adobe Dynamic Media Classic. Um schema é definido por um prefixo, um namespace e uma lista de propriedades.

* **Nome**  - UI-Name do schema. Usado para identificar as propriedades nas Exibições de metadados e na Pesquisa avançada. Semelhante a XMP seções como Básico, IPTC, PDF.

* **Prefixo**  - Identificador exclusivo técnico para o esquema. Restrito às letras a-z e A-Z. O prefixo não está visível na interface do usuário do Adobe Dynamic Media Classic, mas é usado quando os metadados de um ativo são armazenados no bloco de XMP e no banco de dados. O prefixo é usado para identificar exclusivamente campos de metadados em consultas de pesquisa de metadados no Servidor de Metadados ou na importação.

* **Namespace**  - Identificador exclusivo técnico para o esquema, normalmente um URL no formulário  `https://your.company.com/name/version/`. Consulte a lista de schemas padrão para obter exemplos. O namespace não é visível na interface do usuário clássica do Adobe Dynamic Media, mas é usado para armazenar metadados no bloco de XMP.

* **Descrição**  - Descrição do formulário gratuito do esquema.

>[!NOTE]
>
>Não é possível editar o prefixo e o espaço de nomes. Para alterar essas propriedades, você deve excluir e recriar o schema.

As propriedades descrevem os metadados que podem ser armazenados com esse esquema no bloco de XMP. Uma propriedade consiste em:

| Propriedade | Descrição |
|--- |--- |
| ID | Identificador técnico para esta propriedade. A ID não está visível na interface do usuário do Adobe Dynamic Media Classic, mas é usada quando os metadados de um ativo são armazenados no bloco de XMP e no banco de dados. A ID é usada para criar consultas de pesquisa no Servidor de Metadados. A ID tem algumas restrições, como: <ul><li>Sem espaços</li><li>Sem &quot;.&quot;, &quot;:&quot;, &quot;$&quot;</li><li>Nenhum número como primeiro caractere</li><li>A prática recomendada é usar a-z ou A-Z como primeiro caractere</li></ul> <br>Depois de criada, a ID não pode ser alterada. |
| Rótulo | UI-Name para esta propriedade. |
| Estrutura | Determina o tipo da propriedade junto com o Tipo de dados. A estrutura pode ser uma das seguintes:<ul><li>Tipo simples: valor único do tipo de dados</li><li>Sequência: uma lista de valores do mesmo tipo de dados</li><li>Opção aberta: selecione um item de uma lista de valores predefinidos ou insira texto livre. Pode ser somente do tipo de dados String ou Integer</li><li>Escolha fechada: selecione um item em uma lista de valores predefinidos (um pop-up ou caixa de combinação)</li></ul> |
| Tipo de dados | Selecione entre estes tipos disponíveis: <ul><li>String</li><li>Número inteiro</li><li>Flutuar</li><li>Sim/Não (Booleano)</li><li>Data</li></ul> |

Quando a propriedade tiver a estrutura Escolha aberta ou Escolha fechada, você deverá fornecer pelo menos um Valor de escolha. A opção Abrir pode ser alterada. Não é possível alterar a opção Fechada. Todos os valores de escolha têm o tipo de dados da propriedade.

| Propriedade | Descrição |
|--- |--- |
| ID | Identificador técnico para este valor. A ID não está visível na interface do usuário do Adobe Dynamic Media Classic, mas é usada quando os metadados de um ativo são armazenados no bloco de XMP e no banco de dados. A ID é usada em consultas de pesquisa no Servidor de Metadados. A ID não pode conter espaços. Depois de criada, a ID não pode ser alterada. |
| Rótulo | UI-Name para este valor. |

>[!MORELIKETHIS]
>
>* [Predefinições do visualizador](application-setup.md#viewer_presets)
>* [Predefinições de metadados](application-setup.md#metadata_presets)

