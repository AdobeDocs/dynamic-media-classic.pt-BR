---
title: Pesquisar ativos do Dynamic Media Classic
description: Saiba como pesquisar ativos no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3f690c-7dff-4bf0-9366-085ba918fe6b
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 0%

---

# Pesquisar ativos no Adobe Dynamic Media Classic{#searching-assets}

Para localizar ativos de arquivos no Adobe Dynamic Media Classic, você pode visualizar ativos por tipo, classificar ativos no painel Procurar, realizar uma pesquisa simples, realizar uma Pesquisa avançada e filtrar ativos.

>[!NOTE]
>
>A página Configuração Pessoal oferece opções para escolher como você deseja realizar pesquisas. Por exemplo, você pode escolher um tipo de pesquisa padrão e escolher se deseja incluir campos definidos pelo usuário em pesquisas. Para obter mais informações, consulte [Configuração Pessoal](personal-setup.md#personal_setup).

## Exibir ativos por tipo {#viewing-assets-by-type}

Para ver apenas os arquivos de determinado tipo enquanto você navega, na Biblioteca de Ativos no lado esquerdo da lista suspensa **[!UICONTROL Show]**, escolha um tipo de arquivo. Somente ativos do tipo escolhido para exibição aparecem na Biblioteca de ativos.

>[!NOTE]
>
>Se não vir o painel Biblioteca de ativos no lado esquerdo, clique na seta de triângulo para a direita no lado esquerdo, na metade da janela do Dynamic Media Classic, para abrir a Biblioteca de ativos.

## Classificar arquivos no painel Procurar {#sorting-files-in-the-browse-panel}

Você pode classificar o conteúdo de uma pasta ou os resultados da pesquisa exibidos no painel Procurar à direita. Na barra Navegação Global, selecione **[!UICONTROL Sort]** e escolha uma opção. As opções são **[!UICONTROL Name]**, **[!UICONTROL Size (KB)]**, **[!UICONTROL Type]**, **[!UICONTROL Date Created]** e **[!UICONTROL Last Modified]**.

Você também pode escolher **[!UICONTROL Ascending]** ou **[!UICONTROL Descending]** para classificar ativos em ordem crescente ou decrescente pelos critérios escolhidos.

Na Exibição de lista, você pode classificar selecionando um nome de coluna.

## Realizar uma pesquisa simples {#conducting-a-simple-search}

Use o campo Pesquisar na Biblioteca de ativos para realizar pesquisas simples. Você pode pesquisar itens por nome ou pesquisar itens cujos metadados contenham uma palavra-chave.

1. Na Biblioteca de ativos, no painel **[!UICONTROL Folders]**, selecione a pasta a ser pesquisada em uma determinada pasta e suas subpastas.
1. À esquerda do campo Pesquisar na Biblioteca de ativos, selecione o ícone **[!UICONTROL Magnifying Glass]** para abrir a lista suspensa.
1. Na lista suspensa, escolha uma opção que descreva o quão estreita ou ampla você deseja que a pesquisa seja. Você pode escolher **[!UICONTROL Within All Files & Folders]**, **[!UICONTROL Within Selected Folder]** ou **[!UICONTROL Within Selected Folder & Subfolders]**.
1. No campo Pesquisar, informe um termo de pesquisa.
1. À direita do campo Pesquisa, selecione **[!UICONTROL Go]** ou pressione **[!UICONTROL Enter]**.

   Os resultados da pesquisa são exibidos no painel Procurar à direita.

<!-- Does not appear to be working anymore >[!NOTE]
>
>Adobe Dynamic Media Classic tracks searches. To run a search a second time, select **[!UICONTROL Search]** and choose the name of a search at the bottom of the Search menu. -->

## Realizar uma pesquisa avançada {#conducting-an-advanced-search}

Na Biblioteca de ativos, logo abaixo do campo Pesquisar, selecione **[!UICONTROL Advanced Search]** para pesquisar usando muitos critérios, incluindo valores em campos de metadados.

Especifique qualquer um dos critérios a seguir na pesquisa avançada:

* **Filtrar por tipo de ativo**: restrinja sua pesquisa a apenas um tipo de ativo. Escolha um tipo de ativo no menu.

* **Arquivos e pastas**: escolha onde deseja pesquisar: **[!UICONTROL Within All Files & Folders]**, **[!UICONTROL Within Selected Folder]** ou **[!UICONTROL Within Selected Folder & Subfolders]**.

* **Todos os estados de publicação**: procure arquivos marcados como prontos para publicação, não marcados como prontos para publicação ou todos os arquivos.

* **Condições**: se você especificar critérios de metadados para pesquisa, selecione se a pesquisa deve corresponder a todas as condições (uma pesquisa ALL) ou a qualquer condição (uma pesquisa OR).

* **Critérios de pesquisa**: crie um ou mais campos de pesquisa para pesquisar metadados. Para criar campos de pesquisa:

   1. Na Pesquisa Avançada, no cabeçalho **[!UICONTROL Search criteria]**, e à esquerda do menu **[!UICONTROL Add a Field]**, selecione o ícone de seta para baixo do triângulo para abrir a lista suspensa. Escolha uma visualização de metadados. Você pode escolher **[!UICONTROL All properties with values]**, **[!UICONTROL Compact View]**, **[!UICONTROL IPTC]**, **[!UICONTROL Metadata Server Publish Fields]** ou **[!UICONTROL XMP]**.
   1. Selecione o menu suspenso **[!UICONTROL Add a Field]** e escolha um nome de campo.
   1. Escolha uma opção de **[!UICONTROL Contains]**: **[!UICONTROL Contains]**, **[!UICONTROL Does Not Contain]**, **[!UICONTROL Begins With]**, **[!UICONTROL Ends With]** ou **[!UICONTROL Equals]**.
   1. Para campos numéricos, escolha um valor ou insira um intervalo de datas personalizado.
   1. (Opcional) Repita as etapas 1 a 4 para criar mais campos de pesquisa.

Selecione o ícone **[!UICONTROL Remove a search field]** (círculo com &quot;X&quot; dentro) para que o campo de pesquisa seja excluído.

No canto inferior direito do painel Pesquisa Avançada, selecione **[!UICONTROL Search]** para iniciar sua pesquisa. Os resultados da pesquisa são exibidos no painel Procurar à direita. Você pode alterar qualquer condição de pesquisa e selecionar **[!UICONTROL Search]** para executar a pesquisa novamente.

Selecione **[!UICONTROL Clear]** se quiser limpar os critérios de pesquisa e iniciar uma nova pesquisa. Selecione **[!UICONTROL Close]** quando terminar a pesquisa para fechar o painel Pesquisar.

## Filtrar ativos usando metadados {#filter-assets-using-metadata}

Filtre ativos na guia Filtros da Biblioteca de ativos. Para filtrar ativos, use valores de metadados como critérios. Após escolher um campo de metadados para filtrar, a guia Filtros lista todos os valores de metadados inseridos no campo escolhido. Ele também lista o número de ativos que foram atribuídos a cada valor. Por exemplo, em uma operação de filtro no campo de metadados **[!UICONTROL Creator]**, a guia **[!UICONTROL Filters]** lista todos os nomes inseridos no campo de metadados **[!UICONTROL Creator]** para ativos diferentes. Também lista, para cada nome, o número de ativos atribuídos ao nome. Em seguida, selecione um valor de metadados para ver todos os ativos que foram atribuídos a esse valor. No exemplo, selecione o valor de metadados `Prairie Cat` para ver todos os ativos nos quais o nome `Prairie Cat` foi inserido no campo de metadados **[!UICONTROL Creator]**. É possível filtrar usando mais de um campo de metadados como critério de filtragem.

É possível salvar operações de filtro para executá-las várias vezes.

>[!NOTE]
>
>Somente os campos de metadados na Exibição de Metadados padrão podem ser usados para operações de filtro. A página Views de Metadados mostra o nome da View de Metadados default.

Consulte [Exibições de Metadados](application-setup.md#metadata_views).

### Executar uma operação de filtro {#running-a-filter-operation}

Siga estas etapas para localizar ativos filtrando por seus valores de metadados:

1. Na Biblioteca de ativos, selecione a guia **[!UICONTROL Filters]**.

   Os critérios da operação de filtro anterior aparecem no painel Filtros. O painel Filtros é dividido em painéis, com cada painel representando um campo de metadados. Use os painéis para escolher com quais campos de metadados filtrar e, em cada campo, para escolher um valor de metadados para a operação de filtro.

   Para executar uma operação de filtro criada e salva, selecione **[!UICONTROL Select Preset]** e escolha o nome da operação no menu.

   Consulte [Salvar, repetir e excluir operações de filtro](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. Clique em **[!UICONTROL Field]** em um painel e siga estas instruções para exibir o menu de filtragem e criar a operação de filtro:

   * **Escolher um campo de metadados**: selecione o nome do campo no menu de filtragem.

     >[!NOTE]
     >
     >Somente os nomes dos campos de metadados na Visualização de metadados padrão aparecem no menu de filtragem.

     Consulte [Exibições de Metadados](application-setup.md#metadata_views).

   * **Adicionar um campo de metadados**: Selecione **[!UICONTROL Add a Panel]**. Depois que o painel for exibido no painel Filtros, selecione o botão **[!UICONTROL Field]** e escolha o nome de um campo de metadados no menu de filtragem.

   * **Remover um campo de metadados**: selecione **[!UICONTROL Remove This Panel]** no menu de filtragem.

   Quando você escolhe um campo de metadados, seu painel lista o seguinte:

   * Todos os valores de metadados são inseridos no campo.
   * Para cada valor de metadados, o número de ativos dado o valor.

1. Repita a Etapa 2 quantas vezes forem necessárias para listar todos os campos de metadados para a operação de filtro em painéis.
1. Em cada painel, selecione um valor de metadados para filtrar. Não é possível selecionar mais de um valor de metadados em cada painel.

   As Assets que correspondem a todos os valores selecionados aparecem no painel Procurar.

   >[!NOTE]
   >
   >Remova temporariamente um campo da operação de filtro clicando em **[!UICONTROL Deselect All]**. Essa opção está na parte superior de cada painel, acima dos valores de metadados.

1. (Opcional) Para salvar a operação de filtro e executá-la posteriormente, selecione **[!UICONTROL Select Preset]** > **[!UICONTROL Save Current As New Presets]** e digite um nome na caixa de diálogo **[!UICONTROL Save]**.

### Salvar, repetir e excluir operações de filtro {#saving-repeating-and-deleting-filter-operations}

Siga estas instruções na guia Filtros para salvar, repetir e excluir operações de filtro:

* **Salvar uma operação de filtro**: vá para **[!UICONTROL Select Preset]** > **[!UICONTROL Save Current As New Presets]** e digite um nome na caixa de diálogo **[!UICONTROL Save]**.

* **Repetir uma operação de filtro**: escolha **[!UICONTROL Select Preset]** e escolha o nome de uma operação de filtro no menu. O menu lista as operações de filtro que você salvou.

* **Excluir uma operação de filtro do menu Selecionar Predefinição**: execute a operação de filtro. Em seguida, vá para **[!UICONTROL Select Preset]** > **[!UICONTROL Delete Preset]** no menu.

## Usar o servidor de metadados {#using-the-metadata-server}

O servidor de metadados é uma API pública que pode ser usada para pesquisar ativos por metadados por meio de solicitações http.

Para configurar o servidor de metadados, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Metadata Server]**.

A página Publicar do servidor de metadados permite definir as seguintes opções:

* **[!UICONTROL Instant Publish]**: envia automaticamente quaisquer alterações de metadados quando são feitas, incluindo novos ativos, alterações de palavra-chave e assim por diante.

* **[!UICONTROL XMP Packet]**: Publica o Pacote XMP. Esse pacote não é usado para pesquisa, mas fornece o XMP mais atualizado.

* **[!UICONTROL Keywords]**: Publica suas palavras-chave no servidor de metadados para uso em pesquisas.

* **[!UICONTROL Metadata Server Publish Fields]**: Selecione os campos a serem incluídos nos metadados. Essa opção permite determinar quanta informação sobre seus ativos está disponível para o público. Esses campos também são exibidos em Exibições de metadados, mas só podem ser alterados no servidor de metadados.

Selecione **[!UICONTROL Publish Now]** para iniciar o trabalho. Uma confirmação é exibida, informando que o job foi iniciado.

>[!MORELIKETHIS]
>
>* [Noções básicas de navegação](navigation-basics.md#navigation_basics)
>* [Exibir, adicionar e exportar metadados](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
