---
title: Pesquisar ativos
seo-title: Pesquisar ativos
description: nulo
seo-description: Saiba como pesquisar ativos.
uuid: 058209bc-bac4-4d5c-8261-e242a543beaf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: effef4e7-37c5-42e2-9266-ecd026cad628
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1407'
ht-degree: 0%

---


# Pesquisar ativos{#searching-assets}

Para localizar ativos de arquivo no Dynamic Media Classic, você pode visualização ativos por tipo, classificar ativos no Painel de navegação, realizar uma pesquisa simples, realizar uma pesquisa avançada e filtrar ativos.

>[!NOTE]
>
>A tela Configuração pessoal oferta opções para escolher como deseja realizar pesquisas. Por exemplo, você pode escolher um tipo de pesquisa padrão e escolher se deseja incluir campos definidos pelo usuário nas pesquisas. Para obter mais informações, consulte Configuração [pessoal](personal-setup.md#personal_setup).

## Exibir ativos por tipo {#viewing-assets-by-type}

Para ver somente arquivos de um determinado tipo ao navegar, abra o menu suspenso Mostrar na Biblioteca de ativos e escolha um tipo de arquivo. Somente os ativos do tipo escolhido aparecem na Biblioteca de ativos.

## Classificação de arquivos no painel Procurar {#sorting-files-in-the-browse-panel}

Para classificar o conteúdo de uma pasta ou os resultados da pesquisa no Painel de navegação, selecione o menu Classificar e escolha uma opção. As opções são Nome, Tamanho, Tipo, Data de criação e Última modificação.

Você pode escolher Crescente ou Decrescente para classificar ativos em ordem crescente ou decrescente de acordo com os critérios escolhidos.

Na Visualização da Lista, é possível classificar clicando no nome de uma coluna.

## Conduzindo uma pesquisa simples {#conducting-a-simple-search}

Use o campo Pesquisar para realizar pesquisas simples. Você pode procurar itens por nome ou procurar itens cujos metadados contenham uma palavra-chave.

Para realizar uma pesquisa simples:

1. Selecione a pasta na Biblioteca de ativos para pesquisar em uma pasta específica e em suas subpastas
1. Clique na Biblioteca de ativos e escolha uma opção que descreva o quão estreita ou ampla você deseja que a pesquisa seja. Você pode escolher Dentro de todos os arquivos e pastas, Dentro da pasta selecionada ou Dentro da pasta e subpastas selecionadas.
1. Insira um termo de pesquisa.
1. Clique em Ir ou pressione Enter.

   Os resultados de sua pesquisa são exibidos no Painel de navegação.

>[!NOTE]
>
>O Dynamic Media Classic rastreia pesquisas. Para executar uma pesquisa pela segunda vez, selecione o botão Pesquisar e escolha o nome de uma pesquisa na parte inferior do menu Pesquisar.

## Condução de uma pesquisa avançada {#conducting-an-advanced-search}

Clique em Pesquisa avançada na Biblioteca de ativos para pesquisar usando muitos critérios, incluindo valores nos campos de metadados.

Especifique qualquer um dos seguintes critérios em sua pesquisa:

**Filtrar por tipo** de ativo Restrinja sua pesquisa a apenas um tipo de ativo escolhendo um tipo de ativo no menu.

**Arquivos e pastas** Escolha onde deseja pesquisar: Em Todos os arquivos e pastas, na pasta selecionada ou em pastas e subpastas selecionadas.

**Todos os estados** de publicação Pesquisar arquivos marcados como prontos para publicação, não estão marcados como prontos para publicação ou todos os arquivos.

**Condições** Se você especificar critérios de metadados para pesquisa, selecione se a pesquisa deve corresponder a todas as condições (uma pesquisa ALL) ou a qualquer condição (uma pesquisa OU).

**Especificar critérios** de pesquisa de metadados Crie um ou mais campos de pesquisa para pesquisar metadados. Para criar campos de pesquisa:

1. Abra a lista Visualização Metadados (à esquerda do menu Adicionar um campo) e escolha uma Visualização de Metadados. Você pode escolher Visualização compacta, IPTC, XMP ou uma visualização configurada pelo administrador.
1. Selecione o menu Adicionar um campo e escolha um nome de campo na lista suspensa.
1. Escolha uma opção Contém (Contém, Não Contém, Começa com, Termina com ou Igual).
1. Para campos numéricos, escolha um valor ou insira um intervalo de datas personalizado.
1. (Opcional) Repita as etapas de 1 a 4 para criar mais campos de pesquisa.

Você pode clicar no botão Remover campo de pesquisa para remover um campo de pesquisa.

Clique em Pesquisar para iniciar sua pesquisa. Os resultados da pesquisa são exibidos no Painel de navegação. Você pode alterar qualquer condição de pesquisa e clicar em Pesquisar para executar a pesquisa novamente.

Clique em Limpar para apagar os critérios de pesquisa e start uma nova pesquisa. Clique em Fechar quando terminar de pesquisar para fechar o painel Pesquisar.

## Filtrar ativos usando metadados {#filter-assets-using-metadata}

Filtre os ativos na guia Filtros da Biblioteca de ativos. Para filtrar ativos, use valores de metadados como critérios. Depois de escolher um campo de metadados que deseja usar para filtragem, a guia Filtros lista todos os valores de metadados inseridos no campo que você escolheu e o número de ativos aos quais foi atribuído cada valor. Por exemplo, em uma operação de filtro no campo de metadados do Criador, a guia Filtros lista todos os nomes inseridos no campo de metadados do Criador para ativos diferentes e, para cada nome, o número de ativos atribuídos ao nome. Em seguida, clique em um valor de metadados para ver todos os ativos que receberam esse valor. No exemplo, clique no valor de metadados do Jimmy para ver todos os ativos nos quais o nome Jimmy foi inserido no campo de metadados do Criador. É possível filtrar usando mais de um campo de metadados como critério de filtragem.

É possível salvar operações de filtro para executá-las muitas vezes.

>[!NOTE]
>
>Somente os campos de metadados na Visualização Metadados padrão podem ser usados para operações de filtro. A tela Visualizações de metadados mostra o nome da Visualização de metadados padrão.

Consulte Visualizações [de metadados](application-setup.md#metadata_views).

### Execução de uma operação de filtro {#running-a-filter-operation}

Siga estas etapas para localizar ativos filtrando com seus valores de metadados:

1. Clique na guia Filtros na Biblioteca de ativos.

   Os critérios da operação de filtro anterior são exibidos no painel Filtros. O painel Filtros é dividido em painéis, com cada painel representando um campo de metadados. Use os painéis para escolher quais campos de metadados filtrar e dentro de cada campo, para escolher um valor de metadados para a operação de filtro.

   Para executar uma operação de filtro criada e salva, clique no botão Selecionar predefinição e escolha o nome da operação no menu.

   Consulte [Salvar, repetir e excluir operações](searching-assets.md#saving_repeating_and_deleting_filter_operations)de filtro.

1. Ao clicar no botão Campo em um painel, siga estas instruções para exibir o menu de filtragem e construir a operação de filtro:

   **Seleção de um campo** de metadados Selecione o nome do campo no menu de filtragem.

   ***observação **: Somente os nomes dos campos de metadados na Visualização Metadados padrão aparecem no menu de filtragem.*

   Consulte Visualizações [de metadados](application-setup.md#metadata_views).

   **Adicionando um campo** de metadados Escolha Adicionar um painel. Depois que o painel for exibido no painel Filtros, clique no botão Campo e escolha o nome de um campo de metadados no menu de filtragem.

   **Removendo um campo** de metadados Escolha Remover este painel no menu de filtragem.

   Ao escolher um campo de metadados, seu painel lista:

   * Todos os valores de metadados inseridos no campo.
   * Para cada valor de metadados, o número de ativos que recebeu o valor.

1. Repita a Etapa 2 quantas vezes forem necessárias para lista todos os campos de metadados para a operação de filtro nos painéis.
1. Em cada painel, selecione um valor de metadados para filtrar. Não é possível selecionar mais de um valor de metadados em cada painel.

   Os ativos que correspondem a todos os valores selecionados são exibidos no painel Procurar.

   >[!NOTE]
   >
   >Para remover temporariamente um campo da operação de filtro, clique em Desmarcar tudo. Essa opção está localizada na parte superior de cada painel, acima dos valores de metadados.

1. (Opcional) Para salvar a operação de filtro e executá-la posteriormente, clique no botão Selecionar predefinição, escolha Salvar atual como novas predefinições e insira um nome na caixa de diálogo Salvar.

### Salvar, repetir e excluir operações de filtro {#saving-repeating-and-deleting-filter-operations}

Siga estas instruções na guia Filtros para salvar, repetir e excluir operações de filtro:

**Salvando uma operação** de filtro Clique no botão Selecionar predefinição, escolha Salvar atual como novas predefinições e digite um nome na caixa de diálogo Salvar.

**Repetindo uma operação** de filtro Clique no botão Selecionar predefinição e escolha o nome de uma operação de filtro no menu. As listas de menu filtram as operações que você salvou.

**Excluindo uma operação de filtro do menu** Selecionar predefinido Execute a operação de filtro. Em seguida, clique no botão Selecionar predefinição e escolha Excluir predefinição no menu.

## Uso do servidor de metadados {#using-the-metadata-server}

O servidor de metadados é uma API pública que pode ser usada para pesquisar ativos por metadados por meio de solicitações http.

Para configurar o servidor de metadados, clique em Configuração > Configuração do aplicativo > Configuração de publicação > Servidor de metadados.

A tela Publicação do Servidor de Metadados é aberta. Essa tela permite que você defina as seguintes opções:

**A Publicação** instantânea envia automaticamente quaisquer alterações de metadados quando são feitas, incluindo novos ativos, alterações de palavras-chave e assim por diante.

**XMP Packet** Publica o XMP Packet. Este pacote não é usado para pesquisa, mas fornece o XMP/

**Palavras-chave** Publica suas palavras-chave no servidor de metadados para uso em pesquisas.

**Campos** de publicação do servidor de metadados Selecione os campos a serem incluídos nos metadados. Isso permite que você determine quantas informações sobre seus ativos estão disponíveis para o público. Esses campos também são exibidos nas Visualizações de Metadados, mas só podem ser alterados no servidor de metadados.

Clique em **Publicar agora** para start do trabalho. Uma confirmação é exibida informando que o trabalho foi iniciado.

>[!MORELIKETHIS]
>
>* [Noções básicas de navegação](navigation-basics.md#navigation_basics)
>* [Exibição, adição e exportação de metadados](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

