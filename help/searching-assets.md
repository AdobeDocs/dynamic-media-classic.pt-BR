---
title: Pesquisar ativos
description: Saiba como pesquisar ativos.
uuid: 058209bc-bac4-4d5c-8261-e242a543beaf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: effef4e7-37c5-42e2-9266-ecd026cad628
feature: Dynamic Media Classic,Gerenciamento de ativos
role: Business Practitioner
exl-id: 4b3f690c-7dff-4bf0-9366-085ba918fe6b
translation-type: tm+mt
source-git-commit: a5a6596213e273d806fbc012e2c63bf3458127b0
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---

# Pesquisar ativos{#searching-assets}

Para localizar ativos de arquivo no Dynamic Media Classic, você pode exibir ativos por tipo, classificar ativos no Painel de navegação, realizar uma pesquisa simples, realizar uma pesquisa avançada e filtrar ativos.

>[!NOTE]
>
>A tela Configuração pessoal oferece opções para escolher como você deseja realizar pesquisas. Por exemplo, você pode escolher um tipo de pesquisa padrão e escolher se deseja incluir campos definidos pelo usuário em pesquisas. Para obter mais informações, consulte [Configuração Pessoal](personal-setup.md#personal_setup).

## Exibir ativos por tipo {#viewing-assets-by-type}

Para ver apenas arquivos de um determinado tipo ao navegar, abra o menu suspenso Mostrar na Biblioteca de ativos e escolha um tipo de arquivo. Somente os ativos do tipo escolhido aparecem na Biblioteca de ativos.

## Classificação de arquivos no Painel de navegação {#sorting-files-in-the-browse-panel}

Para classificar o conteúdo de uma pasta ou os resultados de pesquisa no Painel de navegação, selecione o menu Classificar e escolha uma opção. As opções são Nome, Tamanho, Tipo, Data de criação e Última modificação.

Você pode escolher Crescente ou Decrescente para classificar ativos em ordem crescente ou decrescente de acordo com os critérios escolhidos.

Na Exibição de lista, é possível classificar clicando no nome de uma coluna.

## Realização de uma pesquisa simples {#conducting-a-simple-search}

Use o campo Pesquisa para realizar pesquisas simples. Você pode pesquisar itens por nome ou pesquisar itens cujos metadados contenham uma palavra-chave.

Para realizar uma pesquisa simples:

1. Selecione a pasta na Biblioteca de ativos para pesquisar em uma pasta específica e em suas subpastas
1. Clique em na Biblioteca de ativos e escolha uma opção que descreva o quão estreita ou ampla você deseja que a pesquisa seja. Você pode escolher Dentro de todos os arquivos e pastas, Dentro da pasta selecionada ou Dentro da pasta e subpastas selecionadas.
1. Insira um termo de pesquisa.
1. Clique em Ir ou pressione Enter.

   Os resultados da sua pesquisa são exibidos no painel Procurar.

>[!NOTE]
>
>O Dynamic Media Classic rastreia pesquisas. Para executar uma pesquisa pela segunda vez, selecione o botão Pesquisar e escolha o nome de uma pesquisa na parte inferior do menu Pesquisar.

## Realizar uma pesquisa avançada {#conducting-an-advanced-search}

Clique em Pesquisa avançada na Biblioteca de ativos para pesquisar usando muitos critérios, incluindo valores em campos de metadados.

Especifique qualquer um dos seguintes critérios em sua pesquisa:

**Filtrar por** tipo de ativoRestrinja sua pesquisa a apenas um tipo de ativo escolhendo um tipo de ativo no menu.

**Arquivos e** pastasEscolha onde deseja pesquisar: Em Todos os Arquivos e Pastas, Dentro da Pasta Selecionada ou Dentro da Pasta e Subpastas Selecionadas.

**Todos os** estados de publicaçãoProcure por arquivos que estão marcados como prontos para publicação, não estão marcados como prontos para publicação ou todos os arquivos.

**** CondiçõesSe você especificar critérios de metadados para a pesquisa, selecione se a pesquisa deve corresponder a todas as condições (uma pesquisa ALL) ou qualquer condição (uma pesquisa OR).

**Especificar** critérios de pesquisa de metadadosCrie um ou mais campos de pesquisa para pesquisar metadados. Para criar campos de pesquisa:

1. Abra a lista Exibição de metadados (à esquerda do menu Adicionar um campo) e escolha uma Exibição de metadados. Você pode escolher compacta Exibição, IPTC, XMP ou exibir a configuração do administrador.
1. Selecione o menu Adicionar um campo e escolha um nome de campo na lista suspensa.
1. Escolha uma opção Contém (Contém, Não Contém, Começa com, Termina com ou Igual).
1. Para campos numéricos, escolha um valor ou insira um intervalo de datas personalizado.
1. (Opcional) Repita as etapas 1 a 4 para criar mais campos de pesquisa.

Você pode clicar no botão Remover campo de pesquisa para remover um campo de pesquisa.

Clique em Pesquisar para iniciar a pesquisa. Os resultados da pesquisa são exibidos no painel Procurar. Você pode alterar qualquer condição de pesquisa e clicar em Pesquisar para executar a pesquisa novamente.

Clique em Limpar para apagar os critérios de pesquisa e iniciar uma nova pesquisa. Clique em Fechar quando terminar a pesquisa para fechar o painel Pesquisar.

## Filtrar ativos usando metadados {#filter-assets-using-metadata}

Filtrar ativos na guia Filtros da Biblioteca de ativos. Para filtrar ativos, você usa valores de metadados como critério. Depois de escolher um campo de metadados que deseja usar para filtragem, a guia Filtros lista todos os valores de metadados inseridos no campo que você escolheu e o número de ativos aos quais foi atribuído cada valor. Por exemplo, em uma operação de filtro no campo de metadados Creator , a guia Filters lista todos os nomes que foram inseridos no campo de metadados Creator para diferentes ativos e, para cada nome, o número de ativos atribuídos ao nome. Em seguida, clique em um valor de metadados para ver todos os ativos que receberam esse valor. No exemplo, você clica no valor dos metadados Jimmy para ver todos os ativos em que o nome Jimmy foi inserido no campo de metadados Creator . Você pode filtrar usando mais de um campo de metadados como um critério de filtragem.

Você pode salvar operações de filtro para executá-las várias vezes.

>[!NOTE]
>
>Somente campos de metadados na Exibição de metadados padrão podem ser usados para operações de filtro. A tela Visualizações de metadados mostra o nome da Visualização de metadados padrão.

Consulte [Visualizações de metadados](application-setup.md#metadata_views).

### Executando uma operação de filtro {#running-a-filter-operation}

Siga estas etapas para localizar ativos filtrando com seus valores de metadados:

1. Clique na guia Filtros na Biblioteca de ativos.

   Os critérios da operação de filtro anterior aparecem no painel Filtros . O painel Filtros é dividido em painéis, e cada painel representa um campo de metadados. Use os painéis para escolher quais campos de metadados serão filtrados e, em cada campo, para escolher um valor de metadados para a operação de filtro.

   Para executar uma operação de filtro que você criou e salvou, clique no botão Selecionar predefinição e escolha o nome da operação no menu.

   Consulte [Salvar, repetir e excluir operações de filtro](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. Ao clicar no botão Field em um painel, siga estas instruções para exibir o menu de filtragem e criar a operação de filtro:

   **Escolha de um** campo de metadadosSelecione o nome do campo no menu de filtragem.

   ***observação **: Somente os nomes dos campos de metadados na Exibição de metadados padrão são exibidos no menu de filtragem.*

   Consulte [Visualizações de metadados](application-setup.md#metadata_views).

   **Adicionando um** campo de metadadosEscolha Adicionar um Painel. Depois que o painel for exibido no painel Filtros , clique no botão Campo e escolha o nome de um campo de metadados no menu de filtragem.

   **Removendo um** campo de metadadosEscolha Remover este painel no menu de filtragem.

   Ao escolher um campo de metadados, o painel lista:

   * Todos os valores de metadados inseridos no campo.
   * Para cada valor de metadados, o número de ativos que recebeu o valor.

1. Repita a Etapa 2 quantas vezes forem necessárias para listar todos os campos de metadados para a operação de filtro em painéis.
1. Em cada painel, selecione um valor de metadados para filtrar. Não é possível selecionar mais de um valor de metadados em cada painel.

   Os ativos que correspondem a todos os valores selecionados aparecem no painel Procurar.

   >[!NOTE]
   >
   >Para remover temporariamente um campo da operação de filtro, clique em Desmarcar tudo. Essa opção está localizada na parte superior de cada painel, acima dos valores de metadados.

1. (Opcional) Para salvar a operação de filtro e executá-la posteriormente, clique no botão Selecionar predefinição, escolha Salvar atual como novas predefinições e insira um nome na caixa de diálogo Salvar.

### Salvar, repetir e excluir operações de filtro {#saving-repeating-and-deleting-filter-operations}

Siga estas instruções na guia Filters para salvar, repetir e excluir operações de filtro:

**Salvar uma** operação de filtroClique no botão Selecionar predefinição, escolha Salvar atual como novas predefinições e insira um nome na caixa de diálogo Salvar.

**Repetindo uma** operação de filtroClique no botão Selecionar predefinição e escolha o nome de uma operação de filtro no menu. O menu lista as operações de filtro que você salvou.

**Excluindo uma operação de filtro no** menu Selecionar predefiniçãoExecute a operação de filtro. Em seguida, clique no botão Selecionar predefinição e escolha Excluir predefinição no menu.

## Uso do servidor de metadados {#using-the-metadata-server}

O servidor de metadados é uma API pública que pode ser usada para pesquisar ativos por metadados por meio de solicitações http.

Para configurar o servidor de metadados, clique em Configuração > Configuração do aplicativo > Configuração de publicação > Servidor de metadados.

A tela Publicação do servidor de metadados é aberta. Essa tela permite que você defina as seguintes opções:

**** Publicação instantâneaImpulsa automaticamente todas as alterações de metadados quando são feitas, incluindo novos ativos, alterações de palavras-chave e assim por diante.

**XMP** PacotePublica o XMP Pacote. Este pacote não é usado para pesquisa, mas fornece os XMP/

**** Palavras-chave Publica suas palavras-chave no servidor de metadados para uso em pesquisas.

**Campos de publicação do servidor de metadados** Selecione os campos a serem incluídos nos metadados. Isso permite determinar quantas informações sobre seus ativos estão disponíveis para o público. Esses campos também são exibidos nas Exibições de metadados, mas só podem ser alterados no servidor de metadados.

Clique em **Publicar agora** para iniciar a tarefa. Uma confirmação é exibida informando que o trabalho foi iniciado.

>[!MORELIKETHIS]
>
>* [Elementos básicos de navegação](navigation-basics.md#navigation_basics)
>* [Exibição, adição e exportação de metadados](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

